# Comparing `tmp/osm_easy_api-3.0.0.tar.gz` & `tmp/osm_easy_api-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm_easy_api-3.0.0.tar", last modified: Tue Mar 19 12:57:47 2024, max compression
+gzip compressed data, was "osm_easy_api-3.0.1.tar", last modified: Tue May 21 12:00:59 2024, max compression
```

## Comparing `osm_easy_api-3.0.0.tar` & `osm_easy_api-3.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-03-19 12:57:47.179006 osm_easy_api-3.0.0/
--rw-rw-rw-   0        0        0     7369 2024-03-19 12:52:01.000000 osm_easy_api-3.0.0/CHANGELOG.md
--rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-3.0.0/LICENSE.md
--rw-rw-rw-   0        0        0    49555 2024-03-19 12:57:47.178000 osm_easy_api-3.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     5209 2024-03-19 12:50:31.000000 osm_easy_api-3.0.0/README.md
--rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-3.0.0/pyproject.toml
--rw-rw-rw-   0        0        0     1197 2024-03-19 12:57:47.186113 osm_easy_api-3.0.0/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-3.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:57:47.109506 osm_easy_api-3.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-03-19 12:57:47.117135 osm_easy_api-3.0.0/src/osm_easy_api/
--rw-rw-rw-   0        0        0      176 2024-03-19 12:52:24.000000 osm_easy_api-3.0.0/src/osm_easy_api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:57:47.152780 osm_easy_api-3.0.0/src/osm_easy_api/api/
--rw-rw-rw-   0        0        0     3469 2024-03-18 17:24:42.000000 osm_easy_api-3.0.0/src/osm_easy_api/api/_URLs.py
--rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-3.0.0/src/osm_easy_api/api/__init__.py
--rw-rw-rw-   0        0        0     2978 2024-03-18 18:44:46.000000 osm_easy_api-3.0.0/src/osm_easy_api/api/api.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:57:47.159952 osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/
--rw-rw-rw-   0        0        0      549 2024-03-16 21:33:55.000000 osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/__init__.py
--rw-rw-rw-   0        0        0    12577 2024-03-19 12:41:19.000000 osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/changeset.py
--rw-rw-rw-   0        0        0     2652 2024-03-16 22:33:05.000000 osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/changeset_discussion.py
--rw-rw-rw-   0        0        0    13869 2024-03-19 10:37:25.000000 osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/elements.py
--rw-rw-rw-   0        0        0     6080 2024-03-19 10:33:51.000000 osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/gpx.py
--rw-rw-rw-   0        0        0     5288 2024-03-17 21:58:52.000000 osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/misc.py
--rw-rw-rw-   0        0        0    10304 2024-03-19 10:34:04.000000 osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/notes.py
--rw-rw-rw-   0        0        0     6414 2024-03-16 22:33:15.000000 osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/user.py
--rw-rw-rw-   0        0        0     1896 2024-03-16 21:44:37.000000 osm_easy_api-3.0.0/src/osm_easy_api/api/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:57:47.170214 osm_easy_api-3.0.0/src/osm_easy_api/data_classes/
--rw-rw-rw-   0        0        0     1843 2024-03-17 22:21:21.000000 osm_easy_api-3.0.0/src/osm_easy_api/data_classes/GpxFile.py
--rw-rw-rw-   0        0        0     8032 2024-03-11 21:43:27.000000 osm_easy_api-3.0.0/src/osm_easy_api/data_classes/OsmChange.py
--rw-rw-rw-   0        0        0      480 2024-03-17 21:52:59.000000 osm_easy_api-3.0.0/src/osm_easy_api/data_classes/__init__.py
--rw-rw-rw-   0        0        0     1785 2024-03-17 15:13:08.000000 osm_easy_api-3.0.0/src/osm_easy_api/data_classes/changeset.py
--rw-rw-rw-   0        0        0     1510 2024-03-18 18:31:21.000000 osm_easy_api-3.0.0/src/osm_easy_api/data_classes/node.py
--rw-rw-rw-   0        0        0     4022 2023-03-22 21:29:55.000000 osm_easy_api-3.0.0/src/osm_easy_api/data_classes/note.py
--rw-rw-rw-   0        0        0     3440 2024-03-18 18:57:57.000000 osm_easy_api-3.0.0/src/osm_easy_api/data_classes/osm_object_primitive.py
--rw-rw-rw-   0        0        0     3607 2024-03-18 18:58:08.000000 osm_easy_api-3.0.0/src/osm_easy_api/data_classes/relation.py
--rw-rw-rw-   0        0        0     1403 2023-03-22 23:13:07.000000 osm_easy_api-3.0.0/src/osm_easy_api/data_classes/tags.py
--rw-rw-rw-   0        0        0     2099 2023-03-22 20:09:45.000000 osm_easy_api-3.0.0/src/osm_easy_api/data_classes/user.py
--rw-rw-rw-   0        0        0     2080 2024-03-18 18:58:36.000000 osm_easy_api-3.0.0/src/osm_easy_api/data_classes/way.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:57:47.172460 osm_easy_api-3.0.0/src/osm_easy_api/diff/
--rw-rw-rw-   0        0        0      111 2024-03-17 14:41:52.000000 osm_easy_api-3.0.0/src/osm_easy_api/diff/__init__.py
--rw-rw-rw-   0        0        0     6373 2024-03-19 10:57:07.000000 osm_easy_api-3.0.0/src/osm_easy_api/diff/diff.py
--rw-rw-rw-   0        0        0     4012 2024-03-19 10:36:55.000000 osm_easy_api-3.0.0/src/osm_easy_api/diff/diff_parser.py
--rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-3.0.0/src/osm_easy_api/py.typed
-drwxrwxrwx   0        0        0        0 2024-03-19 12:57:47.176058 osm_easy_api-3.0.0/src/osm_easy_api/utils/
--rw-rw-rw-   0        0        0      140 2024-03-18 18:54:53.000000 osm_easy_api-3.0.0/src/osm_easy_api/utils/__init__.py
--rw-rw-rw-   0        0        0      596 2024-03-19 10:39:15.000000 osm_easy_api-3.0.0/src/osm_easy_api/utils/element_to_osm_object.py
--rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-3.0.0/src/osm_easy_api/utils/join_url.py
--rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-3.0.0/src/osm_easy_api/utils/write_gzip_to_file.py
-drwxrwxrwx   0        0        0        0 2024-03-19 12:57:47.176991 osm_easy_api-3.0.0/src/osm_easy_api.egg-info/
--rw-rw-rw-   0        0        0    49555 2024-03-19 12:57:47.000000 osm_easy_api-3.0.0/src/osm_easy_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1545 2024-03-19 12:57:47.000000 osm_easy_api-3.0.0/src/osm_easy_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-19 12:57:47.000000 osm_easy_api-3.0.0/src/osm_easy_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-24 09:45:20.000000 osm_easy_api-3.0.0/src/osm_easy_api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       90 2024-03-19 12:57:47.000000 osm_easy_api-3.0.0/src/osm_easy_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-03-19 12:57:47.000000 osm_easy_api-3.0.0/src/osm_easy_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 12:00:59.726378 osm_easy_api-3.0.1/
+-rw-rw-rw-   0        0        0     7470 2024-05-21 11:59:52.000000 osm_easy_api-3.0.1/CHANGELOG.md
+-rw-rw-rw-   0        0        0    35821 2023-03-07 21:14:41.000000 osm_easy_api-3.0.1/LICENSE.md
+-rw-rw-rw-   0        0        0    49673 2024-05-21 12:00:59.726378 osm_easy_api-3.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5173 2024-03-19 13:22:11.000000 osm_easy_api-3.0.1/README.md
+-rw-rw-rw-   0        0        0       97 2023-03-07 21:14:41.000000 osm_easy_api-3.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0     1239 2024-05-21 12:00:59.730390 osm_easy_api-3.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-03-07 21:14:41.000000 osm_easy_api-3.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:00:59.607216 osm_easy_api-3.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 12:00:59.623849 osm_easy_api-3.0.1/src/osm_easy_api/
+-rw-rw-rw-   0        0        0      176 2024-05-21 11:52:28.000000 osm_easy_api-3.0.1/src/osm_easy_api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:00:59.665064 osm_easy_api-3.0.1/src/osm_easy_api/api/
+-rw-rw-rw-   0        0        0     3469 2024-03-18 17:24:42.000000 osm_easy_api-3.0.1/src/osm_easy_api/api/_URLs.py
+-rw-rw-rw-   0        0        0      101 2023-03-07 21:14:41.000000 osm_easy_api-3.0.1/src/osm_easy_api/api/__init__.py
+-rw-rw-rw-   0        0        0     2978 2024-03-18 18:44:46.000000 osm_easy_api-3.0.1/src/osm_easy_api/api/api.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:00:59.682984 osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/
+-rw-rw-rw-   0        0        0      549 2024-03-16 21:33:55.000000 osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/__init__.py
+-rw-rw-rw-   0        0        0    12577 2024-03-19 12:41:19.000000 osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/changeset.py
+-rw-rw-rw-   0        0        0     2652 2024-03-16 22:33:05.000000 osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/changeset_discussion.py
+-rw-rw-rw-   0        0        0    13869 2024-03-19 10:37:25.000000 osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/elements.py
+-rw-rw-rw-   0        0        0     6080 2024-03-19 10:33:51.000000 osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/gpx.py
+-rw-rw-rw-   0        0        0     5288 2024-03-17 21:58:52.000000 osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/misc.py
+-rw-rw-rw-   0        0        0    10304 2024-03-19 10:34:04.000000 osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/notes.py
+-rw-rw-rw-   0        0        0     6414 2024-03-16 22:33:15.000000 osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/user.py
+-rw-rw-rw-   0        0        0     1896 2024-03-16 21:44:37.000000 osm_easy_api-3.0.1/src/osm_easy_api/api/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:00:59.707298 osm_easy_api-3.0.1/src/osm_easy_api/data_classes/
+-rw-rw-rw-   0        0        0     1843 2024-03-17 22:21:21.000000 osm_easy_api-3.0.1/src/osm_easy_api/data_classes/GpxFile.py
+-rw-rw-rw-   0        0        0     8032 2024-03-11 21:43:27.000000 osm_easy_api-3.0.1/src/osm_easy_api/data_classes/OsmChange.py
+-rw-rw-rw-   0        0        0      480 2024-03-17 21:52:59.000000 osm_easy_api-3.0.1/src/osm_easy_api/data_classes/__init__.py
+-rw-rw-rw-   0        0        0     1785 2024-03-17 15:13:08.000000 osm_easy_api-3.0.1/src/osm_easy_api/data_classes/changeset.py
+-rw-rw-rw-   0        0        0     1510 2024-03-18 18:31:21.000000 osm_easy_api-3.0.1/src/osm_easy_api/data_classes/node.py
+-rw-rw-rw-   0        0        0     4022 2023-03-22 21:29:55.000000 osm_easy_api-3.0.1/src/osm_easy_api/data_classes/note.py
+-rw-rw-rw-   0        0        0     3440 2024-03-18 18:57:57.000000 osm_easy_api-3.0.1/src/osm_easy_api/data_classes/osm_object_primitive.py
+-rw-rw-rw-   0        0        0     3607 2024-03-18 18:58:08.000000 osm_easy_api-3.0.1/src/osm_easy_api/data_classes/relation.py
+-rw-rw-rw-   0        0        0     1403 2023-03-22 23:13:07.000000 osm_easy_api-3.0.1/src/osm_easy_api/data_classes/tags.py
+-rw-rw-rw-   0        0        0     2099 2023-03-22 20:09:45.000000 osm_easy_api-3.0.1/src/osm_easy_api/data_classes/user.py
+-rw-rw-rw-   0        0        0     2080 2024-03-18 18:58:36.000000 osm_easy_api-3.0.1/src/osm_easy_api/data_classes/way.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:00:59.713599 osm_easy_api-3.0.1/src/osm_easy_api/diff/
+-rw-rw-rw-   0        0        0      111 2024-03-17 14:41:52.000000 osm_easy_api-3.0.1/src/osm_easy_api/diff/__init__.py
+-rw-rw-rw-   0        0        0     6373 2024-03-19 10:57:07.000000 osm_easy_api-3.0.1/src/osm_easy_api/diff/diff.py
+-rw-rw-rw-   0        0        0     4012 2024-03-19 10:36:55.000000 osm_easy_api-3.0.1/src/osm_easy_api/diff/diff_parser.py
+-rw-rw-rw-   0        0        0        0 2023-03-07 21:14:41.000000 osm_easy_api-3.0.1/src/osm_easy_api/py.typed
+drwxrwxrwx   0        0        0        0 2024-05-21 12:00:59.721866 osm_easy_api-3.0.1/src/osm_easy_api/utils/
+-rw-rw-rw-   0        0        0      140 2024-03-18 18:54:53.000000 osm_easy_api-3.0.1/src/osm_easy_api/utils/__init__.py
+-rw-rw-rw-   0        0        0      596 2024-03-19 10:39:15.000000 osm_easy_api-3.0.1/src/osm_easy_api/utils/element_to_osm_object.py
+-rw-rw-rw-   0        0        0      166 2023-03-07 21:14:41.000000 osm_easy_api-3.0.1/src/osm_easy_api/utils/join_url.py
+-rw-rw-rw-   0        0        0      397 2023-03-07 21:14:41.000000 osm_easy_api-3.0.1/src/osm_easy_api/utils/write_gzip_to_file.py
+drwxrwxrwx   0        0        0        0 2024-05-21 12:00:59.723867 osm_easy_api-3.0.1/src/osm_easy_api.egg-info/
+-rw-rw-rw-   0        0        0    49673 2024-05-21 12:00:59.000000 osm_easy_api-3.0.1/src/osm_easy_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1545 2024-05-21 12:00:59.000000 osm_easy_api-3.0.1/src/osm_easy_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 12:00:59.000000 osm_easy_api-3.0.1/src/osm_easy_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-24 09:45:20.000000 osm_easy_api-3.0.1/src/osm_easy_api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       91 2024-05-21 12:00:59.000000 osm_easy_api-3.0.1/src/osm_easy_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-21 12:00:59.000000 osm_easy_api-3.0.1/src/osm_easy_api.egg-info/top_level.txt
```

### Comparing `osm_easy_api-3.0.0/CHANGELOG.md` & `osm_easy_api-3.0.1/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [3.0.1] - 2024-05-21
+### Added
+- Support for python 3.12
+
+### Fixed
+- Dependencies update
+
 ## [3.0.0] - 2024-03-19
 ### Added
 - Support for `oAuth2`: `access_token` parameter in `Api` class constructor.
 - `Unauthorized` exception. (No access token.)
 - `Forbidden` exception. (The access token does not support the needed scope or you must be a moderator.)
 - `gpx.create()` endpoint.
 - `GpxFile` data class.
