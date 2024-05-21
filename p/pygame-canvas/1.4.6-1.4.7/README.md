# Comparing `tmp/pygame_canvas-1.4.6.tar.gz` & `tmp/pygame_canvas-1.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygame_canvas-1.4.6.tar", last modified: Tue May 21 14:58:22 2024, max compression
+gzip compressed data, was "pygame_canvas-1.4.7.tar", last modified: Tue May 21 15:04:19 2024, max compression
```

## Comparing `pygame_canvas-1.4.6.tar` & `pygame_canvas-1.4.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:58:22.042747 pygame_canvas-1.4.6/
--rw-rw-rw-   0        0        0     1881 2024-05-21 14:58:22.040721 pygame_canvas-1.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     1638 2024-05-21 14:32:25.000000 pygame_canvas-1.4.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 14:58:22.017773 pygame_canvas-1.4.6/pygame_canvas/
--rw-rw-rw-   0        0        0       27 2024-05-21 14:58:05.000000 pygame_canvas-1.4.6/pygame_canvas/__init__.py
--rw-rw-rw-   0        0        0    16821 2024-05-21 14:44:17.000000 pygame_canvas-1.4.6/pygame_canvas/pygame_canvas.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:58:22.040214 pygame_canvas-1.4.6/pygame_canvas.egg-info/
--rw-rw-rw-   0        0        0     1881 2024-05-21 14:58:21.000000 pygame_canvas-1.4.6/pygame_canvas.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      274 2024-05-21 14:58:21.000000 pygame_canvas-1.4.6/pygame_canvas.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:58:21.000000 pygame_canvas-1.4.6/pygame_canvas.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-21 14:58:21.000000 pygame_canvas-1.4.6/pygame_canvas.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-21 14:58:21.000000 pygame_canvas-1.4.6/pygame_canvas.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       95 2024-05-21 13:50:24.000000 pygame_canvas-1.4.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-21 14:58:22.042747 pygame_canvas-1.4.6/setup.cfg
--rw-rw-rw-   0        0        0      520 2024-05-21 14:58:13.000000 pygame_canvas-1.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:04:19.913055 pygame_canvas-1.4.7/
+-rw-rw-rw-   0        0        0     1797 2024-05-21 15:04:19.912039 pygame_canvas-1.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1554 2024-05-21 15:04:12.000000 pygame_canvas-1.4.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 15:04:19.894287 pygame_canvas-1.4.7/pygame_canvas/
+-rw-rw-rw-   0        0        0       28 2024-05-21 14:59:55.000000 pygame_canvas-1.4.7/pygame_canvas/__init__.py
+-rw-rw-rw-   0        0        0    16813 2024-05-21 15:01:48.000000 pygame_canvas-1.4.7/pygame_canvas/pygame_canvas.py
+drwxrwxrwx   0        0        0        0 2024-05-21 15:04:19.911007 pygame_canvas-1.4.7/pygame_canvas.egg-info/
+-rw-rw-rw-   0        0        0     1797 2024-05-21 15:04:19.000000 pygame_canvas-1.4.7/pygame_canvas.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      274 2024-05-21 15:04:19.000000 pygame_canvas-1.4.7/pygame_canvas.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 15:04:19.000000 pygame_canvas-1.4.7/pygame_canvas.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 15:04:19.000000 pygame_canvas-1.4.7/pygame_canvas.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 15:04:19.000000 pygame_canvas-1.4.7/pygame_canvas.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       95 2024-05-21 13:50:24.000000 pygame_canvas-1.4.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 15:04:19.913055 pygame_canvas-1.4.7/setup.cfg
+-rw-rw-rw-   0        0        0      520 2024-05-21 15:02:25.000000 pygame_canvas-1.4.7/setup.py
```

### Comparing `pygame_canvas-1.4.6/PKG-INFO` & `pygame_canvas-1.4.7/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_canvas
-Version: 1.4.6
+Version: 1.4.7
 Summary: A library for canvas operations using pygame
 Home-page: https://x.com/gioseaxmc
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 
 Canvas
@@ -20,25 +20,18 @@
 Usage
 Installation
 To use Canvas, you'll need Python installed on your system along with the Pygame library. You can install Pygame using pip:
 
 
 pip install pygame
 
-Example Usage
+# Example Usage
 Here's a simple example demonstrating how to use Canvas to create a window and display a sprite:
 
