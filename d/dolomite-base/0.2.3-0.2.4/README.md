# Comparing `tmp/dolomite_base-0.2.3.tar.gz` & `tmp/dolomite_base-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolomite_base-0.2.3.tar", last modified: Mon May 20 22:59:43 2024, max compression
+gzip compressed data, was "dolomite_base-0.2.4.tar", last modified: Tue May 21 19:44:22 2024, max compression
```

## Comparing `dolomite_base-0.2.3.tar` & `dolomite_base-0.2.4.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:59:43.010438 dolomite_base-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:59:42.998438 dolomite_base-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:59:43.002438 dolomite_base-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/.github/workflows/build-docs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/.github/workflows/publish-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/.github/workflows/run-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    20827 2024-05-20 22:59:43.010438 dolomite_base-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19884 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:59:43.002438 dolomite_base-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:59:43.002438 dolomite_base-0.2.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:59:43.002438 dolomite_base-0.2.3/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/lib/CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:59:43.002438 dolomite_base-0.2.3/lib/src/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/lib/src/init.cpp
--rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/lib/src/load_list.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/lib/src/utils.h
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/lib/src/validate.cpp
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-20 22:59:43.010438 dolomite_base-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:59:42.998438 dolomite_base-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:59:43.006438 dolomite_base-0.2.3/src/dolomite_base/
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/_utils_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/_utils_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/_utils_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/alt_read_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/alt_save_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/choose_missing_placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/load_vector_from_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/read_atomic_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/read_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     3028 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/read_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/read_object_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/read_simple_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/read_string_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/save_atomic_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/save_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2521 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/save_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/save_object_file.py
--rw-r--r--   0 runner    (1001) docker     (127)    15410 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/save_simple_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/save_string_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/validate_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/src/dolomite_base/write_vector_to_hdf5.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:59:43.010438 dolomite_base-0.2.3/src/dolomite_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20827 2024-05-20 22:59:42.000000 dolomite_base-0.2.3/src/dolomite_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-20 22:59:42.000000 dolomite_base-0.2.3/src/dolomite_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:59:42.000000 dolomite_base-0.2.3/src/dolomite_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:59:42.000000 dolomite_base-0.2.3/src/dolomite_base.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-20 22:59:42.000000 dolomite_base-0.2.3/src/dolomite_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 22:59:42.000000 dolomite_base-0.2.3/src/dolomite_base.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:59:43.010438 dolomite_base-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/tests/test_atomic_vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/tests/test_choose_missing_placeholder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/tests/test_data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/tests/test_load_vector_from_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/tests/test_read_object.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/tests/test_save_object.py
--rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/tests/test_simple_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/tests/test_string_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/tests/test_validate_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/tests/test_write_vector_to_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-20 22:59:36.000000 dolomite_base-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:44:22.251935 dolomite_base-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:44:22.239935 dolomite_base-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:44:22.243935 dolomite_base-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/.github/workflows/build-docs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/.github/workflows/publish-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/.github/workflows/run-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13555 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    20814 2024-05-21 19:44:22.251935 dolomite_base-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19884 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:44:22.243935 dolomite_base-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:44:22.243935 dolomite_base-0.2.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10423 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:44:22.243935 dolomite_base-0.2.4/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/lib/CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:44:22.243935 dolomite_base-0.2.4/lib/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/lib/src/init.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)     7830 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/lib/src/load_list.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/lib/src/utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/lib/src/validate.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-05-21 19:44:22.255935 dolomite_base-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:44:22.239935 dolomite_base-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:44:22.247935 dolomite_base-0.2.4/src/dolomite_base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/_utils_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/_utils_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/_utils_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/alt_read_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/alt_save_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/choose_missing_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/load_vector_from_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/read_atomic_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/read_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/read_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/read_object_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/read_simple_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/read_string_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4643 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/save_atomic_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/save_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/save_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/save_object_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15410 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/save_simple_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/save_string_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/validate_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/src/dolomite_base/write_vector_to_hdf5.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:44:22.251935 dolomite_base-0.2.4/src/dolomite_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20814 2024-05-21 19:44:22.000000 dolomite_base-0.2.4/src/dolomite_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-21 19:44:22.000000 dolomite_base-0.2.4/src/dolomite_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:44:22.000000 dolomite_base-0.2.4/src/dolomite_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:44:22.000000 dolomite_base-0.2.4/src/dolomite_base.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-21 19:44:22.000000 dolomite_base-0.2.4/src/dolomite_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 19:44:22.000000 dolomite_base-0.2.4/src/dolomite_base.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:44:22.251935 dolomite_base-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/tests/test_atomic_vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4712 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/tests/test_choose_missing_placeholder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14189 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/tests/test_data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6903 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/tests/test_load_vector_from_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/tests/test_read_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/tests/test_save_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11403 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/tests/test_simple_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/tests/test_string_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/tests/test_validate_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5987 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/tests/test_write_vector_to_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-05-21 19:44:15.000000 dolomite_base-0.2.4/tox.ini
```

### Comparing `dolomite_base-0.2.3/.coveragerc` & `dolomite_base-0.2.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/.github/workflows/build-docs.yml` & `dolomite_base-0.2.4/.github/workflows/build-docs.yml`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/.github/workflows/publish-pypi.yml` & `dolomite_base-0.2.4/.github/workflows/publish-pypi.yml`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/.github/workflows/run-tests.yml` & `dolomite_base-0.2.4/.github/workflows/run-tests.yml`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/.gitignore` & `dolomite_base-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/.readthedocs.yml` & `dolomite_base-0.2.4/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/CONTRIBUTING.md` & `dolomite_base-0.2.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/LICENSE.txt` & `dolomite_base-0.2.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/PKG-INFO` & `dolomite_base-0.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: dolomite-base
-Version: 0.2.3
+Version: 0.2.4
 Summary: Save and load Bioconductor objects in Python
 Home-page: https://github.com/ArtifactDB/dolomite-base
 Author: Aaron Lun
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/dolomite-base
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: biocutils<0.2.0,>=0.1.5
-Requires-Dist: biocframe<0.6.0,>=0.5.7
+Requires-Dist: biocutils>=0.1.5
+Requires-Dist: biocframe>=0.5.10
 Requires-Dist: numpy
 Requires-Dist: jsonschema
-Requires-Dist: dolomite-schemas>=0.0.7
+Requires-Dist: dolomite-schemas>=0.0.8
 Requires-Dist: h5py
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 <!-- These are examples of badges you might want to add to your README:
```

