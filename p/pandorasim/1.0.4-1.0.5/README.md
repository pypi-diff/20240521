# Comparing `tmp/pandorasim-1.0.4.tar.gz` & `tmp/pandorasim-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandorasim-1.0.4.tar", max compression
+gzip compressed data, was "pandorasim-1.0.5.tar", max compression
```

## Comparing `pandorasim-1.0.4.tar` & `pandorasim-1.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1073 2022-08-04 17:51:49.568934 pandorasim-1.0.4/LICENSE
--rw-r--r--   0        0        0      229 2024-05-21 17:26:54.940213 pandorasim-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      419 2024-05-21 17:27:00.156611 pandorasim-1.0.4/src/pandorasim/__init__.py
--rw-r--r--   0        0        0     4727 2024-05-21 02:31:51.097149 pandorasim-1.0.4/src/pandorasim/docstrings.py
--rw-r--r--   0        0        0    14831 2024-05-21 17:26:05.474937 pandorasim-1.0.4/src/pandorasim/nirsim.py
--rw-r--r--   0        0        0     6368 2024-05-21 17:25:58.109880 pandorasim-1.0.4/src/pandorasim/sim.py
--rw-r--r--   0        0        0    10482 2024-05-21 02:31:51.097745 pandorasim-1.0.4/src/pandorasim/utils.py
--rw-r--r--   0        0        0    20033 2024-05-21 17:26:34.804258 pandorasim-1.0.4/src/pandorasim/visiblesim.py
--rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 pandorasim-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1073 2022-08-04 17:51:49.568934 pandorasim-1.0.5/LICENSE
+-rw-r--r--   0        0        0      229 2024-05-21 17:31:07.918832 pandorasim-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      419 2024-05-21 17:31:01.645650 pandorasim-1.0.5/src/pandorasim/__init__.py
+-rw-r--r--   0        0        0     4727 2024-05-21 02:31:51.097149 pandorasim-1.0.5/src/pandorasim/docstrings.py
+-rw-r--r--   0        0        0    14831 2024-05-21 17:26:05.474937 pandorasim-1.0.5/src/pandorasim/nirsim.py
+-rw-r--r--   0        0        0     6368 2024-05-21 17:25:58.109880 pandorasim-1.0.5/src/pandorasim/sim.py
+-rw-r--r--   0        0        0    10482 2024-05-21 02:31:51.097745 pandorasim-1.0.5/src/pandorasim/utils.py
+-rw-r--r--   0        0        0    20033 2024-05-21 17:26:34.804258 pandorasim-1.0.5/src/pandorasim/visiblesim.py
+-rw-r--r--   0        0        0      485 1970-01-01 00:00:00.000000 pandorasim-1.0.5/PKG-INFO
```

### Comparing `pandorasim-1.0.4/LICENSE` & `pandorasim-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.4/src/pandorasim/docstrings.py` & `pandorasim-1.0.5/src/pandorasim/docstrings.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.4/src/pandorasim/nirsim.py` & `pandorasim-1.0.5/src/pandorasim/nirsim.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.4/src/pandorasim/sim.py` & `pandorasim-1.0.5/src/pandorasim/sim.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.4/src/pandorasim/utils.py` & `pandorasim-1.0.5/src/pandorasim/utils.py`

 * *Files identical despite different names*

### Comparing `pandorasim-1.0.4/src/pandorasim/visiblesim.py` & `pandorasim-1.0.5/src/pandorasim/visiblesim.py`

 * *Files identical despite different names*

