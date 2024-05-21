# Comparing `tmp/fisspy-1.1.1.tar.gz` & `tmp/fisspy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fisspy-1.1.1.tar", last modified: Fri May  3 00:39:10 2024, max compression
+gzip compressed data, was "fisspy-1.1.2.tar", last modified: Tue May 21 11:01:10 2024, max compression
```

## Comparing `fisspy-1.1.1.tar` & `fisspy-1.1.2.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.677339 fisspy-1.1.1/
--rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.1.1/LICENSE.txt
--rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-03 00:39:10.677159 fisspy-1.1.1/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.1.1/README.md
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.672242 fisspy-1.1.1/fisspy/
--rw-r--r--   0 jhkang     (501) staff       (20)      430 2024-05-03 00:37:44.000000 fisspy-1.1.1/fisspy/__init__.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.673250 fisspy-1.1.1/fisspy/align/
--rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/align/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15179 2024-04-24 08:05:01.000000 fisspy-1.1.1/fisspy/align/alignment.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-25 11:40:56.000000 fisspy-1.1.1/fisspy/align/base.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.674174 fisspy-1.1.1/fisspy/analysis/
--rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/analysis/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-25 11:37:49.000000 fisspy-1.1.1/fisspy/analysis/doppler.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/analysis/filter.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-25 11:30:36.000000 fisspy-1.1.1/fisspy/analysis/forecast.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/analysis/ofe.py
--rw-r--r--   0 jhkang     (501) staff       (20)    35498 2024-04-25 11:29:47.000000 fisspy-1.1.1/fisspy/analysis/tdmap.py
--rw-r--r--   0 jhkang     (501) staff       (20)    33907 2024-04-25 11:35:30.000000 fisspy-1.1.1/fisspy/analysis/wavelet.py
--rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.1.1/fisspy/cm.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.674617 fisspy-1.1.1/fisspy/correction/
--rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/correction/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-05-01 13:33:13.000000 fisspy-1.1.1/fisspy/correction/correction.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-30 00:59:33.000000 fisspy-1.1.1/fisspy/correction/get_inform.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.675064 fisspy-1.1.1/fisspy/data/
--rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.1.1/fisspy/data/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.1.1/fisspy/data/_sample.py
--rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.1.1/fisspy/data/download.py
--rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.1.1/fisspy/data/sample.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.675430 fisspy-1.1.1/fisspy/image/
--rw-r--r--   0 jhkang     (501) staff       (20)       73 2024-04-25 10:45:58.000000 fisspy-1.1.1/fisspy/image/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    30375 2024-05-03 00:32:43.000000 fisspy-1.1.1/fisspy/image/interactive_image.py
--rw-r--r--   0 jhkang     (501) staff       (20)    12849 2024-05-01 06:38:35.000000 fisspy-1.1.1/fisspy/image/raster_set.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.675673 fisspy-1.1.1/fisspy/inversion/
--rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/inversion/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/inversion/_mlsi.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.675890 fisspy-1.1.1/fisspy/io/
--rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.1.1/fisspy/io/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.1.1/fisspy/io/read.py
--rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/makevideo.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.676504 fisspy-1.1.1/fisspy/preprocess/
--rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/preprocess/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    52752 2024-04-27 05:54:30.000000 fisspy-1.1.1/fisspy/preprocess/proc_base.py
--rw-r--r--   0 jhkang     (501) staff       (20)   146937 2024-04-27 10:55:16.000000 fisspy-1.1.1/fisspy/preprocess/proc_gui.py
--rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/preprocess/t_y_sh.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.676874 fisspy-1.1.1/fisspy/read/
--rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.1.1/fisspy/read/__init__.py
--rw-r--r--   0 jhkang     (501) staff       (20)    50267 2024-05-01 14:11:45.000000 fisspy-1.1.1/fisspy/read/read_factory.py
--rw-r--r--   0 jhkang     (501) staff       (20)     6847 2024-04-25 06:03:54.000000 fisspy-1.1.1/fisspy/read/readbase.py
-drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-03 00:39:10.672880 fisspy-1.1.1/fisspy.egg-info/
--rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-03 00:39:10.000000 fisspy-1.1.1/fisspy.egg-info/PKG-INFO
--rw-r--r--   0 jhkang     (501) staff       (20)     1079 2024-05-03 00:39:10.000000 fisspy-1.1.1/fisspy.egg-info/SOURCES.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-03 00:39:10.000000 fisspy-1.1.1/fisspy.egg-info/dependency_links.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-03 00:39:10.000000 fisspy-1.1.1/fisspy.egg-info/not-zip-safe
--rw-r--r--   0 jhkang     (501) staff       (20)      137 2024-05-03 00:39:10.000000 fisspy-1.1.1/fisspy.egg-info/requires.txt
--rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-05-03 00:39:10.000000 fisspy-1.1.1/fisspy.egg-info/top_level.txt
--rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-05-03 00:39:10.677382 fisspy-1.1.1/setup.cfg
--rw-r--r--   0 jhkang     (501) staff       (20)      582 2024-05-03 00:37:41.000000 fisspy-1.1.1/setup.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.727981 fisspy-1.1.2/
+-rw-r--r--   0 jhkang     (501) staff       (20)     1305 2023-07-14 01:35:52.000000 fisspy-1.1.2/LICENSE.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-21 11:01:10.727778 fisspy-1.1.2/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1988 2024-04-23 12:48:39.000000 fisspy-1.1.2/README.md
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.719081 fisspy-1.1.2/fisspy/
+-rw-r--r--   0 jhkang     (501) staff       (20)      430 2024-05-21 10:57:52.000000 fisspy-1.1.2/fisspy/__init__.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.720480 fisspy-1.1.2/fisspy/align/
+-rw-r--r--   0 jhkang     (501) staff       (20)       44 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/align/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15179 2024-04-24 08:05:01.000000 fisspy-1.1.2/fisspy/align/alignment.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11470 2024-04-25 11:40:56.000000 fisspy-1.1.2/fisspy/align/base.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.721888 fisspy-1.1.2/fisspy/analysis/
+-rw-r--r--   0 jhkang     (501) staff       (20)      317 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/analysis/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12577 2024-04-25 11:37:49.000000 fisspy-1.1.2/fisspy/analysis/doppler.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1030 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/analysis/filter.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2988 2024-04-25 11:30:36.000000 fisspy-1.1.2/fisspy/analysis/forecast.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15224 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/analysis/ofe.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    35716 2024-05-21 10:49:50.000000 fisspy-1.1.2/fisspy/analysis/tdmap.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    33907 2024-04-25 11:35:30.000000 fisspy-1.1.2/fisspy/analysis/wavelet.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    19011 2023-07-14 01:35:52.000000 fisspy-1.1.2/fisspy/cm.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.722394 fisspy-1.1.2/fisspy/correction/
+-rw-r--r--   0 jhkang     (501) staff       (20)       51 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/correction/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    11372 2024-05-01 13:33:13.000000 fisspy-1.1.2/fisspy/correction/correction.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2337 2024-04-30 00:59:33.000000 fisspy-1.1.2/fisspy/correction/get_inform.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.723177 fisspy-1.1.2/fisspy/data/
+-rw-r--r--   0 jhkang     (501) staff       (20)       64 2023-07-25 08:49:17.000000 fisspy-1.1.2/fisspy/data/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1072 2023-07-25 08:49:17.000000 fisspy-1.1.2/fisspy/data/_sample.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     2965 2023-07-25 08:49:17.000000 fisspy-1.1.2/fisspy/data/download.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      394 2023-07-14 01:35:52.000000 fisspy-1.1.2/fisspy/data/sample.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.723830 fisspy-1.1.2/fisspy/image/
+-rw-r--r--   0 jhkang     (501) staff       (20)       73 2024-04-25 10:45:58.000000 fisspy-1.1.2/fisspy/image/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    30919 2024-05-21 08:38:40.000000 fisspy-1.1.2/fisspy/image/interactive_image.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    12849 2024-05-01 06:38:35.000000 fisspy-1.1.2/fisspy/image/raster_set.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.724056 fisspy-1.1.2/fisspy/inversion/
+-rw-r--r--   0 jhkang     (501) staff       (20)        0 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/inversion/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)      181 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/inversion/_mlsi.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.724524 fisspy-1.1.2/fisspy/io/
+-rw-r--r--   0 jhkang     (501) staff       (20)      320 2023-07-14 01:35:52.000000 fisspy-1.1.2/fisspy/io/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    15840 2023-07-14 01:35:52.000000 fisspy-1.1.2/fisspy/io/read.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     4974 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/makevideo.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.726820 fisspy-1.1.2/fisspy/preprocess/
+-rw-r--r--   0 jhkang     (501) staff       (20)       29 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/preprocess/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    55166 2024-05-21 00:20:39.000000 fisspy-1.1.2/fisspy/preprocess/proc_base.py
+-rw-r--r--   0 jhkang     (501) staff       (20)   151958 2024-05-21 03:46:35.000000 fisspy-1.1.2/fisspy/preprocess/proc_gui.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     1685 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/preprocess/t_y_sh.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.727522 fisspy-1.1.2/fisspy/read/
+-rw-r--r--   0 jhkang     (501) staff       (20)      195 2024-04-20 02:57:09.000000 fisspy-1.1.2/fisspy/read/__init__.py
+-rw-r--r--   0 jhkang     (501) staff       (20)    50279 2024-05-10 13:45:00.000000 fisspy-1.1.2/fisspy/read/read_factory.py
+-rw-r--r--   0 jhkang     (501) staff       (20)     6847 2024-04-25 06:03:54.000000 fisspy-1.1.2/fisspy/read/readbase.py
+drwxr-xr-x   0 jhkang     (501) staff       (20)        0 2024-05-21 11:01:10.719853 fisspy-1.1.2/fisspy.egg-info/
+-rw-r--r--   0 jhkang     (501) staff       (20)      574 2024-05-21 11:01:10.000000 fisspy-1.1.2/fisspy.egg-info/PKG-INFO
+-rw-r--r--   0 jhkang     (501) staff       (20)     1079 2024-05-21 11:01:10.000000 fisspy-1.1.2/fisspy.egg-info/SOURCES.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-21 11:01:10.000000 fisspy-1.1.2/fisspy.egg-info/dependency_links.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        1 2024-05-21 11:01:10.000000 fisspy-1.1.2/fisspy.egg-info/not-zip-safe
+-rw-r--r--   0 jhkang     (501) staff       (20)      137 2024-05-21 11:01:10.000000 fisspy-1.1.2/fisspy.egg-info/requires.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)        7 2024-05-21 11:01:10.000000 fisspy-1.1.2/fisspy.egg-info/top_level.txt
+-rw-r--r--   0 jhkang     (501) staff       (20)       38 2024-05-21 11:01:10.728020 fisspy-1.1.2/setup.cfg
+-rw-r--r--   0 jhkang     (501) staff       (20)      582 2024-05-21 10:59:23.000000 fisspy-1.1.2/setup.py
```

### Comparing `fisspy-1.1.1/LICENSE.txt` & `fisspy-1.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/PKG-INFO` & `fisspy-1.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisspy
-Version: 1.1.1
+Version: 1.1.2
 Summary: fisspy: Python analysis tools for GST/FISS
 Home-page: http://fiss.snu.ac.kr
 Author: Juhyung Kang
 Author-email: jhkang@astro.snu.ac.kr
 License: BSD-2
 Requires-Python: >=3.6
 License-File: LICENSE.txt
