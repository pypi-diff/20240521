# Comparing `tmp/textmark-0.4.0.tar.gz` & `tmp/textmark-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textmark-0.4.0.tar", last modified: Wed Mar 13 18:20:19 2024, max compression
+gzip compressed data, was "textmark-0.5.0.tar", last modified: Mon May 20 23:04:32 2024, max compression
```

## Comparing `textmark-0.4.0.tar` & `textmark-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:20:19.046773 textmark-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-13 18:20:14.000000 textmark-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-13 18:20:19.046773 textmark-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-03-13 18:20:14.000000 textmark-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-13 18:20:14.000000 textmark-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-13 18:20:19.046773 textmark-0.4.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:20:19.046773 textmark-0.4.0/textmark/
--rw-r--r--   0 runner    (1001) docker     (127)    15978 2024-03-13 18:20:14.000000 textmark-0.4.0/textmark/TextAnnotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8684 2024-03-13 18:20:14.000000 textmark-0.4.0/textmark/Visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-13 18:20:14.000000 textmark-0.4.0/textmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-03-13 18:20:14.000000 textmark-0.4.0/textmark/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 18:20:19.046773 textmark-0.4.0/textmark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-03-13 18:20:19.000000 textmark-0.4.0/textmark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-03-13 18:20:19.000000 textmark-0.4.0/textmark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 18:20:19.000000 textmark-0.4.0/textmark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-13 18:20:19.000000 textmark-0.4.0/textmark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-13 18:20:19.000000 textmark-0.4.0/textmark.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:04:32.936237 textmark-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-05-20 23:04:28.000000 textmark-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-20 23:04:32.936237 textmark-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2024-05-20 23:04:28.000000 textmark-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-20 23:04:28.000000 textmark-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-20 23:04:32.936237 textmark-0.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:04:32.936237 textmark-0.5.0/textmark/
+-rw-r--r--   0 runner    (1001) docker     (127)    15978 2024-05-20 23:04:28.000000 textmark-0.5.0/textmark/TextAnnotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9084 2024-05-20 23:04:28.000000 textmark-0.5.0/textmark/Visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-20 23:04:28.000000 textmark-0.5.0/textmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-20 23:04:28.000000 textmark-0.5.0/textmark/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:04:32.936237 textmark-0.5.0/textmark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2024-05-20 23:04:32.000000 textmark-0.5.0/textmark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-20 23:04:32.000000 textmark-0.5.0/textmark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 23:04:32.000000 textmark-0.5.0/textmark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-20 23:04:32.000000 textmark-0.5.0/textmark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 23:04:32.000000 textmark-0.5.0/textmark.egg-info/top_level.txt
```

### Comparing `textmark-0.4.0/LICENSE` & `textmark-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textmark-0.4.0/PKG-INFO` & `textmark-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textmark
-Version: 0.4.0
+Version: 0.5.0
 Summary: Text annotation utilities for computer vision pipelines.
 Author-email: David Jones <d.t.jones@outlook.com>
 Maintainer-email: David Jones <d.t.jones@outlook.com>
 License: Copyright (c) 2024 David Jones
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

### Comparing `textmark-0.4.0/README.md` & `textmark-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `textmark-0.4.0/pyproject.toml` & `textmark-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "textmark"
-version = "0.4.0"
+version = "0.5.0"
 description = "Text annotation utilities for computer vision pipelines."
 authors = [
     { name = "David Jones", email = "d.t.jones@outlook.com" },
 ]
 maintainers = [
     { name = "David Jones", email = "d.t.jones@outlook.com" },
 ]
```

### Comparing `textmark-0.4.0/textmark/TextAnnotation.py` & `textmark-0.5.0/textmark/TextAnnotation.py`

 * *Files identical despite different names*

### Comparing `textmark-0.4.0/textmark/Visualizer.py` & `textmark-0.5.0/textmark/Visualizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,16 @@
 
     def visualize(
         self,
         save_path=None,
         draw_language_name=False,
         draw_vertex_numbers=False,
         draw_annotation_order=False,
+        outline_width="auto",
+        font_height="auto"
     ):
         """
         Visualize the image.
 
         astype: Provide an annotation type (e.g., BoxAnnotation) to visualize
             the annotation as that type.
 
@@ -72,16 +74,25 @@
         draw_vertex_numbers if useful to verify that your representation is
             expected.
         """
         vis_image = self.image.copy()
         transparent_layer = Image.new("RGBA", self.image.size, (0, 0, 0, 0))
         draw = ImageDraw.Draw(transparent_layer)
 
-        outline_width = max(int(self.image_height * 0.01), 1)
-        font_height = int(self.image_height * 0.03)
+        if outline_width == "auto":
+            outline_width = max(int(self.image_height * 0.01), 1)
+        else:
+            if not isinstance(outline_width, int):
+                raise ValueError("outline_width must be an integer")
+
+        if font_height == "auto":
+            font_height = int(self.image_height * 0.03)
+        else:
+            if not isinstance(font_height, int):
+                raise ValueError("font_height must be an integer")
 
         lang_name_font = ImageFont.truetype(
             font=self.font_handler.get_font("NotoSans"),
             size=font_height,
         )
 
         for idx, annotation in enumerate(self.annotations):
```

### Comparing `textmark-0.4.0/textmark/tools.py` & `textmark-0.5.0/textmark/tools.py`

 * *Files identical despite different names*

### Comparing `textmark-0.4.0/textmark.egg-info/PKG-INFO` & `textmark-0.5.0/textmark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textmark
-Version: 0.4.0
+Version: 0.5.0
 Summary: Text annotation utilities for computer vision pipelines.
 Author-email: David Jones <d.t.jones@outlook.com>
 Maintainer-email: David Jones <d.t.jones@outlook.com>
 License: Copyright (c) 2024 David Jones
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
```

