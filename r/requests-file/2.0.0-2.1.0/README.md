# Comparing `tmp/requests-file-2.0.0.tar.gz` & `tmp/requests_file-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests-file-2.0.0.tar", last modified: Mon Jan 29 18:50:18 2024, max compression
+gzip compressed data, was "requests_file-2.1.0.tar", last modified: Tue May 21 16:20:14 2024, max compression
```

## Comparing `requests-file-2.0.0.tar` & `requests_file-2.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 dshea    (21182) dshea    (21182)        0 2024-01-29 18:50:18.400350 requests-file-2.0.0/
-drwxr-xr-x   0 dshea    (21182) dshea    (21182)        0 2024-01-29 18:50:18.398350 requests-file-2.0.0/.github/
-drwxr-xr-x   0 dshea    (21182) dshea    (21182)        0 2024-01-29 18:50:18.399350 requests-file-2.0.0/.github/workflows/
--rw-r--r--   0 dshea    (21182) dshea    (21182)     1171 2024-01-29 18:14:36.000000 requests-file-2.0.0/.github/workflows/test.yml
--rw-r--r--   0 dshea    (21182) dshea    (21182)       63 2024-01-29 18:08:04.000000 requests-file-2.0.0/.gitignore
--rw-r--r--   0 dshea    (21182) dshea    (21182)     1569 2024-01-29 18:27:18.000000 requests-file-2.0.0/CHANGES.rst
--rw-r--r--   0 dshea    (21182) dshea    (21182)      581 2024-01-29 18:08:04.000000 requests-file-2.0.0/LICENSE
--rw-r--r--   0 dshea    (21182) dshea    (21182)       79 2024-01-29 18:08:04.000000 requests-file-2.0.0/MANIFEST.in
--rw-r--r--   0 dshea    (21182) dshea    (21182)     1696 2024-01-29 18:50:18.400350 requests-file-2.0.0/PKG-INFO
--rw-r--r--   0 dshea    (21182) dshea    (21182)     1134 2024-01-29 18:08:04.000000 requests-file-2.0.0/README.rst
--rw-r--r--   0 dshea    (21182) dshea    (21182)      820 2024-01-29 18:14:36.000000 requests-file-2.0.0/pyproject.toml
-drwxr-xr-x   0 dshea    (21182) dshea    (21182)        0 2024-01-29 18:50:18.400350 requests-file-2.0.0/requests_file.egg-info/
--rw-r--r--   0 dshea    (21182) dshea    (21182)     1696 2024-01-29 18:50:18.000000 requests-file-2.0.0/requests_file.egg-info/PKG-INFO
--rw-r--r--   0 dshea    (21182) dshea    (21182)      324 2024-01-29 18:50:18.000000 requests-file-2.0.0/requests_file.egg-info/SOURCES.txt
--rw-r--r--   0 dshea    (21182) dshea    (21182)        1 2024-01-29 18:50:18.000000 requests-file-2.0.0/requests_file.egg-info/dependency_links.txt
--rw-r--r--   0 dshea    (21182) dshea    (21182)       16 2024-01-29 18:50:18.000000 requests-file-2.0.0/requests_file.egg-info/requires.txt
--rw-r--r--   0 dshea    (21182) dshea    (21182)       14 2024-01-29 18:50:18.000000 requests-file-2.0.0/requests_file.egg-info/top_level.txt
--rw-r--r--   0 dshea    (21182) dshea    (21182)     4794 2024-01-29 18:14:36.000000 requests-file-2.0.0/requests_file.py
--rw-r--r--   0 dshea    (21182) dshea    (21182)       38 2024-01-29 18:50:18.400350 requests-file-2.0.0/setup.cfg
-drwxr-xr-x   0 dshea    (21182) dshea    (21182)        0 2024-01-29 18:50:18.399350 requests-file-2.0.0/tests/
--rw-r--r--   0 dshea    (21182) dshea    (21182)     7347 2024-01-29 18:08:04.000000 requests-file-2.0.0/tests/test_requests_file.py
+drwxr-xr-x   0 dshea     (1000) dshea     (1000)        0 2024-05-21 16:20:14.997106 requests_file-2.1.0/
+drwxr-xr-x   0 dshea     (1000) dshea     (1000)        0 2024-05-21 16:20:14.993106 requests_file-2.1.0/.github/
+drwxr-xr-x   0 dshea     (1000) dshea     (1000)        0 2024-05-21 16:20:14.995106 requests_file-2.1.0/.github/workflows/
+-rw-r--r--   0 dshea     (1000) dshea     (1000)     1171 2024-01-20 13:36:07.000000 requests_file-2.1.0/.github/workflows/test.yml
+-rw-r--r--   0 dshea     (1000) dshea     (1000)       63 2022-10-20 14:11:26.000000 requests_file-2.1.0/.gitignore
+-rw-r--r--   0 dshea     (1000) dshea     (1000)     1669 2024-05-21 16:18:08.000000 requests_file-2.1.0/CHANGES.rst
+-rw-r--r--   0 dshea     (1000) dshea     (1000)      581 2022-10-20 14:11:26.000000 requests_file-2.1.0/LICENSE
+-rw-r--r--   0 dshea     (1000) dshea     (1000)       79 2022-10-20 14:11:26.000000 requests_file-2.1.0/MANIFEST.in
+-rw-r--r--   0 dshea     (1000) dshea     (1000)     1696 2024-05-21 16:20:14.997106 requests_file-2.1.0/PKG-INFO
+-rw-r--r--   0 dshea     (1000) dshea     (1000)     1134 2022-10-20 14:11:26.000000 requests_file-2.1.0/README.rst
+-rw-r--r--   0 dshea     (1000) dshea     (1000)      820 2024-05-21 16:18:08.000000 requests_file-2.1.0/pyproject.toml
+drwxr-xr-x   0 dshea     (1000) dshea     (1000)        0 2024-05-21 16:20:14.997106 requests_file-2.1.0/requests_file.egg-info/
+-rw-r--r--   0 dshea     (1000) dshea     (1000)     1696 2024-05-21 16:20:14.000000 requests_file-2.1.0/requests_file.egg-info/PKG-INFO
+-rw-r--r--   0 dshea     (1000) dshea     (1000)      324 2024-05-21 16:20:14.000000 requests_file-2.1.0/requests_file.egg-info/SOURCES.txt
+-rw-r--r--   0 dshea     (1000) dshea     (1000)        1 2024-05-21 16:20:14.000000 requests_file-2.1.0/requests_file.egg-info/dependency_links.txt
+-rw-r--r--   0 dshea     (1000) dshea     (1000)       16 2024-05-21 16:20:14.000000 requests_file-2.1.0/requests_file.egg-info/requires.txt
+-rw-r--r--   0 dshea     (1000) dshea     (1000)       14 2024-05-21 16:20:14.000000 requests_file-2.1.0/requests_file.egg-info/top_level.txt
+-rw-r--r--   0 dshea     (1000) dshea     (1000)     4825 2024-05-21 16:18:08.000000 requests_file-2.1.0/requests_file.py
+-rw-r--r--   0 dshea     (1000) dshea     (1000)       38 2024-05-21 16:20:14.997106 requests_file-2.1.0/setup.cfg
+drwxr-xr-x   0 dshea     (1000) dshea     (1000)        0 2024-05-21 16:20:14.996106 requests_file-2.1.0/tests/
+-rw-r--r--   0 dshea     (1000) dshea     (1000)     7347 2022-10-20 14:11:26.000000 requests_file-2.1.0/tests/test_requests_file.py
```

### Comparing `requests-file-2.0.0/.github/workflows/test.yml` & `requests_file-2.1.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `requests-file-2.0.0/CHANGES.rst` & `requests_file-2.1.0/CHANGES.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2.1.0 (21 May 2024)
+===================
+- Set the request property in the returned Response object
+
 2.0.0 (29 Jan 2024)
 ===================
 - Correct a typo in requests_file.py (github PR #21)
 - Remove dependency on six (github PR #23)
 - Move metadata to pyproject.toml (github PR #26)
   - Remove support for Python 2
   - Remove support for raw distutils
```

