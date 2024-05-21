# Comparing `tmp/stac-pydantic-3.0.0.tar.gz` & `tmp/stac_pydantic-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac-pydantic-3.0.0.tar", last modified: Thu Jan 25 13:15:55 2024, max compression
+gzip compressed data, was "stac_pydantic-3.1.0.tar", last modified: Tue May 21 17:31:05 2024, max compression
```

## Comparing `stac-pydantic-3.0.0.tar` & `stac_pydantic-3.1.0.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:15:55.854678 stac-pydantic-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-01-25 13:15:55.854678 stac-pydantic-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6136 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 13:15:55.854678 stac-pydantic-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:15:55.846678 stac-pydantic-3.0.0/stac_pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:15:55.850678 stac-pydantic-3.0.0/stac_pydantic/api/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/conformance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:15:55.850678 stac-pydantic-3.0.0/stac_pydantic/api/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/extensions/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/extensions/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/extensions/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/extensions/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/item_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/landing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     4690 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:15:55.850678 stac-pydantic-3.0.0/stac_pydantic/api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/utils/link_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/api/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/item.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/item_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/links.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:15:55.850678 stac-pydantic-3.0.0/stac_pydantic/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/stac_pydantic/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:15:55.850678 stac-pydantic-3.0.0/stac_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-01-25 13:15:55.000000 stac-pydantic-3.0.0/stac_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-25 13:15:55.000000 stac-pydantic-3.0.0/stac_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 13:15:55.000000 stac-pydantic-3.0.0/stac_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-01-25 13:15:55.000000 stac-pydantic-3.0.0/stac_pydantic.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-01-25 13:15:55.000000 stac-pydantic-3.0.0/stac_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-01-25 13:15:55.000000 stac-pydantic-3.0.0/stac_pydantic.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 13:15:55.850678 stac-pydantic-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/tests/test_item_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     8580 2024-01-25 13:15:37.000000 stac-pydantic-3.0.0/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:05.728784 stac_pydantic-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-05-21 17:31:05.728784 stac_pydantic-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6214 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2647 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 17:31:05.728784 stac_pydantic-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:05.720784 stac_pydantic-3.1.0/stac_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:05.724784 stac_pydantic-3.1.0/stac_pydantic/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/conformance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:05.724784 stac_pydantic-3.1.0/stac_pydantic/api/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/extensions/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/extensions/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/extensions/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1922 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/item_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2003 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/landing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5365 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:05.724784 stac_pydantic-3.1.0/stac_pydantic/api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/utils/link_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/api/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/item_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:05.724784 stac_pydantic-3.1.0/stac_pydantic/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5933 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/stac_pydantic/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:05.724784 stac_pydantic-3.1.0/stac_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-05-21 17:31:05.000000 stac_pydantic-3.1.0/stac_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-21 17:31:05.000000 stac_pydantic-3.1.0/stac_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:31:05.000000 stac_pydantic-3.1.0/stac_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-21 17:31:05.000000 stac_pydantic-3.1.0/stac_pydantic.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-21 17:31:05.000000 stac_pydantic-3.1.0/stac_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 17:31:05.000000 stac_pydantic-3.1.0/stac_pydantic.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:31:05.724784 stac_pydantic-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/tests/test_item_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-21 17:30:54.000000 stac_pydantic-3.1.0/tests/test_models.py
```

### Comparing `stac-pydantic-3.0.0/LICENSE` & `stac_pydantic-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stac-pydantic-3.0.0/PKG-INFO` & `stac_pydantic-3.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: stac-pydantic
-Version: 3.0.0
+Version: 3.1.0
 Summary: Pydantic data models for the STAC spec
 Author-email: Arturo Engineering <engineering@arturo.ai>
 License: MIT
 Project-URL: homepage, https://github.com/stac-utils/stac-pydantic
 Project-URL: repository, https://github.com/stac-utils/stac-pydantic.git
 Keywords: stac,pydantic,validation
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8.1.7
 Requires-Dist: pydantic>=2.4.1
 Requires-Dist: geojson-pydantic>=1.0.0
 Provides-Extra: dev
