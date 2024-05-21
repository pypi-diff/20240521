# Comparing `tmp/pandorasim-1.0.2.tar.gz` & `tmp/pandorasim-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandorasim-1.0.2.tar", max compression
+gzip compressed data, was "pandorasim-1.0.3.tar", max compression
```

## Comparing `pandorasim-1.0.2.tar` & `pandorasim-1.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2022-08-04 17:51:49.568934 pandorasim-1.0.2/LICENSE
--rw-r--r--   0        0        0      228 2024-05-21 03:25:14.531084 pandorasim-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      419 2024-05-21 03:25:28.317846 pandorasim-1.0.2/src/pandorasim/__init__.py
--rw-r--r--   0        0        0     4727 2024-05-21 02:31:51.097149 pandorasim-1.0.2/src/pandorasim/docstrings.py
--rw-r--r--   0        0        0    14831 2024-05-21 02:31:51.097349 pandorasim-1.0.2/src/pandorasim/nirsim.py
--rw-r--r--   0        0        0     6351 2024-05-21 02:31:51.097525 pandorasim-1.0.2/src/pandorasim/sim.py
--rw-r--r--   0        0        0    10482 2024-05-21 02:31:51.097745 pandorasim-1.0.2/src/pandorasim/utils.py
--rw-r--r--   0        0        0    19887 2024-05-21 02:31:51.097951 pandorasim-1.0.2/src/pandorasim/visiblesim.py
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 pandorasim-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-08-04 17:51:49.568934 pandorasim-1.0.3/LICENSE
+-rw-r--r--   0        0        0      229 2024-05-21 03:54:38.629003 pandorasim-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      419 2024-05-21 03:54:47.765205 pandorasim-1.0.3/src/pandorasim/__init__.py
+-rw-r--r--   0        0        0     4727 2024-05-21 02:31:51.097149 pandorasim-1.0.3/src/pandorasim/docstrings.py
+-rw-r--r--   0        0        0    14831 2024-05-21 02:31:51.097349 pandorasim-1.0.3/src/pandorasim/nirsim.py
+-rw-r--r--   0        0        0     6351 2024-05-21 02:31:51.097525 pandorasim-1.0.3/src/pandorasim/sim.py
+-rw-r--r--   0        0        0    10482 2024-05-21 02:31:51.097745 pandorasim-1.0.3/src/pandorasim/utils.py
+-rw-r--r--   0        0        0    19887 2024-05-21 02:31:51.097951 pandorasim-1.0.3/src/pandorasim/visiblesim.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 pandorasim-1.0.3/PKG-INFO
```

### Comparing `pandorasim-1.0.2/LICENSE` & `pandorasim-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.2/src/pandorasim/docstrings.py` & `pandorasim-1.0.3/src/pandorasim/docstrings.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.2/src/pandorasim/nirsim.py` & `pandorasim-1.0.3/src/pandorasim/nirsim.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.2/src/pandorasim/sim.py` & `pandorasim-1.0.3/src/pandorasim/sim.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.2/src/pandorasim/utils.py` & `pandorasim-1.0.3/src/pandorasim/utils.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.2/src/pandorasim/visiblesim.py` & `pandorasim-1.0.3/src/pandorasim/visiblesim.py`

 * *Files identical despite different names*

