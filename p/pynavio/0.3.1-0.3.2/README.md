# Comparing `tmp/pynavio-0.3.1.tar.gz` & `tmp/pynavio-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynavio-0.3.1.tar", last modified: Tue Jan 23 16:45:52 2024, max compression
+gzip compressed data, was "pynavio-0.3.2.tar", last modified: Tue May 21 16:39:11 2024, max compression
```

## Comparing `pynavio-0.3.1.tar` & `pynavio-0.3.2.tar`

### file list

```diff
@@ -1,60 +1,70 @@
-drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-01-23 16:45:52.801621 pynavio-0.3.1/
--rw-r--r--   0 clarareolid   (501) staff       (20)      146 2024-01-22 11:10:05.000000 pynavio-0.3.1/AUTHORS.rst
--rw-r--r--   0 clarareolid   (501) staff       (20)     3945 2024-01-23 16:15:51.000000 pynavio-0.3.1/HISTORY.rst
--rw-r--r--   0 clarareolid   (501) staff       (20)     1069 2023-10-31 13:03:40.000000 pynavio-0.3.1/LICENSE
--rw-r--r--   0 clarareolid   (501) staff       (20)      237 2024-01-22 11:10:05.000000 pynavio-0.3.1/MANIFEST.in
--rw-r--r--   0 clarareolid   (501) staff       (20)     7170 2024-01-23 16:45:52.801477 pynavio-0.3.1/PKG-INFO
--rw-r--r--   0 clarareolid   (501) staff       (20)     2389 2024-01-23 16:32:48.000000 pynavio-0.3.1/README.rst
-drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-01-23 16:45:52.789807 pynavio-0.3.1/docs/
--rw-r--r--   0 clarareolid   (501) staff       (20)      608 2023-10-31 13:03:40.000000 pynavio-0.3.1/docs/Makefile
--rw-r--r--   0 clarareolid   (501) staff       (20)       28 2023-10-31 13:03:40.000000 pynavio-0.3.1/docs/authors.rst
--rwxr-xr-x   0 clarareolid   (501) staff       (20)     4772 2023-10-31 13:03:40.000000 pynavio-0.3.1/docs/conf.py
--rw-r--r--   0 clarareolid   (501) staff       (20)       33 2023-10-31 13:03:40.000000 pynavio-0.3.1/docs/contributing.rst
--rw-r--r--   0 clarareolid   (501) staff       (20)       28 2023-10-31 13:03:40.000000 pynavio-0.3.1/docs/history.rst
--rw-r--r--   0 clarareolid   (501) staff       (20)      304 2023-10-31 13:03:40.000000 pynavio-0.3.1/docs/index.rst
--rw-r--r--   0 clarareolid   (501) staff       (20)     1138 2023-10-31 13:03:40.000000 pynavio-0.3.1/docs/installation.rst
--rw-r--r--   0 clarareolid   (501) staff       (20)      769 2023-10-31 13:03:40.000000 pynavio-0.3.1/docs/make.bat
--rw-r--r--   0 clarareolid   (501) staff       (20)       27 2023-10-31 13:03:40.000000 pynavio-0.3.1/docs/readme.rst
--rw-r--r--   0 clarareolid   (501) staff       (20)       69 2023-10-31 13:03:40.000000 pynavio-0.3.1/docs/usage.rst
-drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-01-23 16:45:52.792969 pynavio-0.3.1/pynavio/
--rw-r--r--   0 clarareolid   (501) staff       (20)      774 2024-01-23 16:15:51.000000 pynavio-0.3.1/pynavio/__init__.py
--rw-r--r--   0 clarareolid   (501) staff       (20)     4136 2024-01-22 11:10:05.000000 pynavio-0.3.1/pynavio/_code.py
--rw-r--r--   0 clarareolid   (501) staff       (20)    26039 2024-01-22 11:10:05.000000 pynavio-0.3.1/pynavio/_mlflow.py
--rw-r--r--   0 clarareolid   (501) staff       (20)     7750 2024-01-22 11:10:05.000000 pynavio-0.3.1/pynavio/client.py
--rw-r--r--   0 clarareolid   (501) staff       (20)     3823 2024-01-22 11:10:05.000000 pynavio-0.3.1/pynavio/dependencies.py
--rw-r--r--   0 clarareolid   (501) staff       (20)     1008 2023-10-31 13:03:40.000000 pynavio-0.3.1/pynavio/image.py
--rw-r--r--   0 clarareolid   (501) staff       (20)     1935 2024-01-22 11:10:05.000000 pynavio-0.3.1/pynavio/model_helpers.py
--rw-r--r--   0 clarareolid   (501) staff       (20)     3025 2023-10-31 13:03:40.000000 pynavio-0.3.1/pynavio/schema.py
--rw-r--r--   0 clarareolid   (501) staff       (20)     2258 2023-10-31 13:03:40.000000 pynavio-0.3.1/pynavio/traits.py
-drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-01-23 16:45:52.797160 pynavio-0.3.1/pynavio/utils/
--rw-r--r--   0 clarareolid   (501) staff       (20)      182 2023-10-31 13:03:40.000000 pynavio-0.3.1/pynavio/utils/__init__.py
--rw-r--r--   0 clarareolid   (501) staff       (20)      983 2023-10-31 13:03:40.000000 pynavio-0.3.1/pynavio/utils/common.py
--rw-r--r--   0 clarareolid   (501) staff       (20)     1455 2024-01-22 11:10:05.000000 pynavio-0.3.1/pynavio/utils/conda.py
--rw-r--r--   0 clarareolid   (501) staff       (20)      215 2023-10-31 13:03:40.000000 pynavio-0.3.1/pynavio/utils/json_encoder.py
--rw-r--r--   0 clarareolid   (501) staff       (20)     3488 2024-01-22 11:10:05.000000 pynavio-0.3.1/pynavio/utils/schemas.py
--rw-r--r--   0 clarareolid   (501) staff       (20)       99 2023-10-31 13:03:40.000000 pynavio-0.3.1/pynavio/utils/styling.py
-drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-01-23 16:45:52.794878 pynavio-0.3.1/pynavio.egg-info/
--rw-r--r--   0 clarareolid   (501) staff       (20)     7170 2024-01-23 16:45:52.000000 pynavio-0.3.1/pynavio.egg-info/PKG-INFO
--rw-r--r--   0 clarareolid   (501) staff       (20)     1193 2024-01-23 16:45:52.000000 pynavio-0.3.1/pynavio.egg-info/SOURCES.txt
--rw-r--r--   0 clarareolid   (501) staff       (20)        1 2024-01-23 16:45:52.000000 pynavio-0.3.1/pynavio.egg-info/dependency_links.txt
--rw-r--r--   0 clarareolid   (501) staff       (20)        1 2024-01-23 16:45:52.000000 pynavio-0.3.1/pynavio.egg-info/not-zip-safe
--rw-r--r--   0 clarareolid   (501) staff       (20)       75 2024-01-23 16:45:52.000000 pynavio-0.3.1/pynavio.egg-info/requires.txt
--rw-r--r--   0 clarareolid   (501) staff       (20)        8 2024-01-23 16:45:52.000000 pynavio-0.3.1/pynavio.egg-info/top_level.txt
--rw-r--r--   0 clarareolid   (501) staff       (20)      424 2024-01-23 16:45:52.802193 pynavio-0.3.1/setup.cfg
--rw-r--r--   0 clarareolid   (501) staff       (20)     1338 2024-01-23 16:15:51.000000 pynavio-0.3.1/setup.py
-drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-01-23 16:45:52.797822 pynavio-0.3.1/tests/
--rw-r--r--   0 clarareolid   (501) staff       (20)       37 2023-10-31 13:03:40.000000 pynavio-0.3.1/tests/__init__.py
--rw-r--r--   0 clarareolid   (501) staff       (20)      223 2024-01-22 11:10:05.000000 pynavio-0.3.1/tests/conftest.py
-drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-01-23 16:45:52.799424 pynavio-0.3.1/tests/test_pynavio/
-drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-01-23 16:45:52.783664 pynavio-0.3.1/tests/test_pynavio/fixtures/
-drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-01-23 16:45:52.800067 pynavio-0.3.1/tests/test_pynavio/fixtures/schemas/
--rw-r--r--   0 clarareolid   (501) staff       (20)      984 2024-01-22 11:10:05.000000 pynavio-0.3.1/tests/test_pynavio/fixtures/schemas/example_request.json
--rw-r--r--   0 clarareolid   (501) staff       (20)      987 2024-01-22 11:10:05.000000 pynavio-0.3.1/tests/test_pynavio/fixtures/schemas/example_request_nested.json
--rw-r--r--   0 clarareolid   (501) staff       (20)     6615 2024-01-22 11:10:05.000000 pynavio-0.3.1/tests/test_pynavio/test_client.py
--rw-r--r--   0 clarareolid   (501) staff       (20)     2145 2023-10-31 13:03:40.000000 pynavio-0.3.1/tests/test_pynavio/test_dependencies.py
--rw-r--r--   0 clarareolid   (501) staff       (20)      905 2023-10-31 13:03:40.000000 pynavio-0.3.1/tests/test_pynavio/test_dependencies_file_only.py
--rw-r--r--   0 clarareolid   (501) staff       (20)     9224 2024-01-22 11:10:05.000000 pynavio-0.3.1/tests/test_pynavio/test_mlflow.py
--rw-r--r--   0 clarareolid   (501) staff       (20)     3424 2023-10-31 13:03:40.000000 pynavio-0.3.1/tests/test_pynavio/test_schema.py
-drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-01-23 16:45:52.800883 pynavio-0.3.1/tests/test_pynavio/test_utils/
--rw-r--r--   0 clarareolid   (501) staff       (20)     1949 2024-01-22 11:10:05.000000 pynavio-0.3.1/tests/test_pynavio/test_utils/test_conda.py
--rw-r--r--   0 clarareolid   (501) staff       (20)     1712 2023-11-20 14:24:52.000000 pynavio-0.3.1/tests/test_pynavio/test_utils/test_conda.py.orig
+drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-05-21 16:39:11.982142 pynavio-0.3.2/
+-rw-r--r--   0 clarareolid   (501) staff       (20)      146 2024-01-22 11:10:05.000000 pynavio-0.3.2/AUTHORS.rst
+-rw-r--r--   0 clarareolid   (501) staff       (20)     4074 2024-05-21 16:22:02.000000 pynavio-0.3.2/HISTORY.rst
+-rw-r--r--   0 clarareolid   (501) staff       (20)     1069 2023-10-31 13:03:40.000000 pynavio-0.3.2/LICENSE
+-rw-r--r--   0 clarareolid   (501) staff       (20)      291 2024-05-21 15:57:40.000000 pynavio-0.3.2/MANIFEST.in
+-rw-r--r--   0 clarareolid   (501) staff       (20)     7333 2024-05-21 16:39:11.981978 pynavio-0.3.2/PKG-INFO
+-rw-r--r--   0 clarareolid   (501) staff       (20)     2389 2024-05-21 15:57:14.000000 pynavio-0.3.2/README.rst
+drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-05-21 16:39:11.966505 pynavio-0.3.2/docs/
+-rw-r--r--   0 clarareolid   (501) staff       (20)      608 2023-10-31 13:03:40.000000 pynavio-0.3.2/docs/Makefile
+-rw-r--r--   0 clarareolid   (501) staff       (20)       28 2023-10-31 13:03:40.000000 pynavio-0.3.2/docs/authors.rst
+-rwxr-xr-x   0 clarareolid   (501) staff       (20)     4772 2023-10-31 13:03:40.000000 pynavio-0.3.2/docs/conf.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)       33 2023-10-31 13:03:40.000000 pynavio-0.3.2/docs/contributing.rst
+-rw-r--r--   0 clarareolid   (501) staff       (20)       28 2023-10-31 13:03:40.000000 pynavio-0.3.2/docs/history.rst
+-rw-r--r--   0 clarareolid   (501) staff       (20)      304 2023-10-31 13:03:40.000000 pynavio-0.3.2/docs/index.rst
+-rw-r--r--   0 clarareolid   (501) staff       (20)     1138 2023-10-31 13:03:40.000000 pynavio-0.3.2/docs/installation.rst
+-rw-r--r--   0 clarareolid   (501) staff       (20)      769 2023-10-31 13:03:40.000000 pynavio-0.3.2/docs/make.bat
+-rw-r--r--   0 clarareolid   (501) staff       (20)       27 2023-10-31 13:03:40.000000 pynavio-0.3.2/docs/readme.rst
+-rw-r--r--   0 clarareolid   (501) staff       (20)       69 2023-10-31 13:03:40.000000 pynavio-0.3.2/docs/usage.rst
+drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-05-21 16:39:11.969452 pynavio-0.3.2/pynavio/
+-rw-r--r--   0 clarareolid   (501) staff       (20)      774 2024-05-21 15:57:40.000000 pynavio-0.3.2/pynavio/__init__.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)     4136 2024-01-22 11:10:05.000000 pynavio-0.3.2/pynavio/_code.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)    26039 2024-03-05 13:08:36.000000 pynavio-0.3.2/pynavio/_mlflow.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)     7750 2024-01-22 11:10:05.000000 pynavio-0.3.2/pynavio/client.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)     3823 2024-05-21 09:46:42.000000 pynavio-0.3.2/pynavio/dependencies.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)     1008 2023-10-31 13:03:40.000000 pynavio-0.3.2/pynavio/image.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)     1935 2024-01-22 11:10:05.000000 pynavio-0.3.2/pynavio/model_helpers.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)     3025 2023-10-31 13:03:40.000000 pynavio-0.3.2/pynavio/schema.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)     2258 2023-10-31 13:03:40.000000 pynavio-0.3.2/pynavio/traits.py
+drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-05-21 16:39:11.973814 pynavio-0.3.2/pynavio/utils/
+-rw-r--r--   0 clarareolid   (501) staff       (20)      182 2023-10-31 13:03:40.000000 pynavio-0.3.2/pynavio/utils/__init__.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)      983 2023-10-31 13:03:40.000000 pynavio-0.3.2/pynavio/utils/common.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)     1455 2024-03-05 13:08:36.000000 pynavio-0.3.2/pynavio/utils/conda.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)      215 2023-10-31 13:03:40.000000 pynavio-0.3.2/pynavio/utils/json_encoder.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)     3488 2024-01-22 11:10:05.000000 pynavio-0.3.2/pynavio/utils/schemas.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)       99 2023-10-31 13:03:40.000000 pynavio-0.3.2/pynavio/utils/styling.py
+drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-05-21 16:39:11.971639 pynavio-0.3.2/pynavio.egg-info/
+-rw-r--r--   0 clarareolid   (501) staff       (20)     7333 2024-05-21 16:39:11.000000 pynavio-0.3.2/pynavio.egg-info/PKG-INFO
+-rw-r--r--   0 clarareolid   (501) staff       (20)     1465 2024-05-21 16:39:11.000000 pynavio-0.3.2/pynavio.egg-info/SOURCES.txt
+-rw-r--r--   0 clarareolid   (501) staff       (20)        1 2024-05-21 16:39:11.000000 pynavio-0.3.2/pynavio.egg-info/dependency_links.txt
+-rw-r--r--   0 clarareolid   (501) staff       (20)        1 2024-05-21 16:39:11.000000 pynavio-0.3.2/pynavio.egg-info/not-zip-safe
+-rw-r--r--   0 clarareolid   (501) staff       (20)      109 2024-05-21 16:39:11.000000 pynavio-0.3.2/pynavio.egg-info/requires.txt
+-rw-r--r--   0 clarareolid   (501) staff       (20)        8 2024-05-21 16:39:11.000000 pynavio-0.3.2/pynavio.egg-info/top_level.txt
+-rw-r--r--   0 clarareolid   (501) staff       (20)      113 2024-05-21 15:57:40.000000 pynavio-0.3.2/requirements.txt
+-rw-r--r--   0 clarareolid   (501) staff       (20)      554 2024-03-05 13:08:36.000000 pynavio-0.3.2/requirements_dev.txt
+-rw-r--r--   0 clarareolid   (501) staff       (20)      424 2024-05-21 16:39:11.982808 pynavio-0.3.2/setup.cfg
+-rw-r--r--   0 clarareolid   (501) staff       (20)     1338 2024-05-21 15:57:40.000000 pynavio-0.3.2/setup.py
+drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-05-21 16:39:11.975002 pynavio-0.3.2/tests/
+-rw-r--r--   0 clarareolid   (501) staff       (20)       37 2023-10-31 13:03:40.000000 pynavio-0.3.2/tests/__init__.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)      223 2024-03-05 13:08:36.000000 pynavio-0.3.2/tests/conftest.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)     2524 2024-05-21 15:57:40.000000 pynavio-0.3.2/tests/test_image.py
+drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-05-21 16:39:11.978075 pynavio-0.3.2/tests/test_pynavio/
+-rw-r--r--   0 clarareolid   (501) staff       (20)    53248 2024-04-09 15:32:59.000000 pynavio-0.3.2/tests/test_pynavio/.coverage
+drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-05-21 16:39:11.959733 pynavio-0.3.2/tests/test_pynavio/fixtures/
+drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-05-21 16:39:11.979177 pynavio-0.3.2/tests/test_pynavio/fixtures/Images/
+-rw-r--r--   0 clarareolid   (501) staff       (20)    65764 2024-05-21 15:57:40.000000 pynavio-0.3.2/tests/test_pynavio/fixtures/Images/num_img.jpeg
+-rw-r--r--   0 clarareolid   (501) staff       (20)    23752 2024-05-21 12:17:52.000000 pynavio-0.3.2/tests/test_pynavio/fixtures/Images/num_img_out.jpeg
+drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-05-21 16:39:11.979984 pynavio-0.3.2/tests/test_pynavio/fixtures/schemas/
+-rw-r--r--   0 clarareolid   (501) staff       (20)      984 2024-01-22 11:10:05.000000 pynavio-0.3.2/tests/test_pynavio/fixtures/schemas/example_request.json
+-rw-r--r--   0 clarareolid   (501) staff       (20)      987 2024-01-22 11:10:05.000000 pynavio-0.3.2/tests/test_pynavio/fixtures/schemas/example_request_nested.json
+drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-05-21 16:39:11.980339 pynavio-0.3.2/tests/test_pynavio/python-test-reports/
+-rw-r--r--   0 clarareolid   (501) staff       (20)      221 2024-04-09 15:32:59.000000 pynavio-0.3.2/tests/test_pynavio/python-test-reports/pynavio.xml
+-rw-r--r--   0 clarareolid   (501) staff       (20)     6615 2024-01-22 11:10:05.000000 pynavio-0.3.2/tests/test_pynavio/test_client.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)     2145 2023-10-31 13:03:40.000000 pynavio-0.3.2/tests/test_pynavio/test_dependencies.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)      905 2024-05-21 09:46:42.000000 pynavio-0.3.2/tests/test_pynavio/test_dependencies_file_only.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)    10027 2024-05-21 15:57:40.000000 pynavio-0.3.2/tests/test_pynavio/test_mlflow.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)     3424 2023-10-31 13:03:40.000000 pynavio-0.3.2/tests/test_pynavio/test_schema.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)      709 2024-05-21 15:57:40.000000 pynavio-0.3.2/tests/test_pynavio/test_traits.py
+drwxr-xr-x   0 clarareolid   (501) staff       (20)        0 2024-05-21 16:39:11.981048 pynavio-0.3.2/tests/test_pynavio/test_utils/
+-rw-r--r--   0 clarareolid   (501) staff       (20)     1949 2024-03-05 13:08:36.000000 pynavio-0.3.2/tests/test_pynavio/test_utils/test_conda.py
+-rw-r--r--   0 clarareolid   (501) staff       (20)     1712 2023-11-20 14:24:52.000000 pynavio-0.3.2/tests/test_pynavio/test_utils/test_conda.py.orig
```

### Comparing `pynavio-0.3.1/HISTORY.rst` & `pynavio-0.3.2/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -123,7 +123,12 @@
 * adds possibility to add extra pip dependencies to the inferred environment
 
 0.3.1 (2024-01-23)
 ------------------
 
 * minor reformatting fix
 
