# Comparing `tmp/mriqa-0.2.14.tar.gz` & `tmp/mriqa-0.2.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mriqa-0.2.14.tar", last modified: Mon May 20 21:39:08 2024, max compression
+gzip compressed data, was "mriqa-0.2.15.tar", last modified: Tue May 21 00:04:15 2024, max compression
```

## Comparing `mriqa-0.2.14.tar` & `mriqa-0.2.15.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-05-20 21:39:08.614713 mriqa-0.2.14/
--rw-r--r--   0 ron        (501) staff       (20)     2637 2024-05-20 21:39:08.614456 mriqa-0.2.14/PKG-INFO
--rw-r--r--   0 ron        (501) staff       (20)     1425 2024-04-08 19:56:00.000000 mriqa-0.2.14/README.md
-drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-05-20 21:39:08.549143 mriqa-0.2.14/mriqa/
--rw-r--r--   0 ron        (501) staff       (20)       34 2024-04-01 11:37:15.000000 mriqa-0.2.14/mriqa/__init__.py
--rw-r--r--   0 ron        (501) staff       (20)   104042 2024-04-08 19:56:00.000000 mriqa-0.2.14/mriqa/dcmio.py
--rw-r--r--   0 ron        (501) staff       (20)    43877 2024-04-08 19:56:00.000000 mriqa-0.2.14/mriqa/fbirn.py
--rw-r--r--   0 ron        (501) staff       (20)     5251 2024-04-01 11:37:15.000000 mriqa-0.2.14/mriqa/ghosting.py
--rw-r--r--   0 ron        (501) staff       (20)     5395 2024-04-01 11:37:15.000000 mriqa-0.2.14/mriqa/mfxarray.py
--rw-r--r--   0 ron        (501) staff       (20)    30659 2024-04-08 19:56:00.000000 mriqa-0.2.14/mriqa/nistadc.py
--rw-r--r--   0 ron        (501) staff       (20)    24884 2024-04-22 14:35:03.000000 mriqa-0.2.14/mriqa/phantoms.py
-drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-05-20 21:39:08.584975 mriqa-0.2.14/mriqa/reports/
--rw-r--r--   0 ron        (501) staff       (20)      993 2024-04-01 11:37:15.000000 mriqa-0.2.14/mriqa/reports/__init__.py
--rw-r--r--   0 ron        (501) staff       (20)    20047 2024-04-01 11:37:15.000000 mriqa-0.2.14/mriqa/reports/diffusion.py
--rw-r--r--   0 ron        (501) staff       (20)    10144 2024-04-08 19:56:00.000000 mriqa-0.2.14/mriqa/reports/flow.py
--rw-r--r--   0 ron        (501) staff       (20)    28059 2024-04-08 19:56:00.000000 mriqa-0.2.14/mriqa/reports/geometry.py
--rw-r--r--   0 ron        (501) staff       (20)     7015 2024-04-08 19:56:00.000000 mriqa-0.2.14/mriqa/reports/ghosting.py
--rw-r--r--   0 ron        (501) staff       (20)     7919 2024-04-01 11:37:15.000000 mriqa-0.2.14/mriqa/reports/noras.py
--rw-r--r--   0 ron        (501) staff       (20)      148 2024-04-01 11:37:15.000000 mriqa-0.2.14/mriqa/reports/reports.py
--rw-r--r--   0 ron        (501) staff       (20)    35723 2024-04-08 19:56:00.000000 mriqa-0.2.14/mriqa/reports/resolution.py
--rw-r--r--   0 ron        (501) staff       (20)    12128 2024-04-08 19:56:00.000000 mriqa-0.2.14/mriqa/reports/slice.py
--rw-r--r--   0 ron        (501) staff       (20)    32243 2024-04-08 19:56:00.000000 mriqa-0.2.14/mriqa/reports/snr.py
--rw-r--r--   0 ron        (501) staff       (20)    12243 2024-04-01 11:37:15.000000 mriqa-0.2.14/mriqa/reports/spectroscopy.py
--rw-r--r--   0 ron        (501) staff       (20)    13646 2024-04-01 11:37:15.000000 mriqa-0.2.14/mriqa/reports/stability.py
--rw-r--r--   0 ron        (501) staff       (20)     7164 2024-04-08 19:56:00.000000 mriqa-0.2.14/mriqa/reports/uniformity.py
--rw-r--r--   0 ron        (501) staff       (20)    46632 2024-04-08 19:56:00.000000 mriqa-0.2.14/mriqa/tools.py
--rw-r--r--   0 ron        (501) staff       (20)       23 2024-04-08 19:56:00.000000 mriqa-0.2.14/mriqa/version.py
-drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-05-20 21:39:08.587048 mriqa-0.2.14/mriqa/xmlqa/
--rw-r--r--   0 ron        (501) staff       (20)        0 2024-04-01 11:37:15.000000 mriqa-0.2.14/mriqa/xmlqa/__init__.py
--rw-r--r--   0 ron        (501) staff       (20)    22233 2024-04-08 19:56:00.000000 mriqa-0.2.14/mriqa/xmlqa/coilqa.py
-drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-05-20 21:39:08.613440 mriqa-0.2.14/mriqa.egg-info/
--rw-r--r--   0 ron        (501) staff       (20)     2637 2024-05-20 21:39:08.000000 mriqa-0.2.14/mriqa.egg-info/PKG-INFO
--rw-r--r--   0 ron        (501) staff       (20)      834 2024-05-20 21:39:08.000000 mriqa-0.2.14/mriqa.egg-info/SOURCES.txt
--rw-r--r--   0 ron        (501) staff       (20)        1 2024-05-20 21:39:08.000000 mriqa-0.2.14/mriqa.egg-info/dependency_links.txt
--rw-r--r--   0 ron        (501) staff       (20)      164 2024-05-20 21:39:08.000000 mriqa-0.2.14/mriqa.egg-info/requires.txt
--rw-r--r--   0 ron        (501) staff       (20)        6 2024-05-20 21:39:08.000000 mriqa-0.2.14/mriqa.egg-info/top_level.txt
--rw-r--r--   0 ron        (501) staff       (20)       79 2024-05-20 21:39:08.615651 mriqa-0.2.14/setup.cfg
--rw-r--r--   0 ron        (501) staff       (20)     1936 2024-05-20 21:37:45.000000 mriqa-0.2.14/setup.py
-drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-05-20 21:39:08.611726 mriqa-0.2.14/tests/
--rw-r--r--   0 ron        (501) staff       (20)    73997 2024-04-08 19:56:00.000000 mriqa-0.2.14/tests/test_dcmio.py
--rw-r--r--   0 ron        (501) staff       (20)    17106 2024-04-08 19:56:00.000000 mriqa-0.2.14/tests/test_fmriqa.py
--rw-r--r--   0 ron        (501) staff       (20)      841 2024-04-08 19:56:00.000000 mriqa-0.2.14/tests/test_ghosting.py
--rw-r--r--   0 ron        (501) staff       (20)     3537 2024-04-08 19:56:00.000000 mriqa-0.2.14/tests/test_phantoms.py
--rw-r--r--   0 ron        (501) staff       (20)     3438 2024-04-08 19:56:00.000000 mriqa-0.2.14/tests/test_reports_snr.py
--rw-r--r--   0 ron        (501) staff       (20)     6354 2024-04-08 19:56:00.000000 mriqa-0.2.14/tests/test_tools.py
+drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-05-21 00:04:15.404345 mriqa-0.2.15/
+-rw-r--r--   0 ron        (501) staff       (20)     2637 2024-05-21 00:04:15.403792 mriqa-0.2.15/PKG-INFO
+-rw-r--r--   0 ron        (501) staff       (20)     1425 2024-05-20 23:31:18.000000 mriqa-0.2.15/README.md
+drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-05-21 00:04:15.348056 mriqa-0.2.15/mriqa/
+-rw-r--r--   0 ron        (501) staff       (20)       34 2024-04-01 11:37:15.000000 mriqa-0.2.15/mriqa/__init__.py
+-rw-r--r--   0 ron        (501) staff       (20)   104042 2024-05-20 23:31:18.000000 mriqa-0.2.15/mriqa/dcmio.py
+-rw-r--r--   0 ron        (501) staff       (20)    43877 2024-05-20 23:31:18.000000 mriqa-0.2.15/mriqa/fbirn.py
+-rw-r--r--   0 ron        (501) staff       (20)     5251 2024-04-01 11:37:15.000000 mriqa-0.2.15/mriqa/ghosting.py
+-rw-r--r--   0 ron        (501) staff       (20)     5395 2024-04-01 11:37:15.000000 mriqa-0.2.15/mriqa/mfxarray.py
+-rw-r--r--   0 ron        (501) staff       (20)    30659 2024-05-20 23:31:18.000000 mriqa-0.2.15/mriqa/nistadc.py
+-rw-r--r--   0 ron        (501) staff       (20)    24884 2024-05-20 23:31:18.000000 mriqa-0.2.15/mriqa/phantoms.py
+drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-05-21 00:04:15.385225 mriqa-0.2.15/mriqa/reports/
+-rw-r--r--   0 ron        (501) staff       (20)      993 2024-04-01 11:37:15.000000 mriqa-0.2.15/mriqa/reports/__init__.py
+-rw-r--r--   0 ron        (501) staff       (20)    20047 2024-04-01 11:37:15.000000 mriqa-0.2.15/mriqa/reports/diffusion.py
+-rw-r--r--   0 ron        (501) staff       (20)    10144 2024-05-20 23:31:18.000000 mriqa-0.2.15/mriqa/reports/flow.py
+-rw-r--r--   0 ron        (501) staff       (20)    28059 2024-05-20 23:31:18.000000 mriqa-0.2.15/mriqa/reports/geometry.py
+-rw-r--r--   0 ron        (501) staff       (20)     7015 2024-05-20 23:31:18.000000 mriqa-0.2.15/mriqa/reports/ghosting.py
+-rw-r--r--   0 ron        (501) staff       (20)     7919 2024-04-01 11:37:15.000000 mriqa-0.2.15/mriqa/reports/noras.py
+-rw-r--r--   0 ron        (501) staff       (20)      148 2024-04-01 11:37:15.000000 mriqa-0.2.15/mriqa/reports/reports.py
+-rw-r--r--   0 ron        (501) staff       (20)    35723 2024-05-20 23:31:18.000000 mriqa-0.2.15/mriqa/reports/resolution.py
+-rw-r--r--   0 ron        (501) staff       (20)    12128 2024-05-20 23:31:18.000000 mriqa-0.2.15/mriqa/reports/slice.py
+-rw-r--r--   0 ron        (501) staff       (20)    32243 2024-04-08 19:56:00.000000 mriqa-0.2.15/mriqa/reports/snr.py
+-rw-r--r--   0 ron        (501) staff       (20)    12243 2024-04-01 11:37:15.000000 mriqa-0.2.15/mriqa/reports/spectroscopy.py
+-rw-r--r--   0 ron        (501) staff       (20)    13646 2024-04-01 11:37:15.000000 mriqa-0.2.15/mriqa/reports/stability.py
+-rw-r--r--   0 ron        (501) staff       (20)     7164 2024-04-08 19:56:00.000000 mriqa-0.2.15/mriqa/reports/uniformity.py
+-rw-r--r--   0 ron        (501) staff       (20)    46632 2024-05-20 23:31:18.000000 mriqa-0.2.15/mriqa/tools.py
+-rw-r--r--   0 ron        (501) staff       (20)       23 2024-05-20 23:31:18.000000 mriqa-0.2.15/mriqa/version.py
+drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-05-21 00:04:15.387278 mriqa-0.2.15/mriqa/xmlqa/
+-rw-r--r--   0 ron        (501) staff       (20)        0 2024-04-01 11:37:15.000000 mriqa-0.2.15/mriqa/xmlqa/__init__.py
+-rw-r--r--   0 ron        (501) staff       (20)    22233 2024-04-08 19:56:00.000000 mriqa-0.2.15/mriqa/xmlqa/coilqa.py
+drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-05-21 00:04:15.400640 mriqa-0.2.15/mriqa.egg-info/
+-rw-r--r--   0 ron        (501) staff       (20)     2637 2024-05-21 00:04:15.000000 mriqa-0.2.15/mriqa.egg-info/PKG-INFO
+-rw-r--r--   0 ron        (501) staff       (20)      834 2024-05-21 00:04:15.000000 mriqa-0.2.15/mriqa.egg-info/SOURCES.txt
+-rw-r--r--   0 ron        (501) staff       (20)        1 2024-05-21 00:04:15.000000 mriqa-0.2.15/mriqa.egg-info/dependency_links.txt
+-rw-r--r--   0 ron        (501) staff       (20)      164 2024-05-21 00:04:15.000000 mriqa-0.2.15/mriqa.egg-info/requires.txt
+-rw-r--r--   0 ron        (501) staff       (20)        6 2024-05-21 00:04:15.000000 mriqa-0.2.15/mriqa.egg-info/top_level.txt
+-rw-r--r--   0 ron        (501) staff       (20)       79 2024-05-21 00:04:15.405476 mriqa-0.2.15/setup.cfg
+-rw-r--r--   0 ron        (501) staff       (20)     1936 2024-05-20 23:31:18.000000 mriqa-0.2.15/setup.py
+drwxr-xr-x   0 ron        (501) staff       (20)        0 2024-05-21 00:04:15.396469 mriqa-0.2.15/tests/
+-rw-r--r--   0 ron        (501) staff       (20)    73997 2024-05-20 23:31:18.000000 mriqa-0.2.15/tests/test_dcmio.py
+-rw-r--r--   0 ron        (501) staff       (20)    17106 2024-05-20 23:31:18.000000 mriqa-0.2.15/tests/test_fmriqa.py
+-rw-r--r--   0 ron        (501) staff       (20)      841 2024-05-20 23:31:18.000000 mriqa-0.2.15/tests/test_ghosting.py
+-rw-r--r--   0 ron        (501) staff       (20)     3537 2024-05-20 23:31:18.000000 mriqa-0.2.15/tests/test_phantoms.py
+-rw-r--r--   0 ron        (501) staff       (20)     3438 2024-05-20 23:31:18.000000 mriqa-0.2.15/tests/test_reports_snr.py
+-rw-r--r--   0 ron        (501) staff       (20)     6354 2024-05-20 23:31:18.000000 mriqa-0.2.15/tests/test_tools.py
```

### Comparing `mriqa-0.2.14/PKG-INFO` & `mriqa-0.2.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mriqa
-Version: 0.2.14
+Version: 0.2.15
 Summary: Tools for MRI QA
 Home-page: https://bitbucket.org/rtrhd/mriqa.git
