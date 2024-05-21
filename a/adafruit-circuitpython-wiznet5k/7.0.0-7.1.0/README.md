# Comparing `tmp/adafruit_circuitpython_wiznet5k-7.0.0.tar.gz` & `tmp/adafruit_circuitpython_wiznet5k-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_wiznet5k-7.0.0.tar", last modified: Tue Apr 30 15:57:36 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_wiznet5k-7.1.0.tar", last modified: Tue May 21 16:18:29 2024, max compression
```

## Comparing `adafruit_circuitpython_wiznet5k-7.0.0.tar` & `adafruit_circuitpython_wiznet5k-7.1.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.893717 adafruit_circuitpython_wiznet5k-7.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.897717 adafruit_circuitpython_wiznet5k-7.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.897717 adafruit_circuitpython_wiznet5k-7.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.897717 adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-04-30 15:57:36.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-30 15:57:36.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 15:57:36.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-30 15:57:36.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 15:57:36.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51779 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    26273 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)    31487 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socketpool.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_aio_post.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2159 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_cheerlights.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1085 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_httpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_simpleserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_simpletest_manual_network.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-04-30 15:57:34.000000 adafruit_circuitpython_wiznet5k-7.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-30 15:57:28.000000 adafruit_circuitpython_wiznet5k-7.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 15:57:36.901717 adafruit_circuitpython_wiznet5k-7.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:18:29.319536 adafruit_circuitpython_wiznet5k-7.1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:18:29.311536 adafruit_circuitpython_wiznet5k-7.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:18:29.315536 adafruit_circuitpython_wiznet5k-7.1.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:18:29.315536 adafruit_circuitpython_wiznet5k-7.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:18:29.315536 adafruit_circuitpython_wiznet5k-7.1.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-21 16:18:29.319536 adafruit_circuitpython_wiznet5k-7.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4592 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:18:29.319536 adafruit_circuitpython_wiznet5k-7.1.0/adafruit_circuitpython_wiznet5k.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5504 2024-05-21 16:18:29.000000 adafruit_circuitpython_wiznet5k-7.1.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-21 16:18:29.000000 adafruit_circuitpython_wiznet5k-7.1.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 16:18:29.000000 adafruit_circuitpython_wiznet5k-7.1.0/adafruit_circuitpython_wiznet5k.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-21 16:18:29.000000 adafruit_circuitpython_wiznet5k-7.1.0/adafruit_circuitpython_wiznet5k.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 16:18:29.000000 adafruit_circuitpython_wiznet5k-7.1.0/adafruit_circuitpython_wiznet5k.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:18:29.319536 adafruit_circuitpython_wiznet5k-7.1.0/adafruit_wiznet5k/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/adafruit_wiznet5k/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51779 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/adafruit_wiznet5k/adafruit_wiznet5k.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26273 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11431 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31187 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/adafruit_wiznet5k/adafruit_wiznet5k_socketpool.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:18:29.319536 adafruit_circuitpython_wiznet5k-7.1.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:18:29.319536 adafruit_circuitpython_wiznet5k-7.1.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:18:29.319536 adafruit_circuitpython_wiznet5k-7.1.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_aio_post.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2159 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_cheerlights.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1085 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_cpython_client_for_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_httpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_simpleserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_simpletest_manual_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-21 16:18:26.000000 adafruit_circuitpython_wiznet5k-7.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-21 16:18:18.000000 adafruit_circuitpython_wiznet5k-7.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 16:18:29.319536 adafruit_circuitpython_wiznet5k-7.1.0/setup.cfg
```

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_wiznet5k-7.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/.gitignore` & `adafruit_circuitpython_wiznet5k-7.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/.pre-commit-config.yaml` & `adafruit_circuitpython_wiznet5k-7.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/.pylintrc` & `adafruit_circuitpython_wiznet5k-7.1.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_wiznet5k-7.1.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/LICENSE` & `adafruit_circuitpython_wiznet5k-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_wiznet5k-7.1.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/MIT.txt` & `adafruit_circuitpython_wiznet5k-7.1.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_wiznet5k-7.1.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/PKG-INFO` & `adafruit_circuitpython_wiznet5k-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 7.0.0
+Version: 7.1.0
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/README.rst` & `adafruit_circuitpython_wiznet5k-7.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO` & `adafruit_circuitpython_wiznet5k-7.1.0/adafruit_circuitpython_wiznet5k.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wiznet5k
-Version: 7.0.0
+Version: 7.1.0
 Summary: Pure-Python interface for WIZNET 5k ethernet modules.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k
 Keywords: adafruit,blinka,circuitpython,micropython,wiznet5k,ethernet,,wiznet,,w5500,,w5200,,internet,,iot
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt` & `adafruit_circuitpython_wiznet5k-7.1.0/adafruit_circuitpython_wiznet5k.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k.py` & `adafruit_circuitpython_wiznet5k-7.1.0/adafruit_wiznet5k/adafruit_wiznet5k.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         import digitalio
 
         IpAddress4Raw = Union[bytes, Tuple[int, int, int, int]]
         MacAddressRaw = Union[bytes, Tuple[int, int, int, int, int, int]]
 except ImportError:
     pass
 
-__version__ = "7.0.0"
+__version__ = "7.1.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k.git"
 
 from random import randint
 import time
 import gc
 from micropython import const
 from adafruit_ticks import ticks_ms, ticks_diff
```

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py` & `adafruit_circuitpython_wiznet5k-7.1.0/adafruit_wiznet5k/adafruit_wiznet5k_debug.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py` & `adafruit_circuitpython_wiznet5k-7.1.0/adafruit_wiznet5k/adafruit_wiznet5k_dhcp.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py` & `adafruit_circuitpython_wiznet5k-7.1.0/adafruit_wiznet5k/adafruit_wiznet5k_dns.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/adafruit_wiznet5k/adafruit_wiznet5k_socketpool.py` & `adafruit_circuitpython_wiznet5k-7.1.0/adafruit_wiznet5k/adafruit_wiznet5k_socketpool.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,17 +17,17 @@
     from typing import TYPE_CHECKING, List, Optional, Tuple, Union
 
     if TYPE_CHECKING:
         from adafruit_wiznet5k.adafruit_wiznet5k import WIZNET5K
 except ImportError:
     pass
 
