# Comparing `tmp/sanghyunjo-1.1.0.tar.gz` & `tmp/sanghyunjo-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\sanghyunjo-1.1.0.tar", last modified: Mon May 20 07:11:26 2024, max compression
+gzip compressed data, was "dist\sanghyunjo-1.2.0.tar", last modified: Tue May 21 03:00:41 2024, max compression
```

## Comparing `sanghyunjo-1.1.0.tar` & `sanghyunjo-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 07:11:26.869385 sanghyunjo-1.1.0/
--rw-rw-rw-   0        0        0     1087 2024-05-16 07:32:54.000000 sanghyunjo-1.1.0/LICENSE
--rw-rw-rw-   0        0        0       53 2024-05-16 07:24:52.000000 sanghyunjo-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      365 2024-05-20 07:11:26.868386 sanghyunjo-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1029 2024-05-16 07:32:26.000000 sanghyunjo-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 07:11:26.846438 sanghyunjo-1.1.0/sanghyunjo/
--rw-rw-rw-   0        0        0      188 2024-05-20 07:11:20.000000 sanghyunjo-1.1.0/sanghyunjo/__init__.py
--rw-rw-rw-   0        0        0     8772 2024-05-20 07:10:55.000000 sanghyunjo-1.1.0/sanghyunjo/cv.py
-drwxrwxrwx   0        0        0        0 2024-05-20 07:11:26.866391 sanghyunjo-1.1.0/sanghyunjo/fonts/
--rw-rw-rw-   0        0        0    34888 2023-07-19 08:59:35.000000 sanghyunjo-1.1.0/sanghyunjo/fonts/Times New Roman MT Std.otf
--rw-rw-rw-   0        0        0      358 2024-05-20 07:08:56.000000 sanghyunjo-1.1.0/sanghyunjo/json_utils.py
--rw-rw-rw-   0        0        0     2795 2024-05-16 07:13:32.000000 sanghyunjo-1.1.0/sanghyunjo/misc.py
-drwxrwxrwx   0        0        0        0 2024-05-20 07:11:26.867389 sanghyunjo-1.1.0/sanghyunjo.egg-info/
--rw-rw-rw-   0        0        0      365 2024-05-20 07:11:26.000000 sanghyunjo-1.1.0/sanghyunjo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-05-20 07:11:26.000000 sanghyunjo-1.1.0/sanghyunjo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 07:11:26.000000 sanghyunjo-1.1.0/sanghyunjo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-16 07:28:15.000000 sanghyunjo-1.1.0/sanghyunjo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       11 2024-05-20 07:11:26.000000 sanghyunjo-1.1.0/sanghyunjo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 07:11:26.869385 sanghyunjo-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      828 2024-05-20 07:09:32.000000 sanghyunjo-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 03:00:41.531730 sanghyunjo-1.2.0/
+-rw-rw-rw-   0        0        0     1087 2024-05-16 07:32:54.000000 sanghyunjo-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0       53 2024-05-16 07:24:52.000000 sanghyunjo-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      365 2024-05-21 03:00:41.530736 sanghyunjo-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1029 2024-05-16 07:32:26.000000 sanghyunjo-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 03:00:41.510429 sanghyunjo-1.2.0/sanghyunjo/
+-rw-rw-rw-   0        0        0      194 2024-05-21 03:00:35.000000 sanghyunjo-1.2.0/sanghyunjo/__init__.py
+-rw-rw-rw-   0        0        0     9124 2024-05-21 02:58:48.000000 sanghyunjo-1.2.0/sanghyunjo/cv_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-21 03:00:41.521399 sanghyunjo-1.2.0/sanghyunjo/fonts/
+-rw-rw-rw-   0        0        0    34888 2023-07-19 08:59:35.000000 sanghyunjo-1.2.0/sanghyunjo/fonts/Times New Roman MT Std.otf
+-rw-rw-rw-   0        0        0      358 2024-05-20 07:08:56.000000 sanghyunjo-1.2.0/sanghyunjo/json_utils.py
+-rw-rw-rw-   0        0        0     3046 2024-05-21 01:07:13.000000 sanghyunjo-1.2.0/sanghyunjo/misc.py
+drwxrwxrwx   0        0        0        0 2024-05-21 03:00:41.522396 sanghyunjo-1.2.0/sanghyunjo.egg-info/
+-rw-rw-rw-   0        0        0      365 2024-05-21 03:00:41.000000 sanghyunjo-1.2.0/sanghyunjo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2024-05-21 03:00:41.000000 sanghyunjo-1.2.0/sanghyunjo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 03:00:41.000000 sanghyunjo-1.2.0/sanghyunjo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-05-16 07:28:15.000000 sanghyunjo-1.2.0/sanghyunjo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       11 2024-05-21 03:00:41.000000 sanghyunjo-1.2.0/sanghyunjo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 03:00:41.531730 sanghyunjo-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      828 2024-05-20 07:09:32.000000 sanghyunjo-1.2.0/setup.py
```

### Comparing `sanghyunjo-1.1.0/LICENSE` & `sanghyunjo-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.1.0/README.md` & `sanghyunjo-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.1.0/sanghyunjo/cv.py` & `sanghyunjo-1.2.0/sanghyunjo/cv_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,14 +171,17 @@
     drw = ImageDraw.Draw(pillow_image)
     drw.ellipse(
         [(x-size, y-size), (x+size, y+size)], 
         (b, g, r, 0), (eb, eg, er, 0), edge_size
     )
     image[:, :, :] = np.asarray(pillow_image)
 
+def draw_rect(image, xyxy, color=(79, 244, 255), thickness=1):
+    cv2.rectangle(image, tuple(xyxy[:2]), tuple(xyxy[2:]), color, thickness)
+
 def show_image(winname, image, wait=-1, title=''):
     cv2.imshow(winname, image)
 
     if len(title) > 0:
         cv2.setWindowTitle(winname, title)
 
     key = None
@@ -276,8 +279,17 @@
         )
 
     def __call__(self, frame):
         self.writer.write(frame)
         
     def close(self):
         self.writer.release()
-        self.writer = None
+        self.writer = None
+
+def vstack(images):
+    return np.concatenate(images, axis=0)
+
+def hstack(images):
+    return np.concatenate(images, axis=1)
+
+def gray2bgr(image):
+    return cv2.cvtColor(image, cv2.COLOR_GRAY2BGR)
```

### Comparing `sanghyunjo-1.1.0/sanghyunjo/fonts/Times New Roman MT Std.otf` & `sanghyunjo-1.2.0/sanghyunjo/fonts/Times New Roman MT Std.otf`

 * *Files identical despite different names*

### Comparing `sanghyunjo-1.1.0/sanghyunjo/misc.py` & `sanghyunjo-1.2.0/sanghyunjo/misc.py`

 * *Files 12% similar despite different names*

```diff
@@ -52,19 +52,25 @@
     def __init__(self):
         self.start = time.time()
 
     def __enter__(self):
         self.start = time.time()
         return self
     
-    def get(self):
+    def get(self, duration='milliseconds'):
         end = time.time()
         interval = end - self.start
-
-        # print(interval, self.start, end)
+        
+        if duration is not None:
+            if duration == 'seconds':
+                interval = f'{int(interval)}s'
+            elif duration == 'milliseconds':
+                interval = f'{int(interval*1000)}ms'
+            else:
+                pass
         
         self.start = end
         return interval
     
     def __exit__(self, _type, _value, _trackback):
         pass
```

### Comparing `sanghyunjo-1.1.0/setup.py` & `sanghyunjo-1.2.0/setup.py`

 * *Files identical despite different names*

