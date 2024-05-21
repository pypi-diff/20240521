# Comparing `tmp/revampdeployer-0.1.1.tar.gz` & `tmp/revampdeployer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revampdeployer-0.1.1.tar", last modified: Tue May 21 12:09:18 2024, max compression
+gzip compressed data, was "revampdeployer-0.1.2.tar", last modified: Tue May 21 12:11:50 2024, max compression
```

## Comparing `revampdeployer-0.1.1.tar` & `revampdeployer-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 12:09:18.637691 revampdeployer-0.1.1/
--rw-r--r--   0 evsi       (501) staff       (20)     1069 2024-05-12 12:06:08.000000 revampdeployer-0.1.1/LICENSE
--rw-r--r--   0 evsi       (501) staff       (20)     2121 2024-05-21 12:09:18.637272 revampdeployer-0.1.1/PKG-INFO
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 12:09:18.636231 revampdeployer-0.1.1/revampdeployer/
--rw-r--r--   0 evsi       (501) staff       (20)       22 2024-05-21 11:41:29.000000 revampdeployer-0.1.1/revampdeployer/__init__.py
--rw-r--r--   0 evsi       (501) staff       (20)      103 2024-05-21 11:41:20.000000 revampdeployer-0.1.1/revampdeployer/__main__.py
--rw-r--r--   0 evsi       (501) staff       (20)     6289 2024-05-21 12:07:09.000000 revampdeployer-0.1.1/revampdeployer/deployer.py
-drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 12:09:18.636993 revampdeployer-0.1.1/revampdeployer.egg-info/
--rw-r--r--   0 evsi       (501) staff       (20)     2121 2024-05-21 12:09:18.000000 revampdeployer-0.1.1/revampdeployer.egg-info/PKG-INFO
--rw-r--r--   0 evsi       (501) staff       (20)      290 2024-05-21 12:09:18.000000 revampdeployer-0.1.1/revampdeployer.egg-info/SOURCES.txt
--rw-r--r--   0 evsi       (501) staff       (20)        1 2024-05-21 12:09:18.000000 revampdeployer-0.1.1/revampdeployer.egg-info/dependency_links.txt
--rw-r--r--   0 evsi       (501) staff       (20)       64 2024-05-21 12:09:18.000000 revampdeployer-0.1.1/revampdeployer.egg-info/entry_points.txt
--rw-r--r--   0 evsi       (501) staff       (20)       15 2024-05-21 12:09:18.000000 revampdeployer-0.1.1/revampdeployer.egg-info/top_level.txt
--rw-r--r--   0 evsi       (501) staff       (20)       38 2024-05-21 12:09:18.637740 revampdeployer-0.1.1/setup.cfg
--rw-r--r--   0 evsi       (501) staff       (20)      558 2024-05-21 12:09:17.000000 revampdeployer-0.1.1/setup.py
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 12:11:50.005268 revampdeployer-0.1.2/
+-rw-r--r--   0 evsi       (501) staff       (20)     1069 2024-05-12 12:06:08.000000 revampdeployer-0.1.2/LICENSE
+-rw-r--r--   0 evsi       (501) staff       (20)     2121 2024-05-21 12:11:50.004953 revampdeployer-0.1.2/PKG-INFO
+-rw-r--r--   0 evsi       (501) staff       (20)     1999 2024-05-21 11:45:28.000000 revampdeployer-0.1.2/README.md
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 12:11:50.003793 revampdeployer-0.1.2/revampdeployer/
+-rw-r--r--   0 evsi       (501) staff       (20)       22 2024-05-21 11:41:29.000000 revampdeployer-0.1.2/revampdeployer/__init__.py
+-rw-r--r--   0 evsi       (501) staff       (20)      103 2024-05-21 11:41:20.000000 revampdeployer-0.1.2/revampdeployer/__main__.py
+-rw-r--r--   0 evsi       (501) staff       (20)     6289 2024-05-21 12:07:09.000000 revampdeployer-0.1.2/revampdeployer/deployer.py
+drwxr-xr-x   0 evsi       (501) staff       (20)        0 2024-05-21 12:11:50.004686 revampdeployer-0.1.2/revampdeployer.egg-info/
+-rw-r--r--   0 evsi       (501) staff       (20)     2121 2024-05-21 12:11:49.000000 revampdeployer-0.1.2/revampdeployer.egg-info/PKG-INFO
+-rw-r--r--   0 evsi       (501) staff       (20)      300 2024-05-21 12:11:49.000000 revampdeployer-0.1.2/revampdeployer.egg-info/SOURCES.txt
+-rw-r--r--   0 evsi       (501) staff       (20)        1 2024-05-21 12:11:49.000000 revampdeployer-0.1.2/revampdeployer.egg-info/dependency_links.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       64 2024-05-21 12:11:49.000000 revampdeployer-0.1.2/revampdeployer.egg-info/entry_points.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       15 2024-05-21 12:11:49.000000 revampdeployer-0.1.2/revampdeployer.egg-info/top_level.txt
+-rw-r--r--   0 evsi       (501) staff       (20)       38 2024-05-21 12:11:50.005313 revampdeployer-0.1.2/setup.cfg
+-rw-r--r--   0 evsi       (501) staff       (20)      558 2024-05-21 12:11:36.000000 revampdeployer-0.1.2/setup.py
```

### Comparing `revampdeployer-0.1.1/LICENSE` & `revampdeployer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `revampdeployer-0.1.1/PKG-INFO` & `revampdeployer-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revampdeployer
-Version: 0.1.1
+Version: 0.1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RevampDeployer
 
 RevampDeployer - это инструмент для управления и автоматизации процесса развёртывания приложений на удалённых серверах.
```

### Comparing `revampdeployer-0.1.1/revampdeployer/deployer.py` & `revampdeployer-0.1.2/revampdeployer/deployer.py`

 * *Files identical despite different names*

### Comparing `revampdeployer-0.1.1/revampdeployer.egg-info/PKG-INFO` & `revampdeployer-0.1.2/revampdeployer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revampdeployer
-Version: 0.1.1
+Version: 0.1.2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # RevampDeployer
 
 RevampDeployer - это инструмент для управления и автоматизации процесса развёртывания приложений на удалённых серверах.
```

### Comparing `revampdeployer-0.1.1/setup.py` & `revampdeployer-0.1.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 # Читаем содержимое файла README.md
-with open("ReadMe.md", "r", encoding="utf-8") as f:
+with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="revampdeployer",
-    version="0.1.1",
+    version="0.1.2",
     packages=find_packages(),
     entry_points={
         "console_scripts": [
             "revampdeployer = revampdeployer.__main__:main"
         ]
     },
     # Добавляем описание пакета из README.md
```