```

### Comparing `osm_easy_api-3.0.0/LICENSE.md` & `osm_easy_api-3.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/PKG-INFO` & `osm_easy_api-3.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm_easy_api
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python package for parsing osm diffs and communicating with the osm api.
 Home-page: https://github.com/docentYT/osm_easy_api
 License: GPLv3
 Keywords: openstreetmap,osm,api,wrapper,diff
 Platform: unix
 Platform: linux
 Platform: osx
@@ -14,28 +14,29 @@
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests>=2
 Provides-Extra: testing
-Requires-Dist: tox>=4.4.0; extra == "testing"
-Requires-Dist: responses>=0.22.0; extra == "testing"
-Requires-Dist: coverage>=7.2.0; extra == "testing"
+Requires-Dist: tox>=4.15.0; extra == "testing"
+Requires-Dist: responses>=0.25.0; extra == "testing"
+Requires-Dist: coverage>=7.5.0; extra == "testing"
 Requires-Dist: coverage-badge>=1.1.0; extra == "testing"
 
 <h1 align="center">osm_easy_api</h1>
 <p align="center">
   <img src="https://github.com/docentYT/automated-python-tests-testing-repo/actions/workflows/tests.yaml/badge.svg" />
-  <img src="https://raw.githubusercontent.com/docentYT/osm_easy_api/3889ae626be35183253485646b7be9e235a2fc27/coverage-badge.svg" />
+  <img src="https://raw.githubusercontent.com/docentYT/osm_easy_api/main/coverage-badge.svg" />
   <a href="https://pypi.org/project/osm-easy-api/">
     <img src="https://img.shields.io/pypi/v/osm_easy_api" />
   </a>
   <a href="https://pypi.org/project/osm-easy-api/">
     <img src="https://img.shields.io/pypi/dm/osm_easy_api" alt="pypi downloads">
   </a>
   <a href="https://pypi.org/project/osm-easy-api/">