-Requires-Dist: arrow>=1.2.3; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: pytest-icdiff>=0.8; extra == "dev"
 Requires-Dist: requests>=2.31.0; extra == "dev"
 Requires-Dist: shapely>=2.0.1; extra == "dev"
 Requires-Dist: dictdiffer>=0.9.0; extra == "dev"
 Requires-Dist: jsonschema>=4.19.1; extra == "dev"
@@ -52,29 +52,30 @@
 
 The main purpose of this library is to provide reusable request/response models for tools such as [fastapi](https://fastapi.tiangolo.com/).
 For more comprehensive schema validation and robust extension support, use [pystac](https://github.com/stac-utils/pystac).
 
 ## Installation
 
 ```shell
-pip install stac-pydantic
+python -m pip install stac-pydantic
 ```
 
 For local development:
 
 ```shell
-pip install -e '.[dev,lint]'
+python -m pip install -e '.[dev,lint]'
 ```
 
 | stac-pydantic | STAC Version | STAC API Version | Pydantic Version |
 |--------------|---------------|------------------|-----------------|
 | 1.2.x         | 1.0.0-beta.1 | <1* | ^1.6 |
 | 1.3.x         | 1.0.0-beta.2 | <1* | ^1.6 |
 | 2.0.x         | 1.0.0        | <1* | ^1.6 |
 | 3.0.x         | 1.0.0        | 1.0.0 | ^2.4 |
+| 3.1.x         | 1.0.0        | 1.0.0 | ^2.4 |
 
 \* various beta releases, specs not fully implemented
 
 ## Development
 
 Install the [pre-commit](https://pre-commit.com/) hooks:
 
@@ -99,15 +100,15 @@
 ```shell
 tox
 ```
 
 Run a single test case using the standard pytest convention:
 
 ```shell
-pytest -v tests/test_models.py::test_item_extensions
+python -m pytest -v tests/test_models.py::test_item_extensions
 ```
 
 ## Usage
 
 ### Loading Models
 
 Load data into models with standard pydantic:
```

### Comparing `stac-pydantic-3.0.0/README.md` & `stac_pydantic-3.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,29 +7,30 @@
 
 The main purpose of this library is to provide reusable request/response models for tools such as [fastapi](https://fastapi.tiangolo.com/).
 For more comprehensive schema validation and robust extension support, use [pystac](https://github.com/stac-utils/pystac).
 
 ## Installation
 
 ```shell
-pip install stac-pydantic
+python -m pip install stac-pydantic
 ```
 
 For local development:
 
 ```shell
-pip install -e '.[dev,lint]'
+python -m pip install -e '.[dev,lint]'
 ```
 
 | stac-pydantic | STAC Version | STAC API Version | Pydantic Version |
 |--------------|---------------|------------------|-----------------|
 | 1.2.x         | 1.0.0-beta.1 | <1* | ^1.6 |
 | 1.3.x         | 1.0.0-beta.2 | <1* | ^1.6 |
 | 2.0.x         | 1.0.0        | <1* | ^1.6 |
 | 3.0.x         | 1.0.0        | 1.0.0 | ^2.4 |
+| 3.1.x         | 1.0.0        | 1.0.0 | ^2.4 |
 
 \* various beta releases, specs not fully implemented
 
 ## Development
 
 Install the [pre-commit](https://pre-commit.com/) hooks:
 
@@ -54,15 +55,15 @@
 ```shell
 tox
 ```
 
 Run a single test case using the standard pytest convention:
 
 ```shell
-pytest -v tests/test_models.py::test_item_extensions
+python -m pytest -v tests/test_models.py::test_item_extensions
 ```
 
 ## Usage
 
 ### Loading Models
 
 Load data into models with standard pydantic:
```

### Comparing `stac-pydantic-3.0.0/pyproject.toml` & `stac_pydantic-3.1.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -9,16 +9,17 @@
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: MIT License",
-    ]
+]
 keywords=["stac", "pydantic", "validation"]
 authors=[{ name = "Arturo Engineering", email = "engineering@arturo.ai"}]
 license= { text = "MIT" }
 requires-python=">=3.8"
 dependencies = ["click>=8.1.7", "pydantic>=2.4.1", "geojson-pydantic>=1.0.0"]
 dynamic = ["version", "readme"]
 
@@ -26,33 +27,37 @@
 stac-pydantic = "stac_pydantic.scripts.cli:app"
 
 [project.urls]
 homepage = "https://github.com/stac-utils/stac-pydantic"
 repository ="https://github.com/stac-utils/stac-pydantic.git"
 
 [project.optional-dependencies]
-dev = ["arrow>=1.2.3",
+dev = [
         "pytest>=7.4.2",
         "pytest-cov>=4.1.0",
         "pytest-icdiff>=0.8",
         "requests>=2.31.0",
         "shapely>=2.0.1",
         "dictdiffer>=0.9.0",
         "jsonschema>=4.19.1",
-        "pyyaml>=6.0.1"]
-lint = ["types-requests>=2.31.0.5",
+        "pyyaml>=6.0.1"
+]
+
+lint = [
+        "types-requests>=2.31.0.5",
         "types-jsonschema>=4.19.0.3",
         "types-PyYAML>=6.0.12.12",
         "black>=23.9.1",
         "isort>=5.12.0",
         "flake8>=6.1.0",
         "Flake8-pyproject>=1.2.3",
         "mypy>=1.5.1",
         "pre-commit>=3.4.0",
-        "tox>=4.11.3"]
+        "tox>=4.11.3"
+]
 
 [tool.setuptools.dynamic]
 version = { attr = "stac_pydantic.version.__version__" }
 readme = {file = ["README.md"], content-type = "text/markdown"}
 
 [tool.setuptools.package-data]
 stac_pydantic= ["*.typed"]
@@ -60,27 +65,33 @@
 [tool.setuptools.packages.find]
 include = ["stac_pydantic*"]
 exclude = ["tests*"]
 
 [tool.pytest.ini_options]
 addopts = "-sv --cov stac_pydantic --cov-report xml --cov-report term-missing  --cov-fail-under 95"
 
-[tool.black]
-line-length = 88
-target-version = ["py311"]
-
 [tool.isort]
 profile = "black"
 known_first_party = "stac_pydantic"
 known_third_party = ["pydantic", "geojson-pydantic", "click"]
 default_section = "THIRDPARTY"
 
 [tool.mypy]
-plugins = "pydantic.mypy"
 ignore_missing_imports = true
 exclude = ["tests", ".venv"]
 
-[tool.flake8]
-ignore = ["E203", "E501"]
-select = ["C","E","F","W","B","B950"]
-exclude = ["tests", ".venv"]
-max-line-length = 88
+[tool.ruff]
+line-length = 88
+
+[tool.ruff.lint]
+select = [
+        "C",
+        "E",
+        "F",
+        "W",
+        "B",
+]
+ignore = [
+    "E203",  # line too long, handled by black
+    "E501",  # do not perform function calls in argument defaults
+    "B028",  # No explicit `stacklevel` keyword argument found
+]
```

### Comparing `stac-pydantic-3.0.0/stac_pydantic/api/collection.py` & `stac_pydantic-3.1.0/stac_pydantic/api/collection.py`

 * *Files identical despite different names*

### Comparing `stac-pydantic-3.0.0/stac_pydantic/api/collections.py` & `stac_pydantic-3.1.0/stac_pydantic/api/collections.py`

 * *Files identical despite different names*

### Comparing `stac-pydantic-3.0.0/stac_pydantic/api/extensions/fields.py` & `stac_pydantic-3.1.0/stac_pydantic/api/extensions/fields.py`

 * *Files identical despite different names*

### Comparing `stac-pydantic-3.0.0/stac_pydantic/api/extensions/query.py` & `stac_pydantic-3.1.0/stac_pydantic/api/extensions/query.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,58 @@
+"""Query Extension."""
+
+import warnings
 from enum import auto
 from types import DynamicClassAttribute
 from typing import Any, Callable
 
 from stac_pydantic.utils import AutoValueEnum
 
 # TODO: These are defined in the spec but aren't currently implemented by the operator syntax
 UNSUPPORTED_OPERATORS = {"startsWith", "endsWith", "contains", "in"}
 
 _OPERATIONS = {
     "eq": lambda x, y: x == y,
-    "ne": lambda x, y: x != y,
+    "ne": lambda x, y: x != y,  # deprecated
+    "neq": lambda x, y: x != y,
     "lt": lambda x, y: x < y,
-    "le": lambda x, y: x <= y,
+    "le": lambda x, y: x <= y,  # deprecated
+    "lte": lambda x, y: x <= y,
     "gt": lambda x, y: x > y,
-    "ge": lambda x, y: x >= y,
+    "ge": lambda x, y: x >= y,  # deprecated
+    "gte": lambda x, y: x >= y,
     "startsWith": lambda x, y: x.startsWith(y),
     "endsWith": lambda x, y: x.endsWith(y),
     "contains": lambda x, y: y in x,
 }
 
 
 class Operator(str, AutoValueEnum):
     """
     https://github.com/radiantearth/stac-api-spec/tree/master/extensions/query#query-api-extension
     """
 
     eq = auto()
-    ne = auto()
+    ne = auto()  # deprecated
+    neq = auto()
     lt = auto()
-    le = auto()
+    le = auto()  # deprecated
+    lte = auto()
     gt = auto()
-    ge = auto()
+    ge = auto()  # deprecated
+    gte = auto()
     startsWith = auto()
     endsWith = auto()
     contains = auto()
 
     @DynamicClassAttribute
     def operator(self) -> Callable[[Any, Any], bool]:
         """Return python operator"""
+        if self._value_ in ["ne", "ge", "le"]:
+            newvalue = self._value_.replace("e", "te")
+            warnings.warn(
+                f"`{self._value_}` is deprecated, please use `{newvalue}`",
+                DeprecationWarning,
+                stacklevel=3,
+            )
+
         return _OPERATIONS[self._value_]
```

### Comparing `stac-pydantic-3.0.0/stac_pydantic/api/item.py` & `stac_pydantic-3.1.0/stac_pydantic/api/item.py`

 * *Files identical despite different names*

### Comparing `stac-pydantic-3.0.0/stac_pydantic/api/item_collection.py` & `stac_pydantic-3.1.0/stac_pydantic/api/item_collection.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Optional, Sequence
 from urllib.parse import urlparse
 
 from pydantic import model_validator
 
-from stac_pydantic.api.extensions.context import ContextExtension
 from stac_pydantic.api.item import Item
 from stac_pydantic.api.links import Links
 from stac_pydantic.item_collection import ItemCollection as BaseItemCollection
 from stac_pydantic.links import Relations
 
 
 class ItemCollection(BaseItemCollection):
@@ -17,17 +16,14 @@
     """
 
     features: Sequence[Item]
     links: Optional[Links] = None
     numberMatched: Optional[int] = None
     numberReturned: Optional[int] = None
 
-    # Context Extension
-    context: Optional[ContextExtension] = None
-
     @model_validator(mode="after")
     def required_links(self) -> "ItemCollection":
         if self.links:
             links_rel = [link.rel for link in self.links.root]
             if Relations.self in links_rel:
                 self_href = [link for link in self.links.root if link.rel == "self"][0]
                 item_collection_type = urlparse(self_href.href).path.split("/")[-1]
```

### Comparing `stac-pydantic-3.0.0/stac_pydantic/api/landing.py` & `stac_pydantic-3.1.0/stac_pydantic/api/landing.py`

 * *Files identical despite different names*

### Comparing `stac-pydantic-3.0.0/stac_pydantic/api/links.py` & `stac_pydantic-3.1.0/stac_pydantic/api/links.py`

 * *Files identical despite different names*

### Comparing `stac-pydantic-3.0.0/stac_pydantic/api/search.py` & `stac_pydantic-3.1.0/stac_pydantic/api/search.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,69 +1,65 @@
 from datetime import datetime as dt
 from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
-from geojson_pydantic.geometries import (  # type: ignore
+from geojson_pydantic.geometries import (
     GeometryCollection,
     LineString,
     MultiLineString,
     MultiPoint,
     MultiPolygon,
     Point,
     Polygon,
 )
-from pydantic import BaseModel, Field, field_validator, model_validator
+from pydantic import BaseModel, Field, TypeAdapter, field_validator, model_validator
 
 from stac_pydantic.api.extensions.fields import FieldsExtension
 from stac_pydantic.api.extensions.query import Operator
 from stac_pydantic.api.extensions.sort import SortExtension
-from stac_pydantic.shared import BBox
-from stac_pydantic.utils import parse_datetime
+from stac_pydantic.shared import BBox, UtcDatetime
 
 Intersection = Union[
     Point,
     MultiPoint,
     LineString,
     MultiLineString,
     Polygon,
     MultiPolygon,
     GeometryCollection,
 ]
 
+SearchDatetime = TypeAdapter(Optional[UtcDatetime])
+
 
 class Search(BaseModel):
     """
     The base class for STAC API searches.
 
     https://github.com/radiantearth/stac-api-spec/blob/v1.0.0/item-search/README.md#query-parameter-table
     """
 
     collections: Optional[List[str]] = None
     ids: Optional[List[str]] = None
     bbox: Optional[BBox] = None
     intersects: Optional[Intersection] = None
     datetime: Optional[str] = None
-    limit: int = 10
+    limit: Optional[int] = 10
+
+    # Private properties to store the parsed datetime values. Not part of the model schema.
+    _start_date: Optional[dt] = None
+    _end_date: Optional[dt] = None
 
+    # Properties to return the private values
     @property
     def start_date(self) -> Optional[dt]:
-        values = (self.datetime or "").split("/")
-        if len(values) == 1:
-            return None
-        if values[0] == ".." or values[0] == "":
-            return None
-        return parse_datetime(values[0])
+        return self._start_date
 
     @property
     def end_date(self) -> Optional[dt]:
-        values = (self.datetime or "").split("/")
-        if len(values) == 1:
-            return parse_datetime(values[0])
-        if values[1] == ".." or values[1] == "":
-            return None
-        return parse_datetime(values[1])
+        return self._end_date
 
     # Check https://docs.pydantic.dev/dev-v2/migration/#changes-to-validators for more information.
     @model_validator(mode="before")
     def validate_spatial(cls, values: Dict[str, Any]) -> Dict[str, Any]:
         if values.get("intersects") and values.get("bbox") is not None:
             raise ValueError("intersects and bbox parameters are mutually exclusive")
         return values
@@ -98,37 +94,51 @@
             if xmin < -180 or ymin < -90 or xmax > 180 or ymax > 90:
                 raise ValueError("Bounding box must be within (-180, -90, 180, 90)")
 
         return v
 
     @field_validator("datetime")
     @classmethod
-    def validate_datetime(cls, v: str) -> str:
-        if "/" in v:
-            values = v.split("/")
-        else:
-            # Single date is interpreted as end date
-            values = ["..", v]
-
-        dates = []
-        for value in values:
-            if value == ".." or value == "":
-                dates.append("..")
-                continue
-
-            parse_datetime(value)
-            dates.append(value)
+    def validate_datetime(cls, value: str) -> str:
+        # Split on "/" and replace no value or ".." with None
+        values = [v if v and v != ".." else None for v in value.split("/")]
+
+        # If there are more than 2 dates, it's invalid
+        if len(values) > 2:
+            raise ValueError(
+                "Invalid datetime range. Too many values. Must match format: {begin_date}/{end_date}"
+            )
 
-        if ".." not in dates:
-            if parse_datetime(dates[0]) > parse_datetime(dates[1]):
-                raise ValueError(
-                    "Invalid datetime range, must match format (begin_date, end_date)"
-                )
+        # If there is only one date, duplicate to use for both start and end dates
+        if len(values) == 1:
+            values = [values[0], values[0]]
 
-        return v
+        # Cast because pylance gets confused by the type adapter and annotated type
+        dates = cast(
+            List[Optional[dt]],
+            [
+                # Use the type adapter to validate the datetime strings, strict is necessary
+                # due to pydantic issues #8736 and #8762
+                SearchDatetime.validate_strings(v, strict=True) if v else None
+                for v in values
+            ],
+        )
+
+        # If there is a start and end date, check that the start date is before the end date
+        if dates[0] and dates[1] and dates[0] > dates[1]:
+            raise ValueError(
+                "Invalid datetime range. Begin date after end date. "
+                "Must match format: {begin_date}/{end_date}"
+            )
+
+        # Store the parsed dates
+        cls._start_date = dates[0]
+        cls._end_date = dates[1]
+        # Return the original string value
+        return value
 
     @property
     def spatial_filter(self) -> Optional[Intersection]:
         """Return a geojson-pydantic object representing the spatial filter for the search request.
 
         Check for both because the ``bbox`` and ``intersects`` parameters are mutually exclusive.
         """
```

### Comparing `stac-pydantic-3.0.0/stac_pydantic/api/utils/link_factory.py` & `stac_pydantic-3.1.0/stac_pydantic/api/utils/link_factory.py`

 * *Files identical despite different names*

### Comparing `stac-pydantic-3.0.0/stac_pydantic/catalog.py` & `stac_pydantic-3.1.0/stac_pydantic/catalog.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,8 +19,8 @@
     stac_extensions: Optional[List[AnyUrl]] = []
     title: Optional[str] = None
     type: str
     model_config = ConfigDict(use_enum_values=True, extra="allow")
 
 
 class Catalog(_Catalog):
-    type: Literal["Catalog"] = "Catalog"
+    type: Literal["Catalog"]
```

### Comparing `stac-pydantic-3.0.0/stac_pydantic/collection.py` & `stac_pydantic-3.1.0/stac_pydantic/collection.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,8 +48,8 @@
     assets: Optional[Dict[str, Asset]] = None
     license: str = Field(..., alias="license", min_length=1)
     extent: Extent
     title: Optional[str] = None
     keywords: Optional[List[str]] = None
     providers: Optional[List[Provider]] = None
     summaries: Optional[Dict[str, Union[Range, List[Any], Dict[str, Any]]]] = None
-    type: Literal["Collection"] = "Collection"
+    type: Literal["Collection"]
```

### Comparing `stac-pydantic-3.0.0/stac_pydantic/extensions.py` & `stac_pydantic-3.1.0/stac_pydantic/extensions.py`

 * *Files identical despite different names*

### Comparing `stac-pydantic-3.0.0/stac_pydantic/item_collection.py` & `stac_pydantic-3.1.0/stac_pydantic/item_collection.py`

 * *Files identical despite different names*

### Comparing `stac-pydantic-3.0.0/stac_pydantic/links.py` & `stac_pydantic-3.1.0/stac_pydantic/links.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     href: str = Field(..., alias="href", min_length=1)
     rel: str = Field(..., alias="rel", min_length=1)
     type: Optional[MimeTypes] = None
     title: Optional[str] = None
 
     # Label extension
     label: Optional[str] = Field(default=None, alias="label:assets")
-    model_config = ConfigDict(use_enum_values=True, extra="forbid")
+    model_config = ConfigDict(use_enum_values=True, extra="allow")
 
     def resolve(self, base_url: str) -> None:
         """resolve a link to the given base URL"""
         self.href = urljoin(base_url, self.href)
 
 
 class Links(RootModel[List[Link]]):
@@ -74,7 +74,8 @@
     search = auto()
     preview = auto()
     canonical = auto()
     via = auto()
     data = auto()
     service_desc = "service-desc"
     service_doc = "service-doc"
+    queryables = "http://www.opengis.net/def/rel/ogc/1.0/queryables"
```

### Comparing `stac-pydantic-3.0.0/stac_pydantic/scripts/cli.py` & `stac_pydantic-3.1.0/stac_pydantic/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `stac-pydantic-3.0.0/stac_pydantic.egg-info/PKG-INFO` & `stac_pydantic-3.1.0/stac_pydantic.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 Metadata-Version: 2.1
 Name: stac-pydantic
-Version: 3.0.0
+Version: 3.1.0
 Summary: Pydantic data models for the STAC spec
 Author-email: Arturo Engineering <engineering@arturo.ai>
 License: MIT
 Project-URL: homepage, https://github.com/stac-utils/stac-pydantic
 Project-URL: repository, https://github.com/stac-utils/stac-pydantic.git
 Keywords: stac,pydantic,validation
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: click>=8.1.7
 Requires-Dist: pydantic>=2.4.1
 Requires-Dist: geojson-pydantic>=1.0.0
 Provides-Extra: dev
-Requires-Dist: arrow>=1.2.3; extra == "dev"
 Requires-Dist: pytest>=7.4.2; extra == "dev"
 Requires-Dist: pytest-cov>=4.1.0; extra == "dev"
 Requires-Dist: pytest-icdiff>=0.8; extra == "dev"
 Requires-Dist: requests>=2.31.0; extra == "dev"
 Requires-Dist: shapely>=2.0.1; extra == "dev"
 Requires-Dist: dictdiffer>=0.9.0; extra == "dev"
 Requires-Dist: jsonschema>=4.19.1; extra == "dev"
@@ -52,29 +52,30 @@
 
 The main purpose of this library is to provide reusable request/response models for tools such as [fastapi](https://fastapi.tiangolo.com/).
 For more comprehensive schema validation and robust extension support, use [pystac](https://github.com/stac-utils/pystac).
 
 ## Installation
 
 ```shell
-pip install stac-pydantic
+python -m pip install stac-pydantic
 ```
 
 For local development:
 
 ```shell
-pip install -e '.[dev,lint]'
+python -m pip install -e '.[dev,lint]'
 ```
 
 | stac-pydantic | STAC Version | STAC API Version | Pydantic Version |
 |--------------|---------------|------------------|-----------------|
 | 1.2.x         | 1.0.0-beta.1 | <1* | ^1.6 |
 | 1.3.x         | 1.0.0-beta.2 | <1* | ^1.6 |
 | 2.0.x         | 1.0.0        | <1* | ^1.6 |
 | 3.0.x         | 1.0.0        | 1.0.0 | ^2.4 |
+| 3.1.x         | 1.0.0        | 1.0.0 | ^2.4 |
 
 \* various beta releases, specs not fully implemented
 
 ## Development
 
 Install the [pre-commit](https://pre-commit.com/) hooks:
 
@@ -99,15 +100,15 @@
 ```shell
 tox
 ```
 
 Run a single test case using the standard pytest convention:
 
 ```shell
-pytest -v tests/test_models.py::test_item_extensions
+python -m pytest -v tests/test_models.py::test_item_extensions
 ```
 
 ## Usage
 
 ### Loading Models
 
 Load data into models with standard pydantic:
```

### Comparing `stac-pydantic-3.0.0/stac_pydantic.egg-info/SOURCES.txt` & `stac_pydantic-3.1.0/stac_pydantic.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 stac_pydantic/api/item.py
 stac_pydantic/api/item_collection.py
 stac_pydantic/api/landing.py
 stac_pydantic/api/links.py
 stac_pydantic/api/search.py
 stac_pydantic/api/version.py
 stac_pydantic/api/extensions/__init__.py
-stac_pydantic/api/extensions/context.py
 stac_pydantic/api/extensions/fields.py
 stac_pydantic/api/extensions/query.py
 stac_pydantic/api/extensions/sort.py
 stac_pydantic/api/utils/__init__.py
 stac_pydantic/api/utils/link_factory.py
 stac_pydantic/scripts/__init__.py
 stac_pydantic/scripts/cli.py
```

### Comparing `stac-pydantic-3.0.0/tests/test_item_collection.py` & `stac_pydantic-3.1.0/tests/test_item_collection.py`

 * *Files identical despite different names*

### Comparing `stac-pydantic-3.0.0/tests/test_models.py` & `stac_pydantic-3.1.0/tests/test_models.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 from typing import Literal
 
 import pytest
 from pydantic import ConfigDict, ValidationError
 from shapely.geometry import shape
 
 from stac_pydantic import Collection, Item, ItemProperties
-from stac_pydantic.api.extensions.context import ContextExtension
 from stac_pydantic.extensions import validate_extensions
 from stac_pydantic.links import Link, Links
-from stac_pydantic.shared import MimeTypes
+from stac_pydantic.shared import MimeTypes, StacCommonMetadata
 
 from .conftest import dict_match, request
 
 COLLECTION = "landsat-collection.json"
 ITEM_COLLECTION = "itemcollection-sample-full.json"
 SINGLE_FILE_STAC = "example-search.json"
 
@@ -61,17 +60,17 @@
     valid_item = Item(**test_item).model_dump()
     dict_match(test_item, valid_item)
 
 
 def test_proj_extension() -> None:
     # The example item uses an invalid band name
     test_item = request(PROJ_EXTENSION)
-    test_item["stac_extensions"][
-        1
-    ] = "https://raw.githubusercontent.com/stac-extensions/projection/v1.0.0/json-schema/schema.json"
+    test_item["stac_extensions"][1] = (
+        "https://raw.githubusercontent.com/stac-extensions/projection/v1.0.0/json-schema/schema.json"
+    )
     test_item["assets"]["B8"]["eo:bands"][0]["common_name"] = "pan"
 
     valid_item = Item.model_validate(test_item).model_dump()
     dict_match(test_item, valid_item)
 
 
 def test_version_extension_item() -> None:
@@ -145,29 +144,85 @@
 
 def test_asset_extras() -> None:
     test_item = request(EO_EXTENSION)
     for asset in test_item["assets"]:
         test_item["assets"][asset]["foo"] = "bar"
 
     item = Item(**test_item)
-    for asset_name, asset in item.assets.items():
+    for _, asset in item.assets.items():
         assert asset.foo == "bar"
 
 
 def test_geo_interface() -> None:
     test_item = request(EO_EXTENSION)
     item = Item(**test_item)
     geom = shape(item.geometry)
     test_item["geometry"] = geom
     Item(**test_item)
 
 
-def test_api_context_extension() -> None:
-    context = {"returned": 10, "limit": 10, "matched": 100}
-    ContextExtension(**context)
+@pytest.mark.parametrize(
+    "args",
+    [
+        {"datetime": "2024-01-01T00:00:00Z"},
+        {
+            "datetime": None,
+            "start_datetime": "2024-01-01T00:00:00Z",
+            "end_datetime": "2024-01-02T00:00:00Z",
+        },
+        {
+            "datetime": "2024-01-01T00:00:00Z",
+            "start_datetime": "2024-01-01T00:00:00Z",
+            "end_datetime": "2024-01-02T00:00:00Z",
+        },
+    ],
+)
+def test_stac_common_dates(args) -> None:
+    StacCommonMetadata(**args)
+
+
+def test_stac_null_datetime_required() -> None:
+    with pytest.raises(ValidationError):
+        StacCommonMetadata(
+            **{
+                "start_datetime": "2024-01-01T00:00:00Z",
+                "end_datetime": "2024-01-02T00:00:00Z",
+            }
+        )
+
+
+@pytest.mark.parametrize(
+    "args",
+    [
+        {"datetime": None},
+        {"datetime": None, "start_datetime": "2024-01-01T00:00:00Z"},
+        {"datetime": None, "end_datetime": "2024-01-01T00:00:00Z"},
+    ],
+)
+def test_stac_common_no_dates(args) -> None:
+    with pytest.raises(
+        ValueError,
+        match="start_datetime and end_datetime must be specified when datetime is null",
+    ):
+        StacCommonMetadata(**args)
+
+
+@pytest.mark.parametrize(
+    "args",
+    [
+        {"datetime": "2024-01-01T00:00:00Z", "start_datetime": "2024-01-01T00:00:00Z"},
+        {"datetime": "2024-01-01T00:00:00Z", "end_datetime": "2024-01-01T00:00:00Z"},
+    ],
+)
+def test_stac_common_start_and_end(args) -> None:
+    with pytest.raises(
+        ValueError,
+        match="use of start_datetime or end_datetime requires the use of the other",
+    ):
+        StacCommonMetadata(**args)
 
 
 def test_declared_model() -> None:
     class TestProperties(ItemProperties):
         foo: str
         bar: int
```

