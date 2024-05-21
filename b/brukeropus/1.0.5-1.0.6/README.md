# Comparing `tmp/brukeropus-1.0.5.tar.gz` & `tmp/brukeropus-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brukeropus-1.0.5.tar", last modified: Mon May 13 16:56:20 2024, max compression
+gzip compressed data, was "brukeropus-1.0.6.tar", last modified: Tue May 21 14:10:14 2024, max compression
```

## Comparing `brukeropus-1.0.5.tar` & `brukeropus-1.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-13 16:56:20.617534 brukeropus-1.0.5/
--rw-rw-rw-   0        0        0     1087 2024-02-29 18:02:08.000000 brukeropus-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     5274 2024-05-13 16:56:20.617534 brukeropus-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     4523 2024-05-03 14:26:32.000000 brukeropus-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-13 16:56:20.586363 brukeropus-1.0.5/brukeropus/
--rw-rw-rw-   0        0        0     2581 2024-05-03 13:47:15.000000 brukeropus-1.0.5/brukeropus/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:56:20.601990 brukeropus-1.0.5/brukeropus/control/
--rw-rw-rw-   0        0        0     1746 2024-04-24 01:13:04.000000 brukeropus-1.0.5/brukeropus/control/__init__.py
--rw-rw-rw-   0        0        0     9678 2024-04-23 16:48:27.000000 brukeropus-1.0.5/brukeropus/control/dde.py
--rw-rw-rw-   0        0        0    11639 2024-04-24 00:59:48.000000 brukeropus-1.0.5/brukeropus/control/opus.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:56:20.617534 brukeropus-1.0.5/brukeropus/file/
--rw-rw-rw-   0        0        0    17333 2024-04-23 18:20:14.000000 brukeropus-1.0.5/brukeropus/file/__init__.py
--rw-rw-rw-   0        0        0     9467 2024-05-11 03:08:24.000000 brukeropus-1.0.5/brukeropus/file/constants.py
--rw-rw-rw-   0        0        0    26469 2024-05-13 16:22:48.000000 brukeropus-1.0.5/brukeropus/file/file.py
--rw-rw-rw-   0        0        0    13123 2024-05-11 02:12:49.000000 brukeropus-1.0.5/brukeropus/file/parser.py
--rw-rw-rw-   0        0        0    10049 2024-05-13 12:38:12.000000 brukeropus-1.0.5/brukeropus/file/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-13 16:56:20.617534 brukeropus-1.0.5/brukeropus.egg-info/
--rw-rw-rw-   0        0        0     5274 2024-05-13 16:56:20.000000 brukeropus-1.0.5/brukeropus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      440 2024-05-13 16:56:20.000000 brukeropus-1.0.5/brukeropus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-13 16:56:20.000000 brukeropus-1.0.5/brukeropus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2024-05-13 16:56:20.000000 brukeropus-1.0.5/brukeropus.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-13 16:56:20.000000 brukeropus-1.0.5/brukeropus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      816 2024-05-13 16:53:58.000000 brukeropus-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-13 16:56:20.617534 brukeropus-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 14:10:14.996617 brukeropus-1.0.6/
+-rw-rw-rw-   0        0        0     1087 2024-02-29 18:02:08.000000 brukeropus-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     5274 2024-05-21 14:10:14.996617 brukeropus-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4523 2024-05-03 14:26:32.000000 brukeropus-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 14:10:14.914381 brukeropus-1.0.6/brukeropus/
+-rw-rw-rw-   0        0        0     2612 2024-05-21 13:56:11.000000 brukeropus-1.0.6/brukeropus/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:10:14.945874 brukeropus-1.0.6/brukeropus/control/
+-rw-rw-rw-   0        0        0     1746 2024-04-24 01:13:04.000000 brukeropus-1.0.6/brukeropus/control/__init__.py
+-rw-rw-rw-   0        0        0     9678 2024-04-23 16:48:27.000000 brukeropus-1.0.6/brukeropus/control/dde.py
+-rw-rw-rw-   0        0        0    11639 2024-04-24 00:59:48.000000 brukeropus-1.0.6/brukeropus/control/opus.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:10:14.996617 brukeropus-1.0.6/brukeropus/file/
+-rw-rw-rw-   0        0        0    17333 2024-04-23 18:20:14.000000 brukeropus-1.0.6/brukeropus/file/__init__.py
+-rw-rw-rw-   0        0        0     9471 2024-05-21 13:54:25.000000 brukeropus-1.0.6/brukeropus/file/constants.py
+-rw-rw-rw-   0        0        0    26469 2024-05-13 16:57:34.000000 brukeropus-1.0.6/brukeropus/file/file.py
+-rw-rw-rw-   0        0        0    13123 2024-05-11 02:12:49.000000 brukeropus-1.0.6/brukeropus/file/parser.py
+-rw-rw-rw-   0        0        0    10049 2024-05-13 12:38:12.000000 brukeropus-1.0.6/brukeropus/file/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:10:14.996617 brukeropus-1.0.6/brukeropus.egg-info/
+-rw-rw-rw-   0        0        0     5274 2024-05-21 14:10:14.000000 brukeropus-1.0.6/brukeropus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      440 2024-05-21 14:10:14.000000 brukeropus-1.0.6/brukeropus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:10:14.000000 brukeropus-1.0.6/brukeropus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2024-05-21 14:10:14.000000 brukeropus-1.0.6/brukeropus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-21 14:10:14.000000 brukeropus-1.0.6/brukeropus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      816 2024-05-21 14:08:02.000000 brukeropus-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:10:14.996617 brukeropus-1.0.6/setup.cfg
```

### Comparing `brukeropus-1.0.5/LICENSE` & `brukeropus-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.5/PKG-INFO` & `brukeropus-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brukeropus
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python package for communicating with Bruker OPUS spectroscopy software and reading its binary file format.
 Author-email: Josh Duran <josh.m.duran@gmail.com>
 Project-URL: Homepage, https://github.com/joshduran/brukeropus
 Project-URL: Issues, https://github.com/joshduran/brukeropus/issues
 Project-URL: Documentation, https://joshduran.github.io/brukeropus/brukeropus.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `brukeropus-1.0.5/README.md` & `brukeropus-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.5/brukeropus/__init__.py` & `brukeropus-1.0.6/brukeropus/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,8 +57,12 @@
 plt.legend()
 plt.show()
 ```
 More detailed documentation on the control submodule can be found in `brukeropus.control`.
 '''
 
 from brukeropus.file import OPUSFile, read_opus, find_opus_files
-from brukeropus.control import Opus
+
+try:
+    from brukeropus.control import Opus
+except:
+    pass
```