### Comparing `requests-file-2.0.0/LICENSE` & `requests_file-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `requests-file-2.0.0/PKG-INFO` & `requests_file-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-file
-Version: 2.0.0
+Version: 2.1.0
 Summary: File transport adapter for Requests
 Author-email: David Shea <reallylongword@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/dashea/requests-file
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
```

### Comparing `requests-file-2.0.0/README.rst` & `requests_file-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `requests-file-2.0.0/pyproject.toml` & `requests_file-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `requests-file-2.0.0/requests_file.egg-info/PKG-INFO` & `requests_file-2.1.0/requests_file.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests-file
-Version: 2.0.0
+Version: 2.1.0
 Summary: File transport adapter for Requests
 Author-email: David Shea <reallylongword@gmail.com>
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/dashea/requests-file
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Plugins
 Classifier: Intended Audience :: Developers
```

### Comparing `requests-file-2.0.0/requests_file.py` & `requests_file-2.1.0/requests_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
         url_parts = urlparse(request.url)
 
         # Reject URLs with a hostname component
         if url_parts.netloc and url_parts.netloc != "localhost":
             raise ValueError("file: URLs with hostname components are not permitted")
 
         resp = Response()
+        resp.request = request
 
         # Open the file, translate certain errors into HTTP responses
         # Use urllib's unquote to translate percent escapes into whatever
         # they actually need to be
         try:
             # Split the path on / (the URL directory separator) and decode any
             # % escapes in the parts
```

### Comparing `requests-file-2.0.0/tests/test_requests_file.py` & `requests_file-2.1.0/tests/test_requests_file.py`

 * *Files identical despite different names*