+0.3.2 (2024-05-21)
+------------------
+
+* bump Pillow from 9.3.0 to >=8.0.0, <11.0.0
+* bump plotly from 5.9.0 to >=4.10.0, <6.0.0
```

### Comparing `pynavio-0.3.1/LICENSE` & `pynavio-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/PKG-INFO` & `pynavio-0.3.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynavio
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python lib for navio
 Home-page: https://github.com/craftworksgmbh/craftworks-pynavio
 Author: craftworks
 Author-email: dev-accounts@craftworks.at
 License: MIT license
 Keywords: pynavio
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,19 +14,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: mlflow>=1.20.1
-Requires-Dist: Pillow==9.3.0
-Requires-Dist: plotly==5.9.0
-Requires-Dist: pigar==0.10.0
+Requires-Dist: mlflow!=1.27.*,!=1.28.*,>=1.20.1
+Requires-Dist: Pillow<11.0.0,>=8.0.0
+Requires-Dist: plotly<6.0.0,>=4.10.0
 Requires-Dist: jsonschema>=3.2.0
+Requires-Dist: pigar==0.10.0
 
 =========
 pynavio
 =========
 
 
 .. image:: https://img.shields.io/pypi/v/pynavio.svg
@@ -207,7 +207,12 @@
 * adds possibility to add extra pip dependencies to the inferred environment
 
 0.3.1 (2024-01-23)
 ------------------
 
 * minor reformatting fix
 
