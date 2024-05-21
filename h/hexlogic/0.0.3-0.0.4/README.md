# Comparing `tmp/hexlogic-0.0.3.tar.gz` & `tmp/hexlogic-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexlogic-0.0.3.tar", last modified: Fri Jan 26 10:18:18 2024, max compression
+gzip compressed data, was "hexlogic-0.0.4.tar", last modified: Tue May 21 13:14:48 2024, max compression
```

## Comparing `hexlogic-0.0.3.tar` & `hexlogic-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-01-26 10:18:18.843646 hexlogic-0.0.3/
--rw-rw-rw-   0        0        0     1095 2023-11-04 08:27:53.000000 hexlogic-0.0.3/LICENSE
--rw-rw-rw-   0        0        0    14633 2024-01-26 10:18:18.841623 hexlogic-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    13676 2024-01-26 09:56:40.000000 hexlogic-0.0.3/README.md
--rw-rw-rw-   0        0        0      957 2024-01-26 10:17:15.000000 hexlogic-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-26 10:18:18.843646 hexlogic-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1351 2023-12-17 10:20:42.000000 hexlogic-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-26 10:18:18.730825 hexlogic-0.0.3/src/
-drwxrwxrwx   0        0        0        0 2024-01-26 10:18:18.839606 hexlogic-0.0.3/src/hexlogic.egg-info/
--rw-rw-rw-   0        0        0    14633 2024-01-26 10:18:18.000000 hexlogic-0.0.3/src/hexlogic.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      201 2024-01-26 10:18:18.000000 hexlogic-0.0.3/src/hexlogic.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-26 10:18:18.000000 hexlogic-0.0.3/src/hexlogic.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-01-26 10:18:18.000000 hexlogic-0.0.3/src/hexlogic.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    67256 2024-01-26 09:53:38.000000 hexlogic-0.0.3/src/hexlogic.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:14:48.462692 hexlogic-0.0.4/
+-rw-rw-rw-   0        0        0     1095 2023-11-04 08:27:53.000000 hexlogic-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0    14850 2024-05-21 13:14:48.460676 hexlogic-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    13893 2024-05-21 12:53:34.000000 hexlogic-0.0.4/README.md
+-rw-rw-rw-   0        0        0      957 2024-05-13 12:20:47.000000 hexlogic-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:14:48.462692 hexlogic-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1351 2024-05-11 05:54:59.000000 hexlogic-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:14:48.432441 hexlogic-0.0.4/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 13:14:48.458677 hexlogic-0.0.4/src/hexlogic.egg-info/
+-rw-rw-rw-   0        0        0    14850 2024-05-21 13:14:48.000000 hexlogic-0.0.4/src/hexlogic.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      201 2024-05-21 13:14:48.000000 hexlogic-0.0.4/src/hexlogic.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 13:14:48.000000 hexlogic-0.0.4/src/hexlogic.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-21 13:14:48.000000 hexlogic-0.0.4/src/hexlogic.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    69465 2024-05-21 12:59:31.000000 hexlogic-0.0.4/src/hexlogic.py
```

### Comparing `hexlogic-0.0.3/LICENSE` & `hexlogic-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hexlogic-0.0.3/PKG-INFO` & `hexlogic-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexlogic
-Version: 0.0.3
+Version: 0.0.4
 Summary: HexLogic aims to be a Python package, without dependencies outside of the built-in library, providing fully-documented functions to deal with the relations between objects on a hexagon tiled grid. Including conversion from „hexagonal“ to „pixel“ coordinates and pathfinding with varying movement cost. As well as various operations like line-drawing.
 Home-page: https://github.com/MaximilianHauser/HexLogic
 Author: Maximilian Hauser
 Author-email: Maximilian Hauser <maxi.hauser@protonmail.com>
 Project-URL: Homepage, https://github.com/MaximilianHauser/HexLogic
 Project-URL: Bug Tracker, https://github.com/MaximilianHauser/HexLogic/issues
 Classifier: Programming Language :: Python :: 3
@@ -151,14 +151,17 @@
 Set q r and s attribute of obj to specified values.
     
 **hex_to_pixel(qrs:object|tuple|HexCoords, tile_width:int=64, tile_height:int=64, return_coords_obj:bool=False) -> tuple|RectCoords:**  
 Converts cube coordinates to pixel coordinates.
     
 **pixel_to_hex(xy:object|tuple|RectCoords, tile_width:int=64, tile_height:int=64, return_coords_obj:bool=False) -> tuple|HexCoords:**  
 Converts pixel coordinates to cube coordinates.
