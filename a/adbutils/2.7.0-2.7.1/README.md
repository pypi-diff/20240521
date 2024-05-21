# Comparing `tmp/adbutils-2.7.0.tar.gz` & `tmp/adbutils-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbutils-2.7.0.tar", last modified: Mon May 20 10:16:27 2024, max compression
+gzip compressed data, was "adbutils-2.7.1.tar", last modified: Tue May 21 03:49:20 2024, max compression
```

## Comparing `adbutils-2.7.0.tar` & `adbutils-2.7.1.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-20 10:16:21.000000 adbutils-2.7.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.136951 adbutils-2.7.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-20 10:16:21.000000 adbutils-2.7.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.136951 adbutils-2.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-20 10:16:21.000000 adbutils-2.7.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-20 10:16:21.000000 adbutils-2.7.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-20 10:16:21.000000 adbutils-2.7.0/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-20 10:16:27.000000 adbutils-2.7.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-20 10:16:27.000000 adbutils-2.7.0/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-20 10:16:21.000000 adbutils-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-20 10:16:27.140951 adbutils-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-05-20 10:16:21.000000 adbutils-2.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/adbutils/
--rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)    16918 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/adbutils/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/binaries/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/binaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/pidcat.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/screenrecord.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/screenshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    19829 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-05-20 10:16:21.000000 adbutils-2.7.0/adbutils/sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/adbutils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 10:16:27.000000 adbutils-2.7.0/adbutils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.136951 adbutils-2.7.0/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-05-20 10:16:21.000000 adbutils-2.7.0/assets/images/pidcat.png
--rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-05-20 10:16:21.000000 adbutils-2.7.0/build_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 10:16:21.000000 adbutils-2.7.0/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-20 10:16:21.000000 adbutils-2.7.0/docs/PROTOCOL.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-20 10:16:21.000000 adbutils-2.7.0/examples/reset-offline.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-20 10:16:21.000000 adbutils-2.7.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-20 10:16:21.000000 adbutils-2.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-20 10:16:27.144951 adbutils-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-20 10:16:21.000000 adbutils-2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/test_real_device/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_forward_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-20 10:16:21.000000 adbutils-2.7.0/test_real_device/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:16:27.140951 adbutils-2.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-20 10:16:21.000000 adbutils-2.7.0/tests/adb_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-20 10:16:21.000000 adbutils-2.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-20 10:16:21.000000 adbutils-2.7.0/tests/test_adb_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-20 10:16:21.000000 adbutils-2.7.0/tests/test_adb_shell.py
--rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-20 10:16:21.000000 adbutils-2.7.0/tests/test_forward.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:49:20.928032 adbutils-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-21 03:49:14.000000 adbutils-2.7.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:49:20.924032 adbutils-2.7.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-21 03:49:14.000000 adbutils-2.7.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:49:20.924032 adbutils-2.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-21 03:49:14.000000 adbutils-2.7.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-21 03:49:14.000000 adbutils-2.7.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-21 03:49:14.000000 adbutils-2.7.1/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-21 03:49:20.000000 adbutils-2.7.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-21 03:49:20.000000 adbutils-2.7.1/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-21 03:49:14.000000 adbutils-2.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-21 03:49:20.928032 adbutils-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15478 2024-05-21 03:49:14.000000 adbutils-2.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:49:20.924032 adbutils-2.7.1/adbutils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3388 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11923 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12835 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16918 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8433 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:49:20.924032 adbutils-2.7.1/adbutils/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/binaries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/binaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5587 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12853 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/pidcat.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     8931 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/screenrecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/screenshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19748 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8962 2024-05-21 03:49:14.000000 adbutils-2.7.1/adbutils/sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:49:20.924032 adbutils-2.7.1/adbutils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-21 03:49:20.000000 adbutils-2.7.1/adbutils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-21 03:49:20.000000 adbutils-2.7.1/adbutils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 03:49:20.000000 adbutils-2.7.1/adbutils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 03:49:20.000000 adbutils-2.7.1/adbutils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 03:49:20.000000 adbutils-2.7.1/adbutils.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 03:49:20.000000 adbutils-2.7.1/adbutils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 03:49:20.000000 adbutils-2.7.1/adbutils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:49:20.920032 adbutils-2.7.1/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:49:20.928032 adbutils-2.7.1/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   127305 2024-05-21 03:49:14.000000 adbutils-2.7.1/assets/images/pidcat.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6132 2024-05-21 03:49:14.000000 adbutils-2.7.1/build_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-21 03:49:14.000000 adbutils-2.7.1/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:49:20.928032 adbutils-2.7.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3153 2024-05-21 03:49:14.000000 adbutils-2.7.1/docs/PROTOCOL.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:49:20.928032 adbutils-2.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-21 03:49:14.000000 adbutils-2.7.1/examples/reset-offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-21 03:49:14.000000 adbutils-2.7.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 03:49:14.000000 adbutils-2.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-21 03:49:20.928032 adbutils-2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-21 03:49:14.000000 adbutils-2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:49:20.928032 adbutils-2.7.1/test_real_device/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-21 03:49:14.000000 adbutils-2.7.1/test_real_device/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-21 03:49:14.000000 adbutils-2.7.1/test_real_device/test_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-21 03:49:14.000000 adbutils-2.7.1/test_real_device/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9601 2024-05-21 03:49:14.000000 adbutils-2.7.1/test_real_device/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-21 03:49:14.000000 adbutils-2.7.1/test_real_device/test_forward_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-21 03:49:14.000000 adbutils-2.7.1/test_real_device/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-21 03:49:14.000000 adbutils-2.7.1/test_real_device/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-21 03:49:14.000000 adbutils-2.7.1/test_real_device/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:49:20.928032 adbutils-2.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-21 03:49:14.000000 adbutils-2.7.1/tests/adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-21 03:49:14.000000 adbutils-2.7.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-21 03:49:14.000000 adbutils-2.7.1/tests/test_adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2403 2024-05-21 03:49:14.000000 adbutils-2.7.1/tests/test_adb_shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-05-21 03:49:14.000000 adbutils-2.7.1/tests/test_forward.py
```

### Comparing `adbutils-2.7.0/.coveragerc` & `adbutils-2.7.1/.coveragerc`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/.github/workflows/main.yml` & `adbutils-2.7.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/.github/workflows/publish-to-pypi.yml` & `adbutils-2.7.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/.travis.yml` & `adbutils-2.7.1/.travis.yml`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/LICENSE` & `adbutils-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/PKG-INFO` & `adbutils-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.7.0
+Version: 2.7.1
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.7.0/README.md` & `adbutils-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils/__init__.py` & `adbutils-2.7.1/adbutils/__init__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils/__main__.py` & `adbutils-2.7.1/adbutils/__main__.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils/_adb.py` & `adbutils-2.7.1/adbutils/_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils/_deprecated.py` & `adbutils-2.7.1/adbutils/_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils/_device.py` & `adbutils-2.7.1/adbutils/_device.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils/_proto.py` & `adbutils-2.7.1/adbutils/_proto.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils/_utils.py` & `adbutils-2.7.1/adbutils/_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils/errors.py` & `adbutils-2.7.1/adbutils/errors.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils/install.py` & `adbutils-2.7.1/adbutils/install.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils/pidcat.py` & `adbutils-2.7.1/adbutils/pidcat.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils/screenrecord.py` & `adbutils-2.7.1/adbutils/screenrecord.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils/screenshot.py` & `adbutils-2.7.1/adbutils/screenshot.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils/shell.py` & `adbutils-2.7.1/adbutils/shell.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,33 +160,30 @@
 
         Returns:
             WindowSize
         
         Raises:
             AdbError
         """
-        try:
-            logger.debug("get window size from 'dumpsys display'")
-            return self._dumpsys_window_size()
-        except AdbError:
-            logger.debug("get window size from 'wm size'")
-            wsize = self._wm_size()
-            horizontal = self.rotation() % 2 == 1
-            return WindowSize(wsize.height, wsize.width) if horizontal else wsize
+        wsize = self._wm_size()
+        horizontal = self.rotation() % 2 == 1
+        logger.debug("get window size from 'wm size'", wsize, horizontal)
+        return WindowSize(wsize.height, wsize.width) if horizontal else wsize
     
-    def _dumpsys_window_size(self) -> WindowSize:
-        output = self.shell("dumpsys display")
-        for line in output.splitlines():
-            m = _DISPLAY_RE.search(line, 0)
-            if not m:
-                continue
-            w = int(m.group("width"))
-            h = int(m.group("height"))
-            return WindowSize(w, h)
-        raise AdbError("get window size from 'dumpsys display' failed", output)
+    # the ", deviceHeight=xxx}]" is not correct
+    # def _dumpsys_window_size(self) -> WindowSize:
+    #     output = self.shell("dumpsys display")
+    #     for line in output.splitlines():
+    #         m = _DISPLAY_RE.search(line, 0)
+    #         if not m:
+    #             continue
+    #         w = int(m.group("width"))
+    #         h = int(m.group("height"))
+    #         return WindowSize(w, h)
+    #     raise AdbError("get window size from 'dumpsys display' failed", output)
     
     def _wm_size(self) -> WindowSize:
         output = self.shell("wm size")
         o = re.search(r"Override size: (\d+)x(\d+)", output)
         if o:
             w, h = o.group(1), o.group(2)
             return WindowSize(int(w), int(h))
```

### Comparing `adbutils-2.7.0/adbutils/sync.py` & `adbutils-2.7.1/adbutils/sync.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/adbutils.egg-info/PKG-INFO` & `adbutils-2.7.1/adbutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adbutils
-Version: 2.7.0
+Version: 2.7.1
 Summary: Pure Python Adb Library
 Home-page: https://github.com/openatx/adbutils
 Author: codeskyblue
 Author-email: codeskyblue@gmail.com
 License: MIT
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `adbutils-2.7.0/adbutils.egg-info/SOURCES.txt` & `adbutils-2.7.1/adbutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/assets/images/pidcat.png` & `adbutils-2.7.1/assets/images/pidcat.png`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/build_wheel.py` & `adbutils-2.7.1/build_wheel.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/docs/PROTOCOL.md` & `adbutils-2.7.1/docs/PROTOCOL.md`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/examples/reset-offline.py` & `adbutils-2.7.1/examples/reset-offline.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/setup.cfg` & `adbutils-2.7.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/test_real_device/conftest.py` & `adbutils-2.7.1/test_real_device/conftest.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/test_real_device/test_adb.py` & `adbutils-2.7.1/test_real_device/test_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/test_real_device/test_deprecated.py` & `adbutils-2.7.1/test_real_device/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/test_real_device/test_device.py` & `adbutils-2.7.1/test_real_device/test_device.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/test_real_device/test_forward_reverse.py` & `adbutils-2.7.1/test_real_device/test_forward_reverse.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/test_real_device/test_utils.py` & `adbutils-2.7.1/test_real_device/test_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/tests/adb_server.py` & `adbutils-2.7.1/tests/adb_server.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/tests/conftest.py` & `adbutils-2.7.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/tests/test_adb_server.py` & `adbutils-2.7.1/tests/test_adb_server.py`

 * *Files identical despite different names*

### Comparing `adbutils-2.7.0/tests/test_adb_shell.py` & `adbutils-2.7.1/tests/test_adb_shell.py`

 * *Files identical despite different names*
