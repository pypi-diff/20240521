# Comparing `tmp/open-ephys-python-tools-0.1.7.tar.gz` & `tmp/open_ephys_python_tools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-ephys-python-tools-0.1.7.tar", last modified: Mon Oct  9 17:15:17 2023, max compression
+gzip compressed data, was "open_ephys_python_tools-0.1.8.tar", last modified: Tue May 21 00:00:53 2024, max compression
```

## Comparing `open-ephys-python-tools-0.1.7.tar` & `open_ephys_python_tools-0.1.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-10-09 17:15:17.922524 open-ephys-python-tools-0.1.7/
--rw-rw-r--   0 joshs     (1001) joshs     (1001)      137 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/.gitignore
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     1577 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/CHANGELOG.md
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     1049 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/LICENSE
--rw-r--r--   0 joshs     (1001) joshs     (1001)     5760 2023-10-09 17:15:17.922524 open-ephys-python-tools-0.1.7/PKG-INFO
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     5277 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/README.md
--rw-rw-r--   0 joshs     (1001) joshs     (1001)   367061 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/logo.png
--rw-rw-r--   0 joshs     (1001) joshs     (1001)      664 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/pyproject.toml
--rw-rw-r--   0 joshs     (1001) joshs     (1001)       38 2023-10-09 17:15:17.922524 open-ephys-python-tools-0.1.7/setup.cfg
--rw-rw-r--   0 joshs     (1001) joshs     (1001)       68 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/setup.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-10-09 17:15:17.918524 open-ephys-python-tools-0.1.7/src/
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-10-09 17:15:17.918524 open-ephys-python-tools-0.1.7/src/open_ephys/
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)       21 2023-10-09 17:08:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/__init__.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-10-09 17:15:17.918524 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     9764 2023-10-09 17:08:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/README.md
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)       63 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/__init__.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-10-09 17:15:17.918524 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/formats/
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)    14487 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/formats/BinaryRecording.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)     8271 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/formats/NwbRecording.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)    18590 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/formats/OpenEphysRecording.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)      134 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/formats/__init__.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-10-09 17:15:17.918524 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/formats/helpers/
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)       75 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/formats/helpers/__init__.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)     8852 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/formats/helpers/oe_fast_loader.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)    13647 2023-10-09 17:08:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/recording.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)     3048 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/recordnode.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)     2984 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/analysis/session.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-10-09 17:15:17.918524 open-ephys-python-tools-0.1.7/src/open_ephys/control/
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     1926 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/control/README.md
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)       88 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/control/__init__.py
--rw-rw-r--   0 joshs     (1001) joshs     (1001)    17600 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/control/http_server.py
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)     4888 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/control/network_control.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-10-09 17:15:17.918524 open-ephys-python-tools-0.1.7/src/open_ephys/streaming/
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     2123 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/streaming/README.md
--rwxrwxr-x   0 joshs     (1001) joshs     (1001)       41 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/streaming/__init__.py
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     4008 2023-10-09 16:00:45.000000 open-ephys-python-tools-0.1.7/src/open_ephys/streaming/event_listener.py
-drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2023-10-09 17:15:17.922524 open-ephys-python-tools-0.1.7/src/open_ephys_python_tools.egg-info/
--rw-r--r--   0 joshs     (1001) joshs     (1001)     5760 2023-10-09 17:15:17.000000 open-ephys-python-tools-0.1.7/src/open_ephys_python_tools.egg-info/PKG-INFO
--rw-rw-r--   0 joshs     (1001) joshs     (1001)     1105 2023-10-09 17:15:17.000000 open-ephys-python-tools-0.1.7/src/open_ephys_python_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 joshs     (1001) joshs     (1001)        1 2023-10-09 17:15:17.000000 open-ephys-python-tools-0.1.7/src/open_ephys_python_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 joshs     (1001) joshs     (1001)       31 2023-10-09 17:15:17.000000 open-ephys-python-tools-0.1.7/src/open_ephys_python_tools.egg-info/requires.txt
--rw-rw-r--   0 joshs     (1001) joshs     (1001)       11 2023-10-09 17:15:17.000000 open-ephys-python-tools-0.1.7/src/open_ephys_python_tools.egg-info/top_level.txt
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2024-05-21 00:00:53.261078 open_ephys_python_tools-0.1.8/
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)      137 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/.gitignore
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     1577 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/CHANGELOG.md
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     1049 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/LICENSE
+-rw-r--r--   0 joshs     (1001) joshs     (1001)     5760 2024-05-21 00:00:53.261078 open_ephys_python_tools-0.1.8/PKG-INFO
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     5277 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/README.md
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)   367061 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/logo.png
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)      664 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/pyproject.toml
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)       38 2024-05-21 00:00:53.261078 open_ephys_python_tools-0.1.8/setup.cfg
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)       68 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/setup.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2024-05-21 00:00:53.257078 open_ephys_python_tools-0.1.8/src/
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2024-05-21 00:00:53.261078 open_ephys_python_tools-0.1.8/src/open_ephys/
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)       21 2024-05-21 00:00:19.000000 open_ephys_python_tools-0.1.8/src/open_ephys/__init__.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2024-05-21 00:00:53.261078 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     9764 2023-10-09 17:08:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/README.md
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)       63 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/__init__.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2024-05-21 00:00:53.261078 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/formats/
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)    14487 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/formats/BinaryRecording.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)     8272 2024-05-20 23:57:50.000000 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/formats/NwbRecording.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)    18590 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/formats/OpenEphysRecording.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)      134 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/formats/__init__.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2024-05-21 00:00:53.261078 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/formats/helpers/
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)       75 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/formats/helpers/__init__.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)     8852 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/formats/helpers/oe_fast_loader.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)    13647 2023-10-09 17:08:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/recording.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)     3048 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/recordnode.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)     2984 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/analysis/session.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2024-05-21 00:00:53.261078 open_ephys_python_tools-0.1.8/src/open_ephys/control/
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     1926 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/control/README.md
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)       88 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/control/__init__.py
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)    17600 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/control/http_server.py
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)     4888 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/control/network_control.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2024-05-21 00:00:53.261078 open_ephys_python_tools-0.1.8/src/open_ephys/streaming/
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     2123 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/streaming/README.md
+-rwxrwxr-x   0 joshs     (1001) joshs     (1001)       41 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/streaming/__init__.py
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     4008 2023-10-09 16:00:45.000000 open_ephys_python_tools-0.1.8/src/open_ephys/streaming/event_listener.py
+drwxrwxr-x   0 joshs     (1001) joshs     (1001)        0 2024-05-21 00:00:53.261078 open_ephys_python_tools-0.1.8/src/open_ephys_python_tools.egg-info/
+-rw-r--r--   0 joshs     (1001) joshs     (1001)     5760 2024-05-21 00:00:53.000000 open_ephys_python_tools-0.1.8/src/open_ephys_python_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)     1105 2024-05-21 00:00:53.000000 open_ephys_python_tools-0.1.8/src/open_ephys_python_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)        1 2024-05-21 00:00:53.000000 open_ephys_python_tools-0.1.8/src/open_ephys_python_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)       31 2024-05-21 00:00:53.000000 open_ephys_python_tools-0.1.8/src/open_ephys_python_tools.egg-info/requires.txt
+-rw-rw-r--   0 joshs     (1001) joshs     (1001)       11 2024-05-21 00:00:53.000000 open_ephys_python_tools-0.1.8/src/open_ephys_python_tools.egg-info/top_level.txt
```

### Comparing `open-ephys-python-tools-0.1.7/CHANGELOG.md` & `open_ephys_python_tools-0.1.8/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/LICENSE` & `open_ephys_python_tools-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/PKG-INFO` & `open_ephys_python_tools-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-ephys-python-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Software tools for interfacing with the Open Ephys GUI
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `open-ephys-python-tools-0.1.7/README.md` & `open_ephys_python_tools-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/logo.png` & `open_ephys_python_tools-0.1.8/logo.png`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/pyproject.toml` & `open_ephys_python_tools-0.1.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys/analysis/README.md` & `open_ephys_python_tools-0.1.8/src/open_ephys/analysis/README.md`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys/analysis/formats/BinaryRecording.py` & `open_ephys_python_tools-0.1.8/src/open_ephys/analysis/formats/BinaryRecording.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys/analysis/formats/NwbRecording.py` & `open_ephys_python_tools-0.1.8/src/open_ephys/analysis/formats/NwbRecording.py`

 * *Files 1% similar despite different names*

