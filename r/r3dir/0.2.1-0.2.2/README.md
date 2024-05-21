# Comparing `tmp/r3dir-0.2.1.tar.gz` & `tmp/r3dir-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "r3dir-0.2.1.tar", last modified: Mon May 20 15:43:32 2024, max compression
+gzip compressed data, was "r3dir-0.2.2.tar", last modified: Tue May 21 13:12:55 2024, max compression
```

## Comparing `r3dir-0.2.1.tar` & `r3dir-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-20 15:43:32.237931 r3dir-0.2.1/
--rw-r--r--   0 vladyslav   (501) staff       (20)    11357 2023-02-22 16:24:18.000000 r3dir-0.2.1/LICENSE
--rw-r--r--   0 vladyslav   (501) staff       (20)     4608 2024-05-20 15:43:32.237748 r3dir-0.2.1/PKG-INFO
--rw-r--r--   0 vladyslav   (501) staff       (20)     4073 2024-05-20 15:31:46.000000 r3dir-0.2.1/PYPIREADME.md
--rw-r--r--   0 vladyslav   (501) staff       (20)     8758 2024-05-20 15:23:08.000000 r3dir-0.2.1/README.md
--rw-r--r--   0 vladyslav   (501) staff       (20)      763 2024-05-20 15:43:17.000000 r3dir-0.2.1/pyproject.toml
-drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-20 15:43:32.235190 r3dir-0.2.1/r3dir/
--rw-r--r--   0 vladyslav   (501) staff       (20)        0 2023-02-22 16:24:18.000000 r3dir-0.2.1/r3dir/__init__.py
--rw-r--r--   0 vladyslav   (501) staff       (20)     4840 2024-05-20 15:30:32.000000 r3dir-0.2.1/r3dir/_cli.py
--rw-r--r--   0 vladyslav   (501) staff       (20)     5016 2024-05-14 16:39:37.000000 r3dir-0.2.1/r3dir/encoder.py
--rw-r--r--   0 vladyslav   (501) staff       (20)      484 2023-04-05 17:33:07.000000 r3dir-0.2.1/r3dir/exceptions.py
-drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-20 15:43:32.236113 r3dir-0.2.1/r3dir/hackvertor/
--rw-r--r--   0 vladyslav   (501) staff       (20)    57159 2024-05-20 12:52:49.000000 r3dir-0.2.1/r3dir/hackvertor/encoder.js
-drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-20 15:43:32.237530 r3dir-0.2.1/r3dir.egg-info/
--rw-r--r--   0 vladyslav   (501) staff       (20)     4608 2024-05-20 15:43:32.000000 r3dir-0.2.1/r3dir.egg-info/PKG-INFO
--rw-r--r--   0 vladyslav   (501) staff       (20)      341 2024-05-20 15:43:32.000000 r3dir-0.2.1/r3dir.egg-info/SOURCES.txt
--rw-r--r--   0 vladyslav   (501) staff       (20)        1 2024-05-20 15:43:32.000000 r3dir-0.2.1/r3dir.egg-info/dependency_links.txt
--rw-r--r--   0 vladyslav   (501) staff       (20)       42 2024-05-20 15:43:32.000000 r3dir-0.2.1/r3dir.egg-info/entry_points.txt
--rw-r--r--   0 vladyslav   (501) staff       (20)       23 2024-05-20 15:43:32.000000 r3dir-0.2.1/r3dir.egg-info/requires.txt
--rw-r--r--   0 vladyslav   (501) staff       (20)        6 2024-05-20 15:43:32.000000 r3dir-0.2.1/r3dir.egg-info/top_level.txt
--rw-r--r--   0 vladyslav   (501) staff       (20)       38 2024-05-20 15:43:32.237973 r3dir-0.2.1/setup.cfg
-drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-20 15:43:32.236255 r3dir-0.2.1/tests/
--rw-r--r--   0 vladyslav   (501) staff       (20)     9098 2024-05-14 09:22:39.000000 r3dir-0.2.1/tests/test_encoder.py
+drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-21 13:12:55.337128 r3dir-0.2.2/
+-rw-r--r--   0 vladyslav   (501) staff       (20)    11357 2023-02-22 16:24:18.000000 r3dir-0.2.2/LICENSE
+-rw-r--r--   0 vladyslav   (501) staff       (20)     4608 2024-05-21 13:12:55.336909 r3dir-0.2.2/PKG-INFO
+-rw-r--r--   0 vladyslav   (501) staff       (20)     4073 2024-05-20 15:31:46.000000 r3dir-0.2.2/PYPIREADME.md
+-rw-r--r--   0 vladyslav   (501) staff       (20)     8758 2024-05-20 15:23:08.000000 r3dir-0.2.2/README.md
+-rw-r--r--   0 vladyslav   (501) staff       (20)      763 2024-05-21 13:11:56.000000 r3dir-0.2.2/pyproject.toml
+drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-21 13:12:55.333749 r3dir-0.2.2/r3dir/
+-rw-r--r--   0 vladyslav   (501) staff       (20)        0 2023-02-22 16:24:18.000000 r3dir-0.2.2/r3dir/__init__.py
+-rw-r--r--   0 vladyslav   (501) staff       (20)     4840 2024-05-20 15:30:32.000000 r3dir-0.2.2/r3dir/_cli.py
+-rw-r--r--   0 vladyslav   (501) staff       (20)     4983 2024-05-21 13:10:14.000000 r3dir-0.2.2/r3dir/encoder.py
+-rw-r--r--   0 vladyslav   (501) staff       (20)      484 2023-04-05 17:33:07.000000 r3dir-0.2.2/r3dir/exceptions.py
+drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-21 13:12:55.334841 r3dir-0.2.2/r3dir/hackvertor/
+-rw-r--r--   0 vladyslav   (501) staff       (20)    57236 2024-05-21 13:10:33.000000 r3dir-0.2.2/r3dir/hackvertor/encoder.js
+drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-21 13:12:55.336609 r3dir-0.2.2/r3dir.egg-info/
+-rw-r--r--   0 vladyslav   (501) staff       (20)     4608 2024-05-21 13:12:55.000000 r3dir-0.2.2/r3dir.egg-info/PKG-INFO
+-rw-r--r--   0 vladyslav   (501) staff       (20)      341 2024-05-21 13:12:55.000000 r3dir-0.2.2/r3dir.egg-info/SOURCES.txt
+-rw-r--r--   0 vladyslav   (501) staff       (20)        1 2024-05-21 13:12:55.000000 r3dir-0.2.2/r3dir.egg-info/dependency_links.txt
+-rw-r--r--   0 vladyslav   (501) staff       (20)       42 2024-05-21 13:12:55.000000 r3dir-0.2.2/r3dir.egg-info/entry_points.txt
+-rw-r--r--   0 vladyslav   (501) staff       (20)       23 2024-05-21 13:12:55.000000 r3dir-0.2.2/r3dir.egg-info/requires.txt
+-rw-r--r--   0 vladyslav   (501) staff       (20)        6 2024-05-21 13:12:55.000000 r3dir-0.2.2/r3dir.egg-info/top_level.txt
+-rw-r--r--   0 vladyslav   (501) staff       (20)       38 2024-05-21 13:12:55.337170 r3dir-0.2.2/setup.cfg
+drwxr-xr-x   0 vladyslav   (501) staff       (20)        0 2024-05-21 13:12:55.335796 r3dir-0.2.2/tests/
+-rw-r--r--   0 vladyslav   (501) staff       (20)     9098 2024-05-14 09:22:39.000000 r3dir-0.2.2/tests/test_encoder.py
```

### Comparing `r3dir-0.2.1/LICENSE` & `r3dir-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `r3dir-0.2.1/PKG-INFO` & `r3dir-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r3dir
-Version: 0.2.1
+Version: 0.2.2
 Summary: r3dir encoder/decoder package with CLI tool
 Author: Horlad
 Project-URL: Homepage, https://github.com/Horlad/r3dir
 Project-URL: Bug Tracker, https://github.com/Horlad/r3dir/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `r3dir-0.2.1/PYPIREADME.md` & `r3dir-0.2.2/PYPIREADME.md`

 * *Files identical despite different names*

### Comparing `r3dir-0.2.1/README.md` & `r3dir-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `r3dir-0.2.1/pyproject.toml` & `r3dir-0.2.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "r3dir"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   {name="Horlad"},
 ]
 description = "r3dir encoder/decoder package with CLI tool"
 readme = "PYPIREADME.md" 
 requires-python = ">=3.10"
 dependencies = [
```