+
+**get_angle(obj_a:object|tuple|HexCoords, obj_b:object|tuple|HexCoords) -> float:**  
+Returns the angle from a line through obj_a and abj_b relative to the x-axis of a two dimensional cartesian coordinate system.
     
 **neighbors(qrs:object|tuple|HexCoords) -> set:**  
 Return a List of coordinates of neighboring hexagons.
     
 **distance(obj_a:object|tuple|HexCoords, obj_b:object|tuple|HexCoords) -> int|float:**
 Returns distance from one Object to another in a cube coordinate system.
```

### Comparing `hexlogic-0.0.3/README.md` & `hexlogic-0.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -135,14 +135,17 @@
 Set q r and s attribute of obj to specified values.
     
 **hex_to_pixel(qrs:object|tuple|HexCoords, tile_width:int=64, tile_height:int=64, return_coords_obj:bool=False) -> tuple|RectCoords:**  
 Converts cube coordinates to pixel coordinates.
     
 **pixel_to_hex(xy:object|tuple|RectCoords, tile_width:int=64, tile_height:int=64, return_coords_obj:bool=False) -> tuple|HexCoords:**  
 Converts pixel coordinates to cube coordinates.
+
+**get_angle(obj_a:object|tuple|HexCoords, obj_b:object|tuple|HexCoords) -> float:**  
+Returns the angle from a line through obj_a and abj_b relative to the x-axis of a two dimensional cartesian coordinate system.
     
 **neighbors(qrs:object|tuple|HexCoords) -> set:**  
 Return a List of coordinates of neighboring hexagons.
     
 **distance(obj_a:object|tuple|HexCoords, obj_b:object|tuple|HexCoords) -> int|float:**
 Returns distance from one Object to another in a cube coordinate system.
