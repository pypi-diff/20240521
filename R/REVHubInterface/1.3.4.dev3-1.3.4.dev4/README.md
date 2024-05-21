# Comparing `tmp/revhubinterface-1.3.4.dev3.tar.gz` & `tmp/revhubinterface-1.3.4.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revhubinterface-1.3.4.dev3.tar", last modified: Tue May 21 02:32:34 2024, max compression
+gzip compressed data, was "revhubinterface-1.3.4.dev4.tar", last modified: Tue May 21 02:45:41 2024, max compression
```

## Comparing `revhubinterface-1.3.4.dev3.tar` & `revhubinterface-1.3.4.dev4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:32:34.956588 revhubinterface-1.3.4.dev3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:32:34.948588 revhubinterface-1.3.4.dev3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:32:34.952588 revhubinterface-1.3.4.dev3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/.github/workflows/flatpak.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/.github/workflows/pyinstaller.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-21 02:32:34.956588 revhubinterface-1.3.4.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:32:34.956588 revhubinterface-1.3.4.dev3/REVHubInterface/
--rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface/REV2mSensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface/REVADC.py
--rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface/REVColorSensorV3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface/REVComPorts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface/REVDIO.py
--rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface/REVI2C.py
--rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface/REVModule.py
--rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface/REVMotor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface/REVServo.py
--rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface/REVcomm.py
--rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface/REVmessages.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61395 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-21 02:32:34.000000 revhubinterface-1.3.4.dev3/REVHubInterface/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:32:34.956588 revhubinterface-1.3.4.dev3/REVHubInterface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-21 02:32:34.000000 revhubinterface-1.3.4.dev3/REVHubInterface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-21 02:32:34.000000 revhubinterface-1.3.4.dev3/REVHubInterface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 02:32:34.000000 revhubinterface-1.3.4.dev3/REVHubInterface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-21 02:32:34.000000 revhubinterface-1.3.4.dev3/REVHubInterface.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 02:32:34.000000 revhubinterface-1.3.4.dev3/REVHubInterface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 02:32:34.000000 revhubinterface-1.3.4.dev3/REVHubInterface.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/REVHubInterface.spec
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:32:34.956588 revhubinterface-1.3.4.dev3/flatpak/
--rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/flatpak/flatpak-pip-generator
--rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/flatpak/org.unofficialrevport.REVHubInterface.desktop
--rw-r--r--   0 runner    (1001) docker     (127)     2593 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/flatpak/org.unofficialrevport.REVHubInterface.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/flatpak/python3-requirements.json
--rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/org.unofficialrevport.REVHubInterface.Devel.svg
--rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/org.unofficialrevport.REVHubInterface.Source.svg
--rw-r--r--   0 runner    (1001) docker     (127)    99970 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/org.unofficialrevport.REVHubInterface.icns
--rw-r--r--   0 runner    (1001) docker     (127)    33388 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/org.unofficialrevport.REVHubInterface.ico
--rw-r--r--   0 runner    (1001) docker     (127)     4600 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/org.unofficialrevport.REVHubInterface.metainfo.xml
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/org.unofficialrevport.REVHubInterface.svg
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/pyinstaller-build-reqs.txt
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 02:32:30.000000 revhubinterface-1.3.4.dev3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 02:32:34.956588 revhubinterface-1.3.4.dev3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:41.322526 revhubinterface-1.3.4.dev4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:41.314526 revhubinterface-1.3.4.dev4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:41.318526 revhubinterface-1.3.4.dev4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      543 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/.github/workflows/flatpak.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/.github/workflows/pyinstaller.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-21 02:45:41.322526 revhubinterface-1.3.4.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5835 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:41.318526 revhubinterface-1.3.4.dev4/REVHubInterface/
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REV2mSensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVADC.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5165 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVColorSensorV3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVComPorts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2552 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVDIO.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15925 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVI2C.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4757 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVModule.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11713 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVMotor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVServo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16892 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVcomm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73523 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/REVmessages.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61395 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:41.322526 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6167 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 02:45:41.000000 revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)       40 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1887 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/REVHubInterface.spec
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 02:45:41.322526 revhubinterface-1.3.4.dev4/flatpak/
+-rw-r--r--   0 runner    (1001) docker     (127)    17481 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/flatpak/flatpak-pip-generator
+-rwxr-xr-x   0 runner    (1001) docker     (127)      174 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/flatpak/org.unofficialrevport.REVHubInterface.desktop
+-rw-r--r--   0 runner    (1001) docker     (127)     2482 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/flatpak/org.unofficialrevport.REVHubInterface.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3885 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/flatpak/python3-requirements.json
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.Devel.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   384626 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.Source.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    99970 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.icns
+-rw-r--r--   0 runner    (1001) docker     (127)    33388 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.metainfo.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.svg
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/pyinstaller-build-reqs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-21 02:45:36.000000 revhubinterface-1.3.4.dev4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 02:45:41.322526 revhubinterface-1.3.4.dev4/setup.cfg
```

### Comparing `revhubinterface-1.3.4.dev3/.github/workflows/flatpak.yml` & `revhubinterface-1.3.4.dev4/.github/workflows/flatpak.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/.github/workflows/pyinstaller.yml` & `revhubinterface-1.3.4.dev4/.github/workflows/pyinstaller.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/.github/workflows/python-publish.yml` & `revhubinterface-1.3.4.dev4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/LICENSE.txt` & `revhubinterface-1.3.4.dev4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/PKG-INFO` & `revhubinterface-1.3.4.dev4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.4.dev3
+Version: 1.3.4.dev4
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.4.dev3/README.md` & `revhubinterface-1.3.4.dev4/README.md`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface/REV2mSensor.py` & `revhubinterface-1.3.4.dev4/REVHubInterface/REV2mSensor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface/REVADC.py` & `revhubinterface-1.3.4.dev4/REVHubInterface/REVADC.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface/REVColorSensorV3.py` & `revhubinterface-1.3.4.dev4/REVHubInterface/REVColorSensorV3.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface/REVComPorts.py` & `revhubinterface-1.3.4.dev4/REVHubInterface/REVComPorts.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface/REVDIO.py` & `revhubinterface-1.3.4.dev4/REVHubInterface/REVDIO.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface/REVI2C.py` & `revhubinterface-1.3.4.dev4/REVHubInterface/REVI2C.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface/REVModule.py` & `revhubinterface-1.3.4.dev4/REVHubInterface/REVModule.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface/REVMotor.py` & `revhubinterface-1.3.4.dev4/REVHubInterface/REVMotor.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface/REVServo.py` & `revhubinterface-1.3.4.dev4/REVHubInterface/REVServo.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface/REVcomm.py` & `revhubinterface-1.3.4.dev4/REVHubInterface/REVcomm.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface/REVmessages.py` & `revhubinterface-1.3.4.dev4/REVHubInterface/REVmessages.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface/__main__.py` & `revhubinterface-1.3.4.dev4/REVHubInterface/__main__.py`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface.egg-info/PKG-INFO` & `revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: REVHubInterface
-Version: 1.3.4.dev3
+Version: 1.3.4.dev4
 Summary: GUI program for manual control of REV Robotics Expansion Hub from a PC. Unofficial "Community Edition". 
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pyft232==0.12
 Requires-Dist: pyserial==3.5
 Requires-Dist: sv-ttk==2.6.0
