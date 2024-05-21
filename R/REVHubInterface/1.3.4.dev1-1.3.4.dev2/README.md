# Comparing `tmp/revhubinterface-1.3.4.dev1.tar.gz` & `tmp/revhubinterface-1.3.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.4.dev1.tar", last modified: Mon May 20 06:27:45 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.4.dev2.tar", last modified: Mon May 20 07:06:51 2024, max compression
```

## Comparing `revhubinterface-1.3.4.dev1.tar` & `revhubinterface-1.3.4.dev2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:45.807108 revhubinterface-1.3.4.dev1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:45.799108 revhubinterface-1.3.4.dev1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:45.803108 revhubinterface-1.3.4.dev1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-20 06:27:45.807108 revhubinterface-1.3.4.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:45.807108 revhubinterface-1.3.4.dev1/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61395 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:45.807108 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 06:27:45.000000 revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 06:27:45.807108 revhubinterface-1.3.4.dev1/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/flatpak/flatpak-pip-generator
--rwxr-xr-x   0 runner    (1001) docker     (127)      162 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/flatpak/org.unofficialrevport.REVHubInterface.desktop
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.Devel.svg
--rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.Source.svg
--rw-r--r--   0 runner    (1001) docker     (127)    99970 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.icns
--rw-r--r--   0 runner    (1001) docker     (127)    33388 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.ico
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.metainfo.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.svg
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/pyinstaller-build-reqs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 06:27:24.000000 revhubinterface-1.3.4.dev1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 06:27:45.807108 revhubinterface-1.3.4.dev1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:06:51.977563 revhubinterface-1.3.4.dev2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:06:51.965563 revhubinterface-1.3.4.dev2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:06:51.969564 revhubinterface-1.3.4.dev2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-20 07:06:51.977563 revhubinterface-1.3.4.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:06:51.973564 revhubinterface-1.3.4.dev2/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61395 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-20 07:06:51.000000 revhubinterface-1.3.4.dev2/REVHubInterface/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:06:51.977563 revhubinterface-1.3.4.dev2/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-20 07:06:51.000000 revhubinterface-1.3.4.dev2/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-20 07:06:51.000000 revhubinterface-1.3.4.dev2/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 07:06:51.000000 revhubinterface-1.3.4.dev2/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-20 07:06:51.000000 revhubinterface-1.3.4.dev2/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 07:06:51.000000 revhubinterface-1.3.4.dev2/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 07:06:51.000000 revhubinterface-1.3.4.dev2/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 07:06:51.977563 revhubinterface-1.3.4.dev2/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/flatpak/flatpak-pip-generator
+-rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/flatpak/org.unofficialrevport.REVHubInterface.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/org.unofficialrevport.REVHubInterface.Devel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/org.unofficialrevport.REVHubInterface.Source.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    99970 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/org.unofficialrevport.REVHubInterface.icns
+-rw-r--r--   0 runner    (1001) docker     (127)    33388 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/org.unofficialrevport.REVHubInterface.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/org.unofficialrevport.REVHubInterface.metainfo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/org.unofficialrevport.REVHubInterface.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/pyinstaller-build-reqs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-20 07:06:47.000000 revhubinterface-1.3.4.dev2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 07:06:51.977563 revhubinterface-1.3.4.dev2/setup.cfg
```

### Comparing `revhubinterface-1.3.4.dev1/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.4.dev2/.github/workflows/pyinstaller.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/.github/workflows/python-publish.yml` & `revhubinterface-1.3.4.dev2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/LICENSE.txt` & `revhubinterface-1.3.4.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/PKG-INFO` & `revhubinterface-1.3.4.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.4.dev1
+Version: 1.3.4.dev2
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.4.dev1/README.md` & `revhubinterface-1.3.4.dev2/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.4.dev2/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface/REVADC.py` & `revhubinterface-1.3.4.dev2/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.4.dev2/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.4.dev2/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.4.dev2/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.4.dev2/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface/REVModule.py` & `revhubinterface-1.3.4.dev2/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.4.dev2/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface/REVServo.py` & `revhubinterface-1.3.4.dev2/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.4.dev2/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.4.dev2/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface/__main__.py` & `revhubinterface-1.3.4.dev2/REVHubInterface/__main__.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.4.dev2/REVHubInterface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.4.dev1
+Version: 1.3.4.dev2
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.4.dev2/REVHubInterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/REVHubInterface.spec` & `revhubinterface-1.3.4.dev2/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.4.dev2/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.4.dev2/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/flatpak/python3-requirements.json` & `revhubinterface-1.3.4.dev2/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.Devel.svg` & `revhubinterface-1.3.4.dev2/org.unofficialrevport.REVHubInterface.Devel.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.Source.svg` & `revhubinterface-1.3.4.dev2/org.unofficialrevport.REVHubInterface.Source.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.icns` & `revhubinterface-1.3.4.dev2/org.unofficialrevport.REVHubInterface.icns`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.ico` & `revhubinterface-1.3.4.dev2/org.unofficialrevport.REVHubInterface.ico`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.metainfo.xml` & `revhubinterface-1.3.4.dev2/org.unofficialrevport.REVHubInterface.metainfo.xml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/org.unofficialrevport.REVHubInterface.svg` & `revhubinterface-1.3.4.dev2/org.unofficialrevport.REVHubInterface.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev1/pyproject.toml` & `revhubinterface-1.3.4.dev2/pyproject.toml`

 * *Files identical despite different names*

