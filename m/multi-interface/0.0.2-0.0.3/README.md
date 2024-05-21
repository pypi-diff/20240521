# Comparing `tmp/multi_interface-0.0.2.tar.gz` & `tmp/multi_interface-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multi_interface-0.0.2.tar", last modified: Mon May 20 14:05:13 2024, max compression
+gzip compressed data, was "multi_interface-0.0.3.tar", last modified: Tue May 21 14:44:29 2024, max compression
```

## Comparing `multi_interface-0.0.2.tar` & `multi_interface-0.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 14:05:13.235219 multi_interface-0.0.2/
--rw-rw-rw-   0        0        0     1075 2024-05-13 05:05:44.000000 multi_interface-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     6926 2024-05-20 14:05:13.234222 multi_interface-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6515 2024-05-20 13:57:50.000000 multi_interface-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 14:05:13.188145 multi_interface-0.0.2/multi_interface/
--rw-rw-rw-   0        0        0      163 2024-05-20 13:48:31.000000 multi_interface-0.0.2/multi_interface/__init__.py
--rw-rw-rw-   0        0        0     8784 2024-05-20 13:37:26.000000 multi_interface-0.0.2/multi_interface/bnd.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:05:13.220259 multi_interface-0.0.2/multi_interface/crust1.0/
--rw-rw-rw-   0        0        0  4147200 2013-08-28 02:05:51.000000 multi_interface-0.0.2/multi_interface/crust1.0/crust1.bnds
--rw-rw-rw-   0        0        0  3564000 2013-08-28 02:05:51.000000 multi_interface-0.0.2/multi_interface/crust1.0/crust1.rho
--rw-rw-rw-   0        0        0     5478 2024-05-13 06:13:16.000000 multi_interface-0.0.2/multi_interface/data_provider.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:05:13.229236 multi_interface-0.0.2/multi_interface/gravities/
--rw-rw-rw-   0        0        0  1603193 2024-05-09 09:33:52.000000 multi_interface-0.0.2/multi_interface/gravities/delta-g-3.dg
--rw-rw-rw-   0        0        0  1603238 2024-05-09 09:33:53.000000 multi_interface-0.0.2/multi_interface/gravities/delta-g-5.dg
--rw-rw-rw-   0        0        0      381 2024-04-29 16:49:57.000000 multi_interface-0.0.2/multi_interface/metrics.py
--rw-rw-rw-   0        0        0     9051 2024-05-13 06:29:14.000000 multi_interface-0.0.2/multi_interface/plt_tools.py
--rw-rw-rw-   0        0        0     3355 2024-05-20 07:20:14.000000 multi_interface-0.0.2/multi_interface/vgg.py
-drwxrwxrwx   0        0        0        0 2024-05-20 14:05:13.234222 multi_interface-0.0.2/multi_interface.egg-info/
--rw-rw-rw-   0        0        0     6926 2024-05-20 14:05:13.000000 multi_interface-0.0.2/multi_interface.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      538 2024-05-20 14:05:13.000000 multi_interface-0.0.2/multi_interface.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 14:05:13.000000 multi_interface-0.0.2/multi_interface.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-05-20 14:05:13.000000 multi_interface-0.0.2/multi_interface.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-20 14:05:13.000000 multi_interface-0.0.2/multi_interface.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 14:05:13.235219 multi_interface-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      800 2024-05-20 14:00:23.000000 multi_interface-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:44:29.558682 multi_interface-0.0.3/
+-rw-rw-rw-   0        0        0     1075 2024-05-13 05:05:44.000000 multi_interface-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     6926 2024-05-21 14:44:29.557685 multi_interface-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6515 2024-05-20 13:57:50.000000 multi_interface-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 14:44:29.461941 multi_interface-0.0.3/multi_interface/
+-rw-rw-rw-   0        0        0      163 2024-05-20 13:48:31.000000 multi_interface-0.0.3/multi_interface/__init__.py
+-rw-rw-rw-   0        0        0     8784 2024-05-20 13:37:26.000000 multi_interface-0.0.3/multi_interface/bnd.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:44:29.523778 multi_interface-0.0.3/multi_interface/crust1.0/
+-rw-rw-rw-   0        0        0  4147200 2013-08-28 02:05:51.000000 multi_interface-0.0.3/multi_interface/crust1.0/crust1.bnds
+-rw-rw-rw-   0        0        0  3564000 2013-08-28 02:05:51.000000 multi_interface-0.0.3/multi_interface/crust1.0/crust1.rho
+-rw-rw-rw-   0        0        0     5478 2024-05-13 06:13:16.000000 multi_interface-0.0.3/multi_interface/data_provider.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:44:29.552699 multi_interface-0.0.3/multi_interface/gravities/
+-rw-rw-rw-   0        0        0  1603193 2024-05-09 09:33:52.000000 multi_interface-0.0.3/multi_interface/gravities/delta-g-3.dg
+-rw-rw-rw-   0        0        0  1603238 2024-05-09 09:33:53.000000 multi_interface-0.0.3/multi_interface/gravities/delta-g-5.dg
+-rw-rw-rw-   0        0        0      381 2024-04-29 16:49:57.000000 multi_interface-0.0.3/multi_interface/metrics.py
+-rw-rw-rw-   0        0        0     9136 2024-05-21 14:42:46.000000 multi_interface-0.0.3/multi_interface/plt_tools.py
+-rw-rw-rw-   0        0        0     3355 2024-05-20 07:20:14.000000 multi_interface-0.0.3/multi_interface/vgg.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:44:29.556687 multi_interface-0.0.3/multi_interface.egg-info/
+-rw-rw-rw-   0        0        0     6926 2024-05-21 14:44:29.000000 multi_interface-0.0.3/multi_interface.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      538 2024-05-21 14:44:29.000000 multi_interface-0.0.3/multi_interface.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:44:29.000000 multi_interface-0.0.3/multi_interface.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-05-21 14:44:29.000000 multi_interface-0.0.3/multi_interface.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-21 14:44:29.000000 multi_interface-0.0.3/multi_interface.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:44:29.558682 multi_interface-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      800 2024-05-21 14:42:46.000000 multi_interface-0.0.3/setup.py
```

### Comparing `multi_interface-0.0.2/LICENSE.txt` & `multi_interface-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multi_interface-0.0.2/PKG-INFO` & `multi_interface-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-interface
-Version: 0.0.2
+Version: 0.0.3
 Summary: reflection and deflection between Crust1.0 and Vertical Gravity Gradient
 Home-page: https://github.com/WangChao/Chao-interface
 Author: Chao
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: matplotlib>=3.8.4
```

### Comparing `multi_interface-0.0.2/README.md` & `multi_interface-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `multi_interface-0.0.2/multi_interface/bnd.py` & `multi_interface-0.0.3/multi_interface/bnd.py`

 * *Files identical despite different names*

