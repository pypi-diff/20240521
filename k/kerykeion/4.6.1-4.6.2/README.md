# Comparing `tmp/kerykeion-4.6.1.tar.gz` & `tmp/kerykeion-4.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kerykeion-4.6.1.tar", max compression
+gzip compressed data, was "kerykeion-4.6.2.tar", max compression
```

## Comparing `kerykeion-4.6.1.tar` & `kerykeion-4.6.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    34273 2024-05-21 10:10:48.977320 kerykeion-4.6.1/LICENSE
--rw-r--r--   0        0        0     8634 2024-05-21 10:10:48.977579 kerykeion-4.6.1/README.md
--rw-r--r--   0        0        0     3917 2024-05-21 10:10:48.989259 kerykeion-4.6.1/kerykeion/__init__.py
--rw-r--r--   0        0        0      293 2024-05-21 10:10:48.989399 kerykeion-4.6.1/kerykeion/aspects/__init__.py
--rw-r--r--   0        0        0     5832 2024-05-21 10:10:48.989562 kerykeion-4.6.1/kerykeion/aspects/aspects_utils.py
--rw-r--r--   0        0        0     4507 2024-05-21 10:10:48.989667 kerykeion-4.6.1/kerykeion/aspects/natal_aspects.py
--rw-r--r--   0        0        0     3993 2024-05-21 10:10:48.989766 kerykeion-4.6.1/kerykeion/aspects/synastry_aspects.py
--rw-r--r--   0        0        0    22965 2024-05-21 10:10:48.989894 kerykeion-4.6.1/kerykeion/astrological_subject.py
--rw-r--r--   0        0        0      127 2024-05-21 10:10:48.990043 kerykeion-4.6.1/kerykeion/charts/__init__.py
--rw-r--r--   0        0        0     5167 2024-05-21 10:12:32.446413 kerykeion-4.6.1/kerykeion/charts/charts_utils.py
--rwxr-xr-x   0        0        0    64662 2024-05-21 10:12:32.447253 kerykeion-4.6.1/kerykeion/charts/kerykeion_chart_svg.py
--rwxr-xr-x   0        0        0    69874 2024-05-21 10:10:48.990844 kerykeion-4.6.1/kerykeion/charts/templates/chart.xml
--rw-r--r--   0        0        0      965 2024-05-21 10:10:48.990945 kerykeion-4.6.1/kerykeion/enums.py
--rw-r--r--   0        0        0     4444 2024-05-21 10:10:48.991048 kerykeion-4.6.1/kerykeion/fetch_geonames.py
--rw-r--r--   0        0        0      295 2024-05-21 10:10:48.991194 kerykeion-4.6.1/kerykeion/kr_types/__init__.py
--rw-r--r--   0        0        0     1945 2024-05-21 10:10:48.991287 kerykeion-4.6.1/kerykeion/kr_types/chart_types.py
--rw-r--r--   0        0        0      314 2024-05-21 10:10:48.991371 kerykeion-4.6.1/kerykeion/kr_types/kerykeion_exception.py
--rw-r--r--   0        0        0     1267 2024-05-21 10:10:48.991458 kerykeion-4.6.1/kerykeion/kr_types/kr_literals.py
--rw-r--r--   0        0        0     4260 2024-05-21 10:10:48.991553 kerykeion-4.6.1/kerykeion/kr_types/kr_models.py
--rw-r--r--   0        0        0    12743 2024-05-21 10:10:48.991736 kerykeion-4.6.1/kerykeion/kr_types/settings_models.py
--rw-r--r--   0        0        0     6794 2024-05-21 10:10:48.991972 kerykeion-4.6.1/kerykeion/relationship_score.py
--rw-r--r--   0        0        0     2565 2024-05-21 10:10:48.992075 kerykeion-4.6.1/kerykeion/report.py
--rw-r--r--   0        0        0       69 2024-05-21 10:10:48.992209 kerykeion-4.6.1/kerykeion/settings/__init__.py
--rw-r--r--   0        0        0     2347 2024-05-21 10:10:48.992306 kerykeion-4.6.1/kerykeion/settings/kerykeion_settings.py
--rw-r--r--   0        0        0    12282 2024-05-21 10:10:48.992452 kerykeion-4.6.1/kerykeion/settings/kr.config.json
--rw-r--r--   0        0        0       73 2024-05-21 10:10:48.992570 kerykeion-4.6.1/kerykeion/sweph/README.md
--rw-r--r--   0        0        0   223002 2024-05-21 10:10:48.993481 kerykeion-4.6.1/kerykeion/sweph/seas_18.se1
--rw-r--r--   0        0        0    10822 2024-05-21 10:10:48.993609 kerykeion-4.6.1/kerykeion/utilities.py
--rw-r--r--   0        0        0     2354 2024-05-21 10:12:55.547661 kerykeion-4.6.1/pyproject.toml
--rw-r--r--   0        0        0    10311 1970-01-01 00:00:00.000000 kerykeion-4.6.1/PKG-INFO
+-rw-r--r--   0        0        0    34273 2024-03-05 19:55:06.854597 kerykeion-4.6.2/LICENSE
+-rw-r--r--   0        0        0     8634 2024-03-05 19:55:06.855014 kerykeion-4.6.2/README.md
+-rw-r--r--   0        0        0     3917 2024-05-20 21:44:34.775470 kerykeion-4.6.2/kerykeion/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-20 21:44:34.775703 kerykeion-4.6.2/kerykeion/aspects/__init__.py
+-rw-r--r--   0        0        0     5832 2024-05-20 21:44:34.775937 kerykeion-4.6.2/kerykeion/aspects/aspects_utils.py
+-rw-r--r--   0        0        0     4507 2024-05-20 21:44:34.776153 kerykeion-4.6.2/kerykeion/aspects/natal_aspects.py
+-rw-r--r--   0        0        0     3993 2024-05-20 21:44:34.776366 kerykeion-4.6.2/kerykeion/aspects/synastry_aspects.py
+-rw-r--r--   0        0        0    22965 2024-05-20 21:44:34.776635 kerykeion-4.6.2/kerykeion/astrological_subject.py
+-rw-r--r--   0        0        0      127 2024-05-20 21:44:34.776876 kerykeion-4.6.2/kerykeion/charts/__init__.py
+-rw-r--r--   0        0        0     5167 2024-05-21 10:16:22.735355 kerykeion-4.6.2/kerykeion/charts/charts_utils.py
+-rwxr-xr-x   0        0        0    64764 2024-05-21 11:01:53.142967 kerykeion-4.6.2/kerykeion/charts/kerykeion_chart_svg.py
+-rwxr-xr-x   0        0        0    69874 2024-03-05 19:18:31.416341 kerykeion-4.6.2/kerykeion/charts/templates/chart.xml
+-rw-r--r--   0        0        0      965 2024-05-13 20:03:16.436187 kerykeion-4.6.2/kerykeion/enums.py
+-rw-r--r--   0        0        0     4444 2024-05-20 21:44:34.777442 kerykeion-4.6.2/kerykeion/fetch_geonames.py
+-rw-r--r--   0        0        0      295 2024-05-20 21:44:34.777647 kerykeion-4.6.2/kerykeion/kr_types/__init__.py
+-rw-r--r--   0        0        0     1945 2024-03-05 19:18:31.416709 kerykeion-4.6.2/kerykeion/kr_types/chart_types.py
+-rw-r--r--   0        0        0      314 2024-05-20 21:44:34.777837 kerykeion-4.6.2/kerykeion/kr_types/kerykeion_exception.py
+-rw-r--r--   0        0        0     1267 2024-05-20 21:44:34.778024 kerykeion-4.6.2/kerykeion/kr_types/kr_literals.py
+-rw-r--r--   0        0        0     4260 2024-05-20 21:44:34.778212 kerykeion-4.6.2/kerykeion/kr_types/kr_models.py
+-rw-r--r--   0        0        0    12743 2024-05-20 21:44:34.778431 kerykeion-4.6.2/kerykeion/kr_types/settings_models.py
+-rw-r--r--   0        0        0     6794 2024-05-20 21:44:34.778633 kerykeion-4.6.2/kerykeion/relationship_score.py
+-rw-r--r--   0        0        0     2565 2024-03-05 19:18:31.417278 kerykeion-4.6.2/kerykeion/report.py
+-rw-r--r--   0        0        0       69 2024-03-05 19:18:31.417375 kerykeion-4.6.2/kerykeion/settings/__init__.py
+-rw-r--r--   0        0        0     2347 2024-05-20 21:44:34.778844 kerykeion-4.6.2/kerykeion/settings/kerykeion_settings.py
+-rw-r--r--   0        0        0    12282 2024-03-05 19:18:31.417645 kerykeion-4.6.2/kerykeion/settings/kr.config.json
+-rw-r--r--   0        0        0       73 2024-03-05 19:18:31.417768 kerykeion-4.6.2/kerykeion/sweph/README.md
+-rw-r--r--   0        0        0   223002 2024-03-05 19:18:31.418653 kerykeion-4.6.2/kerykeion/sweph/seas_18.se1
+-rw-r--r--   0        0        0    10822 2024-05-20 21:44:34.779112 kerykeion-4.6.2/kerykeion/utilities.py
+-rw-r--r--   0        0        0     2354 2024-05-21 11:02:19.022293 kerykeion-4.6.2/pyproject.toml
+-rw-r--r--   0        0        0    10311 1970-01-01 00:00:00.000000 kerykeion-4.6.2/PKG-INFO
```

### Comparing `kerykeion-4.6.1/LICENSE` & `kerykeion-4.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/README.md` & `kerykeion-4.6.2/README.md`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/__init__.py` & `kerykeion-4.6.2/kerykeion/__init__.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/aspects/aspects_utils.py` & `kerykeion-4.6.2/kerykeion/aspects/aspects_utils.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/aspects/natal_aspects.py` & `kerykeion-4.6.2/kerykeion/aspects/natal_aspects.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/aspects/synastry_aspects.py` & `kerykeion-4.6.2/kerykeion/aspects/synastry_aspects.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/astrological_subject.py` & `kerykeion-4.6.2/kerykeion/astrological_subject.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/charts/charts_utils.py` & `kerykeion-4.6.2/kerykeion/charts/charts_utils.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/charts/kerykeion_chart_svg.py` & `kerykeion-4.6.2/kerykeion/charts/kerykeion_chart_svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1196,56 +1196,49 @@
 
         if end_of_line is None:
             raise KerykeionException("End of line not found")
 
         out += end_of_line
         return out
 
-    def _makeHousesGrid(self):
-        """
-        Generate SVG code for a grid of astrological houses.
-
-        Returns:
-            str: The SVG code for the grid of houses.
-        """
-        # Initialize the SVG group for the grid
-        grid_svg = '<g transform="translate(600,-20)">'
+    def _draw_house_grid(self):
+        out = '<g transform="translate(600,-20)">'
 
-        # Vertical position of the current house in the grid
-        vertical_position = 10
-
-        # Generate SVG code for each house
+        li = 10
         for i in range(12):
-            # Add leading spaces to single-digit house numbers for alignment
-            house_number = str(i + 1).rjust(2, ' ')
-
-            # Start a new SVG group for the current house
-            grid_svg += f'<g transform="translate(0,{vertical_position})">'
-
-            # Add the house label
-            grid_svg += f'<text text-anchor="end" x="40" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{self.language_settings["cusp"]} {house_number}:</text>'
-
-            # Add the zodiac sign symbol for the house
-            zodiac_sign = self.zodiac[self.houses_sign_graph[i]]["name"]
-            grid_svg += f'<g transform="translate(40,-8)"><use transform="scale(0.3)" xlink:href="#{zodiac_sign}" /></g>'
-
-            # Add the position of the house
-            house_position = self._dec2deg(self.user.houses_list[i]["position"])
-            grid_svg += f'<text x="53" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;"> {house_position}</text>'
-
-            # End the SVG group for the current house
-            grid_svg += "</g>"
+            if i < 9:
+                cusp = "&#160;&#160;" + str(i + 1)
+            else:
+                cusp = str(i + 1)
+            out += f'<g transform="translate(0,{li})">'
+            out += f'<text text-anchor="end" x="40" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{self.language_settings["cusp"]} {cusp}:</text>'
+            out += f'<g transform="translate(40,-8)"><use transform="scale(0.3)" xlink:href="#{self.zodiac[self.houses_sign_graph[i]]["name"]}" /></g>'
+            out += f'<text x="53" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;"> {self._dec2deg(self.user.houses_list[i]["position"])}</text>'
+            out += "</g>"
+            li = li + 14
 
-            # Move down for the next house
-            vertical_position += 14
+        out += "</g>"
 
-        # End the SVG group for the grid
-        grid_svg += "</g>"
+        if self.chart_type == "Synastry":
+            out += '<g transform="translate(840, -20)">'
+            li = 10
+            for i in range(12):
+                if i < 9:
+                    cusp = "&#160;&#160;" + str(i + 1)
+                else:
+                    cusp = str(i + 1)
+                out += '<g transform="translate(0,' + str(li) + ')">'
+                out += f'<text text-anchor="end" x="40" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;">{self.language_settings["cusp"]} {cusp}:</text>'
+                out += f'<g transform="translate(40,-8)"><use transform="scale(0.3)" xlink:href="#{self.zodiac[self.t_houses_sign_graph[i]]["name"]}" /></g>'
+                out += f'<text x="53" style="fill:{self.chart_colors_settings["paper_0"]}; font-size: 10px;"> {self._dec2deg(self.t_user.houses_list[i]["position"])}</text>'
+                out += "</g>"
+                li = li + 14
+            out += "</g>"
 
-        return grid_svg
+        return out
 
     def _createTemplateDictionary(self) -> ChartTemplateDictionary:
         # self.chart_type = "Transit"
         # empty element points
         self.fire = 0.0
         self.earth = 0.0
         self.air = 0.0
@@ -1444,22 +1437,21 @@
         td["cfgRotate"] = rotate
         td["cfgTranslate"] = translate
 
         # ---
         # Drawing Functions
         #--- 
 
-        # Drawing the Zodiac slices
         td["makeZodiac"] = self._draw_zodiac_circle_slices(r)
+        td["makeHousesGrid"] = self._draw_house_grid()
         # TODO: Add the rest of the functions
         td["makeHouses"] = self._makeHouses(r)
         td["makePlanets"] = self._make_planets(r)
         td["makeElements"] = self._makeElements(r)
         td["makePlanetGrid"] = self._makePlanetGrid()
-        td["makeHousesGrid"] = self._makeHousesGrid()
 
         return td
 
     def makeTemplate(self):
         """Creates the template for the SVG file"""
         td = self._createTemplateDictionary()
```

