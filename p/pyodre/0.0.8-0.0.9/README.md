# Comparing `tmp/pyodre-0.0.8.tar.gz` & `tmp/pyodre-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "pyodre-0.0.9.tar", last modified: Tue May 21 11:38:38 2024, max compression
```

## Comparing `pyodre-0.0.8.tar` & `pyodre-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 pyodre-0.0.8/.idea/.gitignore
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 pyodre-0.0.8/.idea/.name
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pyodre-0.0.8/.idea/misc.xml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pyodre-0.0.8/.idea/modules.xml
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 pyodre-0.0.8/.idea/pyodre.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pyodre-0.0.8/.idea/vcs.xml
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 pyodre-0.0.8/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pyodre-0.0.8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodre-0.0.8/pyodre/__init__.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 pyodre-0.0.8/pyodre/interpreters.py
--rw-r--r--   0        0        0     4447 2020-02-02 00:00:00.000000 pyodre-0.0.8/pyodre/odre.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 pyodre-0.0.8/pyodre/python_functions.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 pyodre-0.0.8/pyodre/python_interpreter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodre-0.0.8/test/__init__.py
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyodre-0.0.8/LICENSE
--rw-r--r--   0        0        0     9295 2020-02-02 00:00:00.000000 pyodre-0.0.8/README.md
--rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 pyodre-0.0.8/pyproject.toml
--rw-r--r--   0        0        0    22890 2020-02-02 00:00:00.000000 pyodre-0.0.8/PKG-INFO
+drwxr-xr-x   0 andreacimmino   (501) staff       (20)        0 2024-05-21 11:38:38.301355 pyodre-0.0.9/
+-rw-r--r--   0 andreacimmino   (501) staff       (20)    11357 2024-05-21 09:54:40.000000 pyodre-0.0.9/LICENSE
+-rw-r--r--   0 andreacimmino   (501) staff       (20)     9782 2024-05-21 11:38:38.301071 pyodre-0.0.9/PKG-INFO
+-rw-r--r--   0 andreacimmino   (501) staff       (20)     9295 2024-05-08 18:53:08.000000 pyodre-0.0.9/README.md
+drwxr-xr-x   0 andreacimmino   (501) staff       (20)        0 2024-05-21 11:38:38.297957 pyodre-0.0.9/pyodre/
+-rw-r--r--   0 andreacimmino   (501) staff       (20)        0 2024-05-21 11:29:13.000000 pyodre-0.0.9/pyodre/__init__.py
+-rw-r--r--   0 andreacimmino   (501) staff       (20)      273 2024-05-08 17:47:54.000000 pyodre-0.0.9/pyodre/interpreters.py
+-rw-r--r--   0 andreacimmino   (501) staff       (20)     4447 2024-05-21 10:23:12.000000 pyodre-0.0.9/pyodre/odre.py
+-rw-r--r--   0 andreacimmino   (501) staff       (20)      960 2024-05-08 18:01:32.000000 pyodre-0.0.9/pyodre/python_functions.py
+-rw-r--r--   0 andreacimmino   (501) staff       (20)     2668 2024-05-21 10:30:38.000000 pyodre-0.0.9/pyodre/python_interpreter.py
+drwxr-xr-x   0 andreacimmino   (501) staff       (20)        0 2024-05-21 11:38:38.300240 pyodre-0.0.9/pyodre.egg-info/
+-rw-r--r--   0 andreacimmino   (501) staff       (20)     9782 2024-05-21 11:38:38.000000 pyodre-0.0.9/pyodre.egg-info/PKG-INFO
+-rw-r--r--   0 andreacimmino   (501) staff       (20)      320 2024-05-21 11:38:38.000000 pyodre-0.0.9/pyodre.egg-info/SOURCES.txt
+-rw-r--r--   0 andreacimmino   (501) staff       (20)        1 2024-05-21 11:38:38.000000 pyodre-0.0.9/pyodre.egg-info/dependency_links.txt
+-rw-r--r--   0 andreacimmino   (501) staff       (20)       28 2024-05-21 11:38:38.000000 pyodre-0.0.9/pyodre.egg-info/requires.txt
+-rw-r--r--   0 andreacimmino   (501) staff       (20)       12 2024-05-21 11:38:38.000000 pyodre-0.0.9/pyodre.egg-info/top_level.txt
+-rw-r--r--   0 andreacimmino   (501) staff       (20)       93 2024-05-21 11:38:11.000000 pyodre-0.0.9/pyproject.toml
+-rw-r--r--   0 andreacimmino   (501) staff       (20)       38 2024-05-21 11:38:38.301444 pyodre-0.0.9/setup.cfg
+-rw-r--r--   0 andreacimmino   (501) staff       (20)      884 2024-05-21 11:37:54.000000 pyodre-0.0.9/setup.py
+drwxr-xr-x   0 andreacimmino   (501) staff       (20)        0 2024-05-21 11:38:38.300685 pyodre-0.0.9/test/
+-rw-r--r--   0 andreacimmino   (501) staff       (20)        0 2024-05-21 10:42:49.000000 pyodre-0.0.9/test/__init__.py
```

### Comparing `pyodre-0.0.8/pyodre/odre.py` & `pyodre-0.0.9/pyodre/odre.py`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.8/pyodre/python_functions.py` & `pyodre-0.0.9/pyodre/python_functions.py`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.8/pyodre/python_interpreter.py` & `pyodre-0.0.9/pyodre/python_interpreter.py`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.8/LICENSE` & `pyodre-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodre-0.0.8/README.md` & `pyodre-0.0.9/README.md`

 * *Files identical despite different names*

