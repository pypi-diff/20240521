# Comparing `tmp/spacetower_fds_sdk-1.0.2.tar.gz` & `tmp/spacetower_fds_sdk-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spacetower_fds_sdk-1.0.2.tar", max compression
+gzip compressed data, was "spacetower_fds_sdk-1.0.3.tar", max compression
```

## Comparing `spacetower_fds_sdk-1.0.2.tar` & `spacetower_fds_sdk-1.0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0      147 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/README.md
--rw-r--r--   0        0        0       46 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/__init__.py
--rw-r--r--   0        0        0    32653 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/client.py
--rw-r--r--   0        0        0      525 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/config.py
--rw-r--r--   0        0        0      474 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/constants.py
--rw-r--r--   0        0        0      121 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/__init__.py
--rw-r--r--   0        0        0     8204 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/_model.py
--rw-r--r--   0        0        0     2448 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/_use_case.py
--rw-r--r--   0        0        0     8962 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/actions.py
--rw-r--r--   0        0        0        0 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/determination/__init__.py
--rw-r--r--   0        0        0     5265 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/determination/configuration.py
--rw-r--r--   0        0        0     5079 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/determination/requests.py
--rw-r--r--   0        0        0    18902 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/determination/result.py
--rw-r--r--   0        0        0     3942 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/determination/use_case.py
--rw-r--r--   0        0        0     2921 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/ground_station.py
--rw-r--r--   0        0        0        0 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/maneuvers/__init__.py
--rw-r--r--   0        0        0     6069 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/maneuvers/result.py
--rw-r--r--   0        0        0     5505 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/maneuvers/strategy.py
--rw-r--r--   0        0        0     3705 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/maneuvers/use_case.py
--rw-r--r--   0        0        0     9777 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/nmea_processor.py
--rw-r--r--   0        0        0        0 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/orbit_extrapolation/__init__.py
--rw-r--r--   0        0        0    13945 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/orbit_extrapolation/ephemeris.py
--rw-r--r--   0        0        0     3886 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/orbit_extrapolation/events.py
--rw-r--r--   0        0        0    23764 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/orbit_extrapolation/requests.py
--rw-r--r--   0        0        0    17095 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/orbit_extrapolation/result.py
--rw-r--r--   0        0        0    13074 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/orbit_extrapolation/use_case.py
--rw-r--r--   0        0        0    15539 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/orbital_state.py
--rw-r--r--   0        0        0    10771 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/orbits.py
--rw-r--r--   0        0        0    12996 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/quaternion.py
--rw-r--r--   0        0        0    14728 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/roadmaps.py
--rw-r--r--   0        0        0    25353 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/spacecraft.py
--rw-r--r--   0        0        0    20842 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/telemetry.py
--rw-r--r--   0        0        0        0 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/tle_extrapolation/__init__.py
--rw-r--r--   0        0        0      868 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/tle_extrapolation/result.py
--rw-r--r--   0        0        0     1399 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/tle_extrapolation/use_case.py
--rw-r--r--   0        0        0     8294 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/models/two_line_element.py
--rw-r--r--   0        0        0        0 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/utils/__init__.py
--rw-r--r--   0        0        0     2214 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/utils/dates.py
--rw-r--r--   0        0        0     1993 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/utils/dict.py
--rw-r--r--   0        0        0      440 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/utils/enum.py
--rw-r--r--   0        0        0     2756 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/utils/frames.py
--rw-r--r--   0        0        0     1803 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/utils/geometry.py
--rw-r--r--   0        0        0      492 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/utils/log.py
--rw-r--r--   0        0        0     1077 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/utils/math.py
--rw-r--r--   0        0        0    13916 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/fds/utils/orbital_mechanics.py
--rw-r--r--   0        0        0      823 2024-05-21 16:07:39.934429 spacetower_fds_sdk-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 spacetower_fds_sdk-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0      147 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/README.md
+-rw-r--r--   0        0        0       46 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/__init__.py
+-rw-r--r--   0        0        0    32653 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/client.py
+-rw-r--r--   0        0        0      525 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/config.py
+-rw-r--r--   0        0        0      474 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/constants.py
+-rw-r--r--   0        0        0      121 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/__init__.py
+-rw-r--r--   0        0        0     8204 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/_model.py
+-rw-r--r--   0        0        0     2448 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/_use_case.py
+-rw-r--r--   0        0        0     8962 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/actions.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/determination/__init__.py
+-rw-r--r--   0        0        0     5265 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/determination/configuration.py
+-rw-r--r--   0        0        0     5079 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/determination/requests.py
+-rw-r--r--   0        0        0    18902 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/determination/result.py
+-rw-r--r--   0        0        0     3942 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/determination/use_case.py
+-rw-r--r--   0        0        0     2921 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/ground_station.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/maneuvers/__init__.py
+-rw-r--r--   0        0        0     6069 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/maneuvers/result.py
+-rw-r--r--   0        0        0     5505 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/maneuvers/strategy.py
+-rw-r--r--   0        0        0     3705 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/maneuvers/use_case.py
+-rw-r--r--   0        0        0     9777 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/nmea_processor.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/__init__.py
+-rw-r--r--   0        0        0    13945 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/ephemeris.py
+-rw-r--r--   0        0        0     3886 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/events.py
+-rw-r--r--   0        0        0    23764 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/requests.py
+-rw-r--r--   0        0        0    17095 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/result.py
+-rw-r--r--   0        0        0    13074 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/use_case.py
+-rw-r--r--   0        0        0    15539 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbital_state.py
+-rw-r--r--   0        0        0    10771 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/orbits.py
+-rw-r--r--   0        0        0    12996 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/quaternion.py
+-rw-r--r--   0        0        0    14728 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/roadmaps.py
+-rw-r--r--   0        0        0    25353 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/spacecraft.py
+-rw-r--r--   0        0        0    20842 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/telemetry.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/tle_extrapolation/__init__.py
+-rw-r--r--   0        0        0      868 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/tle_extrapolation/result.py
+-rw-r--r--   0        0        0     1399 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/tle_extrapolation/use_case.py
+-rw-r--r--   0        0        0     8294 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/models/two_line_element.py
+-rw-r--r--   0        0        0        0 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/__init__.py
+-rw-r--r--   0        0        0     2214 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/dates.py
+-rw-r--r--   0        0        0     1993 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/dict.py
+-rw-r--r--   0        0        0      440 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/enum.py
+-rw-r--r--   0        0        0     2756 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/frames.py
+-rw-r--r--   0        0        0     1803 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/geometry.py
+-rw-r--r--   0        0        0      492 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/log.py
+-rw-r--r--   0        0        0     1077 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/math.py
+-rw-r--r--   0        0        0    13916 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/fds/utils/orbital_mechanics.py
+-rw-r--r--   0        0        0      921 2024-05-21 16:29:04.673493 spacetower_fds_sdk-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      886 1970-01-01 00:00:00.000000 spacetower_fds_sdk-1.0.3/PKG-INFO
```

### Comparing `spacetower_fds_sdk-1.0.2/fds/client.py` & `spacetower_fds_sdk-1.0.3/fds/client.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/config.py` & `spacetower_fds_sdk-1.0.3/fds/config.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/_model.py` & `spacetower_fds_sdk-1.0.3/fds/models/_model.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/_use_case.py` & `spacetower_fds_sdk-1.0.3/fds/models/_use_case.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/actions.py` & `spacetower_fds_sdk-1.0.3/fds/models/actions.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/determination/configuration.py` & `spacetower_fds_sdk-1.0.3/fds/models/determination/configuration.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/determination/requests.py` & `spacetower_fds_sdk-1.0.3/fds/models/determination/requests.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/determination/result.py` & `spacetower_fds_sdk-1.0.3/fds/models/determination/result.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/determination/use_case.py` & `spacetower_fds_sdk-1.0.3/fds/models/determination/use_case.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/ground_station.py` & `spacetower_fds_sdk-1.0.3/fds/models/ground_station.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/maneuvers/result.py` & `spacetower_fds_sdk-1.0.3/fds/models/maneuvers/result.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/maneuvers/strategy.py` & `spacetower_fds_sdk-1.0.3/fds/models/maneuvers/strategy.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/maneuvers/use_case.py` & `spacetower_fds_sdk-1.0.3/fds/models/maneuvers/use_case.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/nmea_processor.py` & `spacetower_fds_sdk-1.0.3/fds/models/nmea_processor.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/orbit_extrapolation/ephemeris.py` & `spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/ephemeris.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/orbit_extrapolation/events.py` & `spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/events.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/orbit_extrapolation/requests.py` & `spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/requests.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/orbit_extrapolation/result.py` & `spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/result.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/orbit_extrapolation/use_case.py` & `spacetower_fds_sdk-1.0.3/fds/models/orbit_extrapolation/use_case.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/orbital_state.py` & `spacetower_fds_sdk-1.0.3/fds/models/orbital_state.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/orbits.py` & `spacetower_fds_sdk-1.0.3/fds/models/orbits.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/quaternion.py` & `spacetower_fds_sdk-1.0.3/fds/models/quaternion.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/roadmaps.py` & `spacetower_fds_sdk-1.0.3/fds/models/roadmaps.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/spacecraft.py` & `spacetower_fds_sdk-1.0.3/fds/models/spacecraft.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/telemetry.py` & `spacetower_fds_sdk-1.0.3/fds/models/telemetry.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/tle_extrapolation/result.py` & `spacetower_fds_sdk-1.0.3/fds/models/tle_extrapolation/result.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/tle_extrapolation/use_case.py` & `spacetower_fds_sdk-1.0.3/fds/models/tle_extrapolation/use_case.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/models/two_line_element.py` & `spacetower_fds_sdk-1.0.3/fds/models/two_line_element.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/utils/dates.py` & `spacetower_fds_sdk-1.0.3/fds/utils/dates.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/utils/dict.py` & `spacetower_fds_sdk-1.0.3/fds/utils/dict.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/utils/frames.py` & `spacetower_fds_sdk-1.0.3/fds/utils/frames.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/utils/geometry.py` & `spacetower_fds_sdk-1.0.3/fds/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/utils/math.py` & `spacetower_fds_sdk-1.0.3/fds/utils/math.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/fds/utils/orbital_mechanics.py` & `spacetower_fds_sdk-1.0.3/fds/utils/orbital_mechanics.py`

 * *Files identical despite different names*

### Comparing `spacetower_fds_sdk-1.0.2/PKG-INFO` & `spacetower_fds_sdk-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spacetower-fds-sdk
-Version: 1.0.2
+Version: 1.0.3
 Summary: SDK for spacetower Flight Dynamics System API
 License: Proprietary
 Keywords: FDS,API,Exotrail,Flight Dynamics
 Author: Exotrail
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