+import errno
 import gc
 from sys import byteorder
-from errno import ETIMEDOUT
 
 from micropython import const
 from adafruit_ticks import ticks_ms, ticks_diff
 
 import adafruit_wiznet5k as wiznet5k
 
 
@@ -634,15 +634,15 @@
             if self._timeout is None:
                 # blocking mode
                 continue
             if self._timeout == 0:
                 # non-blocking mode
                 break
             if ticks_diff(ticks_ms(), last_read_time) / 1000 > self._timeout:
-                raise timeout("timed out")
+                raise OSError(errno.ETIMEDOUT)
         return num_read
 
     @_check_socket_closed
     def recvfrom_into(  # pylint: disable=unused-argument
         self, buffer: bytearray, nbytes: int = 0, flags: int = 0
     ) -> Tuple[int, Tuple[str, int]]:
         """
@@ -809,15 +809,7 @@
         return self._sock_type
 
     @property
     @_check_socket_closed
     def proto(self):
         """Socket protocol (always 0x00 in this implementation)."""
         return 0
-
-
-class timeout(TimeoutError):  # pylint: disable=invalid-name
-    """TimeoutError class. An instance of this error will be raised by recv_into() if
-    the timeout has elapsed and we haven't received any data yet."""
-
-    def __init__(self, msg):
-        super().__init__(ETIMEDOUT, msg)
```

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/docs/_static/favicon.ico` & `adafruit_circuitpython_wiznet5k-7.1.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/docs/conf.py` & `adafruit_circuitpython_wiznet5k-7.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/docs/index.rst` & `adafruit_circuitpython_wiznet5k-7.1.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_aio_post.py` & `adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_cheerlights.py` & `adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_cpython_client_for_simpleserver.py` & `adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_cpython_client_for_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_httpserver.py` & `adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_httpserver.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_simpleserver.py` & `adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_simpleserver.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_simpletest.py` & `adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/examples/wiznet5k_simpletest_manual_network.py` & `adafruit_circuitpython_wiznet5k-7.1.0/examples/wiznet5k_simpletest_manual_network.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_wiznet5k-7.0.0/pyproject.toml` & `adafruit_circuitpython_wiznet5k-7.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-wiznet5k"
 description = "Pure-Python interface for WIZNET 5k ethernet modules."
-version = "7.0.0"
+version = "7.1.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Wiznet5k"}
 keywords = [
     "adafruit",
```