-Download-URL: https://bitbucket.org/rtrhd/mriqa/get/v0.2.14.zip
+Download-URL: https://bitbucket.org/rtrhd/mriqa/get/v0.2.15.zip
 Author: Ronald Hartley-Davies
 Author-email: R.Hartley-Davies@physics.org
 License: MIT
 Keywords: mri qa phantom
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
```

### Comparing `mriqa-0.2.14/README.md` & `mriqa-0.2.15/README.md`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/dcmio.py` & `mriqa-0.2.15/mriqa/dcmio.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/fbirn.py` & `mriqa-0.2.15/mriqa/fbirn.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/ghosting.py` & `mriqa-0.2.15/mriqa/ghosting.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/mfxarray.py` & `mriqa-0.2.15/mriqa/mfxarray.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/nistadc.py` & `mriqa-0.2.15/mriqa/nistadc.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/phantoms.py` & `mriqa-0.2.15/mriqa/phantoms.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/reports/__init__.py` & `mriqa-0.2.15/mriqa/reports/__init__.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/reports/diffusion.py` & `mriqa-0.2.15/mriqa/reports/diffusion.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/reports/flow.py` & `mriqa-0.2.15/mriqa/reports/flow.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/reports/geometry.py` & `mriqa-0.2.15/mriqa/reports/geometry.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/reports/ghosting.py` & `mriqa-0.2.15/mriqa/reports/ghosting.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/reports/noras.py` & `mriqa-0.2.15/mriqa/reports/noras.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/reports/resolution.py` & `mriqa-0.2.15/mriqa/reports/resolution.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/reports/slice.py` & `mriqa-0.2.15/mriqa/reports/slice.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/reports/snr.py` & `mriqa-0.2.15/mriqa/reports/snr.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/reports/spectroscopy.py` & `mriqa-0.2.15/mriqa/reports/spectroscopy.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/reports/stability.py` & `mriqa-0.2.15/mriqa/reports/stability.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/reports/uniformity.py` & `mriqa-0.2.15/mriqa/reports/uniformity.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/tools.py` & `mriqa-0.2.15/mriqa/tools.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa/xmlqa/coilqa.py` & `mriqa-0.2.15/mriqa/xmlqa/coilqa.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/mriqa.egg-info/PKG-INFO` & `mriqa-0.2.15/mriqa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: mriqa
-Version: 0.2.14
+Version: 0.2.15
 Summary: Tools for MRI QA
 Home-page: https://bitbucket.org/rtrhd/mriqa.git
-Download-URL: https://bitbucket.org/rtrhd/mriqa/get/v0.2.14.zip
+Download-URL: https://bitbucket.org/rtrhd/mriqa/get/v0.2.15.zip
 Author: Ronald Hartley-Davies
 Author-email: R.Hartley-Davies@physics.org
 License: MIT
 Keywords: mri qa phantom
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
```

### Comparing `mriqa-0.2.14/mriqa.egg-info/SOURCES.txt` & `mriqa-0.2.15/mriqa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/setup.py` & `mriqa-0.2.15/setup.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/tests/test_dcmio.py` & `mriqa-0.2.15/tests/test_dcmio.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/tests/test_fmriqa.py` & `mriqa-0.2.15/tests/test_fmriqa.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/tests/test_ghosting.py` & `mriqa-0.2.15/tests/test_ghosting.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/tests/test_phantoms.py` & `mriqa-0.2.15/tests/test_phantoms.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/tests/test_reports_snr.py` & `mriqa-0.2.15/tests/test_reports_snr.py`

 * *Files identical despite different names*

### Comparing `mriqa-0.2.14/tests/test_tools.py` & `mriqa-0.2.15/tests/test_tools.py`

 * *Files identical despite different names*