+0.3.2 (2024-05-21)
+------------------
+
+* bump Pillow from 9.3.0 to >=8.0.0, <11.0.0
+* bump plotly from 5.9.0 to >=4.10.0, <6.0.0
```

### Comparing `pynavio-0.3.1/README.rst` & `pynavio-0.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/docs/Makefile` & `pynavio-0.3.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/docs/conf.py` & `pynavio-0.3.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/docs/installation.rst` & `pynavio-0.3.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/docs/make.bat` & `pynavio-0.3.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/pynavio/__init__.py` & `pynavio-0.3.2/pynavio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for pynavio."""
 
 __author__ = """craftworks"""
 __email__ = 'dev-accounts@craftworks.at'
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 
 from . import _code as code
 from . import _mlflow as mlflow
 from . import dependencies, image, model_helpers, schema, traits, utils
 from ._code import infer_imported_code_path
 from .dependencies import infer_external_dependencies
 from .model_helpers import assert_gpu_available, prediction_call
```

### Comparing `pynavio-0.3.1/pynavio/_code.py` & `pynavio-0.3.2/pynavio/_code.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/pynavio/_mlflow.py` & `pynavio-0.3.2/pynavio/_mlflow.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/pynavio/client.py` & `pynavio-0.3.2/pynavio/client.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/pynavio/dependencies.py` & `pynavio-0.3.2/pynavio/dependencies.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/pynavio/image.py` & `pynavio-0.3.2/pynavio/image.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/pynavio/model_helpers.py` & `pynavio-0.3.2/pynavio/model_helpers.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/pynavio/schema.py` & `pynavio-0.3.2/pynavio/schema.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/pynavio/traits.py` & `pynavio-0.3.2/pynavio/traits.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/pynavio/utils/common.py` & `pynavio-0.3.2/pynavio/utils/common.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/pynavio/utils/conda.py` & `pynavio-0.3.2/pynavio/utils/conda.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/pynavio/utils/schemas.py` & `pynavio-0.3.2/pynavio/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/pynavio.egg-info/PKG-INFO` & `pynavio-0.3.2/pynavio.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynavio
-Version: 0.3.1
+Version: 0.3.2
 Summary: Python lib for navio
 Home-page: https://github.com/craftworksgmbh/craftworks-pynavio
 Author: craftworks
 Author-email: dev-accounts@craftworks.at
 License: MIT license
 Keywords: pynavio
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,19 +14,19 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: mlflow>=1.20.1
-Requires-Dist: Pillow==9.3.0
-Requires-Dist: plotly==5.9.0
-Requires-Dist: pigar==0.10.0
+Requires-Dist: mlflow!=1.27.*,!=1.28.*,>=1.20.1
+Requires-Dist: Pillow<11.0.0,>=8.0.0
+Requires-Dist: plotly<6.0.0,>=4.10.0
 Requires-Dist: jsonschema>=3.2.0
+Requires-Dist: pigar==0.10.0
 
 =========
 pynavio
 =========
 
 
 .. image:: https://img.shields.io/pypi/v/pynavio.svg
@@ -207,7 +207,12 @@
 * adds possibility to add extra pip dependencies to the inferred environment
 
 0.3.1 (2024-01-23)
 ------------------
 
 * minor reformatting fix
 
+0.3.2 (2024-05-21)
+------------------
+
+* bump Pillow from 9.3.0 to >=8.0.0, <11.0.0
+* bump plotly from 5.9.0 to >=4.10.0, <6.0.0
```

### Comparing `pynavio-0.3.1/pynavio.egg-info/SOURCES.txt` & `pynavio-0.3.2/pynavio.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 AUTHORS.rst
 HISTORY.rst
 LICENSE
 MANIFEST.in
 README.rst
+requirements.txt
+requirements_dev.txt
 setup.cfg
 setup.py
 docs/Makefile
 docs/authors.rst
 docs/conf.py
 docs/contributing.rst
 docs/history.rst
@@ -34,16 +36,22 @@
 pynavio/utils/common.py
 pynavio/utils/conda.py
 pynavio/utils/json_encoder.py
 pynavio/utils/schemas.py
 pynavio/utils/styling.py
 tests/__init__.py
 tests/conftest.py
+tests/test_image.py
+tests/test_pynavio/.coverage
 tests/test_pynavio/test_client.py
 tests/test_pynavio/test_dependencies.py
 tests/test_pynavio/test_dependencies_file_only.py
 tests/test_pynavio/test_mlflow.py
 tests/test_pynavio/test_schema.py
+tests/test_pynavio/test_traits.py
+tests/test_pynavio/fixtures/Images/num_img.jpeg
+tests/test_pynavio/fixtures/Images/num_img_out.jpeg
 tests/test_pynavio/fixtures/schemas/example_request.json
 tests/test_pynavio/fixtures/schemas/example_request_nested.json
+tests/test_pynavio/python-test-reports/pynavio.xml
 tests/test_pynavio/test_utils/test_conda.py
 tests/test_pynavio/test_utils/test_conda.py.orig
```

### Comparing `pynavio-0.3.1/setup.py` & `pynavio-0.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,11 +36,11 @@
     include_package_data=True,
     keywords='pynavio',
     name='pynavio',
     packages=find_packages(include=['pynavio', 'pynavio.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/craftworksgmbh/craftworks-pynavio',
-    version='0.3.1',
+    version='0.3.2',
     zip_safe=False,
 
 )
```

### Comparing `pynavio-0.3.1/tests/test_pynavio/fixtures/schemas/example_request.json` & `pynavio-0.3.2/tests/test_pynavio/fixtures/schemas/example_request.json`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/tests/test_pynavio/fixtures/schemas/example_request_nested.json` & `pynavio-0.3.2/tests/test_pynavio/fixtures/schemas/example_request_nested.json`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/tests/test_pynavio/test_client.py` & `pynavio-0.3.2/tests/test_pynavio/test_client.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/tests/test_pynavio/test_dependencies.py` & `pynavio-0.3.2/tests/test_pynavio/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/tests/test_pynavio/test_dependencies_file_only.py` & `pynavio-0.3.2/tests/test_pynavio/test_dependencies_file_only.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/tests/test_pynavio/test_mlflow.py` & `pynavio-0.3.2/tests/test_pynavio/test_mlflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -182,27 +182,54 @@
 
     assert pynavio.mlflow._is_wrapped_by_prediction_call(wrapped_predict) \
            is True
     assert pynavio.mlflow._is_wrapped_by_prediction_call(predict) is False
 
 
 def test_is_model_predict_wrapped_by_prediction_call(tmp_path):
+
+    from pathlib import Path
+    from tempfile import TemporaryDirectory
     import mlflow
 
-    from examples import mlflow_models
-    from examples.mlflow_models import tabular
+    import pynavio
+
+    TARGET = 'target'
+    _columns = ['x', 'y']
+    example_request = pynavio.make_example_request(
+        {
+            TARGET: float(sum(range(len(_columns)))),
+            **{col: float(i) for i, col in enumerate(_columns)}
+        },
+        target=TARGET)
+
+    class SampleModel(mlflow.pyfunc.PythonModel):
+
+        @pynavio.prediction_call
+        def predict(self, context, model_input):
+            return {
+                'prediction': [1.] * model_input.shape[0]
+            }
+
+    def setup(path: Path, *args, **kwargs):
+        with TemporaryDirectory():
+            pynavio.mlflow.to_navio(SampleModel(),
+                                    example_request=example_request,
+                                    code_path=kwargs.get('code_path'),
+                                    path=path,
+                                    pip_packages=['mlflow'])
+
     model_path = str(tmp_path / 'model')
 
     setup_arguments = dict(with_data=False,
                            with_oodd=False,
                            explanations=None,
-                           path=model_path,
-                           code_path=[mlflow_models.__path__[0]])
+                           path=model_path)
 
-    tabular.setup(**setup_arguments)
+    setup(**setup_arguments)
 
     model = mlflow.pyfunc.load_model(model_path)
     try:
         pynavio.mlflow._is_model_predict_wrapped_by_prediction_call(model)
     except AttributeError:
         raise pytest.fail(
             "did raise AttributeError, therefore currently prediction call"
```

### Comparing `pynavio-0.3.1/tests/test_pynavio/test_schema.py` & `pynavio-0.3.2/tests/test_pynavio/test_schema.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/tests/test_pynavio/test_utils/test_conda.py` & `pynavio-0.3.2/tests/test_pynavio/test_utils/test_conda.py`

 * *Files identical despite different names*

### Comparing `pynavio-0.3.1/tests/test_pynavio/test_utils/test_conda.py.orig` & `pynavio-0.3.2/tests/test_pynavio/test_utils/test_conda.py.orig`

 * *Files identical despite different names*