```

### Comparing `hexlogic-0.0.3/pyproject.toml` & `hexlogic-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hexlogic"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Maximilian Hauser", email="maxi.hauser@protonmail.com" },
 ]
 description = "HexLogic aims to be a Python package, without dependencies outside of the built-in library, providing fully-documented functions to deal with the relations between objects on a hexagon tiled grid. Including conversion from „hexagonal“ to „pixel“ coordinates and pathfinding with varying movement cost. As well as various operations like line-drawing."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hexlogic-0.0.3/setup.py` & `hexlogic-0.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # readme -------------------------------------------------------------------- #
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 # setup --------------------------------------------------------------------- #
 setup(name="hexlogic", 
-      version="0.0.3", 
+      version="0.0.4", 
       description="HexLogic aims to be a Python package, without dependencies outside of the built-in library, providing fully-documented functions to deal with the relations between objects on a hexagon tiled grid. Including conversion from „hexagonal“ to „pixel“ coordinates and pathfinding with varying movement cost. As well as various operations like line-drawing.",
       py_modules=["hexlogic"],
       package_dir={"": "src"},
       classifiers=[
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
```

### Comparing `hexlogic-0.0.3/src/hexlogic.egg-info/PKG-INFO` & `hexlogic-0.0.4/src/hexlogic.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexlogic
-Version: 0.0.3
+Version: 0.0.4
 Summary: HexLogic aims to be a Python package, without dependencies outside of the built-in library, providing fully-documented functions to deal with the relations between objects on a hexagon tiled grid. Including conversion from „hexagonal“ to „pixel“ coordinates and pathfinding with varying movement cost. As well as various operations like line-drawing.
 Home-page: https://github.com/MaximilianHauser/HexLogic
 Author: Maximilian Hauser
 Author-email: Maximilian Hauser <maxi.hauser@protonmail.com>
 Project-URL: Homepage, https://github.com/MaximilianHauser/HexLogic
 Project-URL: Bug Tracker, https://github.com/MaximilianHauser/HexLogic/issues
 Classifier: Programming Language :: Python :: 3
@@ -151,14 +151,17 @@
 Set q r and s attribute of obj to specified values.
     
 **hex_to_pixel(qrs:object|tuple|HexCoords, tile_width:int=64, tile_height:int=64, return_coords_obj:bool=False) -> tuple|RectCoords:**  
 Converts cube coordinates to pixel coordinates.
     
 **pixel_to_hex(xy:object|tuple|RectCoords, tile_width:int=64, tile_height:int=64, return_coords_obj:bool=False) -> tuple|HexCoords:**  
 Converts pixel coordinates to cube coordinates.
+
+**get_angle(obj_a:object|tuple|HexCoords, obj_b:object|tuple|HexCoords) -> float:**  
+Returns the angle from a line through obj_a and abj_b relative to the x-axis of a two dimensional cartesian coordinate system.
     
 **neighbors(qrs:object|tuple|HexCoords) -> set:**  
 Return a List of coordinates of neighboring hexagons.
     
 **distance(obj_a:object|tuple|HexCoords, obj_b:object|tuple|HexCoords) -> int|float:**
 Returns distance from one Object to another in a cube coordinate system.
```

### Comparing `hexlogic-0.0.3/src/hexlogic.py` & `hexlogic-0.0.4/src/hexlogic.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,19 @@
 Dependencies:
 -------------
 collections.namedtuple
     Provides a new tuple subclass. The new subclass is used to create tuple-like 
     objects that have fields accessible by attribute lookup as well as being 
     indexable and iterable.
     
+math
+    This module provides access to the mathematical functions defined by the 
+    C standard library.
+    
+    
 unittest
     The unittest unit testing framework supports test automation sharing of 
     setup and shutdown code for tests, aggregation of tests into collections,
     and independence of the tests from the reporting framework.
 
 
 Custom Errors:
@@ -184,14 +189,15 @@
 NumPy Style Guide:
 https://numpydoc.readthedocs.io/en/latest/format.html
 """
 
 
 # import section ------------------------------------------------------------ #
 from collections import namedtuple
+from math import degrees, atan2
 
 
 # custom datatypes to ensure constraints ------------------------------------ #
 # error for a hexagonal_coordinate that violates the zero-sum-constraint ---- #
 class ConstraintViolation(ValueError):
     """
     Custom Error to be raised when a logical constraint is violated. 
@@ -1379,15 +1385,70 @@
         qrs = HexCoords(q, r, s)
     elif return_obj_type.lower() == "list":
         qrs = [q, r, s]
     elif return_obj_type.lower() == "dict":
         qrs = {"q":q, "r":r, "s":s}
         
     return qrs
+
+    
+def get_angle(obj_a:object|tuple|RectCoords|HexCoords, obj_b:object|tuple|RectCoords|HexCoords, *, 
+              expected_len_a:int=3, expected_len_b:int=3) -> float:
+    """
+    Returns the angle in degrees from a line through obj_a and abj_b relative to 
+    the x-axis of a two dimensional cartesian coordinate system. On a screen, 
+    because of the relativ to normal, inverted y-Axis, the angle is clockwise.
     
+    Parameters:
+    -----------
+    obj_a : Object | Tuple | HexCoords
+            A Tuple consisting of an Integer or Float for the x and y, or 
+            q, r and s value, or an Object having x and y or a q, r and s attribute, 
+            the assigned values being an Integer or Float. Needs to adhere to 
+            zero constraint.
+            
+    obj_b : Object | Tuple | HexCoords
+            A Tuple consisting of an Integer or Float for the q, r and s value,
+            or an Object having a q, r and s attribute, the assigned values being an 
+            Integer or Float. Needs to adhere to zero constraint.
+            
+    Raises:
+    -------
+    TypeError: 
+        If x or y is not an Integer or a Float. If q, r or s is not an Integer 
+        or a Float. If a passed Tuple has too many or too few individual values.
+        
+    AttributeError: 
+        If an Object is passed, but is missing the x, y or q, r or s coordinate attributes.
+        
+    ConstraintViolation: 
+        If the q + r + s = 0 constraint is violated.
+        
+    Returns:
+    --------
+    angle(Float): 
+        The angle between a line drawn from A to B, relative to the X-Axis in 
+        radians or in degrees.
+    """
+    
+    a = container_or_object(obj_a, expected_len_a)
+    b = container_or_object(obj_b, expected_len_b)
+    
+    if len(a) == 3:
+        a = hex_to_pixel(a)
+    if len(b) == 3:
+        b = hex_to_pixel(b)
+        
+    angle = atan2(b[1]-a[1], b[0]-a[0])
+    
+    if angle < 0:
+        return 360 + degrees(angle) 
+    else:
+        return degrees(angle) 
+
 
 def neighbors(qrs:object|tuple|HexCoords) -> set:
     """
     Returns a Tuple of coordinates of neighboring hexagons.
         
     Parameters:
     -----------
@@ -1660,8 +1721,7 @@
                     if nbor_coords not in visited:
                         if not blocked:
                             visited.add(nbor_coords)
                             fringes[i].append(nbor_coords)
     
     return visited
 
-
```