### Comparing `r3dir-0.2.1/r3dir/_cli.py` & `r3dir-0.2.2/r3dir/_cli.py`

 * *Files identical despite different names*

### Comparing `r3dir-0.2.1/r3dir/encoder.py` & `r3dir-0.2.2/r3dir/encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 
     main_domain_chunk_count = len(main_domain.split('.'))
 
     subdomains_without_main = subdomains[:-main_domain_chunk_count]
     
     start_of_encoded_target = 0
     if IGNORE_PART_SEP in subdomains_without_main:
-        start_of_encoded_target = len(subdomains_without_main) - subdomains_without_main[::-1].index(IGNORE_PART_SEP)
+        start_of_encoded_target = subdomains_without_main.index(IGNORE_PART_SEP) + 1
     
     encoded_subdomains = subdomains_without_main[start_of_encoded_target:]
 
     if target_url_hash := _is_too_long_target_error(encoded_subdomains):
         raise TooLongTarget(f"The target length has been too long for encoder. Target's SHA-1: {target_url_hash}")
 
     try:
```

### Comparing `r3dir-0.2.1/r3dir/hackvertor/encoder.js` & `r3dir-0.2.2/r3dir/hackvertor/encoder.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1711,15 +1711,15 @@
     const mainDomainChunkCount = mainDomain.split('.').length;
     const subdomainsWithoutMain = subdomains.slice(0, -mainDomainChunkCount);
     let startOfEncodedTarget = 0;
     if (subdomainsWithoutMain.includes(IGNORE_PART_SEP)) {
         startOfEncodedTarget = subdomainsWithoutMain.indexOf(IGNORE_PART_SEP) + 1;
     }
 