```

### Comparing `fisspy-1.1.1/README.md` & `fisspy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/align/alignment.py` & `fisspy-1.1.2/fisspy/align/alignment.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/align/base.py` & `fisspy-1.1.2/fisspy/align/base.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/analysis/doppler.py` & `fisspy-1.1.2/fisspy/analysis/doppler.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/analysis/filter.py` & `fisspy-1.1.2/fisspy/analysis/filter.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/analysis/forecast.py` & `fisspy-1.1.2/fisspy/analysis/forecast.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/analysis/ofe.py` & `fisspy-1.1.2/fisspy/analysis/ofe.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/analysis/tdmap.py` & `fisspy-1.1.2/fisspy/analysis/tdmap.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,14 +132,15 @@
         if self.clim is not None:
             self.im.set_clim(self.clim)
         self.ax.set_title('t = 0 (sec)')
         self.ax.set_xlabel('X (km)')
         self.ax.set_ylabel('Y (km)')
         self.fig.canvas.mpl_connect('key_press_event', self._onKey)
         self.fig.canvas.mpl_connect('motion_notify_event', self._circleHelp)
+        self.fig.canvas.mpl_connect('close_event', self._fclose)
         self.fig.tight_layout()
         self.fig.show()
 
     def _circleHelp(self, event):
         if event.inaxes == self.ax and len(self.slitPoint) == 1:
             if self.lplot is not None:
                 for ii in self.lplot:
@@ -274,14 +275,20 @@
 
     def clear_slit(self):
         lines = self.ax.get_lines()
         for l in lines:
             l.remove()
         self.fig.canvas.draw_idle()
 
+    def _fclose(self, event):
+        self.fig = None
+        if self.h_fig is not None:
+            plt.close(self.hfig)
+            self.h_fig = None
+
     def _onKey(self, event):
         if event.key == 'left':
             self._prev()
         elif event.key == 'right':
             self._next()
         elif event.key == ' ' and event.inaxes == self.ax:
             if self.onSlit:
```

### Comparing `fisspy-1.1.1/fisspy/analysis/wavelet.py` & `fisspy-1.1.2/fisspy/analysis/wavelet.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/cm.py` & `fisspy-1.1.2/fisspy/cm.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/correction/correction.py` & `fisspy-1.1.2/fisspy/correction/correction.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/correction/get_inform.py` & `fisspy-1.1.2/fisspy/correction/get_inform.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/data/_sample.py` & `fisspy-1.1.2/fisspy/data/_sample.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/data/download.py` & `fisspy-1.1.2/fisspy/data/download.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/image/interactive_image.py` & `fisspy-1.1.2/fisspy/image/interactive_image.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         self.wvp = int((WV-self.mwv)/self.dwv+0.5)
         self.xp0 = self.xp
         self.yp0 = self.yp
         self.wvp0 = self.wvp
         self.xpH = self.xp
         self.ypH = self.yp
         self.wvpH = self.wvp
-
+        self.hfig = None
 
         #Keyboard helpBox
         if helpBox:
             helpFig = plt.figure('Keyboard Help Box', figsize=[3.5,3])
             ax = helpFig.add_subplot(111)
             ax.set_position([0,0,1,1])
             ax.set_axis_off()
@@ -106,14 +106,15 @@
             ax.text(0.05,0.5,'down: Move to down')
             ax.text(0.05,0.2,'spacebar: Change to current mouse point')
             ax.text(0.05,0.9,'ctrl/cmd+h: Reset to original setting position')
             ax.text(0.05,0.4,'ctrl/cmd+right: Increase the wavelength')
             ax.text(0.05,0.3,'ctrl/cmd+left: Decrease the wavelength')
             ax.text(0.05,0.1,'ctrl/cmd+b: Show previous point')
             helpFig.show()
+            self.hfig = helpFig
 
 
         #figure setting
         figsize = kwargs.pop('figsize', [15, 9])
         self.cmap = kwargs.pop('cmap', fiss.cmap)
         self.fig = plt.figure(figsize=figsize)
         # self.fig.canvas.set_window_title(self.band)
@@ -179,17 +180,23 @@
         self.vlineProfile = self.axProfile.axvline(self.wv, ls='dashed', c='b')
         self.vlineSpectro = self.axSpectro.axvline(self.wv, ls='dashed', c='lime')
         self.hlineSpectro = self.axSpectro.axhline(self.y, ls='dashed', c='lime')
         self.pointRaster = self.axRaster.scatter(self.x, self.y, 50, marker='x', color='r')
         self.axSpectro.set_aspect(adjustable='box', aspect='auto')
         self.fig.tight_layout()
         self.fig.canvas.mpl_connect('key_press_event', self._onKey)
-
+        self.fig.canvas.mpl_connect('close_event', self._fclose)
         self.fig.show()
 
+    def _fclose(self, event):
+        self.fig = None
+        if self.hfig is not None:
+            plt.close(self.hfig)
+            self.hfig = None
+
     def _onKey(self, event):
         if event.key == 'right':
             self.xp0 = self.xp
             self.yp0 = self.yp
             self.wvp0 = self.wvp
             if self.xp < self.nx-1:
                 self.xp += 1
@@ -470,14 +477,15 @@
         self.yp0 = self.yp
         self.wvpA0 = self.wvpA
         self.wvpB0 = self.wvpB
         self.xpH = self.xp
         self.ypH = self.yp
         self.wvpAH = self.wvpA
         self.wvpBH = self.wvpB
+        self.hfig = None
 
         #Keyboard helpBox
         if helpBox:
             helpFig = plt.figure('Keyboard Help Box', figsize=[5,3])
             ax = helpFig.add_subplot(111)
             ax.set_position([0,0,1,1])
             ax.set_axis_off()
@@ -488,14 +496,15 @@
             ax.text(0.05,0.52,'down: Move to down')
             ax.text(0.05,0.42,'ctrl/cmd+right: Increase the wavelength of the fissA')
             ax.text(0.05,0.32,'ctrl/cmd+left: Decrease the wavelength of the fissA')
             ax.text(0.05,0.22,'ctrl/cmd+up: Increase the wavelength of the fissB')
             ax.text(0.05,0.12,'ctrl/cmd+down: Decrease the wavelength of the fissB')
             ax.text(0.05,0.02,'spacebar: Change to current mouse point')
             helpFig.show()
+            self.hfig = helpFig
 
         #figure setting
         figsize = kwargs.pop('figsize', [12, 6])
         self.fig = plt.figure(figsize=figsize)
         # self.fig.canvas.set_window_title('Dual Band Image')
         self.imInterp = kwargs.get('interpolation', 'bilinear')
         gs = gridspec.GridSpec(2,4)
@@ -572,16 +581,23 @@
         #Reference
         self.vlineProfileA = self.axProfileA.axvline(self.wvA, ls='dashed', c='b')
         self.vlineProfileB = self.axProfileB.axvline(self.wvB, ls='dashed', c='b')
         self.pointRasterA = self.axRasterA.scatter(self.x, self.y, 50, marker='x', color='r')
         self.pointRasterB = self.axRasterB.scatter(self.x, self.y, 50, marker='x', color='r')
         self.fig.tight_layout()
         self.fig.canvas.mpl_connect('key_press_event', self._onKey)
+        self.fig.canvas.mpl_connect('close_event', self._fclose)
         self.fig.show()
 