### Comparing `dolomite_base-0.2.3/README.md` & `dolomite_base-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/docs/Makefile` & `dolomite_base-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/docs/conf.py` & `dolomite_base-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/docs/index.md` & `dolomite_base-0.2.4/docs/index.md`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/lib/CMakeLists.txt` & `dolomite_base-0.2.4/lib/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/lib/src/load_list.cpp` & `dolomite_base-0.2.4/lib/src/load_list.cpp`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/lib/src/utils.h` & `dolomite_base-0.2.4/lib/src/utils.h`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/lib/src/validate.cpp` & `dolomite_base-0.2.4/lib/src/validate.cpp`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/setup.cfg` & `dolomite_base-0.2.4/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -20,19 +20,19 @@
 packages = find_namespace:
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.8
 install_requires = 
 	importlib-metadata; python_version<"3.8"
-	biocutils>=0.1.5,<0.2.0
-	biocframe>=0.5.7,<0.6.0
+	biocutils>=0.1.5
+	biocframe>=0.5.10
 	numpy
 	jsonschema
-	dolomite-schemas>=0.0.7
+	dolomite-schemas>=0.0.8
 	h5py
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `dolomite_base-0.2.3/setup.py` & `dolomite_base-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/__init__.py` & `dolomite_base-0.2.4/src/dolomite_base/__init__.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/_utils_factor.py` & `dolomite_base-0.2.4/src/dolomite_base/_utils_factor.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/_utils_misc.py` & `dolomite_base-0.2.4/src/dolomite_base/_utils_misc.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/_utils_string.py` & `dolomite_base-0.2.4/src/dolomite_base/_utils_string.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/alt_read_object.py` & `dolomite_base-0.2.4/src/dolomite_base/alt_read_object.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/alt_save_object.py` & `dolomite_base-0.2.4/src/dolomite_base/alt_save_object.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/choose_missing_placeholder.py` & `dolomite_base-0.2.4/src/dolomite_base/choose_missing_placeholder.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/load_vector_from_hdf5.py` & `dolomite_base-0.2.4/src/dolomite_base/load_vector_from_hdf5.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/read_atomic_vector.py` & `dolomite_base-0.2.4/src/dolomite_base/read_atomic_vector.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/read_data_frame.py` & `dolomite_base-0.2.4/src/dolomite_base/read_data_frame.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/read_object.py` & `dolomite_base-0.2.4/src/dolomite_base/read_object.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,22 +4,27 @@
 
 
 read_object_registry = {
     "atomic_vector": "dolomite_base.read_atomic_vector",
     "string_factor": "dolomite_base.read_string_factor",
     "simple_list": "dolomite_base.read_simple_list",
     "data_frame": "dolomite_base.read_data_frame",
+
     "dense_array": "dolomite_matrix.read_dense_array",
     "compressed_sparse_matrix": "dolomite_matrix.read_compressed_sparse_matrix",
+    
     "genomic_ranges": "dolomite_ranges.read_genomic_ranges",
     "genomic_ranges_list": "dolomite_ranges.read_genomic_ranges_list",
     "sequence_information": "dolomite_ranges.read_sequence_information",
+    
     "summarized_experiment": "dolomite_se.read_summarized_experiment",
     "range_summarized_experiment": "dolomite_se.read_ranged_summarized_experiment",
+    
     "single_cell_experiment": "dolomite_sce.read_single_cell_experiment",
+    
     "multi_sample_dataset": "dolomite_mae.read_multi_assay_experiment",
 }
 
 
 def read_object(path: str, metadata: Optional[dict] = None, **kwargs) -> Any:
     """
     Read an object from its on-disk representation. This will dispatch to
```