-import canvas as c
+import pygame_canvas as c
 
-# Initialize window
-c.window(title="My Game")
+c.default_template(__file__)
 
-# Create sprite
-sprite = c.sprite(images=[c.rectangle(50, 50, (0, 200, 255))], pos=(240, 180))
-
-# Main game loop
-while c.loop(60):
-    # Update game logic here
-    pass
+The code above will load a default template into the main python script OVERWRITING EVERYTHING ELSE
 
 Documentation
 For detailed documentation and usage examples, refer to the Canvas documentation at: https://docs.google.com/document/d/18SMSY5RbigaOX2WOaGQs0iEUvSFnpfpWjsBxBNwq0nA/edit?usp=sharing.
```

### Comparing `pygame_canvas-1.4.6/README.md` & `pygame_canvas-1.4.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -11,25 +11,18 @@
 Usage
 Installation
 To use Canvas, you'll need Python installed on your system along with the Pygame library. You can install Pygame using pip:
 
 
 pip install pygame
 
-Example Usage
+# Example Usage
 Here's a simple example demonstrating how to use Canvas to create a window and display a sprite:
 
-import canvas as c
+import pygame_canvas as c
 
-# Initialize window
-c.window(title="My Game")
+c.default_template(__file__)
 
-# Create sprite
-sprite = c.sprite(images=[c.rectangle(50, 50, (0, 200, 255))], pos=(240, 180))
-
-# Main game loop
-while c.loop(60):
-    # Update game logic here
-    pass
+The code above will load a default template into the main python script OVERWRITING EVERYTHING ELSE
 
 Documentation
 For detailed documentation and usage examples, refer to the Canvas documentation at: https://docs.google.com/document/d/18SMSY5RbigaOX2WOaGQs0iEUvSFnpfpWjsBxBNwq0nA/edit?usp=sharing.
```

### Comparing `pygame_canvas-1.4.6/pygame_canvas/pygame_canvas.py` & `pygame_canvas-1.4.7/pygame_canvas/pygame_canvas.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,15 +410,15 @@
     fileName should be: __file__
 
     functions loads default template for pygame2.
     """
     with open(fileName, "w") as file:
         file.write("""import pygame-canvas as c
 
-c.window(vSync=1,title = "game")
+c.window(title = "game")
 
 # sprite declaration here:
 object = c.sprite((c.rectangle(50,50,(0,200,255)),),(240,180))
 
 while c.loop(60):
     
     # your code here:
```

### Comparing `pygame_canvas-1.4.6/pygame_canvas.egg-info/PKG-INFO` & `pygame_canvas-1.4.7/pygame_canvas.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygame_canvas
-Version: 1.4.6
+Version: 1.4.7
 Summary: A library for canvas operations using pygame
 Home-page: https://x.com/gioseaxmc
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 
 Canvas
@@ -20,25 +20,18 @@
 Usage
 Installation
 To use Canvas, you'll need Python installed on your system along with the Pygame library. You can install Pygame using pip:
 
 
 pip install pygame
 
-Example Usage
+# Example Usage
 Here's a simple example demonstrating how to use Canvas to create a window and display a sprite:
 
-import canvas as c
+import pygame_canvas as c
 
-# Initialize window
-c.window(title="My Game")
+c.default_template(__file__)
 
-# Create sprite
-sprite = c.sprite(images=[c.rectangle(50, 50, (0, 200, 255))], pos=(240, 180))
-
-# Main game loop
-while c.loop(60):
-    # Update game logic here
-    pass
+The code above will load a default template into the main python script OVERWRITING EVERYTHING ELSE
 
 Documentation
 For detailed documentation and usage examples, refer to the Canvas documentation at: https://docs.google.com/document/d/18SMSY5RbigaOX2WOaGQs0iEUvSFnpfpWjsBxBNwq0nA/edit?usp=sharing.
```

### Comparing `pygame_canvas-1.4.6/setup.py` & `pygame_canvas-1.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_desc = fh.read()
 
 setup(
     name='pygame_canvas',
-    version='1.4.6',
+    version='1.4.7',
     packages=find_packages(),
     include_package_data=True,
     description='A library for canvas operations using pygame',
     long_description=long_desc,
     long_description_content_type='text/markdown',
     url='https://x.com/gioseaxmc',
     install_requires=[
```