+    def _fclose(self, event):
+        self.fig = None
+        if self.hfig is not None:
+            plt.close(self.hfig)
+            self.hfig = None
+
     def _onKey(self, event):
 
         if event.key == 'right':
             self.xp0 = self.xp
             self.yp0 = self.yp
             self.wvpA0 = self.wvpA
             self.wvpB0 = self.wvpB
```

### Comparing `fisspy-1.1.1/fisspy/image/raster_set.py` & `fisspy-1.1.2/fisspy/image/raster_set.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/io/read.py` & `fisspy-1.1.2/fisspy/io/read.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/makevideo.py` & `fisspy-1.1.2/fisspy/makevideo.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/preprocess/proc_base.py` & `fisspy-1.1.2/fisspy/preprocess/proc_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 from astropy.time import Time
 from scipy.signal import find_peaks
 from scipy.interpolate import interp1d
 from scipy.optimize import curve_fit
 from ..analysis.wavelet import Wavelet
 from scipy.fftpack import fft, ifft
 from urllib.request import urlretrieve
+from scipy.signal.windows import tukey
+from statsmodels.tsa.ar_model import AutoReg
+
 
 def fname2isot(f):
     """
     Translate the file name in to isot.
 
     Parameters
     ----------
@@ -139,59 +142,61 @@
         tdata = np.delete(tdata, np.arange(lmsk+minMsk[i], lmsk+maxMsk[i]), axis=axis)
         lmsk -= maxMsk[i] - minMsk[i]
         
     interp = interp1d(xt, tdata, axis=axis, kind=kind)
     mdata = interp(x)
     return mdata
 
-def cal_fringeGauss(wvlet, filterRange=[0,-1]):
+def cal_fringeGauss(wvlet, xc, hw):
     """
     axis: `int`, optional
         0, wavelet along the slit direction
     """
     shape = wvlet.wavelet.shape
     nwl = shape[1]
-    for i in range(2):
-        if filterRange[i] < 0:
-            filterRange[i] = nwl + filterRange[i]
-
+    
     x = np.arange(nwl)
-
-    pars = [None]*3
+    # sig = hw/np.sqrt(2/np.log(2))
+    sig = hw
+    p = [1, xc, sig]
+    GF = Gaussian(x, *p)
     
-    freq = np.arctan2(wvlet.wavelet.imag, wvlet.wavelet.real)
-    coeff = np.zeros((3, shape[0], shape[2]))
-    Awvlet = np.abs(wvlet.wavelet)
-    fringe_wvlet = np.zeros(shape, dtype=complex)
-
-    for ii in range(shape[0]):
-        # if ii % 10 == 0:
-        #     print(f"calculate {ii}-th row")
-        wh = None
-        for jj in range(shape[2]):
-            wv = Awvlet[ii,:,jj]
-            pars[0] = wv[filterRange[0]:filterRange[1]].max()
-            if wh is None:
-                wh = wv[filterRange[0]:filterRange[1]].argmax() + filterRange[0]
-            else:
-                wh = wv[wh-3:wh+3].argmax() + wh-3
-            pars[1] = wh
-            pars[2] = 2
-            try:
-                cp, cov = curve_fit(Gaussian, x[wh-5:wh+5], wv[wh-5:wh+5], p0=pars)
-                coeff[:,ii,jj] = cp
-            except:
-                print(f"catch err at {ii},:,{jj}")
-                return None
-
-    fringe_pwr = Gaussian(x[None,:,None], *coeff[:,:,None,:])
-    fringe_wvlet = fringe_pwr*(np.cos(freq)+1j*np.sin(freq))
-    fringe = wvlet.iwavelet(fringe_wvlet, wvlet.scale)
+    wv = wvlet.wavelet*GF[None,:,None]
+    mwv = np.abs(wv).mean((0,2))
+    return mwv, wvlet.iwavelet(wv, wvlet.scale)
+    # freq = np.arctan2(wvlet.wavelet.imag, wvlet.wavelet.real)
+    # coeff = np.zeros((3, shape[0], shape[2]))
+    # Awvlet = np.abs(wvlet.wavelet)
+    # fringe_wvlet = np.zeros(shape, dtype=complex)
+
+    # for ii in range(shape[0]):
+    #     # if ii % 10 == 0:
+    #     #     print(f"calculate {ii}-th row")
+    #     wh = None
+    #     for jj in range(shape[2]):
+    #         wv = Awvlet[ii,:,jj]
+    #         pars[0] = wv[filterRange[0]:filterRange[1]].max()
+    #         if wh is None:
+    #             wh = wv[filterRange[0]:filterRange[1]].argmax() + filterRange[0]
+    #         else:
+    #             wh = wv[wh-3:wh+3].argmax() + wh-3
+    #         pars[1] = wh
+    #         pars[2] = 2
+    #         try:
+    #             cp, cov = curve_fit(Gaussian, x[wh-5:wh+5], wv[wh-5:wh+5], p0=pars)
+    #             coeff[:,ii,jj] = cp
+    #         except:
+    #             print(f"catch err at {ii},:,{jj}")
+    #             return None
+
+    # fringe_pwr = Gaussian(x[None,:,None], *coeff[:,:,None,:])
+    # fringe_wvlet = fringe_pwr*(np.cos(freq)+1j*np.sin(freq))
+    # fringe = wvlet.iwavelet(fringe_wvlet, wvlet.scale)
 
-    return fringe
+    # return fringe
 
 def cal_fringeSimple(wvlet, filterRange):
     wavelet = wvlet.wavelet.copy()
     shape = wavelet.shape
     
     nwl = shape[1]
 
@@ -435,23 +440,24 @@
                     dwpk[pp,direction*(i+1) + ny//2] += dwpk[pp,direction*(i) + ny//2]
                     prof0 = prof
         dw[f] = np.median(dwpk,axis=0)
 
     dw = dw.mean(0)
 
     y = np.arange(ny)
-    p = np.polyfit(y[10:-10], dw[10:-10], 2)
+    p = np.polyfit(y[10:-10], dw[10:-10], 3)
 
     if show:
         fig, ax = plt.subplots(figsize=[6,4])
         wf = np.polyval(p, y)
         ax.scatter(y, dw, marker='+')
-        p1 = f"$+{p[1]:.2e}x$" if np.sign(p[1]) == 1 else f"${p[1]:.2e}x$"
-        p2 = f"$+{p[2]:.2e}" if np.sign(p[2]) == 1 else f"${p[2]:.2e}"
-        eq = f"$y = {p[0]:.2e}x^2${p1}{p2}"
+        p1 = f"$+{p[1]:.2e}x^2$" if np.sign(p[1]) == 1 else f"${p[1]:.2e}x^2$"
+        p2 = f"$+{p[2]:.2e}x&" if np.sign(p[2]) == 1 else f"${p[2]:.2e}x&"
+        p3 = f"$+{p[3]:.2e}" if np.sign(p[3]) == 1 else f"${p[3]:.2e}"
+        eq = f"$y = {p[0]:.2e}x^3${p1}{p2}{p3}"
         eq = eq.replace('e','^{')
         eq = eq.replace('x','}x')
         eq = eq + '}$'
         ax.plot(y, wf, color='r', label=eq)
         ax.set_xlabel('Slit (pix)')
         ax.set_ylabel('dw (pix)')
         ax.set_title('Curvature')
@@ -720,15 +726,15 @@
                 fig.canvas.manager.window.move(0,1080-350)
             except:
                 pass
             
         return Slit
 
 
-    def gain_calib(self, idata, maxiter=10, msk=None, show=False):
+    def gain_calib(self, idata, maxiter=10, msk=None, show=False, power=4, fsig=1.2):
         """
         Make the master flat following the technique decribed in Chae et al. (2013).
 
         Parameters
         ----------
         maxiter: `int`, optional
             Maximum number of iteration to repeat the calculation for creation master flat.
@@ -745,15 +751,15 @@
 
         if self.logF2 is None:
             logF =  self.logF
         else:
             logF = self.logF2
 
         if msk is None:
-            msk = getMask(10**logF, power=4)
+            msk = getMask(10**logF, power=power, fsig=fsig)
         self.msk = msk
         
         # self.rmFlat2 = self.rmFlat + self.mlf.max(0) # y direction vignetting is removed (that is not intended problems)
         tt = idata
         self.C = (tt*msk).sum((1,2))/msk.sum((1,2))
         self.C -= self.C.mean()
 
@@ -1444,28 +1450,39 @@
         spec = c[:,:,:NC].dot(Evec)
         spec *= 10**c[:,:,-1][:,:,None]
         if Eval is None:
             return Evec, spec, odata
         else:
             return Evec, spec, odata, Eval[NC]
 
+
 def yf2sp(yf, tolRate=1):
     """
     Calculate the slit pattern using the y-directional Fringe pattern
     """
     d2y = np.gradient(np.gradient(yf,axis=0), axis=0).mean(1)
     pks = find_peaks(d2y[5:-5], d2y[5:-5].std()*tolRate)[0]+5
     myf = data_mask_and_fill(yf, [pks-1,pks+2], axis=0, kind='slinear')
     s1 = myf[:,5:-5].mean(1)[:,None]
     sp = yf-myf+s1
     fsp = fft(sp, axis=1)
     fsp[:,10:-9] = 0
     sp = ifft(fsp,axis=1).real
     return sp
 
