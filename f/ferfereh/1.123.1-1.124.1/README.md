# Comparing `tmp/ferfereh-1.123.1.tar.gz` & `tmp/ferfereh-1.124.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ferfereh-1.123.1.tar", last modified: Tue May 21 05:59:27 2024, max compression
+gzip compressed data, was "ferfereh-1.124.1.tar", last modified: Tue May 21 06:01:23 2024, max compression
```

## Comparing `ferfereh-1.123.1.tar` & `ferfereh-1.124.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 05:59:27.388739 ferfereh-1.123.1/
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-21 05:59:00.000000 ferfereh-1.123.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     4901 2024-05-21 05:59:27.388169 ferfereh-1.123.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     4080 2024-02-26 00:07:14.000000 ferfereh-1.123.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 05:59:27.384581 ferfereh-1.123.1/ferfereh/
--rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-21 05:59:17.000000 ferfereh-1.123.1/ferfereh/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      959 2024-02-25 23:42:23.000000 ferfereh-1.123.1/ferfereh/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)     2768 2024-02-25 23:44:02.000000 ferfereh-1.123.1/ferfereh/coords.py
--rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-03-24 00:16:12.000000 ferfereh-1.123.1/ferfereh/logger.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-02-27 00:15:30.000000 ferfereh-1.123.1/ferfereh/urls.py
--rw-r--r--   0 kamangir   (502) staff       (20)      642 2024-03-04 07:37:30.000000 ferfereh-1.123.1/ferfereh/utils.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 05:59:27.387265 ferfereh-1.123.1/ferfereh.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     4901 2024-05-21 05:59:27.000000 ferfereh-1.123.1/ferfereh.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)      336 2024-05-21 05:59:27.000000 ferfereh-1.123.1/ferfereh.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-21 05:59:27.000000 ferfereh-1.123.1/ferfereh.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-21 05:59:27.000000 ferfereh-1.123.1/ferfereh.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-21 05:59:27.000000 ferfereh-1.123.1/ferfereh.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 05:52:18.000000 ferfereh-1.123.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-21 05:56:20.000000 ferfereh-1.123.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-21 05:59:27.388839 ferfereh-1.123.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      226 2024-05-21 05:56:26.000000 ferfereh-1.123.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 06:01:23.675481 ferfereh-1.124.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-21 05:59:00.000000 ferfereh-1.124.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     6224 2024-05-21 06:01:23.674818 ferfereh-1.124.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     4138 2024-05-21 06:01:05.000000 ferfereh-1.124.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 06:01:23.670389 ferfereh-1.124.1/ferfereh/
+-rw-r--r--   0 kamangir   (502) staff       (20)       99 2024-05-21 06:01:13.000000 ferfereh-1.124.1/ferfereh/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      959 2024-02-25 23:42:23.000000 ferfereh-1.124.1/ferfereh/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)     2768 2024-02-25 23:44:02.000000 ferfereh-1.124.1/ferfereh/coords.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       89 2024-03-24 00:16:12.000000 ferfereh-1.124.1/ferfereh/logger.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-02-27 00:15:30.000000 ferfereh-1.124.1/ferfereh/urls.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      642 2024-03-04 07:37:30.000000 ferfereh-1.124.1/ferfereh/utils.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-05-21 06:01:23.673759 ferfereh-1.124.1/ferfereh.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     6224 2024-05-21 06:01:23.000000 ferfereh-1.124.1/ferfereh.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)      336 2024-05-21 06:01:23.000000 ferfereh-1.124.1/ferfereh.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-05-21 06:01:23.000000 ferfereh-1.124.1/ferfereh.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-21 06:01:23.000000 ferfereh-1.124.1/ferfereh.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        9 2024-05-21 06:01:23.000000 ferfereh-1.124.1/ferfereh.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 05:52:18.000000 ferfereh-1.124.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      125 2024-05-21 05:56:20.000000 ferfereh-1.124.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-05-21 06:01:23.675625 ferfereh-1.124.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      226 2024-05-21 05:56:26.000000 ferfereh-1.124.1/setup.py
```

### Comparing `ferfereh-1.123.1/README.md` & `ferfereh-1.124.1/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -21,47 +21,47 @@
 ferfereh publish coords \
 	[~downloads]
  . publish ferfereh coords.
 ferfereh publish 3d-files
  . publish ferfereh 3d-files.
 ```
 
-| [![image](images/gen5.jpg)](#gen5) | [![image](images/gen6-c2.jpg)](#gen6) | [![image](images/gen6-s.jpg)](#gen6) | [![image](images/gen7-2.jpg)](#gen7) |
-| ---------------------------------- | ------------------------------------- | ------------------------------------ | ------------------------------------ |
+| [![image](./images/gen5.jpg)](#gen5) | [![image](./images/gen6-c2.jpg)](#gen6) | [![image](./images/gen6-s.jpg)](#gen6) | [![image](./images/gen7-2.jpg)](#gen7) |
+| ------------------------------------ | --------------------------------------- | -------------------------------------- | -------------------------------------- |
 
 # brackets
 
 ## gen5
 
-![image](images/gen5.png)
+![image](./images/gen5.png)
 
-- [gen5.stl](3d/gen5.stl)
+- [gen5.stl](./3d/gen5.stl)
 
 ## gen6
 
-![image](images/gen6.png)
+![image](./images/gen6.png)
 
-- [gen6-c4](3d/gen6-c4.stl)
-- [gen6-d32](3d/gen6-d32.stl)
-- [gen6-s4](3d/gen6-s4.stl)
+- [gen6-c4](./3d/gen6-c4.stl)
+- [gen6-d32](./3d/gen6-d32.stl)
+- [gen6-s4](./3d/gen6-s4.stl)
 
 ## gen7
 
-![image](images/gen7.png)
+![image](./images/gen7.png)
 
-- [gen7-2](3d/gen7-2.stl)
+- [gen7-2](./3d/gen7-2.stl)
 
 # tools & materials
 
-| item                                                                      | image                                                         | examples                                                                           |
-| ------------------------------------------------------------------------- | ------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
-| 2 mm solid brass rods                                                     | ![image](images/tools/solid-brass-bars.jpeg)                  | https://www.amazon.ca/gp/product/B089LDXN22                                        |
-| aviation snips                                                            | ![image](images/tools/aviation-snips.jpeg)                    |                                                                                    |
-| (multiple) bags to carry the brackets, tools, and other materials to site | ![image](images/tools/bags.jpeg)                              |                                                                                    |
-| cutting nippers                                                           | ![image](images/tools/cutting-nippers.jpeg)                   |                                                                                    |
-| mini pliers                                                               | ![image](images/tools/mini-pliers.jpeg)                       |                                                                                    |
-| propeller fan                                                             | ![image](images/tools/propellers.jpeg)                        | https://www.adafruit.com/product/3896, https://www.amazon.ca/gp/product/B091TBQ7CK |
-| double-sided, outdoor, water-resistant, mounting tape                     | ![image](images/tools/mounting-tape.jpeg)                     |                                                                                    |
-| multi bit electronics screwdriver                                         | ![image](images/tools/multi-bit-electronics-screwdriver.jpeg) |                                                                                    |
-| precision craft knife w/ spare blade                                      | ![image](images/tools/precision-craft-knife.jpeg)             |                                                                                    |
-| small hammer                                                              | ![image](images/tools/small-hammer.jpeg)                      |                                                                                    |
-| M3 Nylon Machine Screws                                                   | ![image](images/tools/screws.jpg)                             | https://www.amazon.ca/gp/product/B012TACIBC                                        |
+| item                                                                      | image                                                           | examples                                                                           |
+| ------------------------------------------------------------------------- | --------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
+| 2 mm solid brass rods                                                     | ![image](./images/tools/solid-brass-bars.jpeg)                  | https://www.amazon.ca/gp/product/B089LDXN22                                        |
+| aviation snips                                                            | ![image](./images/tools/aviation-snips.jpeg)                    |                                                                                    |
+| (multiple) bags to carry the brackets, tools, and other materials to site | ![image](./images/tools/bags.jpeg)                              |                                                                                    |
+| cutting nippers                                                           | ![image](./images/tools/cutting-nippers.jpeg)                   |                                                                                    |
+| mini pliers                                                               | ![image](./images/tools/mini-pliers.jpeg)                       |                                                                                    |
+| propeller fan                                                             | ![image](./images/tools/propellers.jpeg)                        | https://www.adafruit.com/product/3896, https://www.amazon.ca/gp/product/B091TBQ7CK |
+| double-sided, outdoor, water-resistant, mounting tape                     | ![image](./images/tools/mounting-tape.jpeg)                     |                                                                                    |
+| multi bit electronics screwdriver                                         | ![image](./images/tools/multi-bit-electronics-screwdriver.jpeg) |                                                                                    |
+| precision craft knife w/ spare blade                                      | ![image](./images/tools/precision-craft-knife.jpeg)             |                                                                                    |
+| small hammer                                                              | ![image](./images/tools/small-hammer.jpeg)                      |                                                                                    |
+| M3 Nylon Machine Screws                                                   | ![image](./images/tools/screws.jpg)                             | https://www.amazon.ca/gp/product/B012TACIBC                                        |
```

### Comparing `ferfereh-1.123.1/ferfereh/__main__.py` & `ferfereh-1.124.1/ferfereh/__main__.py`

 * *Files identical despite different names*

### Comparing `ferfereh-1.123.1/ferfereh/coords.py` & `ferfereh-1.124.1/ferfereh/coords.py`

 * *Files identical despite different names*

### Comparing `ferfereh-1.123.1/ferfereh/utils.py` & `ferfereh-1.124.1/ferfereh/utils.py`

 * *Files identical despite different names*

