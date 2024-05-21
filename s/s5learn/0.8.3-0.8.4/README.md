# Comparing `tmp/s5learn-0.8.3.tar.gz` & `tmp/s5learn-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s5learn-0.8.3.tar", last modified: Mon May 20 05:29:46 2024, max compression
+gzip compressed data, was "s5learn-0.8.4.tar", last modified: Tue May 21 14:50:06 2024, max compression
```

## Comparing `s5learn-0.8.3.tar` & `s5learn-0.8.4.tar`

### file list

```diff
@@ -1,39 +1,58 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 05:29:46.804750 s5learn-0.8.3/
--rw-rw-rw-   0        0        0       54 2024-05-20 05:29:46.804750 s5learn-0.8.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-20 05:29:46.742252 s5learn-0.8.3/s5learn/
--rw-rw-rw-   0        0        0       28 2024-05-19 23:40:29.000000 s5learn-0.8.3/s5learn/__init__.py
--rw-rw-rw-   0        0        0      249 2024-05-19 21:28:29.000000 s5learn-0.8.3/s5learn/main.py
-drwxrwxrwx   0        0        0        0 2024-05-20 05:29:46.773510 s5learn-0.8.3/s5learn/models/
--rw-rw-rw-   0        0        0      434 2024-05-20 05:29:28.000000 s5learn-0.8.3/s5learn/models/__init__.py
--rw-rw-rw-   0        0        0      439 2024-05-20 05:13:00.000000 s5learn-0.8.3/s5learn/models/aomalarm.py
--rw-rw-rw-   0        0        0     2834 2024-05-20 05:17:20.000000 s5learn-0.8.3/s5learn/models/aommon.py
--rw-rw-rw-   0        0        0      414 2024-05-20 05:00:54.000000 s5learn-0.8.3/s5learn/models/appscript.py
--rw-rw-rw-   0        0        0      655 2024-05-20 04:59:45.000000 s5learn-0.8.3/s5learn/models/confmysql.py
--rw-rw-rw-   0        0        0      768 2024-05-20 05:09:37.000000 s5learn-0.8.3/s5learn/models/diz.py
--rw-rw-rw-   0        0        0     1338 2024-05-20 05:20:45.000000 s5learn-0.8.3/s5learn/models/dizcon.py
--rw-rw-rw-   0        0        0     8081 2024-05-20 05:21:32.000000 s5learn-0.8.3/s5learn/models/docker.py
--rw-rw-rw-   0        0        0     4632 2024-05-20 05:15:31.000000 s5learn-0.8.3/s5learn/models/dockerfile.py
--rw-rw-rw-   0        0        0      827 2024-05-20 04:57:50.000000 s5learn-0.8.3/s5learn/models/impddm.py
--rw-rw-rw-   0        0        0      690 2024-05-20 05:06:05.000000 s5learn-0.8.3/s5learn/models/logaom.py
--rw-rw-rw-   0        0        0     3381 2024-05-20 05:09:26.000000 s5learn-0.8.3/s5learn/models/micro.py
--rw-rw-rw-   0        0        0     2154 2024-05-20 05:02:05.000000 s5learn-0.8.3/s5learn/models/mysqlcnf.py
--rw-rw-rw-   0        0        0      956 2024-05-20 04:57:04.000000 s5learn-0.8.3/s5learn/models/opcart.py
--rw-rw-rw-   0        0        0      570 2024-05-20 05:04:21.000000 s5learn-0.8.3/s5learn/models/sms.py
--rw-rw-rw-   0        0        0     1832 2024-05-20 04:54:51.000000 s5learn-0.8.3/s5learn/models/wpress.py
-drwxrwxrwx   0        0        0        0 2024-05-20 05:29:46.804750 s5learn-0.8.3/s5learn/preprocessing/
--rw-rw-rw-   0        0        0      200 2024-05-19 23:27:53.000000 s5learn-0.8.3/s5learn/preprocessing/__init__.py
--rw-rw-rw-   0        0        0     2753 2024-05-19 22:11:08.000000 s5learn-0.8.3/s5learn/preprocessing/idp.py
--rw-rw-rw-   0        0        0     7318 2024-05-19 22:04:34.000000 s5learn-0.8.3/s5learn/preprocessing/m5.py
--rw-rw-rw-   0        0        0     5940 2024-05-19 22:14:34.000000 s5learn-0.8.3/s5learn/preprocessing/mnv2.py
--rw-rw-rw-   0        0        0     1394 2024-05-19 22:13:21.000000 s5learn-0.8.3/s5learn/preprocessing/mnv2_dp.py
--rw-rw-rw-   0        0        0      979 2024-05-19 22:19:47.000000 s5learn-0.8.3/s5learn/preprocessing/mnv2_dv.py
--rw-rw-rw-   0        0        0     2075 2024-05-19 22:06:44.000000 s5learn-0.8.3/s5learn/preprocessing/ms.py
--rw-rw-rw-   0        0        0     3935 2024-05-19 22:08:10.000000 s5learn-0.8.3/s5learn/preprocessing/mv2_train.py
--rw-rw-rw-   0        0        0     3109 2024-05-19 22:10:02.000000 s5learn-0.8.3/s5learn/preprocessing/t5.py
-drwxrwxrwx   0        0        0        0 2024-05-20 05:29:46.804750 s5learn-0.8.3/s5learn.egg-info/
--rw-rw-rw-   0        0        0       54 2024-05-20 05:29:46.000000 s5learn-0.8.3/s5learn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      855 2024-05-20 05:29:46.000000 s5learn-0.8.3/s5learn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 05:29:46.000000 s5learn-0.8.3/s5learn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-20 05:29:46.000000 s5learn-0.8.3/s5learn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 05:29:46.804750 s5learn-0.8.3/setup.cfg
--rw-rw-rw-   0        0        0     1819 2024-05-20 05:29:28.000000 s5learn-0.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:50:06.051910 s5learn-0.8.4/
+-rw-rw-rw-   0        0        0       54 2024-05-21 14:50:06.051910 s5learn-0.8.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-21 14:50:05.895669 s5learn-0.8.4/s5learn/
+-rw-rw-rw-   0        0        0       28 2024-05-19 23:40:29.000000 s5learn-0.8.4/s5learn/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:50:05.926918 s5learn-0.8.4/s5learn/linear_models/
+-rw-rw-rw-   0        0        0      362 2024-05-21 04:35:18.000000 s5learn-0.8.4/s5learn/linear_models/__init__.py
+-rw-rw-rw-   0        0        0    12290 2024-05-21 03:38:56.000000 s5learn-0.8.4/s5learn/linear_models/cclib.py
+-rw-rw-rw-   0        0        0    10713 2024-05-21 03:39:37.000000 s5learn-0.8.4/s5learn/linear_models/dplib.py
+-rw-rw-rw-   0        0        0     9282 2024-05-21 03:41:49.000000 s5learn-0.8.4/s5learn/linear_models/fdlib.py
+-rw-rw-rw-   0        0        0     9281 2024-05-21 03:42:43.000000 s5learn-0.8.4/s5learn/linear_models/geslib.py
+-rw-rw-rw-   0        0        0      910 2024-05-21 03:56:09.000000 s5learn-0.8.4/s5learn/linear_models/ha10lib.py
+-rw-rw-rw-   0        0        0     1909 2024-05-21 03:45:49.000000 s5learn-0.8.4/s5learn/linear_models/hblib.py
+-rw-rw-rw-   0        0        0     3567 2024-05-21 03:54:13.000000 s5learn-0.8.4/s5learn/linear_models/hpplib.py
+-rw-rw-rw-   0        0        0      931 2024-05-21 03:54:13.000000 s5learn-0.8.4/s5learn/linear_models/kafkalib.py
+-rw-rw-rw-   0        0        0     1599 2024-05-21 03:56:09.000000 s5learn-0.8.4/s5learn/linear_models/luxlib.py
+-rw-rw-rw-   0        0        0     7638 2024-05-21 03:59:30.000000 s5learn-0.8.4/s5learn/linear_models/ofblib.py
+-rw-rw-rw-   0        0        0     5879 2024-05-21 04:01:45.000000 s5learn-0.8.4/s5learn/linear_models/pylib.py
+-rw-rw-rw-   0        0        0    11238 2024-05-21 04:32:15.000000 s5learn-0.8.4/s5learn/linear_models/sparklib.py
+-rw-rw-rw-   0        0        0     2221 2024-05-21 04:32:59.000000 s5learn-0.8.4/s5learn/linear_models/splib.py
+-rw-rw-rw-   0        0        0      249 2024-05-19 21:28:29.000000 s5learn-0.8.4/s5learn/main.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:50:05.989415 s5learn-0.8.4/s5learn/models/
+-rw-rw-rw-   0        0        0      434 2024-05-20 05:29:28.000000 s5learn-0.8.4/s5learn/models/__init__.py
+-rw-rw-rw-   0        0        0      439 2024-05-20 05:13:00.000000 s5learn-0.8.4/s5learn/models/aomalarm.py
+-rw-rw-rw-   0        0        0     2834 2024-05-20 05:17:20.000000 s5learn-0.8.4/s5learn/models/aommon.py
+-rw-rw-rw-   0        0        0      414 2024-05-20 05:00:54.000000 s5learn-0.8.4/s5learn/models/appscript.py
+-rw-rw-rw-   0        0        0      655 2024-05-20 04:59:45.000000 s5learn-0.8.4/s5learn/models/confmysql.py
+-rw-rw-rw-   0        0        0      768 2024-05-20 05:09:37.000000 s5learn-0.8.4/s5learn/models/diz.py
+-rw-rw-rw-   0        0        0     1338 2024-05-20 05:20:45.000000 s5learn-0.8.4/s5learn/models/dizcon.py
+-rw-rw-rw-   0        0        0     8081 2024-05-20 05:21:32.000000 s5learn-0.8.4/s5learn/models/docker.py
+-rw-rw-rw-   0        0        0     4632 2024-05-20 05:15:31.000000 s5learn-0.8.4/s5learn/models/dockerfile.py
+-rw-rw-rw-   0        0        0      827 2024-05-20 04:57:50.000000 s5learn-0.8.4/s5learn/models/impddm.py
+-rw-rw-rw-   0        0        0      690 2024-05-20 05:06:05.000000 s5learn-0.8.4/s5learn/models/logaom.py
+-rw-rw-rw-   0        0        0     3381 2024-05-20 05:09:26.000000 s5learn-0.8.4/s5learn/models/micro.py
+-rw-rw-rw-   0        0        0     2154 2024-05-20 05:02:05.000000 s5learn-0.8.4/s5learn/models/mysqlcnf.py
+-rw-rw-rw-   0        0        0      956 2024-05-20 04:57:04.000000 s5learn-0.8.4/s5learn/models/opcart.py
+-rw-rw-rw-   0        0        0      570 2024-05-20 05:04:21.000000 s5learn-0.8.4/s5learn/models/sms.py
+-rw-rw-rw-   0        0        0     1832 2024-05-20 04:54:51.000000 s5learn-0.8.4/s5learn/models/wpress.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:50:06.036285 s5learn-0.8.4/s5learn/preprocessing/
+-rw-rw-rw-   0        0        0      308 2024-05-21 03:01:42.000000 s5learn-0.8.4/s5learn/preprocessing/__init__.py
+-rw-rw-rw-   0        0        0     2753 2024-05-19 22:11:08.000000 s5learn-0.8.4/s5learn/preprocessing/idp.py
+-rw-rw-rw-   0        0        0     7318 2024-05-19 22:04:34.000000 s5learn-0.8.4/s5learn/preprocessing/m5.py
+-rw-rw-rw-   0        0        0     5940 2024-05-19 22:14:34.000000 s5learn-0.8.4/s5learn/preprocessing/mnv2.py
+-rw-rw-rw-   0        0        0     1394 2024-05-19 22:13:21.000000 s5learn-0.8.4/s5learn/preprocessing/mnv2_dp.py
+-rw-rw-rw-   0        0        0      979 2024-05-19 22:19:47.000000 s5learn-0.8.4/s5learn/preprocessing/mnv2_dv.py
+-rw-rw-rw-   0        0        0     2075 2024-05-19 22:06:44.000000 s5learn-0.8.4/s5learn/preprocessing/ms.py
+-rw-rw-rw-   0        0        0     3935 2024-05-19 22:08:10.000000 s5learn-0.8.4/s5learn/preprocessing/mv2_train.py
+-rw-rw-rw-   0        0        0     3417 2024-05-21 02:49:46.000000 s5learn-0.8.4/s5learn/preprocessing/sp.py
+-rw-rw-rw-   0        0        0     7533 2024-05-21 02:52:04.000000 s5learn-0.8.4/s5learn/preprocessing/ss_seqseq.py
+-rw-rw-rw-   0        0        0     3109 2024-05-19 22:10:02.000000 s5learn-0.8.4/s5learn/preprocessing/t5.py
+-rw-rw-rw-   0        0        0     9982 2024-05-21 02:53:40.000000 s5learn-0.8.4/s5learn/preprocessing/tn.py
+-rw-rw-rw-   0        0        0    12019 2024-05-21 02:55:38.000000 s5learn-0.8.4/s5learn/preprocessing/translate.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:50:06.036285 s5learn-0.8.4/s5learn.egg-info/
+-rw-rw-rw-   0        0        0       54 2024-05-21 14:50:05.000000 s5learn-0.8.4/s5learn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1430 2024-05-21 14:50:05.000000 s5learn-0.8.4/s5learn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:50:05.000000 s5learn-0.8.4/s5learn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-21 14:50:05.000000 s5learn-0.8.4/s5learn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:50:06.051910 s5learn-0.8.4/setup.cfg
+-rw-rw-rw-   0        0        0     1819 2024-05-21 02:48:38.000000 s5learn-0.8.4/setup.py
```

### Comparing `s5learn-0.8.3/s5learn/models/aommon.py` & `s5learn-0.8.4/s5learn/models/aommon.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/models/confmysql.py` & `s5learn-0.8.4/s5learn/models/confmysql.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/models/diz.py` & `s5learn-0.8.4/s5learn/models/diz.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/models/dizcon.py` & `s5learn-0.8.4/s5learn/models/dizcon.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/models/docker.py` & `s5learn-0.8.4/s5learn/models/docker.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/models/dockerfile.py` & `s5learn-0.8.4/s5learn/models/dockerfile.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/models/impddm.py` & `s5learn-0.8.4/s5learn/models/impddm.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/models/logaom.py` & `s5learn-0.8.4/s5learn/models/logaom.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/models/micro.py` & `s5learn-0.8.4/s5learn/models/micro.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/models/mysqlcnf.py` & `s5learn-0.8.4/s5learn/models/mysqlcnf.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/models/opcart.py` & `s5learn-0.8.4/s5learn/models/opcart.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/models/sms.py` & `s5learn-0.8.4/s5learn/models/sms.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/models/wpress.py` & `s5learn-0.8.4/s5learn/models/wpress.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/preprocessing/idp.py` & `s5learn-0.8.4/s5learn/preprocessing/idp.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/preprocessing/m5.py` & `s5learn-0.8.4/s5learn/preprocessing/m5.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/preprocessing/mnv2.py` & `s5learn-0.8.4/s5learn/preprocessing/mnv2.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/preprocessing/mnv2_dp.py` & `s5learn-0.8.4/s5learn/preprocessing/mnv2_dp.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/preprocessing/mnv2_dv.py` & `s5learn-0.8.4/s5learn/preprocessing/mnv2_dv.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/preprocessing/ms.py` & `s5learn-0.8.4/s5learn/preprocessing/ms.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/preprocessing/mv2_train.py` & `s5learn-0.8.4/s5learn/preprocessing/mv2_train.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn/preprocessing/t5.py` & `s5learn-0.8.4/s5learn/preprocessing/t5.py`

 * *Files identical despite different names*

### Comparing `s5learn-0.8.3/s5learn.egg-info/SOURCES.txt` & `s5learn-0.8.4/s5learn.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,28 @@
 setup.py
 s5learn/__init__.py
 s5learn/main.py
 s5learn.egg-info/PKG-INFO
 s5learn.egg-info/SOURCES.txt
 s5learn.egg-info/dependency_links.txt
 s5learn.egg-info/top_level.txt
