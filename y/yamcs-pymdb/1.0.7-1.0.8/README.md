# Comparing `tmp/yamcs_pymdb-1.0.7.tar.gz` & `tmp/yamcs_pymdb-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yamcs_pymdb-1.0.7.tar", last modified: Thu May  9 22:32:47 2024, max compression
+gzip compressed data, was "yamcs_pymdb-1.0.8.tar", last modified: Tue May 21 19:09:48 2024, max compression
```

## Comparing `yamcs_pymdb-1.0.7.tar` & `yamcs_pymdb-1.0.8.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-09 22:32:47.775059 yamcs_pymdb-1.0.7/
--rw-r--r--   0 fdi        (503) staff       (20)     7652 2024-02-09 08:16:29.000000 yamcs_pymdb-1.0.7/LICENSE
--rw-r--r--   0 fdi        (503) staff       (20)       34 2024-02-09 08:18:18.000000 yamcs_pymdb-1.0.7/MANIFEST.in
--rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-05-09 22:32:47.774726 yamcs_pymdb-1.0.7/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)     1007 2024-02-09 09:41:58.000000 yamcs_pymdb-1.0.7/README.md
--rw-r--r--   0 fdi        (503) staff       (20)       38 2024-05-09 22:32:47.775112 yamcs_pymdb-1.0.7/setup.cfg
--rw-r--r--   0 fdi        (503) staff       (20)     1244 2024-05-09 22:25:02.000000 yamcs_pymdb-1.0.7/setup.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-09 22:32:47.744379 yamcs_pymdb-1.0.7/src/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-09 22:32:47.744051 yamcs_pymdb-1.0.7/src/yamcs/
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-09 22:32:47.771254 yamcs_pymdb-1.0.7/src/yamcs/pymdb/
--rw-r--r--   0 fdi        (503) staff       (20)      687 2024-03-14 22:48:46.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/__init__.py
--rw-r--r--   0 fdi        (503) staff       (20)     4166 2024-03-22 09:18:23.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/alarms.py
--rw-r--r--   0 fdi        (503) staff       (20)     6569 2024-04-05 11:18:43.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/algorithms.py
--rw-r--r--   0 fdi        (503) staff       (20)     1173 2024-03-22 09:19:10.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/ancillary.py
--rw-r--r--   0 fdi        (503) staff       (20)     1110 2024-02-23 15:50:36.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/calibrators.py
--rw-r--r--   0 fdi        (503) staff       (20)     6049 2024-04-15 20:41:06.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/ccsds.py
--rw-r--r--   0 fdi        (503) staff       (20)     4561 2024-03-28 20:39:32.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/checks.py
--rw-r--r--   0 fdi        (503) staff       (20)    19695 2024-05-09 20:11:31.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/commands.py
--rw-r--r--   0 fdi        (503) staff       (20)     7716 2024-05-09 21:10:10.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/containers.py
--rw-r--r--   0 fdi        (503) staff       (20)     7999 2024-04-15 21:28:28.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/csp.py
--rw-r--r--   0 fdi        (503) staff       (20)    18235 2024-05-09 19:15:26.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/datatypes.py
--rw-r--r--   0 fdi        (503) staff       (20)     8370 2024-04-05 09:43:14.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/encodings.py
--rw-r--r--   0 fdi        (503) staff       (20)       86 2024-01-04 13:44:01.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/exceptions.py
--rw-r--r--   0 fdi        (503) staff       (20)     4045 2024-03-22 07:37:40.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/expressions.py
--rw-r--r--   0 fdi        (503) staff       (20)    16520 2024-04-04 12:25:17.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/parameters.py
--rw-r--r--   0 fdi        (503) staff       (20)     8350 2024-04-05 09:43:14.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/systems.py
--rw-r--r--   0 fdi        (503) staff       (20)     4427 2024-04-05 09:50:48.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/verifiers.py
--rw-r--r--   0 fdi        (503) staff       (20)    80080 2024-05-09 22:25:02.000000 yamcs_pymdb-1.0.7/src/yamcs/pymdb/xtce.py
-drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-09 22:32:47.774323 yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/
--rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-05-09 22:32:47.000000 yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/PKG-INFO
--rw-r--r--   0 fdi        (503) staff       (20)      737 2024-05-09 22:32:47.000000 yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/SOURCES.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2024-05-09 22:32:47.000000 yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/dependency_links.txt
--rw-r--r--   0 fdi        (503) staff       (20)        1 2023-12-13 14:35:06.000000 yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/not-zip-safe
--rw-r--r--   0 fdi        (503) staff       (20)        6 2024-05-09 22:32:47.000000 yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/top_level.txt
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-21 19:09:48.946582 yamcs_pymdb-1.0.8/
+-rw-r--r--   0 fdi        (503) staff       (20)     7652 2024-02-09 08:16:29.000000 yamcs_pymdb-1.0.8/LICENSE
+-rw-r--r--   0 fdi        (503) staff       (20)       34 2024-02-09 08:18:18.000000 yamcs_pymdb-1.0.8/MANIFEST.in
+-rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-05-21 19:09:48.946328 yamcs_pymdb-1.0.8/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)     1007 2024-02-09 09:41:58.000000 yamcs_pymdb-1.0.8/README.md
+-rw-r--r--   0 fdi        (503) staff       (20)       38 2024-05-21 19:09:48.946758 yamcs_pymdb-1.0.8/setup.cfg
+-rw-r--r--   0 fdi        (503) staff       (20)     1244 2024-05-21 18:45:11.000000 yamcs_pymdb-1.0.8/setup.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-21 19:09:48.880064 yamcs_pymdb-1.0.8/src/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-21 19:09:48.879856 yamcs_pymdb-1.0.8/src/yamcs/
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-21 19:09:48.898927 yamcs_pymdb-1.0.8/src/yamcs/pymdb/
+-rw-r--r--   0 fdi        (503) staff       (20)      687 2024-03-14 22:48:46.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/__init__.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4166 2024-03-22 09:18:23.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/alarms.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6569 2024-04-05 11:18:43.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/algorithms.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1173 2024-03-22 09:19:10.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/ancillary.py
+-rw-r--r--   0 fdi        (503) staff       (20)     1110 2024-02-23 15:50:36.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/calibrators.py
+-rw-r--r--   0 fdi        (503) staff       (20)     6049 2024-04-15 20:41:06.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/ccsds.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4561 2024-03-28 20:39:32.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/checks.py
+-rw-r--r--   0 fdi        (503) staff       (20)    19695 2024-05-09 20:11:31.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/commands.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7716 2024-05-09 21:10:10.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/containers.py
+-rw-r--r--   0 fdi        (503) staff       (20)     7999 2024-04-15 21:28:28.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/csp.py
+-rw-r--r--   0 fdi        (503) staff       (20)    18235 2024-05-21 17:39:46.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/datatypes.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8370 2024-04-05 09:43:14.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/encodings.py
+-rw-r--r--   0 fdi        (503) staff       (20)       86 2024-01-04 13:44:01.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/exceptions.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4045 2024-03-22 07:37:40.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/expressions.py
+-rw-r--r--   0 fdi        (503) staff       (20)    16520 2024-04-04 12:25:17.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/parameters.py
+-rw-r--r--   0 fdi        (503) staff       (20)     8350 2024-04-05 09:43:14.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/systems.py
+-rw-r--r--   0 fdi        (503) staff       (20)     4427 2024-04-05 09:50:48.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/verifiers.py
+-rw-r--r--   0 fdi        (503) staff       (20)    80124 2024-05-21 18:33:30.000000 yamcs_pymdb-1.0.8/src/yamcs/pymdb/xtce.py
+drwxr-xr-x   0 fdi        (503) staff       (20)        0 2024-05-21 19:09:48.945994 yamcs_pymdb-1.0.8/src/yamcs_pymdb.egg-info/
+-rw-r--r--   0 fdi        (503) staff       (20)     1915 2024-05-21 19:09:48.000000 yamcs_pymdb-1.0.8/src/yamcs_pymdb.egg-info/PKG-INFO
+-rw-r--r--   0 fdi        (503) staff       (20)      737 2024-05-21 19:09:48.000000 yamcs_pymdb-1.0.8/src/yamcs_pymdb.egg-info/SOURCES.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2024-05-21 19:09:48.000000 yamcs_pymdb-1.0.8/src/yamcs_pymdb.egg-info/dependency_links.txt
+-rw-r--r--   0 fdi        (503) staff       (20)        1 2023-12-13 14:35:06.000000 yamcs_pymdb-1.0.8/src/yamcs_pymdb.egg-info/not-zip-safe
+-rw-r--r--   0 fdi        (503) staff       (20)        6 2024-05-21 19:09:48.000000 yamcs_pymdb-1.0.8/src/yamcs_pymdb.egg-info/top_level.txt
```

### Comparing `yamcs_pymdb-1.0.7/LICENSE` & `yamcs_pymdb-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/PKG-INFO` & `yamcs_pymdb-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-pymdb
-Version: 1.0.7
+Version: 1.0.8
 Summary: Generate XTCE for use with Yamcs
 Home-page: https://github.com/yamcs/pymdb
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Keywords: packet telemetry ccsds xtce yamcs
 Platform: Posix; MacOS X; Windows