### Comparing `multi_interface-0.0.2/multi_interface/crust1.0/crust1.bnds` & `multi_interface-0.0.3/multi_interface/crust1.0/crust1.bnds`

 * *Files identical despite different names*

### Comparing `multi_interface-0.0.2/multi_interface/crust1.0/crust1.rho` & `multi_interface-0.0.3/multi_interface/crust1.0/crust1.rho`

 * *Files identical despite different names*

### Comparing `multi_interface-0.0.2/multi_interface/data_provider.py` & `multi_interface-0.0.3/multi_interface/data_provider.py`

 * *Files identical despite different names*

### Comparing `multi_interface-0.0.2/multi_interface/gravities/delta-g-3.dg` & `multi_interface-0.0.3/multi_interface/gravities/delta-g-3.dg`

 * *Files identical despite different names*

### Comparing `multi_interface-0.0.2/multi_interface/gravities/delta-g-5.dg` & `multi_interface-0.0.3/multi_interface/gravities/delta-g-5.dg`

 * *Files identical despite different names*

### Comparing `multi_interface-0.0.2/multi_interface/plt_tools.py` & `multi_interface-0.0.3/multi_interface/plt_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         :param name: if None, plt.show else 把图保存到name地址
         :return: None
         """
         pass
 
     # 3D图
     @abstractmethod
-    def plt_3d(self, mtrix, lat=None, lon=None, name=None):
+    def plt_3d(self, mtrix, lat=None, lon=None, title=None, name=None):
         """
         :param mtrix: n * p 的array-like
         :param lat: list,如[-10, -5, 0, 5, 10]
         :param lon: list,如[-10, -5, 0, 5, 10]
         :param name: if None, plt.show else 把图保存到name地址
         :return: None
         """
@@ -94,15 +94,15 @@
             plt.yticks([item for item in np.linspace(0, nrow, len(lat))], lat)
         if name is None:
             plt.show()
         else:
             plt.savefig(name)
 
     @classmethod
-    def plt_3d(cls, mtrix, lat=None, lon=None, name=None):
+    def plt_3d(cls, mtrix, lat=None, lon=None, title=None, name=None):
         fig = plt.figure()
         ax3 = plt.axes(projection='3d')
         nrow, ncol = mtrix.shape
         x, y = np.arange(0, ncol), nrow - np.arange(nrow) - 1
         xx, yy = np.meshgrid(x, y)
         ax3.plot_surface(xx, yy, mtrix, cmap='rainbow')
 
@@ -110,14 +110,16 @@
         plt.xticks(fontsize=20)
         plt.yticks(fontsize=20)
         if lon is not None:
             plt.xticks([item for item in np.linspace(0, ncol, len(lon))], lon)
         if lat is not None:
             plt.yticks([item for item in np.linspace(0, nrow, len(lat))], lat)
         ax3.dist = 8.5
+        if title is not None:
+            plt.title(title)
         if name is None:
             plt.show()
         else:
             plt.savefig(name)
 
     def plt_layer(self, mtrix, lon=None, colors=None, name=None, texts=[], arrows=[]):
         nrow, ncol = mtrix.shape
```

### Comparing `multi_interface-0.0.2/multi_interface/vgg.py` & `multi_interface-0.0.3/multi_interface/vgg.py`

 * *Files identical despite different names*

### Comparing `multi_interface-0.0.2/multi_interface.egg-info/PKG-INFO` & `multi_interface-0.0.3/multi_interface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multi-interface
-Version: 0.0.2
+Version: 0.0.3
 Summary: reflection and deflection between Crust1.0 and Vertical Gravity Gradient
 Home-page: https://github.com/WangChao/Chao-interface
 Author: Chao
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: matplotlib>=3.8.4
```

### Comparing `multi_interface-0.0.2/multi_interface.egg-info/SOURCES.txt` & `multi_interface-0.0.3/multi_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multi_interface-0.0.2/setup.py` & `multi_interface-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='multi-interface',
-    version="0.0.2",
+    version="0.0.3",
     author='Chao',
     description='reflection and deflection between Crust1.0 and Vertical Gravity Gradient',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/WangChao/Chao-interface',
     include_package_data=True,
     package_data={
```

