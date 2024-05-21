# Comparing `tmp/groqon-0.1.4.tar.gz` & `tmp/groqon-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "groqon-0.1.4.tar", max compression
+gzip compressed data, was "groqon-0.1.5.tar", max compression
```

## Comparing `groqon-0.1.4.tar` & `groqon-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     3396 2024-04-26 11:47:58.504342 groqon-0.1.4/README.md
--rw-r--r--   0        0        0      112 2024-04-25 19:21:55.434929 groqon-0.1.4/groqon/__init__.py
--rw-r--r--   0        0        0     2904 2024-05-21 09:51:27.256884 groqon-0.1.4/groqon/element_selectors.py
--rw-r--r--   0        0        0     8280 2024-05-21 09:51:27.257884 groqon-0.1.4/groqon/groq.py
--rw-r--r--   0        0        0      229 2024-05-21 09:51:27.257884 groqon-0.1.4/groqon/groq_config.py
--rw-r--r--   0        0        0     8048 2024-05-21 09:51:27.258884 groqon-0.1.4/groqon/groq_utils.py
--rw-r--r--   0        0        0      930 2024-05-21 09:51:27.258884 groqon-0.1.4/groqon/parsing.py
--rw-r--r--   0        0        0      478 2024-05-21 09:51:27.264884 groqon-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3797 1970-01-01 00:00:00.000000 groqon-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3396 2024-04-26 11:47:58.504342 groqon-0.1.5/README.md
+-rw-r--r--   0        0        0      112 2024-04-25 19:21:55.434929 groqon-0.1.5/groqon/__init__.py
+-rw-r--r--   0        0        0     2904 2024-05-21 09:51:27.256884 groqon-0.1.5/groqon/element_selectors.py
+-rw-r--r--   0        0        0     8280 2024-05-21 09:51:27.257884 groqon-0.1.5/groqon/groq.py
+-rw-r--r--   0        0        0      229 2024-05-21 09:51:27.257884 groqon-0.1.5/groqon/groq_config.py
+-rw-r--r--   0        0        0     8048 2024-05-21 09:51:27.258884 groqon-0.1.5/groqon/groq_utils.py
+-rw-r--r--   0        0        0      930 2024-05-21 09:51:27.258884 groqon-0.1.5/groqon/parsing.py
+-rw-r--r--   0        0        0      471 2024-05-21 09:53:59.730319 groqon-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3847 1970-01-01 00:00:00.000000 groqon-0.1.5/PKG-INFO
```

### Comparing `groqon-0.1.4/README.md` & `groqon-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `groqon-0.1.4/groqon/element_selectors.py` & `groqon-0.1.5/groqon/element_selectors.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.4/groqon/groq.py` & `groqon-0.1.5/groqon/groq.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.4/groqon/groq_utils.py` & `groqon-0.1.5/groqon/groq_utils.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.4/groqon/parsing.py` & `groqon-0.1.5/groqon/parsing.py`

 * *Files identical despite different names*

### Comparing `groqon-0.1.4/PKG-INFO` & `groqon-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: groqon
-Version: 0.1.4
+Version: 0.1.5
 Summary: Use Groq.com as llm
 Author: tikendraw
 Author-email: tikendraksahu1029@gmail.com
-Requires-Python: >=3.11,<3.12
+Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: playwright (>=1.44.0,<2.0.0)
 Requires-Dist: unstructured (>=0.13.4,<0.14.0)
 Description-Content-Type: text/markdown
 
 # GROQ without API : GroqOn
 
 This projects uses playwright to Access [GROQ](https://www.groq.com) using python
```