```

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface.egg-info/SOURCES.txt` & `revhubinterface-1.3.4.dev4/REVHubInterface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/REVHubInterface.spec` & `revhubinterface-1.3.4.dev4/REVHubInterface.spec`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/flatpak/flatpak-pip-generator` & `revhubinterface-1.3.4.dev4/flatpak/flatpak-pip-generator`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/flatpak/org.unofficialrevport.REVHubInterface.yml` & `revhubinterface-1.3.4.dev4/flatpak/org.unofficialrevport.REVHubInterface.yml`

 * *Files 9% similar despite different names*

```diff
@@ -60,11 +60,10 @@
       - python -m setuptools_scm --force-write-version-files
       - pip3 install --verbose --exists-action=i --no-index --find-links="file://${PWD}" --prefix=${FLATPAK_DEST} . --no-build-isolation
       - install -Dm755 REVHubInterface.sh /app/bin/REVHubInterface.sh
       - install -Dm644 -t /app/share/applications flatpak/org.unofficialrevport.REVHubInterface.desktop
       - install -Dm644 -t /app/share/icons/hicolor/scalable/apps org.unofficialrevport.REVHubInterface.svg
       - install -Dm644 -t /app/share/metainfo org.unofficialrevport.REVHubInterface.metainfo.xml
     sources:
-      - type: git
-        url: https://github.com/unofficial-rev-port/REVHubInterface.git
-        commit: 1f759c2868fee59824def38c2946077fa29557c3
+      - type: dir
+        path: ../
```