### Comparing `brukeropus-1.0.5/brukeropus/control/__init__.py` & `brukeropus-1.0.6/brukeropus/control/__init__.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.5/brukeropus/control/dde.py` & `brukeropus-1.0.6/brukeropus/control/dde.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.5/brukeropus/control/opus.py` & `brukeropus-1.0.6/brukeropus/control/opus.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.5/brukeropus/file/__init__.py` & `brukeropus-1.0.6/brukeropus/file/__init__.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.5/brukeropus/file/constants.py` & `brukeropus-1.0.6/brukeropus/file/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import numpy as np
+
+
 PARAM_LABELS = {
     'ACC': 'Accessory',
     'ABP': 'Absolute Peak Pos in Laser*2',
     'ADC': 'External Analog Signals',
     'ADT': 'Additional Data Treatment',
     'AG2': 'Actual Signal Gain Channel 2',
     'AN1': 'Analog Signal 1',
@@ -246,15 +248,15 @@
     {'key': 'mxy', 'fmt': 'd', 'dtype': np.float64},
     {'key': 'csf', 'fmt': 'd', 'dtype': np.float64},
     {'key': 'pka', 'fmt': 'd', 'dtype': np.float64},
     {'key': 'pra', 'fmt': 'd', 'dtype': np.float64},
     {'key': 'pkl', 'fmt': 'l', 'dtype': np.int32},
     {'key': 'prl', 'fmt': 'l', 'dtype': np.int32},
     {'key': 'srt', 'fmt': 'd', 'dtype': np.float64},
-    {'key': 'tim', 'fmt': 'd', 'dtype': np.float64},
+    {'key': 'ert', 'fmt': 'd', 'dtype': np.float64},
 ]
 
 
 Y_LABELS = {
     'sm': 'Sample Spectrum',
     'rf': 'Reference Spectrum',
     'igsm': 'Sample Interferogram',
```

### Comparing `brukeropus-1.0.5/brukeropus/file/file.py` & `brukeropus-1.0.6/brukeropus/file/file.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.5/brukeropus/file/parser.py` & `brukeropus-1.0.6/brukeropus/file/parser.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.5/brukeropus/file/utils.py` & `brukeropus-1.0.6/brukeropus/file/utils.py`

 * *Files identical despite different names*

### Comparing `brukeropus-1.0.5/brukeropus.egg-info/PKG-INFO` & `brukeropus-1.0.6/brukeropus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brukeropus
-Version: 1.0.5
+Version: 1.0.6
 Summary: A python package for communicating with Bruker OPUS spectroscopy software and reading its binary file format.
 Author-email: Josh Duran <josh.m.duran@gmail.com>
 Project-URL: Homepage, https://github.com/joshduran/brukeropus
 Project-URL: Issues, https://github.com/joshduran/brukeropus/issues
 Project-URL: Documentation, https://joshduran.github.io/brukeropus/brukeropus.html
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `brukeropus-1.0.5/pyproject.toml` & `brukeropus-1.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "brukeropus"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Josh Duran", email="josh.m.duran@gmail.com" },
 ]
 description = "A python package for communicating with Bruker OPUS spectroscopy software and reading its binary file format."
 readme = "README.md"
 dependencies = ["numpy"]
 requires-python = ">=3.6"
```

