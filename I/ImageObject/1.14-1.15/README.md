# Comparing `tmp/ImageObject-1.14.tar.gz` & `tmp/ImageObject-1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ImageObject-1.14.tar", last modified: Mon May 20 19:16:06 2024, max compression
+gzip compressed data, was "ImageObject-1.15.tar", last modified: Mon May 20 19:17:33 2024, max compression
```

## Comparing `ImageObject-1.14.tar` & `ImageObject-1.15.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 19:16:06.422782 ImageObject-1.14/
--rw-rw-rw-   0        0        0    18213 2024-05-20 19:14:01.000000 ImageObject-1.14/ImageObject.cpp
-drwxrwxrwx   0        0        0        0 2024-05-20 19:16:06.422782 ImageObject-1.14/ImageObject.egg-info/
--rw-rw-rw-   0        0        0      324 2024-05-20 19:16:06.000000 ImageObject-1.14/ImageObject.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-05-20 19:16:06.000000 ImageObject-1.14/ImageObject.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 19:16:06.000000 ImageObject-1.14/ImageObject.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-20 19:16:06.000000 ImageObject-1.14/ImageObject.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3770 2024-05-20 17:33:33.000000 ImageObject-1.14/ImageObject.h
--rw-rw-rw-   0        0        0     4922 2024-05-20 17:33:33.000000 ImageObject-1.14/ImageObject_old.h
--rw-rw-rw-   0        0        0       15 2024-05-20 19:12:51.000000 ImageObject-1.14/MANIFEST.in
--rw-rw-rw-   0        0        0      324 2024-05-20 19:16:06.422782 ImageObject-1.14/PKG-INFO
--rw-rw-rw-   0        0        0     3921 2024-05-20 19:15:47.000000 ImageObject-1.14/pybind11.cpp
--rw-rw-rw-   0        0        0       42 2024-05-20 19:16:06.422782 ImageObject-1.14/setup.cfg
--rw-rw-rw-   0        0        0      935 2024-05-20 19:16:05.000000 ImageObject-1.14/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 19:17:33.700662 ImageObject-1.15/
+-rw-rw-rw-   0        0        0    18213 2024-05-20 19:14:01.000000 ImageObject-1.15/ImageObject.cpp
+drwxrwxrwx   0        0        0        0 2024-05-20 19:17:33.700662 ImageObject-1.15/ImageObject.egg-info/
+-rw-rw-rw-   0        0        0      324 2024-05-20 19:17:33.000000 ImageObject-1.15/ImageObject.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-05-20 19:17:33.000000 ImageObject-1.15/ImageObject.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 19:17:33.000000 ImageObject-1.15/ImageObject.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-20 19:17:33.000000 ImageObject-1.15/ImageObject.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3770 2024-05-20 17:33:33.000000 ImageObject-1.15/ImageObject.h
+-rw-rw-rw-   0        0        0     4922 2024-05-20 17:33:33.000000 ImageObject-1.15/ImageObject_old.h
+-rw-rw-rw-   0        0        0       15 2024-05-20 19:12:51.000000 ImageObject-1.15/MANIFEST.in
+-rw-rw-rw-   0        0        0      324 2024-05-20 19:17:33.700662 ImageObject-1.15/PKG-INFO
+-rw-rw-rw-   0        0        0     3921 2024-05-20 19:15:47.000000 ImageObject-1.15/pybind11.cpp
+-rw-rw-rw-   0        0        0       42 2024-05-20 19:17:33.700662 ImageObject-1.15/setup.cfg
+-rw-rw-rw-   0        0        0      894 2024-05-20 19:17:31.000000 ImageObject-1.15/setup.py
```

### Comparing `ImageObject-1.14/ImageObject.cpp` & `ImageObject-1.15/ImageObject.cpp`

 * *Files identical despite different names*

### Comparing `ImageObject-1.14/ImageObject.h` & `ImageObject-1.15/ImageObject.h`

 * *Files identical despite different names*

### Comparing `ImageObject-1.14/ImageObject_old.h` & `ImageObject-1.15/ImageObject_old.h`

 * *Files identical despite different names*

### Comparing `ImageObject-1.14/pybind11.cpp` & `ImageObject-1.15/pybind11.cpp`

 * *Files identical despite different names*

### Comparing `ImageObject-1.14/setup.py` & `ImageObject-1.15/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,21 +15,20 @@
     ],
     language='c++',
     extra_compile_args=cpp_args)
 
 
 setup(
     name='ImageObject',
-    version='1.14',
+    version='1.15',
     description='Python package for image object operations',
     ext_modules=[sfc_module],
     author='Lei Wang',
     author_email='leiwang@lsu.edu',
     packages=find_packages(),
-    headers=['includes/ImageObject.h'],
     classifiers=[
     'Programming Language :: C++',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent',
     ],
     python_requires='>=3.6'
 )
```