+def yf2sp_poly(lyf, order=3):
+    data2 = lyf.T
+        
+    ny = data2.shape[0]
+    par = np.polyfit(np.arange(ny), data2, order)
+    y = np.arange(ny)
+    sp = polyval2D(par, y)
+    sp = sp.T
+        
+    return sp
 
 def raw2sp(raw, pks):
     mr = np.log10(raw.mean(0))
     mr = np.nan_to_num(mr, True, 1,1,1)
     mRaw = mr - mr[5:-5].mean(0)
     ft = fft(mRaw, axis=0)
     ft[:10] = 0
@@ -1496,26 +1513,68 @@
     sp = tt-mskTT
     fsp = fft(sp, axis=1)
     fsp[:,10:-9] = 0
     sp = ifft(fsp,axis=1).real
     sp -= sp[5:-5,5:-5].mean()
     return 10**sp
 
+def raw2sp_poly(raw, pks):
+    mr = np.log10(raw.mean(0))
+    mr = np.nan_to_num(mr, True, 1,1,1)
+    k = detrending(mr)
+    shape = k.shape
+    mk = np.median(k[:, 5:-5], 1)
+    yy = np.arange(shape[0])
+    x = mk[pks-2]
+    y = yy[pks-2]
+    for i in range(-1,3):
+        x = np.append(x,mk[pks+i])
+        y = np.append(y,yy[pks+i])
+    idx = y[x.argmin()]
+    xx = np.arange(shape[1])
+    coef = np.polyfit(xx[5:-5], k[idx,5:-5],1)
+    kkf = np.polyval(coef, xx)
+    tmp = k[idx,5:-5] - kkf[5:-5]
+    val = tmp.mean()+tmp.std()
+    wh = tmp > val
+    xx = np.arange(shape[1]-10)
+    ct = xx[len(xx)//2]+5
+    hw = int(len(xx[wh])*1.5 // 2)
+    mm = ct-hw
+    mM = ct+hw
+    tt = data_mask_and_fill(k, [[mm],[mM]], axis=1, kind='slinear')
+    mskTT = data_mask_and_fill(tt, [pks-1,pks+2], axis=0, kind='slinear')
+    sp = tt-mskTT
+    sp = yf2sp_poly(sp)
+    sp -= sp[5:-5,5:-5].mean()
+    return 10**sp
 
 def rawYF(sraw, aws):
     mr = np.log10(sraw.mean(0))
     mr = np.nan_to_num(mr, True, 1,1,1)
     mRaw = mr - mr[5:-5].mean(0) - mr[:, 5:-5].mean(1)[:, None]
     wvlet = Wavelet(mRaw, dt=1, axis=0)
     freq = np.arctan2(wvlet.wavelet.imag, wvlet.wavelet.real)
     wvs = aws*(np.cos(freq) + 1j*np.sin(freq))
     fringe = wvlet.iwavelet(wvs, wvlet.scale)
     fringe -= fringe[5:-5,5:-5].mean()
     return 10**fringe.T
 
+def rawYF2(sraw, aws):
+    mr = np.log10(sraw.mean(0))
+    mr = np.nan_to_num(mr, True, 1,1,1)
+    tmp = detrending(mr)
+    mRaw = detrending(tmp,1)
+    wvlet = Wavelet(mRaw, dt=1, axis=0)
+    freq = np.arctan2(wvlet.wavelet.imag, wvlet.wavelet.real)
+    wvs = aws*(np.cos(freq) + 1j*np.sin(freq))
+    fringe = wvlet.iwavelet(wvs, wvlet.scale)
+    fringe -= fringe[5:-5,5:-5].mean()
+    return 10**fringe.T
+
 def YFart_correction(yf):
     syf = np.zeros(yf.shape)
     sp = np.zeros(yf.shape)
     for i, el in enumerate(yf):
         sp[i] = yf2sp(el)
         syf[i] = el - sp[i]
         wvl = Wavelet(syf[i], dt=1, axis=0)
@@ -1573,7 +1632,31 @@
     else:
         pp = tpks[tpks <= mx+5]
     if pp.size:
         spks = np.append(spks, pp)
     
     return ssp, spks
 
+def polyval2D(par, x):
+    y = np.zeros((len(x), par.shape[1]))
+    for p in par:
+        y = y*x[:,None]+p
+    return y
+
+def detrending(data, axis=0, order=7, alpha=0.01):
+    if axis == 0:
+        data2 = data.copy()
+    elif axis == 1:
+        data2 = data.T
+        
+    ny = data2.shape[0]
+    par = np.polyfit(np.arange(ny), data2, order)
+    w = tukey(ny, alpha=alpha)
+    y = np.arange(ny)
+    cdata = polyval2D(par, y)
+    rdata = data2-cdata
+    rdata *= w[:,None]
+
+    if axis == 1:
+        rdata = rdata.T
+        
+    return rdata
```

### Comparing `fisspy-1.1.1/fisspy/preprocess/proc_gui.py` & `fisspy-1.1.2/fisspy/preprocess/proc_gui.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,16 @@
         self.fflatGBL = [None] * len(self.fflatL)
 
         self.xFringe = None
         self.yFringe = None
         self.p_s7_comp = None
         self.p_s7_prof = None
         self.stop = False
+        self.pwvGx = None
+        self.xGauss = False
 
         for i,f in enumerate(self.fflatL):
             self.fflatGBL[i] = basename(f)
 
         self.fflatL.sort()
         self.stepNum = 0
         self.subStepNum = -1
@@ -502,44 +504,57 @@
             self.LE_s2_p1.setStyleSheet(f"background-color: {self.bg_second}; border: 1px solid {self.font_normal};")
             self.LE_s2_p1.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
 
             self.L_s2_p2 = QtWidgets.QLabel()
             self.L_s2_p2.setText("p2: ")
             self.L_s2_p2.setFont(self.fNormal)
 
+            self.L_s2_p3 = QtWidgets.QLabel()
+            self.L_s2_p3.setText("p3: ")
+            self.L_s2_p3.setFont(self.fNormal)
+
             self.LE_s2_p2 = QtWidgets.QLineEdit()
             self.LE_s2_p2.setText("0")
             self.LE_s2_p2.setStyleSheet(f"background-color: {self.bg_second}; border: 1px solid {self.font_normal};")
             self.LE_s2_p2.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
 
+            self.LE_s2_p3 = QtWidgets.QLineEdit()
+            self.LE_s2_p3.setText("0")
+            self.LE_s2_p3.setStyleSheet(f"background-color: {self.bg_second}; border: 1px solid {self.font_normal};")
+            self.LE_s2_p3.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+
             self.B_s2_Apply = QtWidgets.QPushButton()
             self.B_s2_Apply.setText("Apply")
             self.B_s2_Apply.setFont(self.fNormal)
             self.B_s2_Apply.setStyleSheet(f"background-color: {self.bg_second};")
 
             self.HL_s2_p0 = QtWidgets.QHBoxLayout()
             self.HL_s2_p1 = QtWidgets.QHBoxLayout()
             self.HL_s2_p2 = QtWidgets.QHBoxLayout()
+            self.HL_s2_p3 = QtWidgets.QHBoxLayout()
             
             self.HL_s2_p0.addWidget(self.L_s2_p0)
             self.HL_s2_p0.addWidget(self.LE_s2_p0)
             self.HL_s2_p1.addWidget(self.L_s2_p1)
             self.HL_s2_p1.addWidget(self.LE_s2_p1)
             self.HL_s2_p2.addWidget(self.L_s2_p2)
             self.HL_s2_p2.addWidget(self.LE_s2_p2)
+            self.HL_s2_p3.addWidget(self.L_s2_p3)
+            self.HL_s2_p3.addWidget(self.LE_s2_p3)
 
             self.VL_s2.addLayout(self.HL0_s2)
             self.VL_s2.addLayout(self.HL_s2_p0)
             self.VL_s2.addLayout(self.HL_s2_p1)
             self.VL_s2.addLayout(self.HL_s2_p2)
+            self.VL_s2.addLayout(self.HL_s2_p3)
             self.VL_s2.addWidget(self.B_s2_Apply)
 
             self.vboxCtrl.addLayout(self.VL_s2)
 
-            self.StepWidgets[2] = [self.L_s2_get_curve, self.B_s2_run, self.L_s2_p0, self.LE_s2_p0, self.L_s2_p1, self.LE_s2_p1, self.L_s2_p2, self.LE_s2_p2, self.B_s2_Apply]
+            self.StepWidgets[2] = [self.L_s2_get_curve, self.B_s2_run, self.L_s2_p0, self.LE_s2_p0, self.L_s2_p1, self.LE_s2_p1, self.L_s2_p2, self.LE_s2_p2, self.L_s2_p3, self.LE_s2_p3, self.B_s2_Apply]
 
             self.B_s2_run.clicked.connect(self.s2_Run)
             self.B_s2_Apply.clicked.connect(self.s2_Apply)
 
             self.B_s2_Apply.setEnabled(False)
 
         # create Step3-1 atlas subtraction
@@ -923,22 +938,22 @@
             self.L_s3_4_calFringe.setText("Calculate Fringe:")
             self.L_s3_4_calFringe.setFont(self.fNormal)
 
             self.HL_xFringe = QtWidgets.QHBoxLayout()
             self.B_s3_4_simple = QtWidgets.QPushButton()
             self.B_s3_4_simple.setText("Cal (simple)")
             self.B_s3_4_simple.setFont(self.fNormal)
-            self.B_s3_4_simple.setStyleSheet(f"background-color: {self.btn_1}; color:{self.bg_primary};")
+            self.B_s3_4_simple.setStyleSheet(f"background-color: {self.bg_second};")
             self.B_s3_4_simple.clicked.connect(self.s3_4_simple)
             self.B_s3_4_simple.setEnabled(False)
 
             self.B_s3_4_gauss = QtWidgets.QPushButton()
             self.B_s3_4_gauss.setText("Cal (Gauss)")
             self.B_s3_4_gauss.setFont(self.fNormal)
-            self.B_s3_4_gauss.setStyleSheet(f"background-color: {self.bg_second};")
+            self.B_s3_4_gauss.setStyleSheet(f"background-color: {self.btn_1}; color:{self.bg_primary};")
             self.B_s3_4_gauss.clicked.connect(self.s3_4_gauss)
             self.B_s3_4_gauss.setEnabled(False)
 
             self.B_s3_4_FringeShow = QtWidgets.QPushButton()
             self.B_s3_4_FringeShow.setText("Show")
             self.B_s3_4_FringeShow.setFont(self.fNormal)
             self.B_s3_4_FringeShow.setStyleSheet(f"background-color: {self.bg_second};")
@@ -1069,53 +1084,87 @@
             self.LE_s4_p1.setStyleSheet(f"background-color: {self.bg_second}; border: 1px solid {self.font_normal};")
             self.LE_s4_p1.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
 
             self.L_s4_p2 = QtWidgets.QLabel()
             self.L_s4_p2.setText("p2: ")
             self.L_s4_p2.setFont(self.fNormal)
 
+            self.L_s4_p3 = QtWidgets.QLabel()
+            self.L_s4_p3.setText("p3: ")
+            self.L_s4_p3.setFont(self.fNormal)
+
             self.LE_s4_p2 = QtWidgets.QLineEdit()
             self.LE_s4_p2.setText("0")
             self.LE_s4_p2.setStyleSheet(f"background-color: {self.bg_second}; border: 1px solid {self.font_normal};")
             self.LE_s4_p2.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
 
+            self.LE_s4_p3 = QtWidgets.QLineEdit()
+            self.LE_s4_p3.setText("0")
+            self.LE_s4_p3.setStyleSheet(f"background-color: {self.bg_second}; border: 1px solid {self.font_normal};")
+            self.LE_s4_p3.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+
             self.B_s4_Apply = QtWidgets.QPushButton()
             self.B_s4_Apply.setText("Apply")
             self.B_s4_Apply.setFont(self.fNormal)
             self.B_s4_Apply.setStyleSheet(f"background-color: {self.bg_second};")
             self.B_s4_Apply.setEnabled(False)
 
             self.HL_s4_p0 = QtWidgets.QHBoxLayout()
             self.HL_s4_p1 = QtWidgets.QHBoxLayout()
             self.HL_s4_p2 = QtWidgets.QHBoxLayout()
+            self.HL_s4_p3 = QtWidgets.QHBoxLayout()
             
             self.HL_s4_p0.addWidget(self.L_s4_p0)
             self.HL_s4_p0.addWidget(self.LE_s4_p0)
             self.HL_s4_p1.addWidget(self.L_s4_p1)
             self.HL_s4_p1.addWidget(self.LE_s4_p1)
             self.HL_s4_p2.addWidget(self.L_s4_p2)
             self.HL_s4_p2.addWidget(self.LE_s4_p2)
+            self.HL_s4_p3.addWidget(self.L_s4_p3)
+            self.HL_s4_p3.addWidget(self.LE_s4_p3)
 
             self.VL_s4.addLayout(self.HL0_s4)
             self.VL_s4.addLayout(self.HL_s4_p0)
             self.VL_s4.addLayout(self.HL_s4_p1)
             self.VL_s4.addLayout(self.HL_s4_p2)
+            self.VL_s4.addLayout(self.HL_s4_p3)
             self.VL_s4.addWidget(self.B_s4_Apply)
 
             self.vboxCtrl.addLayout(self.VL_s4)
 
-            self.StepWidgets[4] = [self.L_s4_get_curve, self.B_s4_run, self.L_s4_p0, self.LE_s4_p0, self.L_s4_p1, self.LE_s4_p1, self.L_s4_p2, self.LE_s4_p2, self.B_s4_Apply]
+            self.StepWidgets[4] = [self.L_s4_get_curve, self.B_s4_run, self.L_s4_p0, self.LE_s4_p0, self.L_s4_p1, self.LE_s4_p1, self.L_s4_p2, self.LE_s4_p2, self.L_s4_p3, self.LE_s4_p3, self.B_s4_Apply]
 
             self.B_s4_run.clicked.connect(self.s4_Run)
             self.B_s4_Apply.clicked.connect(self.s4_Apply)
 
         # create Step5 makeFlat
         if True:
             self.VL_s5  = QtWidgets.QVBoxLayout()
-            self.HL_s5  = QtWidgets.QHBoxLayout()
+            
+            self.HL_s5_par = QtWidgets.QHBoxLayout()
+            self.L_s5_pwr = QtWidgets.QLabel()
+            self.L_s5_pwr.setText("power: ")
+            self.L_s5_pwr.setFont(self.fNormal)
+            self.LE_s5_pwr = QtWidgets.QLineEdit()
+            self.LE_s5_pwr.setText("4")
+            self.LE_s5_pwr.setStyleSheet(f"background-color: {self.bg_second}; border: 1px solid {self.font_normal};")
+            self.LE_s5_pwr.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+
+            self.L_s5_sig = QtWidgets.QLabel()
+            self.L_s5_sig.setText("sig: ")
+            self.L_s5_sig.setFont(self.fNormal)
+            self.LE_s5_sig = QtWidgets.QLineEdit()
+            self.LE_s5_sig.setText("1.2")
+            self.LE_s5_sig.setStyleSheet(f"background-color: {self.bg_second}; border: 1px solid {self.font_normal};")
+            self.LE_s5_sig.setAlignment(QtCore.Qt.AlignRight|QtCore.Qt.AlignTrailing|QtCore.Qt.AlignVCenter)
+
+            self.HL_s5_par.addWidget(self.L_s5_pwr)
+            self.HL_s5_par.addWidget(self.L_s5_sig)
+            self.HL_s5_par.addWidget(self.LE_s5_pwr)
+            self.HL_s5_par.addWidget(self.LE_s5_sig)
 
             self.L_s5_label = QtWidgets.QLabel()
             self.L_s5_label.setText("Make Flat: ")
             self.L_s5_label.setFont(self.fNormal)
             self.B_s5_Run = QtWidgets.QPushButton()
             self.B_s5_Run.setText("Run")
             self.B_s5_Run.setFont(self.fNormal)
@@ -1123,14 +1172,15 @@
             self.B_s5_Run.clicked.connect(self.s5_Run)
             self.B_s5_Show = QtWidgets.QPushButton()
             self.B_s5_Show.setText("Show")
             self.B_s5_Show.setFont(self.fNormal)
             self.B_s5_Show.setStyleSheet(f"background-color: {self.bg_second};")
             self.B_s5_Show.clicked.connect(self.s5_Show)
             
+            self.HL_s5  = QtWidgets.QHBoxLayout()
             self.HL_s5.addWidget(self.L_s5_label)
             self.HL_s5.addWidget(self.B_s5_Run)
             self.HL_s5.addWidget(self.B_s5_Show)
             self.B_s5_Show.setEnabled(False)
 
             self.HL_s5_cFlat = QtWidgets.QHBoxLayout()
             self.L_s5_cFlat = QtWidgets.QLabel()
@@ -1210,23 +1260,24 @@
 
             self.HL_s5_frame.addWidget(self.L_s5_frame)
             self.HL_s5_frame.addWidget(self.LE_s5_frame)
             self.HL_s5_frame.addWidget(self.L_s5_nframe)
             self.HL_s5_frame.addWidget(self.B_s5_pf)
             self.HL_s5_frame.addWidget(self.B_s5_nf)
             
+            self.VL_s5.addLayout(self.HL_s5_par)
             self.VL_s5.addLayout(self.HL_s5)
             self.VL_s5.addLayout(self.HL_s5_cFlat)
             self.VL_s5.addLayout(self.HL_s5_msFlat)
             self.VL_s5.addLayout(self.HL_s5_profile)
             self.VL_s5.addLayout(self.HL_s5_frame)
 
             self.vboxCtrl.addLayout(self.VL_s5)
 
-            self.StepWidgets[5] = [self.L_s5_label, self.B_s5_Run, self.B_s5_Show, self.L_s5_cFlat, self.B_s5_cFlat, self.B_s5_Blink, self.L_s5_msFlat, self.B_s5_msFlat, self.L_s5_profile, self.B_s5_profile, self.L_s5_frame, self.LE_s5_frame, self.L_s5_nframe, self.B_s5_pf, self.B_s5_nf]
+            self.StepWidgets[5] = [self.L_s5_label, self.B_s5_Run, self.B_s5_Show, self.L_s5_cFlat, self.B_s5_cFlat, self.B_s5_Blink, self.L_s5_msFlat, self.B_s5_msFlat, self.L_s5_profile, self.B_s5_profile, self.L_s5_frame, self.LE_s5_frame, self.L_s5_nframe, self.B_s5_pf, self.B_s5_nf, self.L_s5_pwr, self.L_s5_sig, self.LE_s5_pwr, self.LE_s5_sig]
 
         # create Step6 Save Flat
         if True:
             self.VL_s6 = QtWidgets.QVBoxLayout()
             self.HL_s6 = QtWidgets.QHBoxLayout()
 
             self.L_s6_save = QtWidgets.QLabel()
@@ -1644,15 +1695,15 @@
                 self.B_s3_4_simple.setEnabled(False)
                 self.B_s3_4_gauss.setEnabled(False)
                 self.B_s3_4_reset.setEnabled(False)
                 self.B_s3_4_FringeShow.setEnabled(False)
                 self.B_s3_4_resShow.setEnabled(False)
                 self.B_s3_4_blink.setEnabled(False)
                 self.s3_4_wvCal()
-                self.s3_4_simple()
+                self.s3_4_gauss()
                 self.B_Next.setEnabled(True)
                 self.B_Prev.setEnabled(True)
                 self.B_s3_4_wvCal.setEnabled(True)
                 self.B_s3_4_wvShow.setEnabled(True)
                 self.B_s3_4_FRapply.setEnabled(True)
                 self.B_s3_4_simple.setEnabled(True)
                 self.B_s3_4_gauss.setEnabled(True)
@@ -1770,31 +1821,33 @@
     def s2_Run(self):
         self.log += "> Calculate curvature coefficient automatically.<br>"
         self._writeLog()
         self.CF.coeff, self.dw = proc_base.get_curve_par(self.CF.rlRF)
         self.LE_s2_p0.setText(f"{self.CF.coeff[0]:.3e}")
         self.LE_s2_p1.setText(f"{self.CF.coeff[1]:.3e}")
         self.LE_s2_p2.setText(f"{self.CF.coeff[2]:.3e}")
+        self.LE_s2_p3.setText(f"{self.CF.coeff[3]:.3e}")
         self.log += f"> Done.<br>"
         self._writeLog()
         self.s2_make()
         self.B_s1_Apply.setEnabled(True)
     
     def s2_make(self):
         self.CF.logF, oimg, cimg, wh = proc_base.curvature_correction(self.CF.rlRF, self.CF.coeff, show=True)
 
         y = np.arange(self.CF.rlRF.shape[1])
         wf = np.polyval(self.CF.coeff, y)
 
         for ax in self.ax[2]:
             ax.cla()
 
-        p1 = f"$+{self.CF.coeff[1]:.2e}x$" if np.sign(self.CF.coeff[1]) == 1 else f"${self.CF.coeff[1]:.2e}x$"
-        p2 = f"$+{self.CF.coeff[2]:.2e}" if np.sign(self.CF.coeff[2]) == 1 else f"${self.CF.coeff[2]:.2e}"
-        eq = f"$y = {self.CF.coeff[0]:.2e}x^2${p1}{p2}"
+        p1 = f"$+{self.CF.coeff[1]:.2e}x^2$" if np.sign(self.CF.coeff[1]) == 1 else f"${self.CF.coeff[1]:.2e}x^2$"
+        p2 = f"$+{self.CF.coeff[2]:.2e}x$" if np.sign(self.CF.coeff[2]) == 1 else f"${self.CF.coeff[2]:.2e}x$"
+        p3 = f"$+{self.CF.coeff[3]:.2e}" if np.sign(self.CF.coeff[3]) == 1 else f"${self.CF.coeff[3]:.2e}"
+        eq = f"$y = {self.CF.coeff[0]:.2e}x^3${p1}{p2}{p3}"
         eq = eq.replace('e','^{')
         eq = eq.replace('x','}x')
         eq = eq + '}$'
         self.ax[2][0].scatter(y, self.dw, marker='+')
         self.ax[2][0].plot(y, wf, color='r', label=eq)
         self.ax[2][0].set_xlabel('Slit (pix)')
         self.ax[2][0].set_ylabel('dw (pix)')
@@ -1822,14 +1875,15 @@
 
     def s2_Apply(self):
         self.log += "> Apply coefficient.<br>"
         self._writeLog()
         self.CF.coeff[0] = float(self.LE_s2_p0.text())
         self.CF.coeff[1] = float(self.LE_s2_p1.text())
         self.CF.coeff[2] = float(self.LE_s2_p2.text())
+        self.CF.coeff[3] = float(self.LE_s2_p3.text())
         self.s2_make()
 
     def s3_1_Run(self):
         self.log += "> Run Atlas subtraction.<br>"
         self._writeLog()
 
         self.CF.atlas_subtraction()
@@ -1877,15 +1931,16 @@
 
     def s3_2_wvCal(self):
         self.log += "> Wavelet calculation.<br>"
         self._writeLog()
         self.wvlet_y = [None]*self.CF.nf
 
         for i in range(self.CF.nf):
-            self.wvlet_y[i] = Wavelet(self.CF.rmFlat[i], dt=1, axis=0, dj=0.05, param=12)
+            data = proc_base.detrending(self.CF.rmFlat[i])
+            self.wvlet_y[i] = Wavelet(data, dt=1, axis=0, dj=0.05, param=12)
 
         self.log += "> Done.<br>"
         self._writeLog()
         self.s3_2_wvShow()
         self.B_s3_wvShow.setEnabled(True)
         self.B_s3_2_FRapply.setEnabled(True)
         self.B_s3_2_simple.setEnabled(True)
@@ -2219,26 +2274,26 @@
         self.log += "> Wavelet calculation.<br>"
         self._writeLog()
         self.wvlet_x = [None]*self.CF.nf
         w = np.zeros(self.CF.nf)
         xwh = np.zeros(self.CF.nf, dtype=int)
         x = np.arange(14)
         for i in range(self.CF.nf):
-            self.wvlet_x[i] = Wavelet(self.ms1[i][5:-5,5:-5], dt=1, axis=1, dj=0.05, param=12)
+            dd = proc_base.detrending(self.ms1[i][5:-5,5:-5], 1)
+            self.wvlet_x[i] = Wavelet(dd, dt=1, axis=1, dj=0.05, param=12)
             data = np.abs(self.wvlet_x[i].wavelet).mean((0,2))
             xwh[i] = data[:-25].argmax()
             hmax = data[:-25].max()/2
             t = x[data[xwh[i]-7:xwh[i]+7] >= hmax]
             w[i] = (t.max() - t.min())/2
 
-        self.xF_hw = int(w.mean()*3)
+        self.xF_hw = int(w.mean()*4)
         self.xF_c = int(xwh.mean())
-
-            
-
+        self.xf_min = self.xF_c - self.xF_hw
+        self.xf_max = self.xF_c + self.xF_hw
 
         self.log += "> Done.<br>"
         self._writeLog()
         self.s3_4_wvShow()
         self.B_s3_4_wvShow.setEnabled(True)
         self.B_s3_4_FRapply.setEnabled(True)
         self.B_s3_4_simple.setEnabled(True)
@@ -2247,14 +2302,16 @@
         self.xwvShow = True
         self.XFshow = False
         self.s2Show = False
         self.ax_sub[3][0].set_visible(True)
         self.ax_sub[3][1].set_visible(False)
         nfreq = self.wvlet_x[self.frameNum].wavelet.shape[1]
         self.ax_sub[3][0].cla()
+        self.pwvGx = None
+        
         data = np.abs(self.wvlet_x[self.frameNum].wavelet).mean((0,2))
         # xwh = data[:nfreq-20].argmax()
         self.xf_min = self.xF_c - self.xF_hw
         self.xf_max = self.xF_c + self.xF_hw
         self.LE_s3_4_FRmin.setText(f"{self.xf_min}")
         self.LE_s3_4_FRmax.setText(f"{self.xf_max}")
         ymax = data[:nfreq-10].max()*1.1
@@ -2262,32 +2319,48 @@
         self.ax_sub[3][0].set_ylim(0,ymax)
         self.ax_sub[3][0].set_xlim(-0.5, nfreq-1)
         self.ax_sub[3][0].set_xlabel('Freq_x (pix)')
         self.ax_sub[3][0].set_ylabel('Amplitude')
         self.ax_sub[3][0].set_title('Averaged Wavelet Spectrum (x-dir)')
         self.pFRmin_x = self.ax_sub[3][0].plot([self.xf_min, self.xf_min], [0, ymax], color='r', ls='dashed')[0]
         self.pFRmax_x = self.ax_sub[3][0].plot([self.xf_max, self.xf_max], [0, ymax], color='r', ls='dashed')[0]
+        if self.xGauss:
+            if self.pwvGx is None:
+                self.pwvGx = self.ax_sub[3][0].plot(self.xF_mwv[self.frameNum])[0]
+            else:
+                self.pwvGx.set_ydata(self.xF_mwv[self.frameNum])
         self.fig.canvas.draw_idle()
 
     def s3_4_FRapply(self):
         self.xf_min = int(self.LE_s3_4_FRmin.text())
         self.xf_max = int(self.LE_s3_4_FRmax.text())
+        self.xF_hw = int((self.xf_max-self.xf_min)/2)
+        xwh = np.zeros(self.CF.nf, dtype=int)
+        for i in range(self.CF.nf):
+            data = np.abs(self.wvlet_x[i].wavelet).mean((0,2))
+            xwh[i] = data[self.xf_min:self.xf_max].argmax() + self.xf_min
+        self.xF_c = int(xwh.mean())
+            
+            
         self.pFRmin_x.set_xdata([self.xf_min, self.xf_min])
         self.pFRmax_x.set_xdata([self.xf_max, self.xf_max])
         self.log += "> Change Frequency Range.<br>"
         self.log += "> Please press the calculate button again to apply this to Fringe pattern.<br>"
         self._writeLog()
 
     def s3_4_simple(self):
-        self.XFshow = True
-        self.xwvShow = False
+        # self.XFshow = True
+        # self.xwvShow = True
         self.log += "> Calculate Fringe Patterns in simple way.<br>"
         self._writeLog()
         self.xFringe = np.zeros([self.CF.nf,self.CF.ny,self.CF.nw])
         self.s2 = np.zeros((self.CF.nf, self.CF.ny, self.CF.nw))
+        if self.pwvGx is not None:
+            self.pwvGx.remove()
+            self.pwvGx = None
         for i in range(self.CF.nf):
             self.xFringe[i][5:-5,5:-5] = proc_base.cal_fringeSimple(self.wvlet_x[i], [self.xf_min, self.xf_max])
             self.xFringe[i][5:-5,5:-5] -= self.xFringe[i][5:-5,5:-5].mean()
             self.s2[i][5:-5,5:-5] = self.s1[i][5:-5,5:-5] - self.xFringe[i][5:-5,5:-5]
         self.log += "> Done.<br>"
         self._writeLog()
         if self.imFx is None:
@@ -2301,32 +2374,38 @@
             self.imFx.set_clim(self.xFringe[self.frameNum][5:-5,5:-5].min(),self.xFringe[self.frameNum].max())
         self.fig.canvas.draw_idle()
         self.B_s3_4_FringeShow.setEnabled(True)
         self.B_s3_4_resShow.setEnabled(True)
         self.B_s3_4_blink.setEnabled(True)
 
     def s3_4_gauss(self):
-        self.XFshow = True
-        self.log += "> Calculate Fringe Patterns by using gaussian fit.<br>"
+        # self.XFshow = True
+        # self.xwvShow = True
+        self.log += "> Calculate Fringe Patterns with using the Gaussian filter.<br>"
         self._writeLog()
-        self.xFringe = [None]*self.CF.nf
+        self.xFringe = np.zeros([self.CF.nf,self.CF.ny,self.CF.nw])
         self.s2 = np.zeros((self.CF.nf, self.CF.ny, self.CF.nw))
+        self.xF_mwv = [None]*self.CF.nf
         for i in range(self.CF.nf):
-            res = proc_base.cal_fringeGauss(self.wvlet_x[i], [self.xf_min, self.xf_max])
+            mwv, res = proc_base.cal_fringeGauss(self.wvlet_x[i], self.xF_c, self.xF_hw)
+            self.xF_mwv[i] = mwv
             if res is None:
                 self.log += f"> <font color='{self.font_err}'> Cannot Calculate Fringe Patterns by using gaussian fit.</font><br>"
                 self._writeLog()
                 return 0
             else:
-                self.xFringe[i] = res
-                self.log += f"> {i}-Frame Done.<br>"
-                self._writeLog()
-            self.s2[i][5:-5,5:-5] = self.s1[i][5:-5,5:-5] - self.xFringe[i]
+                self.xFringe[i][5:-5,5:-5] = res
+            self.s2[i][5:-5,5:-5] = self.s1[i][5:-5,5:-5] - self.xFringe[i][5:-5,5:-5]
         self.log += "> Done.<br>"
         self._writeLog()
+        self.xGauss = True
+        if self.pwvGx is None:
+            self.pwvGx = self.ax_sub[3][0].plot(self.xF_mwv[self.frameNum])[0]
+        else:
+            self.pwvGx.set_ydata(self.xF_mwv[self.frameNum])
         if self.imFx is None:
             self.imFx = self.ax_sub[3][1].imshow(self.xFringe[self.frameNum], plt.cm.gray, origin='lower')
             self.ax_sub[3][1].set_title('Fringe Pattern')
             self.ax_sub[3][1].set_xlabel('Wavelength (pix)')
             self.ax_sub[3][1].set_ylabel('Slit (pix)')
         else:
             self.ax_sub[3][1].set_title('Fringe Pattern')
@@ -2380,14 +2459,15 @@
         
         self.ms1 = self.s1.copy()
         self.s2 = None
         self.xFringe = None
 
         self.ax_sub[3][0].cla()
         self.ax_sub[3][1].cla()
+        self.pwvGx = None
 
         self.fig.canvas.draw_idle()
 
 
     def s3_4_pf(self):
         if self.frameNum <= 0:
             self.frameNum = 0
@@ -2419,14 +2499,19 @@
             data = self.s2[self.frameNum][5:-5,5:-5]
             self.imFx.set_data(data)
         elif self.xwvShow:
             self.ax_sub[3][0].set_visible(True)
             self.ax_sub[3][1].set_visible(False)
             data = np.abs(self.wvlet_x[self.frameNum].wavelet).mean((0,2))
             self.pwvx.set_ydata(data)
+            if self.xGauss:
+                if self.pwvGx is None:
+                    self.pwvGx = self.ax_sub[3][0].plot(self.xF_mwv[self.frameNum])[0]
+                else:
+                    self.pwvGx.set_ydata(self.xF_mwv[self.frameNum])
         else:
             data = self.CF.rmFlat[self.frameNum][5:-5,5:-5]
             self.imFx.set_data(data)
 
         self.fig.canvas.draw_idle()
 
     def s4_Run(self):
@@ -2436,30 +2521,32 @@
         else:
             self.FS_logF = self.CF.logF - self.yFringe - self.xFringe
         self._writeLog()
         self.CF.coeff2, self.dw2 = proc_base.get_curve_par(self.FS_logF)
         self.LE_s4_p0.setText(f"{self.CF.coeff2[0]:.3e}")
         self.LE_s4_p1.setText(f"{self.CF.coeff2[1]:.3e}")
         self.LE_s4_p2.setText(f"{self.CF.coeff2[2]:.3e}")
+        self.LE_s4_p3.setText(f"{self.CF.coeff2[3]:.3e}")
         self.s4_make()
         self.B_s4_Apply.setEnabled(True)
     
     def s4_make(self):
         
         self.CF.logF2, oimg, cimg, wh = proc_base.curvature_correction(self.FS_logF, self.CF.coeff2, show=True)
 
         y = np.arange(self.CF.rlRF.shape[1])
         wf = np.polyval(self.CF.coeff2, y)
 
         for ax in self.ax[4]:
             ax.cla()
 
-        p1 = f"$+{self.CF.coeff2[1]:.2e}x$" if np.sign(self.CF.coeff2[1]) == 1 else f"${self.CF.coeff2[1]:.2e}x$"
-        p2 = f"$+{self.CF.coeff2[2]:.2e}" if np.sign(self.CF.coeff2[2]) == 1 else f"${self.CF.coeff2[2]:.2e}"
-        eq = f"$y = {self.CF.coeff2[0]:.2e}x^2${p1}{p2}"
+        p1 = f"$+{self.CF.coeff2[1]:.2e}x^2$" if np.sign(self.CF.coeff2[1]) == 1 else f"${self.CF.coeff2[1]:.2e}x^2$"
+        p2 = f"$+{self.CF.coeff2[2]:.2e}x$" if np.sign(self.CF.coeff2[2]) == 1 else f"${self.CF.coeff2[2]:.2e}x$"
+        p3 = f"$+{self.CF.coeff2[3]:.2e}" if np.sign(self.CF.coeff2[3]) == 1 else f"${self.CF.coeff2[3]:.2e}"
+        eq = f"$y = {self.CF.coeff2[0]:.2e}x^3${p1}{p2}{p3}"
         eq = eq.replace('e','^{')
         eq = eq.replace('x','}x')
         eq = eq + '}$'
         self.ax[4][0].scatter(y, self.dw2, marker='+')
         self.ax[4][0].plot(y, wf, color='r', label=eq)
         self.ax[4][0].set_xlabel('Slit (pix)')
         self.ax[4][0].set_ylabel('dw (pix)')
@@ -2486,24 +2573,28 @@
         self.fig.canvas.draw_idle()
 
     def s4_Apply(self):
         self.log += "> Apply coefficient.<br>"
         self._writeLog()
         self.CF.coeff2[0] = float(self.LE_s4_p0.text())
         self.CF.coeff2[1] = float(self.LE_s4_p1.text())
-        self.CF.coeff2[2] = float(self.LE_s4_p2.text())
+        self.CF.coeff2[3] = float(self.LE_s4_p3.text())
         self.s2_make()
 
     def s5_Run(self):
         self.log += "> Make Flat running.<br>"
         self._writeLog()
+
+        pwr = int(self.LE_s5_pwr.text())
+        sig = float(self.LE_s5_sig.text())
+
         if self.s2 is None:
-            self.CF.Flat = self.CF.gain_calib(self.s1)
+            self.CF.Flat = self.CF.gain_calib(self.s1, power=pwr, fsig=sig)
         else: 
-            self.CF.Flat = self.CF.gain_calib(self.s2)  
+            self.CF.Flat = self.CF.gain_calib(self.s2, power=pwr, fsig=sig)  
         # self.CF.Flat = self.CF.gain_calib(self.CF.logF2)
         self.s5_img()
 
         self.clogF = self.CF.logF2 - np.log10(self.CF.Flat)
         self.ms_cF = 10**(self.clogF - self.clogF[:,5:-5].mean(1)[:,None,:])
 
         self.B_s5_Show.setEnabled(True)
@@ -2708,17 +2799,19 @@
         flatHDU.header['DATE'] = (self.h['DATE'], 'File Creation Date (UT)')
         flatHDU.header['STRTIME'] = (self.h['STRTIME'], 'Scan Start Time')
         flatHDU.header['ENDTIME'] = (self.h['ENDTIME'], 'Scan Finish Time')
         flatHDU.header['TILT'] = (self.CF.tilt, 'Degree')
         flatHDU.header['COEF1_0'] = (self.CF.coeff[0], 'Curvature correction coeff p0')
         flatHDU.header['COEF1_1'] = (self.CF.coeff[1], 'Curvature correction coeff p1')
         flatHDU.header['COEF1_2'] = (self.CF.coeff[2], 'Curvature correction coeff p2')
+        flatHDU.header['COEF1_3'] = (self.CF.coeff[3], 'Curvature correction coeff p3')
         flatHDU.header['COEF2_0'] = (self.CF.coeff2[0], '2nd Curvature correction coeff p0')
         flatHDU.header['COEF2_1'] = (self.CF.coeff2[1], '2nd Curvature correction coeff p1')
         flatHDU.header['COEF2_2'] = (self.CF.coeff2[2], '2nd Curvature correction coeff p2')
+        flatHDU.header['COEF2_3'] = (self.CF.coeff2[3], '2nd Curvature correction coeff p3')
         flatHDU.header['CCDNAME'] = (self.h['CCDNAME'], 'Prodctname of CCD')
 
         try:
             flatHDU.header['WAVELEN'] = (self.h['WAVELEN'], 'Angstrom')
         except:
             pass
         try:
@@ -2788,14 +2881,16 @@
         self.step(0)
         qSleep(0.1)
 
     def Initialize(self):
         self.subStepNum = -1
         self.xFringe = None
         self.yFringe = None
+        self.pwvGx = None
+        self.xGauss = False
         self.s1 = None
         self.s2 = None
         self.p_s5_ori = None
         self.p_s5_ff = None
         self.im_s5 = None
         self.frameNum = 3
         self.LE_s1_tilt.setText('0')
@@ -2944,22 +3039,22 @@
                     if init:
                         nf, ny, nw = yf.shape
                         lYF = np.zeros((len(lfY), nf, ny, nw))
                         init = False
                     lYF[j] = yf
                     # get slit pattern position
                     lyf = np.log10(yf)
-                    d2y = np.gradient(np.gradient(lyf[nf//2],axis=0), axis=0).mean(1)
-                    pks = find_peaks(d2y[5:-5], d2y[5:-5].std())[0]+5
-                    lpks[j] = pks
                     if yy >= 2023:
-                        sp = proc_base.yf2sp(lyf.mean(0))
+                        sp = proc_base.yf2sp_poly(lyf[nf//2])
                     else:
-                        sp = proc_base.yf2sp(lyf[nf//2])
+                        sp = proc_base.yf2sp_poly(lyf[nf//2])
                     sp -= sp[5:-5,5:-5].mean()
+                    d2y = np.gradient(np.gradient(sp,axis=0), axis=0).mean(1)
+                    pks = find_peaks(d2y[5:-5], d2y[5:-5].std())[0]+5
+                    lpks[j] = pks
 
                     # get wavelet
                     # wvl = Wavelet(lyf[nf//2], dt=1, axis=0)
                     wvl = Wavelet(lyf[nf//2] - sp, dt=1, axis=0)
                     lYFaws[j] = np.abs(wvl.wavelet)
                     lYFJD[j] = Time(proc_base.fname2isot(f)).jd
                     lSP[j] = 10**sp
@@ -3035,22 +3130,24 @@
                         flat = tFlat[idx][wh]
                         fjd = tFlatJD[idx][wh]
                         ch = tFlatHeader[idx][wh]
                         tilt = ch['tilt']
                         p1_0 = ch['coef1_0']
                         p1_1 = ch['coef1_1']
                         p1_2 = ch['coef1_2']
+                        p1_3 = ch['coef1_3']
                         p2_0 = ch['coef2_0']
                         p2_1 = ch['coef2_1']
                         p2_2 = ch['coef2_2']
+                        p2_3 = ch['coef2_3']
 
                         data1 = data-db
 
                         td = proc_base.tilt_correction(data1, tilt, cubic=True)
-                        cd1 = proc_base.curvature_correction(td, [p1_0, p1_1, p1_2])
+                        cd1 = proc_base.curvature_correction(td, [p1_0, p1_1, p1_2, p1_3])
                         
                         if len(tlfYF[idx]):
                             why = yfID[np.abs(tYFJD[idx] - fjd)*24*3600 < 10][0]
                             
                             # image shift correction
                             self.sp = tSP[idx][why]
 
@@ -3062,28 +3159,28 @@
                                 cd1 /= ssp
                                 rsp = proc_base.raw2sp(cd1, spks)
                                 self.rsp = rsp
                                 cd1 /= rsp
                             else:
                                 cd1 /= self.sp 
                             
-                            ryf = proc_base.rawYF(cd1, tYFaws[idx][why])
+                            ryf = proc_base.rawYF2(cd1, tYFaws[idx][why])
                             self.ryf = ryf
                             cd1 /= ryf
 
                             # cd1 /= tYF[idx][why][3]
                             self.cd1 = cd1
 
 
                         if len(tlfXF[idx]):
                             whx = xfID[np.abs(tXFJD[idx] - fjd)*24*3600 < 10][0]
                             XF = tXF[idx][whx]
                             cd1 /= XF[nf//2]
 
-                        cd2 = proc_base.curvature_correction(cd1, [p2_0, p2_1, p2_2])
+                        cd2 = proc_base.curvature_correction(cd1, [p2_0, p2_1, p2_2, p2_3])
                         cd2 /= flat
                         cd2 = cd2[:,5:-5,5:-5].astype('int16')
                         self.cd2 = cd2
                         shape = cd2.shape
 
                         if self.p_s7_prof is None:
                             p0 = int(ch['crpix1']-5)
```

### Comparing `fisspy-1.1.1/fisspy/preprocess/t_y_sh.py` & `fisspy-1.1.2/fisspy/preprocess/t_y_sh.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy/read/read_factory.py` & `fisspy-1.1.2/fisspy/read/read_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 from ..analysis import lambdameter
 from ..image.interactive_image import singleBand
 from ..correction import lineName, wvCalib, smoothingProf, corSLA
 from ..analysis import FourierFilter, Wavelet, makeTDmap
 
 __author__= "Juhyung Kang"
 __email__ = "jhkang0301@gmail.com"
-__all__ = ["FISS", "FD", "AlignCube"]
+__all__ = ["raw", "FISS", "FD", "AlignCube"]
 
-class rawData:
+class raw:
     """
     Read a raw file of the FISS.
 
     Parameters
     ----------
     file : `str`
         File name of the raw fts data file of the FISS.
@@ -183,18 +183,18 @@
         File name of the FISS fts data.
     x1: `int`, optional
         A left limit index of the frame along the scan direction
     x2: `int`, optional
         A right limit index of the frame along the scan direction
         If None, read all data from x1 to the end of the scan direction.
     y1: `int`, optional
-        A left limit index of the frame along the scan direction
+        A left limit index of the frame along the slit direction
     y2: `int`, optional
-        A right limit index of the frame along the scan direction
-        If None, read all data from x1 to the end of the scan direction.
+        A right limit index of the frame along the slit direction
+        If None, read all data from x1 to the end of the slit direction.
     noceff: `int`, optional
         The number of coefficients to be used for
         the construction of frame in a pca file.
     smoothingMethod: `str`, optional
         If it is not given, do not apply the noise filter.
         If 'savgol', apply the Savitzky-Golay noise filter in the wavelength axis.
         If 'gauss', apply the Gaussian noise filter in the wavelength axis.
@@ -244,15 +244,15 @@
         self.dwv = self.wvDelt
         self.date = self.header['date']
         try:
             wvln = self.header['wavelen']
             if type(wvln) == str:
                 self.band = wvln[:4]
             else:
-                wvln = str(wvln)
+                self.band = str(wvln)[:4]
         except:
             self.band = str(self.header['gratwvln'])[:4]
 
         self.refProfile = self.data.mean((0,1))
         self.wave = self.wvCalib(method=wvCalibMethod)
         self.cwv = self.centralWavelength = cwv = self.header['crval1']
```

### Comparing `fisspy-1.1.1/fisspy/read/readbase.py` & `fisspy-1.1.2/fisspy/read/readbase.py`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/fisspy.egg-info/PKG-INFO` & `fisspy-1.1.2/fisspy.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fisspy
-Version: 1.1.1
+Version: 1.1.2
 Summary: fisspy: Python analysis tools for GST/FISS
 Home-page: http://fiss.snu.ac.kr
 Author: Juhyung Kang
 Author-email: jhkang@astro.snu.ac.kr
 License: BSD-2
 Requires-Python: >=3.6
 License-File: LICENSE.txt
```

### Comparing `fisspy-1.1.1/fisspy.egg-info/SOURCES.txt` & `fisspy-1.1.2/fisspy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fisspy-1.1.1/setup.py` & `fisspy-1.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='fisspy',
-    version='1.1.1',
+    version='1.1.2',
     description='fisspy: Python analysis tools for GST/FISS',
     url='http://fiss.snu.ac.kr',
     author='Juhyung Kang',
     author_email='jhkang@astro.snu.ac.kr',
     license='BSD-2',
     python_requires='>=3.6',
     packages=find_packages(exclude=['docs', 'logo']),
```

