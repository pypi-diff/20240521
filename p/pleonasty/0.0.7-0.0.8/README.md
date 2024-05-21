# Comparing `tmp/pleonasty-0.0.7.tar.gz` & `tmp/pleonasty-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pleonasty-0.0.7.tar", last modified: Mon May 20 20:05:17 2024, max compression
+gzip compressed data, was "pleonasty-0.0.8.tar", last modified: Tue May 21 00:09:51 2024, max compression
```

## Comparing `pleonasty-0.0.7.tar` & `pleonasty-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 20:05:17.017531 pleonasty-0.0.7/
--rw-rw-rw-   0        0        0     1089 2024-03-15 19:33:10.000000 pleonasty-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     1385 2024-05-20 20:05:17.017019 pleonasty-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      621 2024-03-15 20:09:12.000000 pleonasty-0.0.7/README.MD
--rw-rw-rw-   0        0        0      830 2024-05-20 20:01:36.000000 pleonasty-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-20 20:05:17.017531 pleonasty-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-20 20:05:17.011737 pleonasty-0.0.7/src/
--rw-rw-rw-   0        0        0        0 2024-03-15 19:46:12.000000 pleonasty-0.0.7/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 20:05:17.016506 pleonasty-0.0.7/src/pleonasty.egg-info/
--rw-rw-rw-   0        0        0     1385 2024-05-20 20:05:16.000000 pleonasty-0.0.7/src/pleonasty.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-05-20 20:05:16.000000 pleonasty-0.0.7/src/pleonasty.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 20:05:16.000000 pleonasty-0.0.7/src/pleonasty.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      106 2024-05-20 20:05:16.000000 pleonasty-0.0.7/src/pleonasty.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-20 20:05:16.000000 pleonasty-0.0.7/src/pleonasty.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    16483 2024-05-20 20:00:02.000000 pleonasty-0.0.7/src/pleonasty.py
+drwxrwxrwx   0        0        0        0 2024-05-21 00:09:51.183772 pleonasty-0.0.8/
+-rw-rw-rw-   0        0        0     1089 2024-03-15 19:33:10.000000 pleonasty-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1385 2024-05-21 00:09:51.182769 pleonasty-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0      621 2024-03-15 20:09:12.000000 pleonasty-0.0.8/README.MD
+-rw-rw-rw-   0        0        0      830 2024-05-21 00:09:08.000000 pleonasty-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-21 00:09:51.183772 pleonasty-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 00:09:51.165770 pleonasty-0.0.8/src/
+-rw-rw-rw-   0        0        0        0 2024-03-15 19:46:12.000000 pleonasty-0.0.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 00:09:51.182769 pleonasty-0.0.8/src/pleonasty.egg-info/
+-rw-rw-rw-   0        0        0     1385 2024-05-21 00:09:51.000000 pleonasty-0.0.8/src/pleonasty.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-05-21 00:09:51.000000 pleonasty-0.0.8/src/pleonasty.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 00:09:51.000000 pleonasty-0.0.8/src/pleonasty.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      106 2024-05-21 00:09:51.000000 pleonasty-0.0.8/src/pleonasty.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-21 00:09:51.000000 pleonasty-0.0.8/src/pleonasty.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    16666 2024-05-21 00:07:30.000000 pleonasty-0.0.8/src/pleonasty.py
```

### Comparing `pleonasty-0.0.7/LICENSE` & `pleonasty-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pleonasty-0.0.7/PKG-INFO` & `pleonasty-0.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pleonasty
-Version: 0.0.7
+Version: 0.0.8
 Summary: A very simple abstraction for LLMs to get single responses to a given input.
 Author-email: "Ryan L. Boyd" <ryan@ryanboyd.io>
 Project-URL: Homepage, https://github.com/ryanboyd/pleonasty
 Project-URL: Issues, https://github.com/ryanboyd/pleonasty/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pleonasty-0.0.7/README.MD` & `pleonasty-0.0.8/README.MD`

 * *Files identical despite different names*

### Comparing `pleonasty-0.0.7/pyproject.toml` & `pleonasty-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 build-backend = "setuptools.build_meta"
 
 
 [project]
 
 name = "pleonasty"
 
-version = "0.0.7"
+version = "0.0.8"
 
 authors = [
   { name="Ryan L. Boyd", email="ryan@ryanboyd.io" },
 ]
 
 description = "A very simple abstraction for LLMs to get single responses to a given input."
```

### Comparing `pleonasty-0.0.7/src/pleonasty.egg-info/PKG-INFO` & `pleonasty-0.0.8/src/pleonasty.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pleonasty
-Version: 0.0.7
+Version: 0.0.8
 Summary: A very simple abstraction for LLMs to get single responses to a given input.
 Author-email: "Ryan L. Boyd" <ryan@ryanboyd.io>
 Project-URL: Homepage, https://github.com/ryanboyd/pleonasty
 Project-URL: Issues, https://github.com/ryanboyd/pleonasty/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pleonasty-0.0.7/src/pleonasty.py` & `pleonasty-0.0.8/src/pleonasty.py`

 * *Files 3% similar despite different names*

```diff
@@ -181,14 +181,18 @@
                              append_to_existing_csv: bool = False,
                              output_encoding: str = "utf-8-sig",
                              max_seq_length: int = 4096,
                              temperature: float = 0.3,
                              top_k: int = 10,
                              ) -> None:
 
+        if not os.path.exists(os.path.dirname(os.path.abspath(csv_output_location))):
+            os.makedirs(os.path.dirname(os.path.abspath(csv_output_location)))
+            
+
         writemode = 'w'
         if append_to_existing_csv:
             writemode = 'a'
 
         with open(csv_output_location, writemode, encoding=output_encoding, newline='') as fout:
 
             csvw = csv.writer(fout)
```