@@ -182,14 +183,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [3.0.1] - 2024-05-21
+### Added
+- Support for python 3.12
+
+### Fixed
+- Dependencies update
+
 ## [3.0.0] - 2024-03-19
 ### Added
 - Support for `oAuth2`: `access_token` parameter in `Api` class constructor.
 - `Unauthorized` exception. (No access token.)
 - `Forbidden` exception. (The access token does not support the needed scope or you must be a moderator.)
 - `gpx.create()` endpoint.
 - `GpxFile` data class.
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: osm_easy_api Version: 3.0.0 Summary: Python package
+Metadata-Version: 2.1 Name: osm_easy_api Version: 3.0.1 Summary: Python package
 for parsing osm diffs and communicating with the osm api. Home-page: https://
 github.com/docentYT/osm_easy_api License: GPLv3 Keywords:
 openstreetmap,osm,api,wrapper,diff Platform: unix Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Topic :: Scientific/Engineering :: GIS Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Python: >=3.10 Description-Content-Type: text/markdown
-License-File: LICENSE.md Requires-Dist: requests>=2 Provides-Extra: testing
-Requires-Dist: tox>=4.4.0; extra == "testing" Requires-Dist: responses>=0.22.0;
-extra == "testing" Requires-Dist: coverage>=7.2.0; extra == "testing" Requires-
-Dist: coverage-badge>=1.1.0; extra == "testing"
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
+Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE.md
+Requires-Dist: requests>=2 Provides-Extra: testing Requires-Dist: tox>=4.15.0;
+extra == "testing" Requires-Dist: responses>=0.25.0; extra == "testing"
+Requires-Dist: coverage>=7.5.0; extra == "testing" Requires-Dist: coverage-
+badge>=1.1.0; extra == "testing"
                           ************ oossmm__eeaassyy__aappii ************
    [https://github.com/docentYT/automated-python-tests-testing-repo/actions/
   workflows/tests.yaml/badge.svg][https://raw.githubusercontent.com/docentYT/
-   osm_easy_api/3889ae626be35183253485646b7be9e235a2fc27/coverage-badge.svg]
- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_o_s_m___e_a_s_y___a_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_s_]_[_p_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
+     osm_easy_api/main/coverage-badge.svg]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
+                _o_s_m___e_a_s_y___a_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_s_]_[_p_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
                               _M_e_ _o_n_ _O_p_e_n_S_t_r_e_e_t_M_a_p
 > Python package for parsing osm diffs and communicating with the OpenStreetMap
 api. ### What's the point of this package? This package was created to provide
 an easy way to create automated scripts and programs that use diff and/or osm
 api. The main advantage is the classes (data_classes) that provide data of
 elements (node, way, relation, OsmChange, etc.) in a readable way and the
 possibility to use them in diff and api without worrying about missing data or
@@ -72,39 +73,41 @@
 Action.DELETE) for node in deleted_nodes: print(node.id) ``` but it can consume
 large amounts of ram and use of this method is not recommended for large
 diff's. ## Tests You will need to install `test-requirements.txt`. You can use
 tox. To run tests manually use `python -m unittest discover`. # Changelog All
 notable changes to this project will be documented in this file. The format is
 based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this
 project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
-## [3.0.0] - 2024-03-19 ### Added - Support for `oAuth2`: `access_token`
-parameter in `Api` class constructor. - `Unauthorized` exception. (No access
-token.) - `Forbidden` exception. (The access token does not support the needed
-scope or you must be a moderator.) - `gpx.create()` endpoint. - `GpxFile` data
-class. - `Visibility` enum. - `gpx.update()` endpoint. - `gpx.delete()`
-endpoint. - `gpx.get_details()` endpoint. - `gpx.get_file()` endpoint. -
-`gpx.list_details()` endpoint. - `order` parameter in `changeset.get_query()`.
-### Fixed - Types in `elements` endpoint. - Missing documentation. -
-`misc.get_map_in_bbox()` endpoint should not yield `string`. ### Changed - The
-way http errors are handled. - In `elements.get()` endpoint the `element`
-parameter has been renamed to `element_type`. - In `elements.history()`
-endpoint the `element` parameter has been renamed to `element_type`. - In
-`elements.version()` endpoint the `element` parameter has been renamed to
-`element_type`. - In `elements.getQuery()` endpoint the `element` parameter has
-been renamed to `element_type`. - In `elements.relations()` endpoint the
-`element` parameter has been renamed to `element_type`. - In `elements.full()`
-endpoint the `element` parameter has been renamed to `element_type`. - Type of
-`user_id` parameter in `changeset.get_query()` was changed from `str` to `int`.
-- `OsmChange_parser_generator()` and `OsmChange_parser()` from `diff` module
-are now 'private' functions. Use `Diff.get()` instead. - `notes.search()`
-endpoint throws `LimitsExceeded` exception instead of `ValueError`. -
-`page_number` paremeter in `gpx.get()` has now default value 0. - Now classes
-are imported from individual modules - not from the main library. See examples
-in the `README.md`. - `gpx.get()` renamed to `gpx.get_gps_points()` ### Removed
-- Support for `HTTP Basic authentication`: `username` and `password` parameters
+## [3.0.1] - 2024-05-21 ### Added - Support for python 3.12 ### Fixed -
+Dependencies update ## [3.0.0] - 2024-03-19 ### Added - Support for `oAuth2`:
+`access_token` parameter in `Api` class constructor. - `Unauthorized`
+exception. (No access token.) - `Forbidden` exception. (The access token does
+not support the needed scope or you must be a moderator.) - `gpx.create()`
+endpoint. - `GpxFile` data class. - `Visibility` enum. - `gpx.update()`
+endpoint. - `gpx.delete()` endpoint. - `gpx.get_details()` endpoint. -
+`gpx.get_file()` endpoint. - `gpx.list_details()` endpoint. - `order` parameter
+in `changeset.get_query()`. ### Fixed - Types in `elements` endpoint. - Missing
+documentation. - `misc.get_map_in_bbox()` endpoint should not yield `string`.
+### Changed - The way http errors are handled. - In `elements.get()` endpoint
+the `element` parameter has been renamed to `element_type`. - In
+`elements.history()` endpoint the `element` parameter has been renamed to
+`element_type`. - In `elements.version()` endpoint the `element` parameter has
+been renamed to `element_type`. - In `elements.getQuery()` endpoint the
+`element` parameter has been renamed to `element_type`. - In
+`elements.relations()` endpoint the `element` parameter has been renamed to
+`element_type`. - In `elements.full()` endpoint the `element` parameter has
+been renamed to `element_type`. - Type of `user_id` parameter in
+`changeset.get_query()` was changed from `str` to `int`. -
+`OsmChange_parser_generator()` and `OsmChange_parser()` from `diff` module are
+now 'private' functions. Use `Diff.get()` instead. - `notes.search()` endpoint
+throws `LimitsExceeded` exception instead of `ValueError`. - `page_number`
+paremeter in `gpx.get()` has now default value 0. - Now classes are imported
+from individual modules - not from the main library. See examples in the
+`README.md`. - `gpx.get()` renamed to `gpx.get_gps_points()` ### Removed -
+Support for `HTTP Basic authentication`: `username` and `password` parameters
 in `Api` class constructor. - Most `# type: ignore`. - `NotAModerator`
 exception. It is now replaced by `Forbidden` exception. ## [2.2.0] - 2024-02-23
 ### Added - Exception for `410` status code in notes endpoint. ## [2.1.1] -
 2024-01-04 ### Fixed - Percent-encoding was not applied on texts entered by the
 user. [#22](https://github.com/docentYT/osm_easy_api/issues/22) ## [2.1.0] -
 2023-09-06 ### Added - `TooManyRequests` exception. - Support for `429` status
 code in `api.changeset.discussion.comment()`. ## [2.0.0] - 2023-08-29 ### Added
```

### Comparing `osm_easy_api-3.0.0/README.md` & `osm_easy_api-3.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 <h1 align="center">osm_easy_api</h1>
 <p align="center">
   <img src="https://github.com/docentYT/automated-python-tests-testing-repo/actions/workflows/tests.yaml/badge.svg" />
-  <img src="https://raw.githubusercontent.com/docentYT/osm_easy_api/3889ae626be35183253485646b7be9e235a2fc27/coverage-badge.svg" />
+  <img src="https://raw.githubusercontent.com/docentYT/osm_easy_api/main/coverage-badge.svg" />
   <a href="https://pypi.org/project/osm-easy-api/">
     <img src="https://img.shields.io/pypi/v/osm_easy_api" />
   </a>
   <a href="https://pypi.org/project/osm-easy-api/">
     <img src="https://img.shields.io/pypi/dm/osm_easy_api" alt="pypi downloads">
   </a>
   <a href="https://pypi.org/project/osm-easy-api/">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
                           ************ oossmm__eeaassyy__aappii ************
    [https://github.com/docentYT/automated-python-tests-testing-repo/actions/
   workflows/tests.yaml/badge.svg][https://raw.githubusercontent.com/docentYT/
-   osm_easy_api/3889ae626be35183253485646b7be9e235a2fc27/coverage-badge.svg]
- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_o_s_m___e_a_s_y___a_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_s_]_[_p_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
+     osm_easy_api/main/coverage-badge.svg]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
+                _o_s_m___e_a_s_y___a_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_s_]_[_p_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
                               _M_e_ _o_n_ _O_p_e_n_S_t_r_e_e_t_M_a_p
 > Python package for parsing osm diffs and communicating with the OpenStreetMap
 api. ### What's the point of this package? This package was created to provide
 an easy way to create automated scripts and programs that use diff and/or osm
 api. The main advantage is the classes (data_classes) that provide data of
 elements (node, way, relation, OsmChange, etc.) in a readable way and the
 possibility to use them in diff and api without worrying about missing data or
```

### Comparing `osm_easy_api-3.0.0/setup.cfg` & `osm_easy_api-3.0.1/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -44,32 +44,35 @@
 000002b0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
 000002c0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
 000002d0: 2033 203a 3a20 4f6e 6c79 0d0a 0950 726f   3 :: Only...Pro
 000002e0: 6772 616d 6d69 6e67 204c 616e 6775 6167  gramming Languag
 000002f0: 6520 3a3a 2050 7974 686f 6e20 3a3a 2033  e :: Python :: 3
 00000300: 2e31 300d 0a09 5072 6f67 7261 6d6d 696e  .10...Programmin
 00000310: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
-00000320: 7468 6f6e 203a 3a20 332e 3131 0d0a 0d0a  thon :: 3.11....
-00000330: 5b6f 7074 696f 6e73 5d0d 0a70 6163 6b61  [options]..packa
-00000340: 6765 7320 3d20 6669 6e64 3a0d 0a69 6e73  ges = find:..ins
-00000350: 7461 6c6c 5f72 6571 7569 7265 7320 3d20  tall_requires = 
-00000360: 7265 7175 6573 7473 3e3d 320d 0a70 7974  requests>=2..pyt
-00000370: 686f 6e5f 7265 7175 6972 6573 203d 203e  hon_requires = >
-00000380: 3d20 332e 3130 0d0a 7061 636b 6167 655f  = 3.10..package_
-00000390: 6469 7220 3d20 3d73 7263 0d0a 7a69 705f  dir = =src..zip_
-000003a0: 7361 6665 203d 206e 6f0d 0a0d 0a5b 6f70  safe = no....[op
-000003b0: 7469 6f6e 732e 7061 636b 6167 6573 2e66  tions.packages.f
-000003c0: 696e 645d 0d0a 7768 6572 6520 3d20 7372  ind]..where = sr
-000003d0: 630d 0a0d 0a5b 6f70 7469 6f6e 732e 6578  c....[options.ex
-000003e0: 7472 6173 5f72 6571 7569 7265 5d0d 0a74  tras_require]..t
-000003f0: 6573 7469 6e67 203d 200d 0a09 746f 7820  esting = ...tox 
-00000400: 3e3d 2034 2e34 2e30 0d0a 0972 6573 706f  >= 4.4.0...respo
-00000410: 6e73 6573 203e 3d20 302e 3232 2e30 0d0a  nses >= 0.22.0..
-00000420: 0963 6f76 6572 6167 6520 3e3d 2037 2e32  .coverage >= 7.2
-00000430: 2e30 0d0a 0963 6f76 6572 6167 652d 6261  .0...coverage-ba
-00000440: 6467 6520 3e3d 2031 2e31 2e30 0d0a 0d0a  dge >= 1.1.0....
-00000450: 5b6f 7074 696f 6e73 2e70 6163 6b61 6765  [options.package
-00000460: 5f64 6174 615d 0d0a 6f73 6d5f 6561 7379  _data]..osm_easy
-00000470: 5f61 7069 203d 2070 792e 7479 7065 640d  _api = py.typed.
-00000480: 0a0d 0a5b 6567 675f 696e 666f 5d0d 0a74  ...[egg_info]..t
-00000490: 6167 5f62 7569 6c64 203d 200d 0a74 6167  ag_build = ..tag
-000004a0: 5f64 6174 6520 3d20 300d 0a0d 0a         _date = 0....
+00000320: 7468 6f6e 203a 3a20 332e 3131 0d0a 0950  thon :: 3.11...P
+00000330: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+00000340: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+00000350: 2033 2e31 320d 0a0d 0a5b 6f70 7469 6f6e   3.12....[option
+00000360: 735d 0d0a 7061 636b 6167 6573 203d 2066  s]..packages = f
+00000370: 696e 643a 0d0a 696e 7374 616c 6c5f 7265  ind:..install_re
+00000380: 7175 6972 6573 203d 2072 6571 7565 7374  quires = request
+00000390: 733e 3d32 0d0a 7079 7468 6f6e 5f72 6571  s>=2..python_req
+000003a0: 7569 7265 7320 3d20 3e3d 2033 2e31 300d  uires = >= 3.10.
+000003b0: 0a70 6163 6b61 6765 5f64 6972 203d 203d  .package_dir = =
+000003c0: 7372 630d 0a7a 6970 5f73 6166 6520 3d20  src..zip_safe = 
+000003d0: 6e6f 0d0a 0d0a 5b6f 7074 696f 6e73 2e70  no....[options.p
+000003e0: 6163 6b61 6765 732e 6669 6e64 5d0d 0a77  ackages.find]..w
+000003f0: 6865 7265 203d 2073 7263 0d0a 0d0a 5b6f  here = src....[o
+00000400: 7074 696f 6e73 2e65 7874 7261 735f 7265  ptions.extras_re
+00000410: 7175 6972 655d 0d0a 7465 7374 696e 6720  quire]..testing 
+00000420: 3d20 0d0a 0974 6f78 203e 3d20 342e 3135  = ...tox >= 4.15
+00000430: 2e30 0d0a 0972 6573 706f 6e73 6573 203e  .0...responses >
+00000440: 3d20 302e 3235 2e30 0d0a 0963 6f76 6572  = 0.25.0...cover
+00000450: 6167 6520 3e3d 2037 2e35 2e30 0d0a 0963  age >= 7.5.0...c
+00000460: 6f76 6572 6167 652d 6261 6467 6520 3e3d  overage-badge >=
+00000470: 2031 2e31 2e30 0d0a 0d0a 5b6f 7074 696f   1.1.0....[optio
+00000480: 6e73 2e70 6163 6b61 6765 5f64 6174 615d  ns.package_data]
+00000490: 0d0a 6f73 6d5f 6561 7379 5f61 7069 203d  ..osm_easy_api =
+000004a0: 2070 792e 7479 7065 640d 0a0d 0a5b 6567   py.typed....[eg
+000004b0: 675f 696e 666f 5d0d 0a74 6167 5f62 7569  g_info]..tag_bui
+000004c0: 6c64 203d 200d 0a74 6167 5f64 6174 6520  ld = ..tag_date 
+000004d0: 3d20 300d 0a0d 0a                        = 0....
```

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/api/_URLs.py` & `osm_easy_api-3.0.1/src/osm_easy_api/api/_URLs.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/api/api.py` & `osm_easy_api-3.0.1/src/osm_easy_api/api/api.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/__init__.py` & `osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/__init__.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/changeset.py` & `osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/changeset.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/changeset_discussion.py` & `osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/changeset_discussion.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/elements.py` & `osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/elements.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/gpx.py` & `osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/gpx.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/misc.py` & `osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/misc.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/notes.py` & `osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/notes.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/api/endpoints/user.py` & `osm_easy_api-3.0.1/src/osm_easy_api/api/endpoints/user.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/api/exceptions.py` & `osm_easy_api-3.0.1/src/osm_easy_api/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/data_classes/GpxFile.py` & `osm_easy_api-3.0.1/src/osm_easy_api/data_classes/GpxFile.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/data_classes/OsmChange.py` & `osm_easy_api-3.0.1/src/osm_easy_api/data_classes/OsmChange.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/data_classes/changeset.py` & `osm_easy_api-3.0.1/src/osm_easy_api/data_classes/changeset.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/data_classes/node.py` & `osm_easy_api-3.0.1/src/osm_easy_api/data_classes/node.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/data_classes/note.py` & `osm_easy_api-3.0.1/src/osm_easy_api/data_classes/note.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/data_classes/osm_object_primitive.py` & `osm_easy_api-3.0.1/src/osm_easy_api/data_classes/osm_object_primitive.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/data_classes/relation.py` & `osm_easy_api-3.0.1/src/osm_easy_api/data_classes/relation.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/data_classes/tags.py` & `osm_easy_api-3.0.1/src/osm_easy_api/data_classes/tags.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/data_classes/user.py` & `osm_easy_api-3.0.1/src/osm_easy_api/data_classes/user.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/data_classes/way.py` & `osm_easy_api-3.0.1/src/osm_easy_api/data_classes/way.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/diff/diff.py` & `osm_easy_api-3.0.1/src/osm_easy_api/diff/diff.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/diff/diff_parser.py` & `osm_easy_api-3.0.1/src/osm_easy_api/diff/diff_parser.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api/utils/element_to_osm_object.py` & `osm_easy_api-3.0.1/src/osm_easy_api/utils/element_to_osm_object.py`

 * *Files identical despite different names*

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api.egg-info/PKG-INFO` & `osm_easy_api-3.0.1/src/osm_easy_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osm_easy_api
-Version: 3.0.0
+Version: 3.0.1
 Summary: Python package for parsing osm diffs and communicating with the osm api.
 Home-page: https://github.com/docentYT/osm_easy_api
 License: GPLv3
 Keywords: openstreetmap,osm,api,wrapper,diff
 Platform: unix
 Platform: linux
 Platform: osx
@@ -14,28 +14,29 @@
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: requests>=2
 Provides-Extra: testing
-Requires-Dist: tox>=4.4.0; extra == "testing"
-Requires-Dist: responses>=0.22.0; extra == "testing"
-Requires-Dist: coverage>=7.2.0; extra == "testing"
+Requires-Dist: tox>=4.15.0; extra == "testing"
+Requires-Dist: responses>=0.25.0; extra == "testing"
+Requires-Dist: coverage>=7.5.0; extra == "testing"
 Requires-Dist: coverage-badge>=1.1.0; extra == "testing"
 
 <h1 align="center">osm_easy_api</h1>
 <p align="center">
   <img src="https://github.com/docentYT/automated-python-tests-testing-repo/actions/workflows/tests.yaml/badge.svg" />
-  <img src="https://raw.githubusercontent.com/docentYT/osm_easy_api/3889ae626be35183253485646b7be9e235a2fc27/coverage-badge.svg" />
+  <img src="https://raw.githubusercontent.com/docentYT/osm_easy_api/main/coverage-badge.svg" />
   <a href="https://pypi.org/project/osm-easy-api/">
     <img src="https://img.shields.io/pypi/v/osm_easy_api" />
   </a>
   <a href="https://pypi.org/project/osm-easy-api/">
     <img src="https://img.shields.io/pypi/dm/osm_easy_api" alt="pypi downloads">
   </a>
   <a href="https://pypi.org/project/osm-easy-api/">
@@ -182,14 +183,21 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [3.0.1] - 2024-05-21
+### Added
+- Support for python 3.12
+
+### Fixed
+- Dependencies update
+
 ## [3.0.0] - 2024-03-19
 ### Added
 - Support for `oAuth2`: `access_token` parameter in `Api` class constructor.
 - `Unauthorized` exception. (No access token.)
 - `Forbidden` exception. (The access token does not support the needed scope or you must be a moderator.)
 - `gpx.create()` endpoint.
 - `GpxFile` data class.
```

#### html2text {}

```diff
@@ -1,27 +1,28 @@
-Metadata-Version: 2.1 Name: osm_easy_api Version: 3.0.0 Summary: Python package
+Metadata-Version: 2.1 Name: osm_easy_api Version: 3.0.1 Summary: Python package
 for parsing osm diffs and communicating with the osm api. Home-page: https://
 github.com/docentYT/osm_easy_api License: GPLv3 Keywords:
 openstreetmap,osm,api,wrapper,diff Platform: unix Platform: linux Platform: osx
 Platform: win32 Classifier: Development Status :: 4 - Beta Classifier: Intended
 Audience :: Developers Classifier: Natural Language :: English Classifier:
 Topic :: Scientific/Engineering :: GIS Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Requires-Python: >=3.10 Description-Content-Type: text/markdown
-License-File: LICENSE.md Requires-Dist: requests>=2 Provides-Extra: testing
-Requires-Dist: tox>=4.4.0; extra == "testing" Requires-Dist: responses>=0.22.0;
-extra == "testing" Requires-Dist: coverage>=7.2.0; extra == "testing" Requires-
-Dist: coverage-badge>=1.1.0; extra == "testing"
+Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
+Python: >=3.10 Description-Content-Type: text/markdown License-File: LICENSE.md
+Requires-Dist: requests>=2 Provides-Extra: testing Requires-Dist: tox>=4.15.0;
+extra == "testing" Requires-Dist: responses>=0.25.0; extra == "testing"
+Requires-Dist: coverage>=7.5.0; extra == "testing" Requires-Dist: coverage-
+badge>=1.1.0; extra == "testing"
                           ************ oossmm__eeaassyy__aappii ************
    [https://github.com/docentYT/automated-python-tests-testing-repo/actions/
   workflows/tests.yaml/badge.svg][https://raw.githubusercontent.com/docentYT/
-   osm_easy_api/3889ae626be35183253485646b7be9e235a2fc27/coverage-badge.svg]
- _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_o_s_m___e_a_s_y___a_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_s_]_[_p_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
+     osm_easy_api/main/coverage-badge.svg]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/
+                _o_s_m___e_a_s_y___a_p_i_]_[_p_y_p_i_ _d_o_w_n_l_o_a_d_s_]_[_p_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
                               _M_e_ _o_n_ _O_p_e_n_S_t_r_e_e_t_M_a_p
 > Python package for parsing osm diffs and communicating with the OpenStreetMap
 api. ### What's the point of this package? This package was created to provide
 an easy way to create automated scripts and programs that use diff and/or osm
 api. The main advantage is the classes (data_classes) that provide data of
 elements (node, way, relation, OsmChange, etc.) in a readable way and the
 possibility to use them in diff and api without worrying about missing data or
@@ -72,39 +73,41 @@
 Action.DELETE) for node in deleted_nodes: print(node.id) ``` but it can consume
 large amounts of ram and use of this method is not recommended for large
 diff's. ## Tests You will need to install `test-requirements.txt`. You can use
 tox. To run tests manually use `python -m unittest discover`. # Changelog All
 notable changes to this project will be documented in this file. The format is
 based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this
 project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
-## [3.0.0] - 2024-03-19 ### Added - Support for `oAuth2`: `access_token`
-parameter in `Api` class constructor. - `Unauthorized` exception. (No access
-token.) - `Forbidden` exception. (The access token does not support the needed
-scope or you must be a moderator.) - `gpx.create()` endpoint. - `GpxFile` data
-class. - `Visibility` enum. - `gpx.update()` endpoint. - `gpx.delete()`
-endpoint. - `gpx.get_details()` endpoint. - `gpx.get_file()` endpoint. -
-`gpx.list_details()` endpoint. - `order` parameter in `changeset.get_query()`.
-### Fixed - Types in `elements` endpoint. - Missing documentation. -
-`misc.get_map_in_bbox()` endpoint should not yield `string`. ### Changed - The
-way http errors are handled. - In `elements.get()` endpoint the `element`
-parameter has been renamed to `element_type`. - In `elements.history()`
-endpoint the `element` parameter has been renamed to `element_type`. - In
-`elements.version()` endpoint the `element` parameter has been renamed to
-`element_type`. - In `elements.getQuery()` endpoint the `element` parameter has
-been renamed to `element_type`. - In `elements.relations()` endpoint the
-`element` parameter has been renamed to `element_type`. - In `elements.full()`
-endpoint the `element` parameter has been renamed to `element_type`. - Type of
-`user_id` parameter in `changeset.get_query()` was changed from `str` to `int`.
-- `OsmChange_parser_generator()` and `OsmChange_parser()` from `diff` module
-are now 'private' functions. Use `Diff.get()` instead. - `notes.search()`
-endpoint throws `LimitsExceeded` exception instead of `ValueError`. -
-`page_number` paremeter in `gpx.get()` has now default value 0. - Now classes
-are imported from individual modules - not from the main library. See examples
-in the `README.md`. - `gpx.get()` renamed to `gpx.get_gps_points()` ### Removed
-- Support for `HTTP Basic authentication`: `username` and `password` parameters
+## [3.0.1] - 2024-05-21 ### Added - Support for python 3.12 ### Fixed -
+Dependencies update ## [3.0.0] - 2024-03-19 ### Added - Support for `oAuth2`:
+`access_token` parameter in `Api` class constructor. - `Unauthorized`
+exception. (No access token.) - `Forbidden` exception. (The access token does
+not support the needed scope or you must be a moderator.) - `gpx.create()`
+endpoint. - `GpxFile` data class. - `Visibility` enum. - `gpx.update()`
+endpoint. - `gpx.delete()` endpoint. - `gpx.get_details()` endpoint. -
+`gpx.get_file()` endpoint. - `gpx.list_details()` endpoint. - `order` parameter
+in `changeset.get_query()`. ### Fixed - Types in `elements` endpoint. - Missing
+documentation. - `misc.get_map_in_bbox()` endpoint should not yield `string`.
+### Changed - The way http errors are handled. - In `elements.get()` endpoint
+the `element` parameter has been renamed to `element_type`. - In
+`elements.history()` endpoint the `element` parameter has been renamed to
+`element_type`. - In `elements.version()` endpoint the `element` parameter has
+been renamed to `element_type`. - In `elements.getQuery()` endpoint the
+`element` parameter has been renamed to `element_type`. - In
+`elements.relations()` endpoint the `element` parameter has been renamed to
+`element_type`. - In `elements.full()` endpoint the `element` parameter has
+been renamed to `element_type`. - Type of `user_id` parameter in
+`changeset.get_query()` was changed from `str` to `int`. -
+`OsmChange_parser_generator()` and `OsmChange_parser()` from `diff` module are
+now 'private' functions. Use `Diff.get()` instead. - `notes.search()` endpoint
+throws `LimitsExceeded` exception instead of `ValueError`. - `page_number`
+paremeter in `gpx.get()` has now default value 0. - Now classes are imported
+from individual modules - not from the main library. See examples in the
+`README.md`. - `gpx.get()` renamed to `gpx.get_gps_points()` ### Removed -
+Support for `HTTP Basic authentication`: `username` and `password` parameters
 in `Api` class constructor. - Most `# type: ignore`. - `NotAModerator`
 exception. It is now replaced by `Forbidden` exception. ## [2.2.0] - 2024-02-23
 ### Added - Exception for `410` status code in notes endpoint. ## [2.1.1] -
 2024-01-04 ### Fixed - Percent-encoding was not applied on texts entered by the
 user. [#22](https://github.com/docentYT/osm_easy_api/issues/22) ## [2.1.0] -
 2023-09-06 ### Added - `TooManyRequests` exception. - Support for `429` status
 code in `api.changeset.discussion.comment()`. ## [2.0.0] - 2023-08-29 ### Added
```

### Comparing `osm_easy_api-3.0.0/src/osm_easy_api.egg-info/SOURCES.txt` & `osm_easy_api-3.0.1/src/osm_easy_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