### Comparing `kerykeion-4.6.1/kerykeion/charts/templates/chart.xml` & `kerykeion-4.6.2/kerykeion/charts/templates/chart.xml`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/enums.py` & `kerykeion-4.6.2/kerykeion/enums.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/fetch_geonames.py` & `kerykeion-4.6.2/kerykeion/fetch_geonames.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/kr_types/chart_types.py` & `kerykeion-4.6.2/kerykeion/kr_types/chart_types.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/kr_types/kr_literals.py` & `kerykeion-4.6.2/kerykeion/kr_types/kr_literals.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/kr_types/kr_models.py` & `kerykeion-4.6.2/kerykeion/kr_types/kr_models.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/kr_types/settings_models.py` & `kerykeion-4.6.2/kerykeion/kr_types/settings_models.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/relationship_score.py` & `kerykeion-4.6.2/kerykeion/relationship_score.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/report.py` & `kerykeion-4.6.2/kerykeion/report.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/settings/kerykeion_settings.py` & `kerykeion-4.6.2/kerykeion/settings/kerykeion_settings.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/settings/kr.config.json` & `kerykeion-4.6.2/kerykeion/settings/kr.config.json`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/sweph/seas_18.se1` & `kerykeion-4.6.2/kerykeion/sweph/seas_18.se1`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/kerykeion/utilities.py` & `kerykeion-4.6.2/kerykeion/utilities.py`

 * *Files identical despite different names*