### Comparing `dolomite_base-0.2.3/src/dolomite_base/read_object_file.py` & `dolomite_base-0.2.4/src/dolomite_base/read_object_file.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/read_simple_list.py` & `dolomite_base-0.2.4/src/dolomite_base/read_simple_list.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/read_string_factor.py` & `dolomite_base-0.2.4/src/dolomite_base/read_string_factor.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/save_atomic_vector.py` & `dolomite_base-0.2.4/src/dolomite_base/save_atomic_vector.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/save_data_frame.py` & `dolomite_base-0.2.4/src/dolomite_base/save_data_frame.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/save_object.py` & `dolomite_base-0.2.4/src/dolomite_base/save_object.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,20 @@
     "SeqInfo": "dolomite_ranges",
 
     "ndarray": "dolomite_matrix",
     "csc_matrix": "dolomite_matrix",
     "csr_matrix": "dolomite_matrix",
     "coo_matrix": "dolomite_matrix",
     "DelayedArray": "dolomite_matrix",
+
+    "SummarizedExperiment": "dolomite_se",
+    "RangedSummarizedExperiment": "dolomite_se",
+
+    "SingleCellExperiment": "dolomite_sce",
+    "MultiAssayExperiment": "dolomite_mae"
 }
 
 
 @singledispatch
 def save_object(x: Any, path: str, **kwargs):
     """
     Save an object to its on-disk representation. **dolomite** extensions
```

### Comparing `dolomite_base-0.2.3/src/dolomite_base/save_object_file.py` & `dolomite_base-0.2.4/src/dolomite_base/save_object_file.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/save_simple_list.py` & `dolomite_base-0.2.4/src/dolomite_base/save_simple_list.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/save_string_factor.py` & `dolomite_base-0.2.4/src/dolomite_base/save_string_factor.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/validate_object.py` & `dolomite_base-0.2.4/src/dolomite_base/validate_object.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base/write_vector_to_hdf5.py` & `dolomite_base-0.2.4/src/dolomite_base/write_vector_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/src/dolomite_base.egg-info/PKG-INFO` & `dolomite_base-0.2.4/src/dolomite_base.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: dolomite-base
-Version: 0.2.3
+Version: 0.2.4
 Summary: Save and load Bioconductor objects in Python
 Home-page: https://github.com/ArtifactDB/dolomite-base
 Author: Aaron Lun
 Author-email: infinite.monkeys.with.keyboards@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/ArtifactDB/dolomite-base
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
-Requires-Dist: biocutils<0.2.0,>=0.1.5
-Requires-Dist: biocframe<0.6.0,>=0.5.7
+Requires-Dist: biocutils>=0.1.5
+Requires-Dist: biocframe>=0.5.10
 Requires-Dist: numpy
 Requires-Dist: jsonschema
-Requires-Dist: dolomite-schemas>=0.0.7
+Requires-Dist: dolomite-schemas>=0.0.8
 Requires-Dist: h5py
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 
 <!-- These are examples of badges you might want to add to your README:
```

### Comparing `dolomite_base-0.2.3/src/dolomite_base.egg-info/SOURCES.txt` & `dolomite_base-0.2.4/src/dolomite_base.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/tests/test_atomic_vector.py` & `dolomite_base-0.2.4/tests/test_atomic_vector.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/tests/test_choose_missing_placeholder.py` & `dolomite_base-0.2.4/tests/test_choose_missing_placeholder.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/tests/test_data_frame.py` & `dolomite_base-0.2.4/tests/test_data_frame.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/tests/test_load_vector_from_hdf5.py` & `dolomite_base-0.2.4/tests/test_load_vector_from_hdf5.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/tests/test_read_object.py` & `dolomite_base-0.2.4/tests/test_read_object.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/tests/test_save_object.py` & `dolomite_base-0.2.4/tests/test_save_object.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/tests/test_simple_list.py` & `dolomite_base-0.2.4/tests/test_simple_list.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/tests/test_string_factor.py` & `dolomite_base-0.2.4/tests/test_string_factor.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/tests/test_validate_object.py` & `dolomite_base-0.2.4/tests/test_validate_object.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/tests/test_write_vector_to_hdf5.py` & `dolomite_base-0.2.4/tests/test_write_vector_to_hdf5.py`

 * *Files identical despite different names*

### Comparing `dolomite_base-0.2.3/tox.ini` & `dolomite_base-0.2.4/tox.ini`

 * *Files identical despite different names*