### Comparing `revhubinterface-1.3.4.dev3/flatpak/python3-requirements.json` & `revhubinterface-1.3.4.dev4/flatpak/python3-requirements.json`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/org.unofficialrevport.REVHubInterface.Devel.svg` & `revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.Devel.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/org.unofficialrevport.REVHubInterface.Source.svg` & `revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.Source.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/org.unofficialrevport.REVHubInterface.icns` & `revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.icns`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/org.unofficialrevport.REVHubInterface.ico` & `revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.ico`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/org.unofficialrevport.REVHubInterface.metainfo.xml` & `revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.metainfo.xml`

 * *Files 5% similar despite different names*

#### Comparing `revhubinterface-1.3.4.dev3/org.unofficialrevport.REVHubInterface.metainfo.xml` & `revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.metainfo.xml`

```diff
@@ -47,35 +47,46 @@
     </screenshot>
     <screenshot>
       <caption>Controlling GPIO ports</caption>
       <image type="source" width="1382" height="1590">https://unofficialrevport.org/revhubinterface/gpiocontrol.png</image>
     </screenshot>
   </screenshots>
   <releases>
-    <release version="1.3.2" date="2024-06-10">
+    <release version="1.3.3" date="2024-05-20">
+      <url type="details">https://github.com/unofficial-rev-port/REVHubInterface/releases/tag/v1.3.3</url>
+      <description>
+        <p>Add Mac DMGs and app icon</p>
+        <ul>
+          <li>Added DMG files compiled for Mac</li>
+          <li>Added app icon</li>
+          <li>Embedded version number into app</li>
+        </ul>
+      </description>
+    </release>
+    <release version="1.3.2" date="2024-05-10">
       <url type="details">https://github.com/unofficial-rev-port/REVHubInterface/releases/tag/v1.3.2</url>
       <description>
         <p>Urgent hotfix release</p>
         <ul>
           <li>Fixed critical bug preventing the main update loop from running, preventing all communication</li>
           <li>Also changed E-STOP button to be red</li>
         </ul>
       </description>
     </release>
-    <release version="1.3.1" date="2024-06-07">
+    <release version="1.3.1" date="2024-05-07">
       <url type="details">https://github.com/unofficial-rev-port/REVHubInterface/releases/tag/v1.3.1</url>
       <description>
         <p>First release with binaries</p>
         <ul>
           <li>Added Pyinstaller and PyPi publishing</li>
           <li>Temporarily disabled firmware flashing</li>
         </ul>
       </description>
     </release>
-    <release version="1.3.0" date="2024-06-07">
+    <release version="1.3.0" date="2024-05-07">
       <url type="details">https://github.com/unofficial-rev-port/REVHubInterface/releases/tag/v1.3.0</url>
       <description>
         <p>First release!</p>
         <ul>
           <li>Ported original to Python 3</li>
           <li>Improved performance significantly</li>
         </ul>
```

### Comparing `revhubinterface-1.3.4.dev3/org.unofficialrevport.REVHubInterface.svg` & `revhubinterface-1.3.4.dev4/org.unofficialrevport.REVHubInterface.svg`

 * *Files identical despite different names*

### Comparing `revhubinterface-1.3.4.dev3/pyproject.toml` & `revhubinterface-1.3.4.dev4/pyproject.toml`

 * *Files identical despite different names*