### Comparing `kerykeion-4.6.1/pyproject.toml` & `kerykeion-4.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kerykeion"
-version = "4.6.1"
+version = "4.6.2"
 authors = ["Giacomo Battaglia <battaglia.giacomo@yahoo.it>"]
 description = "A python library for astrology."
 license = "AGPL-3.0"
 homepage = "https://github.com/g-battaglia/kerykeion"
 repository = "https://github.com/g-battaglia/kerykeion"
 keywords = [
     "astrology",
```

### Comparing `kerykeion-4.6.1/PKG-INFO` & `kerykeion-4.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kerykeion
-Version: 4.6.1
+Version: 4.6.2
 Summary: A python library for astrology.
 Home-page: https://github.com/g-battaglia/kerykeion
 License: AGPL-3.0
 Keywords: astrology,ephemeris,astrology library,birtchart,svg,zodiac,zodiac-sing,astronomical-algorithms,synastry,astrology-calculator
 Author: Giacomo Battaglia
 Author-email: battaglia.giacomo@yahoo.it
 Requires-Python: >=3.9,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: kerykeion Version: 4.6.1 Summary: A python library
+Metadata-Version: 2.1 Name: kerykeion Version: 4.6.2 Summary: A python library
 for astrology. Home-page: https://github.com/g-battaglia/kerykeion License:
 AGPL-3.0 Keywords: astrology,ephemeris,astrology
 library,birtchart,svg,zodiac,zodiac-sing,astronomical-
 algorithms,synastry,astrology-calculator Author: Giacomo Battaglia Author-
 email: battaglia.giacomo@yahoo.it Requires-Python: >=3.9,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: Intended Audience :: Information Technology Classifier:
```