+s5learn/linear_models/__init__.py
+s5learn/linear_models/cclib.py
+s5learn/linear_models/dplib.py
+s5learn/linear_models/fdlib.py
+s5learn/linear_models/geslib.py
+s5learn/linear_models/ha10lib.py
+s5learn/linear_models/hblib.py
+s5learn/linear_models/hpplib.py
+s5learn/linear_models/kafkalib.py
+s5learn/linear_models/luxlib.py
+s5learn/linear_models/ofblib.py
+s5learn/linear_models/pylib.py
+s5learn/linear_models/sparklib.py
+s5learn/linear_models/splib.py
 s5learn/models/__init__.py
 s5learn/models/aomalarm.py
 s5learn/models/aommon.py
 s5learn/models/appscript.py
 s5learn/models/confmysql.py
 s5learn/models/diz.py
 s5learn/models/dizcon.py
@@ -25,8 +39,12 @@
 s5learn/preprocessing/idp.py
 s5learn/preprocessing/m5.py
 s5learn/preprocessing/mnv2.py
 s5learn/preprocessing/mnv2_dp.py
 s5learn/preprocessing/mnv2_dv.py
 s5learn/preprocessing/ms.py
 s5learn/preprocessing/mv2_train.py
-s5learn/preprocessing/t5.py
+s5learn/preprocessing/sp.py
+s5learn/preprocessing/ss_seqseq.py
+s5learn/preprocessing/t5.py
+s5learn/preprocessing/tn.py
+s5learn/preprocessing/translate.py
```

### Comparing `s5learn-0.8.3/setup.py` & `s5learn-0.8.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 setup(
     name='s5learn',
-    version='0.8.3',
+    version='0.8.4',
     packages=find_packages(),
     package_data={'': ['data/*.txt']},
 )
 
 
 
 # import setuptools
```
