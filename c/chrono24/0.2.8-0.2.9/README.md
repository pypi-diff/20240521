# Comparing `tmp/chrono24-0.2.8.tar.gz` & `tmp/chrono24-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chrono24-0.2.8.tar", last modified: Wed May  1 22:37:40 2024, max compression
+gzip compressed data, was "chrono24-0.2.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `chrono24-0.2.8.tar` & `chrono24-0.2.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       83 2023-12-31 20:29:04.122838 chrono24-0.2.8/.flake8
--rw-r--r--   0        0        0      170 2022-12-31 19:48:44.859641 chrono24-0.2.8/.github/dependabot.yaml
--rw-r--r--   0        0        0     1087 2024-05-01 22:16:45.525774 chrono24-0.2.8/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     1799 2023-01-02 19:05:24.745258 chrono24-0.2.8/.gitignore
--rw-r--r--   0        0        0     1068 2023-01-02 19:05:24.745422 chrono24-0.2.8/LICENSE
--rw-r--r--   0        0        0      847 2023-12-31 22:56:54.196916 chrono24-0.2.8/Makefile
--rw-r--r--   0        0        0     5717 2024-05-01 22:16:45.526242 chrono24-0.2.8/README.md
--rw-r--r--   0        0        0      156 2024-05-01 22:37:10.249426 chrono24-0.2.8/chrono24/__init__.py
--rw-r--r--   0        0        0    18621 2024-05-01 22:35:42.518925 chrono24-0.2.8/chrono24/api.py
--rw-r--r--   0        0        0      239 2023-12-31 22:45:10.167411 chrono24-0.2.8/chrono24/exceptions.py
--rw-r--r--   0        0        0     4509 2024-01-01 01:40:19.692191 chrono24-0.2.8/chrono24/session.py
--rw-r--r--   0        0        0        0 2023-12-31 22:43:03.061191 chrono24-0.2.8/conftest.py
--rw-r--r--   0        0        0      887 2023-12-31 18:18:22.048837 chrono24-0.2.8/pyproject.toml
--rw-r--r--   0        0        0       32 2023-12-31 22:50:57.346272 chrono24-0.2.8/requirements-dev.txt
--rw-r--r--   0        0        0       33 2023-12-31 18:16:11.713712 chrono24-0.2.8/requirements.txt
--rw-r--r--   0        0        0     1255 2023-12-31 18:19:07.082258 chrono24-0.2.8/setup.cfg
--rw-r--r--   0        0        0     2974 2024-01-02 03:17:17.072335 chrono24-0.2.8/tests/test_api.py
--rw-r--r--   0        0        0      647 2024-01-01 18:55:58.188389 chrono24-0.2.8/tests/test_exceptions.py
--rw-r--r--   0        0        0     6585 1970-01-01 00:00:00.000000 chrono24-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0       83 2023-12-31 20:29:04.122838 chrono24-0.2.9/.flake8
+-rw-r--r--   0        0        0      170 2022-12-31 19:48:44.859641 chrono24-0.2.9/.github/dependabot.yaml
+-rw-r--r--   0        0        0     1087 2024-05-01 22:16:45.525774 chrono24-0.2.9/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     1799 2023-01-02 19:05:24.745258 chrono24-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1068 2023-01-02 19:05:24.745422 chrono24-0.2.9/LICENSE
+-rw-r--r--   0        0        0      847 2023-12-31 22:56:54.196916 chrono24-0.2.9/Makefile
+-rw-r--r--   0        0        0     5717 2024-05-01 22:16:45.526242 chrono24-0.2.9/README.md
+-rw-r--r--   0        0        0      156 2024-05-07 13:46:43.100566 chrono24-0.2.9/chrono24/__init__.py
+-rw-r--r--   0        0        0    18611 2024-05-07 13:41:53.077154 chrono24-0.2.9/chrono24/api.py
+-rw-r--r--   0        0        0      239 2023-12-31 22:45:10.167411 chrono24-0.2.9/chrono24/exceptions.py
+-rw-r--r--   0        0        0     4509 2024-05-07 13:37:01.859501 chrono24-0.2.9/chrono24/session.py
+-rw-r--r--   0        0        0        0 2023-12-31 22:43:03.061191 chrono24-0.2.9/conftest.py
+-rw-r--r--   0        0        0      887 2023-12-31 18:18:22.048837 chrono24-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-12-31 22:50:57.346272 chrono24-0.2.9/requirements-dev.txt
+-rw-r--r--   0        0        0       33 2023-12-31 18:16:11.713712 chrono24-0.2.9/requirements.txt
+-rw-r--r--   0        0        0     1255 2023-12-31 18:19:07.082258 chrono24-0.2.9/setup.cfg
+-rw-r--r--   0        0        0     2974 2024-01-02 03:17:17.072335 chrono24-0.2.9/tests/test_api.py
+-rw-r--r--   0        0        0      647 2024-01-01 18:55:58.188389 chrono24-0.2.9/tests/test_exceptions.py
+-rw-r--r--   0        0        0     6585 1970-01-01 00:00:00.000000 chrono24-0.2.9/PKG-INFO
```

### Comparing `chrono24-0.2.8/.github/workflows/ci.yaml` & `chrono24-0.2.9/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.8/.gitignore` & `chrono24-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.8/LICENSE` & `chrono24-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.8/Makefile` & `chrono24-0.2.9/Makefile`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.8/README.md` & `chrono24-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.8/chrono24/api.py` & `chrono24-0.2.9/chrono24/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
             Listings: A Listings object containing the fetched listings.
         """
         # Chrono24 will modify the initial query URL - add URL attributes to the modified URL
         listings_url = self.url + self._join_attrs(**kwargs)
         page_number = kwargs.get("showPage", 1)
         # Further modify URL if seeking a listings page greater than 1
         if page_number != 1:
-            listings_url = listings_url.replace("index.htm", f"index-{page_number}.htm")
+            listings_url = listings_url.replace(".htm", f"-{page_number}.htm")
 
         return Listings(get_html(listings_url))
 
     @property
     def _total_page_count(self):
         """Calculate the total number of pages based on the total listing count.
```

### Comparing `chrono24-0.2.8/chrono24/session.py` & `chrono24-0.2.9/chrono24/session.py`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.8/pyproject.toml` & `chrono24-0.2.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.8/setup.cfg` & `chrono24-0.2.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.8/tests/test_api.py` & `chrono24-0.2.9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.8/tests/test_exceptions.py` & `chrono24-0.2.9/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `chrono24-0.2.8/PKG-INFO` & `chrono24-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chrono24
-Version: 0.2.8
+Version: 0.2.9
 Summary: chrono24
 Home-page: https://github.com/irahorecka/chrono24
 Author: Ira Horecka
 Author-email: ira89@icloud.com
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Developers
```

