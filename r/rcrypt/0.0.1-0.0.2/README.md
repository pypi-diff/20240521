# Comparing `tmp/rcrypt-0.0.1.tar.gz` & `tmp/rcrypt-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcrypt-0.0.1.tar", last modified: Sat May 11 07:05:20 2024, max compression
+gzip compressed data, was "rcrypt-0.0.2.tar", last modified: Tue May 21 03:18:18 2024, max compression
```

## Comparing `rcrypt-0.0.1.tar` & `rcrypt-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-11 07:05:20.031411 rcrypt-0.0.1/
--rw-r--r--   0 a08030320   (501) staff       (20)     1073 2024-01-09 12:07:09.000000 rcrypt-0.0.1/LICENSE
--rw-r--r--   0 a08030320   (501) staff       (20)      476 2024-05-11 07:05:20.031107 rcrypt-0.0.1/PKG-INFO
--rw-r--r--   0 a08030320   (501) staff       (20)       81 2024-05-11 06:59:18.000000 rcrypt-0.0.1/README.md
-drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-11 07:05:20.029599 rcrypt-0.0.1/rancrypt/
--rw-r--r--   0 a08030320   (501) staff       (20)     1028 2024-05-11 06:51:00.000000 rcrypt-0.0.1/rancrypt/RCrypt.py
--rw-r--r--   0 a08030320   (501) staff       (20)        0 2024-05-11 06:49:54.000000 rcrypt-0.0.1/rancrypt/__init__.py
-drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-11 07:05:20.030778 rcrypt-0.0.1/rcrypt.egg-info/
--rw-r--r--   0 a08030320   (501) staff       (20)      476 2024-05-11 07:05:19.000000 rcrypt-0.0.1/rcrypt.egg-info/PKG-INFO
--rw-r--r--   0 a08030320   (501) staff       (20)      215 2024-05-11 07:05:19.000000 rcrypt-0.0.1/rcrypt.egg-info/SOURCES.txt
--rw-r--r--   0 a08030320   (501) staff       (20)        1 2024-05-11 07:05:19.000000 rcrypt-0.0.1/rcrypt.egg-info/dependency_links.txt
--rw-r--r--   0 a08030320   (501) staff       (20)       14 2024-05-11 07:05:19.000000 rcrypt-0.0.1/rcrypt.egg-info/requires.txt
--rw-r--r--   0 a08030320   (501) staff       (20)        9 2024-05-11 07:05:19.000000 rcrypt-0.0.1/rcrypt.egg-info/top_level.txt
--rw-r--r--   0 a08030320   (501) staff       (20)       38 2024-05-11 07:05:20.031473 rcrypt-0.0.1/setup.cfg
--rw-r--r--   0 a08030320   (501) staff       (20)     1246 2024-05-11 07:03:04.000000 rcrypt-0.0.1/setup.py
+drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-21 03:18:18.021723 rcrypt-0.0.2/
+-rw-r--r--   0 a08030320   (501) staff       (20)     1073 2024-01-09 12:07:09.000000 rcrypt-0.0.2/LICENSE
+-rw-r--r--   0 a08030320   (501) staff       (20)      512 2024-05-21 03:18:18.021301 rcrypt-0.0.2/PKG-INFO
+-rw-r--r--   0 a08030320   (501) staff       (20)       81 2024-05-11 06:59:18.000000 rcrypt-0.0.2/README.md
+drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-21 03:18:18.019943 rcrypt-0.0.2/rancrypt/
+-rw-r--r--   0 a08030320   (501) staff       (20)     1028 2024-05-11 06:51:00.000000 rcrypt-0.0.2/rancrypt/RCrypt.py
+-rw-r--r--   0 a08030320   (501) staff       (20)     1470 2024-05-21 03:15:01.000000 rcrypt-0.0.2/rancrypt/Rrsa.py
+-rw-r--r--   0 a08030320   (501) staff       (20)        0 2024-05-11 06:49:54.000000 rcrypt-0.0.2/rancrypt/__init__.py
+drwxr-xr-x   0 a08030320   (501) staff       (20)        0 2024-05-21 03:18:18.020954 rcrypt-0.0.2/rcrypt.egg-info/
+-rw-r--r--   0 a08030320   (501) staff       (20)      512 2024-05-21 03:18:17.000000 rcrypt-0.0.2/rcrypt.egg-info/PKG-INFO
+-rw-r--r--   0 a08030320   (501) staff       (20)      232 2024-05-21 03:18:17.000000 rcrypt-0.0.2/rcrypt.egg-info/SOURCES.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)        1 2024-05-21 03:18:17.000000 rcrypt-0.0.2/rcrypt.egg-info/dependency_links.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)       35 2024-05-21 03:18:17.000000 rcrypt-0.0.2/rcrypt.egg-info/requires.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)        9 2024-05-21 03:18:17.000000 rcrypt-0.0.2/rcrypt.egg-info/top_level.txt
+-rw-r--r--   0 a08030320   (501) staff       (20)       38 2024-05-21 03:18:18.021797 rcrypt-0.0.2/setup.cfg
+-rw-r--r--   0 a08030320   (501) staff       (20)     1282 2024-05-21 03:15:40.000000 rcrypt-0.0.2/setup.py
```

### Comparing `rcrypt-0.0.1/LICENSE` & `rcrypt-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rcrypt-0.0.1/rancrypt/RCrypt.py` & `rcrypt-0.0.2/rancrypt/RCrypt.py`

 * *Files identical despite different names*

### Comparing `rcrypt-0.0.1/setup.py` & `rcrypt-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     # 包的分发名称，使用字母、数字、_、-
     name="rcrypt",
-    version="0.0.1",
+    version="0.0.2",
     # 作者名
     author="ranyu",
     # 作者邮箱
     author_email="wy176404@163.com",
     # 包的简介描述
     description="Libraries for encryption and alignment",
     # 包的详细介绍(一般通过加载README.md)
@@ -28,9 +28,10 @@
         # 根据MIT许可证开源
         "License :: OSI Approved :: MIT License",
         # 与操作系统无关
         "Operating System :: OS Independent",
     ],
     install_requires=[
             'bcrypt~=4.1.3',
+            'pycryptodome==3.19.0',
         ]
 )
```