-    const encodedSubdomains = subdomainsWithoutMain.slice(-startOfEncodedTarget);
+    const encodedSubdomains = subdomainsWithoutMain.slice(startOfEncodedTarget);
     const targetUrlHash = isTooLongTargetError(encodedSubdomains);
     if (targetUrlHash) {
         throw new Error(`The target length has been too long for encoder. Target's SHA-1: ${targetUrlHash}`);
     }
 
     let statusCode;
 
@@ -1742,8 +1742,10 @@
 
 // Node.js env detection
 if ((typeof process !== 'undefined') && (process.release.name === 'node')) {
     module.exports = {
         encode,
         decode
     };
-}
+}
+
+const result = decode("62epax54k4z4o2wubwlx57p374.302.r3dir.me", 'r3dir.me');
```

### Comparing `r3dir-0.2.1/r3dir.egg-info/PKG-INFO` & `r3dir-0.2.2/r3dir.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: r3dir
-Version: 0.2.1
+Version: 0.2.2
 Summary: r3dir encoder/decoder package with CLI tool
 Author: Horlad
 Project-URL: Homepage, https://github.com/Horlad/r3dir
 Project-URL: Bug Tracker, https://github.com/Horlad/r3dir/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `r3dir-0.2.1/tests/test_encoder.py` & `r3dir-0.2.2/tests/test_encoder.py`

 * *Files identical despite different names*