```

### Comparing `yamcs_pymdb-1.0.7/README.md` & `yamcs_pymdb-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/setup.py` & `yamcs_pymdb-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with io.open("README.md", encoding="utf-8") as f:
     readme = f.read()
 
 setuptools.setup(
     name="yamcs-pymdb",
-    version="1.0.7",
+    version="1.0.8",
     description="Generate XTCE for use with Yamcs",
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://github.com/yamcs/pymdb",
     author="Space Applications Services",
     author_email="yamcs@spaceapplications.com",
     license="LGPL",
```

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/__init__.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/__init__.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/alarms.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/alarms.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/algorithms.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/algorithms.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/ancillary.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/ancillary.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/calibrators.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/calibrators.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/ccsds.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/ccsds.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/checks.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/checks.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/commands.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/commands.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/containers.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/containers.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/csp.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/csp.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/datatypes.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/datatypes.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/encodings.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/encodings.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/expressions.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/expressions.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/parameters.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/parameters.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/systems.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/systems.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/verifiers.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/verifiers.py`

 * *Files identical despite different names*

### Comparing `yamcs_pymdb-1.0.7/src/yamcs/pymdb/xtce.py` & `yamcs_pymdb-1.0.8/src/yamcs/pymdb/xtce.py`

 * *Files 0% similar despite different names*

```diff
@@ -779,15 +779,15 @@
         if data_type.units:
             unit_set_el = ET.SubElement(el, "UnitSet")
             unit_el = ET.SubElement(unit_set_el, "Unit")
             unit_el.attrib["form"] = "calibrated"
             unit_el.text = data_type.units
 
         if data_type.encoding:
-            self.add_data_encoding(el, system, data_type.encoding)
+            self.add_data_encoding(el, system, data_type.encoding, data_type.calibrator)
 
         if data_type.minimum is not None or data_type.maximum is not None:
             set_el = ET.SubElement(el, "ValidRangeSet")
             set_el.attrib["validRangeAppliesToCalibrated"] = "true"
             range_el = ET.SubElement(set_el, "ValidRange")
             if data_type.minimum is not None:
                 if data_type.minimum_inclusive:
@@ -819,15 +819,15 @@
         if data_type.units:
             unit_set_el = ET.SubElement(el, "UnitSet")
             unit_el = ET.SubElement(unit_set_el, "Unit")
             unit_el.attrib["form"] = "calibrated"
             unit_el.text = data_type.units
 
         if data_type.encoding:
-            self.add_data_encoding(el, system, data_type.encoding)
+            self.add_data_encoding(el, system, data_type.encoding, data_type.calibrator)
 
         if data_type.minimum is not None or data_type.maximum is not None:
             set_el = ET.SubElement(el, "ValidRangeSet")
             set_el.attrib["validRangeAppliesToCalibrated"] = "true"
             range_el = ET.SubElement(set_el, "ValidRange")
             if data_type.minimum is not None:
                 range_el.attrib["minInclusive"] = str(data_type.minimum)
```

### Comparing `yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/PKG-INFO` & `yamcs_pymdb-1.0.8/src/yamcs_pymdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yamcs-pymdb
-Version: 1.0.7
+Version: 1.0.8
 Summary: Generate XTCE for use with Yamcs
 Home-page: https://github.com/yamcs/pymdb
 Author: Space Applications Services
 Author-email: yamcs@spaceapplications.com
 License: LGPL
 Keywords: packet telemetry ccsds xtce yamcs
 Platform: Posix; MacOS X; Windows
```

### Comparing `yamcs_pymdb-1.0.7/src/yamcs_pymdb.egg-info/SOURCES.txt` & `yamcs_pymdb-1.0.8/src/yamcs_pymdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