```diff
@@ -139,15 +139,15 @@
         events = []
         processor_ids = []
         
         for dataset in datasets:
             
             if (dataset[-4:] == '.TTL'):
 
-                processor_id = int(dataset.split('.')[0].split('-')[1])
+                processor_id = int(dataset.split('.')[0].split('-')[-1])
                 stream_name = dataset.split('.')[1]
 
                 if processor_id not in processor_ids:
                     processor_ids.append(processor_id)
                     stream_id = 0
                 else:
                     stream_id += 1
```

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys/analysis/formats/OpenEphysRecording.py` & `open_ephys_python_tools-0.1.8/src/open_ephys/analysis/formats/OpenEphysRecording.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys/analysis/formats/helpers/oe_fast_loader.py` & `open_ephys_python_tools-0.1.8/src/open_ephys/analysis/formats/helpers/oe_fast_loader.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys/analysis/recording.py` & `open_ephys_python_tools-0.1.8/src/open_ephys/analysis/recording.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys/analysis/recordnode.py` & `open_ephys_python_tools-0.1.8/src/open_ephys/analysis/recordnode.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys/analysis/session.py` & `open_ephys_python_tools-0.1.8/src/open_ephys/analysis/session.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys/control/README.md` & `open_ephys_python_tools-0.1.8/src/open_ephys/control/README.md`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys/control/http_server.py` & `open_ephys_python_tools-0.1.8/src/open_ephys/control/http_server.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys/control/network_control.py` & `open_ephys_python_tools-0.1.8/src/open_ephys/control/network_control.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys/streaming/README.md` & `open_ephys_python_tools-0.1.8/src/open_ephys/streaming/README.md`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys/streaming/event_listener.py` & `open_ephys_python_tools-0.1.8/src/open_ephys/streaming/event_listener.py`

 * *Files identical despite different names*

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys_python_tools.egg-info/PKG-INFO` & `open_ephys_python_tools-0.1.8/src/open_ephys_python_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: open-ephys-python-tools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Software tools for interfacing with the Open Ephys GUI
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `open-ephys-python-tools-0.1.7/src/open_ephys_python_tools.egg-info/SOURCES.txt` & `open_ephys_python_tools-0.1.8/src/open_ephys_python_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

