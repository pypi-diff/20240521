# Comparing `tmp/adafruit_circuitpython_minimqtt-7.7.0.tar.gz` & `tmp/adafruit_circuitpython_minimqtt-7.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_minimqtt-7.7.0.tar", last modified: Sun May 12 19:48:15 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_minimqtt-7.8.0.tar", last modified: Mon May 20 22:10:17 2024, max compression
```

## Comparing `adafruit_circuitpython_minimqtt-7.7.0.tar` & `adafruit_circuitpython_minimqtt-7.8.0.tar`

### file list

```diff
@@ -1,82 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.209877 adafruit_circuitpython_minimqtt-7.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.193877 adafruit_circuitpython_minimqtt-7.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.197877 adafruit_circuitpython_minimqtt-7.7.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.197877 adafruit_circuitpython_minimqtt-7.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.201877 adafruit_circuitpython_minimqtt-7.7.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/LICENSES/EPL-1.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-12 19:48:15.209877 adafruit_circuitpython_minimqtt-7.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.209877 adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-12 19:48:15.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-12 19:48:15.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 19:48:15.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-12 19:48:15.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 19:48:15.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.201877 adafruit_circuitpython_minimqtt-7.7.0/adafruit_minimqtt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_minimqtt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45805 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_minimqtt/adafruit_minimqtt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/adafruit_minimqtt/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.201877 adafruit_circuitpython_minimqtt-7.7.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.201877 adafruit_circuitpython_minimqtt-7.7.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.201877 adafruit_circuitpython_minimqtt-7.7.0/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.205877 adafruit_circuitpython_minimqtt-7.7.0/examples/cellular/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3198 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/cellular/minimqtt_adafruitio_cellular.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/cellular/minimqtt_simpletest_cellular.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.205877 adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/minimqtt_adafruitio_cpython.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/minimqtt_simpletest_cpython.py
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/user_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.205877 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_adafruitio_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_certificate_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_simpletest_esp32spi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.205877 adafruit_circuitpython_minimqtt-7.7.0/examples/ethernet/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2671 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/ethernet/minimqtt_adafruitio_eth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/ethernet/minimqtt_simpletest_eth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/minimqtt_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.205877 adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/minimqtt_adafruitio_native_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-12 19:48:15.209877 adafruit_circuitpython_minimqtt-7.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 19:48:15.205877 adafruit_circuitpython_minimqtt-7.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/mocket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/test_backoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/test_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/test_port_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/test_subscribe.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-12 19:48:13.000000 adafruit_circuitpython_minimqtt-7.7.0/tests/test_unsubscribe.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-12 19:48:07.000000 adafruit_circuitpython_minimqtt-7.7.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.410390 adafruit_circuitpython_minimqtt-7.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.402390 adafruit_circuitpython_minimqtt-7.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.402390 adafruit_circuitpython_minimqtt-7.8.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.406390 adafruit_circuitpython_minimqtt-7.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6147 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.406390 adafruit_circuitpython_minimqtt-7.8.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    11219 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/LICENSES/EPL-1.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-20 22:10:17.410390 adafruit_circuitpython_minimqtt-7.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.410390 adafruit_circuitpython_minimqtt-7.8.0/adafruit_circuitpython_minimqtt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-20 22:10:17.000000 adafruit_circuitpython_minimqtt-7.8.0/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-05-20 22:10:17.000000 adafruit_circuitpython_minimqtt-7.8.0/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:10:17.000000 adafruit_circuitpython_minimqtt-7.8.0/adafruit_circuitpython_minimqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-20 22:10:17.000000 adafruit_circuitpython_minimqtt-7.8.0/adafruit_circuitpython_minimqtt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-20 22:10:17.000000 adafruit_circuitpython_minimqtt-7.8.0/adafruit_circuitpython_minimqtt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.406390 adafruit_circuitpython_minimqtt-7.8.0/adafruit_minimqtt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/adafruit_minimqtt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46735 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/adafruit_minimqtt/adafruit_minimqtt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/adafruit_minimqtt/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.406390 adafruit_circuitpython_minimqtt-7.8.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.406390 adafruit_circuitpython_minimqtt-7.8.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5409 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.406390 adafruit_circuitpython_minimqtt-7.8.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.406390 adafruit_circuitpython_minimqtt-7.8.0/examples/cellular/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3198 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/cellular/minimqtt_adafruitio_cellular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/cellular/minimqtt_simpletest_cellular.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.410390 adafruit_circuitpython_minimqtt-7.8.0/examples/cpython/
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/cpython/minimqtt_adafruitio_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/cpython/minimqtt_simpletest_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/cpython/user_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.410390 adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_adafruitio_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_certificate_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3620 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_simpletest_esp32spi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.410390 adafruit_circuitpython_minimqtt-7.8.0/examples/ethernet/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2671 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/ethernet/minimqtt_adafruitio_eth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/ethernet/minimqtt_simpletest_eth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/minimqtt_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.410390 adafruit_circuitpython_minimqtt-7.8.0/examples/native_networking/
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/native_networking/minimqtt_adafruitio_native_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:10:17.410390 adafruit_circuitpython_minimqtt-7.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:10:17.410390 adafruit_circuitpython_minimqtt-7.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/tests/mocket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/tests/test_backoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7994 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/tests/test_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4244 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/tests/test_port_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/tests/test_recv_timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/tests/test_subscribe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-20 22:10:15.000000 adafruit_circuitpython_minimqtt-7.8.0/tests/test_unsubscribe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-20 22:10:08.000000 adafruit_circuitpython_minimqtt-7.8.0/tox.ini
```

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_minimqtt-7.8.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/.gitignore` & `adafruit_circuitpython_minimqtt-7.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/.pre-commit-config.yaml` & `adafruit_circuitpython_minimqtt-7.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/.pylintrc` & `adafruit_circuitpython_minimqtt-7.8.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_minimqtt-7.8.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/LICENSE` & `adafruit_circuitpython_minimqtt-7.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_minimqtt-7.8.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/LICENSES/EPL-1.0.txt` & `adafruit_circuitpython_minimqtt-7.8.0/LICENSES/EPL-1.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/LICENSES/MIT.txt` & `adafruit_circuitpython_minimqtt-7.8.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_minimqtt-7.8.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/PKG-INFO` & `adafruit_circuitpython_minimqtt-7.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-minimqtt
-Version: 7.7.0
+Version: 7.8.0
 Summary: MQTT client library for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT
 Keywords: adafruit,blinka,circuitpython,micropython,minimqtt,mqtt,,client,,socket
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/README.rst` & `adafruit_circuitpython_minimqtt-7.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO` & `adafruit_circuitpython_minimqtt-7.8.0/adafruit_circuitpython_minimqtt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-minimqtt
-Version: 7.7.0
+Version: 7.8.0
 Summary: MQTT client library for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT
 Keywords: adafruit,blinka,circuitpython,micropython,minimqtt,mqtt,,client,,socket
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt` & `adafruit_circuitpython_minimqtt-7.8.0/adafruit_circuitpython_minimqtt.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -56,9 +56,10 @@
 examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py
 examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py
 tests/conftest.py
 tests/mocket.py
 tests/test_backoff.py
 tests/test_loop.py
 tests/test_port_ssl.py
+tests/test_recv_timeout.py
 tests/test_subscribe.py
 tests/test_unsubscribe.py
```

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/adafruit_minimqtt/adafruit_minimqtt.py` & `adafruit_circuitpython_minimqtt-7.8.0/adafruit_minimqtt/adafruit_minimqtt.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 except ImportError:
     pass
 
 from micropython import const
 
 from .matcher import MQTTMatcher
 
-__version__ = "7.7.0"
+__version__ = "7.8.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT.git"
 
 # Client-specific variables
 MQTT_MSG_MAX_SZ = const(268435455)
 MQTT_MSG_SZ_LIM = const(10000000)
 MQTT_TOPIC_LENGTH_LIMIT = const(65535)
 MQTT_TCP_PORT = const(1883)
@@ -68,29 +68,39 @@
 MQTT_SUB = const(0x82)
 MQTT_UNSUB = const(0xA2)
 MQTT_DISCONNECT = b"\xe0\0"
 
 MQTT_PKT_TYPE_MASK = const(0xF0)
 
 
+CONNACK_ERROR_INCORRECT_PROTOCOL = const(0x01)
+CONNACK_ERROR_ID_REJECTED = const(0x02)
+CONNACK_ERROR_SERVER_UNAVAILABLE = const(0x03)
+CONNACK_ERROR_INCORECT_USERNAME_PASSWORD = const(0x04)
+CONNACK_ERROR_UNAUTHORIZED = const(0x05)
+
 CONNACK_ERRORS = {
-    const(0x01): "Connection Refused - Incorrect Protocol Version",
-    const(0x02): "Connection Refused - ID Rejected",
-    const(0x03): "Connection Refused - Server unavailable",
-    const(0x04): "Connection Refused - Incorrect username/password",
-    const(0x05): "Connection Refused - Unauthorized",
+    CONNACK_ERROR_INCORRECT_PROTOCOL: "Connection Refused - Incorrect Protocol Version",
+    CONNACK_ERROR_ID_REJECTED: "Connection Refused - ID Rejected",
+    CONNACK_ERROR_SERVER_UNAVAILABLE: "Connection Refused - Server unavailable",
+    CONNACK_ERROR_INCORECT_USERNAME_PASSWORD: "Connection Refused - Incorrect username/password",
+    CONNACK_ERROR_UNAUTHORIZED: "Connection Refused - Unauthorized",
 }
 
 _default_sock = None  # pylint: disable=invalid-name
 _fake_context = None  # pylint: disable=invalid-name
 
 
 class MMQTTException(Exception):
     """MiniMQTT Exception class."""
 
+    def __init__(self, error, code=None):
+        super().__init__(error, code)
+        self.code = code
+
 
 class NullLogger:
     """Fake logger class that does not do anything"""
 
     # pylint: disable=unused-argument
     def nothing(self, msg: str, *args) -> None:
         """no action"""
@@ -424,25 +434,32 @@
                 )
                 self._reset_reconnect_backoff()
                 return ret
             except (MemoryError, OSError, RuntimeError) as e:
                 self.logger.warning(f"Socket error when connecting: {e}")
                 backoff = False
             except MMQTTException as e:
-                last_exception = e
+                self._close_socket()
                 self.logger.info(f"MMQT error: {e}")
+                if e.code in [
+                    CONNACK_ERROR_INCORECT_USERNAME_PASSWORD,
+                    CONNACK_ERROR_UNAUTHORIZED,
+                ]:
+                    # No sense trying these again, re-raise
+                    raise
+                last_exception = e
                 backoff = True
 
         if self._reconnect_attempts_max > 1:
             exc_msg = "Repeated connect failures"
         else:
             exc_msg = "Connect failure"
+
         if last_exception:
             raise MMQTTException(exc_msg) from last_exception
-
         raise MMQTTException(exc_msg)
 
     # pylint: disable=too-many-branches, too-many-statements, too-many-locals
     def _connect(
         self,
         clean_session: bool = True,
         host: Optional[str] = None,
@@ -531,28 +548,34 @@
         stamp = self.get_monotonic_time()
         while True:
             op = self._wait_for_msg()
             if op == 32:
                 rc = self._sock_exact_recv(3)
                 assert rc[0] == 0x02
                 if rc[2] != 0x00:
-                    raise MMQTTException(CONNACK_ERRORS[rc[2]])
+                    raise MMQTTException(CONNACK_ERRORS[rc[2]], code=rc[2])
                 self._is_connected = True
                 result = rc[0] & 1
                 if self.on_connect is not None:
                     self.on_connect(self, self.user_data, result, rc[2])
 
                 return result
 
             if op is None:
                 if self.get_monotonic_time() - stamp > self._recv_timeout:
                     raise MMQTTException(
                         f"No data received from broker for {self._recv_timeout} seconds."
                     )
 
+    def _close_socket(self):
+        if self._sock:
+            self.logger.debug("Closing socket")
+            self._connection_manager.close_socket(self._sock)
+            self._sock = None
+
     # pylint: disable=no-self-use
     def _encode_remaining_length(
         self, fixed_header: bytearray, remaining_length: int
     ) -> None:
         """Encode Remaining Length [2.2.3]"""
         if remaining_length > 268_435_455:
             raise MMQTTException("invalid remaining length")
@@ -573,40 +596,41 @@
         """Disconnects the MiniMQTT client from the MQTT broker."""
         self._connected()
         self.logger.debug("Sending DISCONNECT packet to broker")
         try:
             self._sock.send(MQTT_DISCONNECT)
         except RuntimeError as e:
             self.logger.warning(f"Unable to send DISCONNECT packet: {e}")
-        self.logger.debug("Closing socket")
-        self._connection_manager.close_socket(self._sock)
+        self._close_socket()
         self._is_connected = False
         self._subscribed_topics = []
         self._last_msg_sent_timestamp = 0
         if self.on_disconnect is not None:
             self.on_disconnect(self, self.user_data, 0)
 
     def ping(self) -> list[int]:
         """Pings the MQTT Broker to confirm if the broker is alive or if
         there is an active network connection.
         Returns packet types of any messages received while waiting for PINGRESP.
         """
         self._connected()
         self.logger.debug("Sending PINGREQ")
         self._sock.send(MQTT_PINGREQ)
-        ping_timeout = self.keep_alive
+        ping_timeout = self._recv_timeout
         stamp = self.get_monotonic_time()
         self._last_msg_sent_timestamp = stamp
         rc, rcs = None, []
         while rc != MQTT_PINGRESP:
             rc = self._wait_for_msg()
             if rc:
                 rcs.append(rc)
             if self.get_monotonic_time() - stamp > ping_timeout:
-                raise MMQTTException("PINGRESP not returned from broker.")
+                raise MMQTTException(
+                    f"PINGRESP not returned from broker within {ping_timeout} seconds."
+                )
         return rcs
 
     # pylint: disable=too-many-branches, too-many-statements
     def publish(
         self,
         topic: str,
         msg: Union[str, int, float, bytes],
@@ -1064,36 +1088,36 @@
             # CPython/Socketpool Impl.
             rc = bytearray(bufsize)
             mv = memoryview(rc)
             recv_len = self._sock.recv_into(rc, bufsize)
             to_read = bufsize - recv_len
             if to_read < 0:
                 raise MMQTTException(f"negative number of bytes to read: {to_read}")
-            read_timeout = timeout if timeout is not None else self.keep_alive
+            read_timeout = timeout if timeout is not None else self._recv_timeout
             mv = mv[recv_len:]
             while to_read > 0:
                 recv_len = self._sock.recv_into(mv, to_read)
                 to_read -= recv_len
                 mv = mv[recv_len:]
                 if self.get_monotonic_time() - stamp > read_timeout:
                     raise MMQTTException(
                         f"Unable to receive {to_read} bytes within {read_timeout} seconds."
                     )
         else:  # ESP32SPI Impl.
-            # This will timeout with socket timeout (not keepalive timeout)
+            # This will time out with socket timeout (not receive timeout).
             rc = self._sock.recv(bufsize)
             if not rc:
                 self.logger.debug("_sock_exact_recv timeout")
                 # If no bytes waiting, raise same exception as socketpool
                 raise OSError(errno.ETIMEDOUT)
             # If any bytes waiting, try to read them all,
             # or raise exception if wait longer than read_timeout
             to_read = bufsize - len(rc)
             assert to_read >= 0
-            read_timeout = self.keep_alive
+            read_timeout = self._recv_timeout
             while to_read > 0:
                 recv = self._sock.recv(to_read)
                 to_read -= len(recv)
                 rc += recv
                 if self.get_monotonic_time() - stamp > read_timeout:
                     raise MMQTTException(
                         f"Unable to receive {to_read} bytes within {read_timeout} seconds."
```

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/adafruit_minimqtt/matcher.py` & `adafruit_circuitpython_minimqtt-7.8.0/adafruit_minimqtt/matcher.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/docs/_static/favicon.ico` & `adafruit_circuitpython_minimqtt-7.8.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/docs/conf.py` & `adafruit_circuitpython_minimqtt-7.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/docs/index.rst` & `adafruit_circuitpython_minimqtt-7.8.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/cellular/minimqtt_adafruitio_cellular.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/cellular/minimqtt_adafruitio_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/cellular/minimqtt_simpletest_cellular.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/cellular/minimqtt_simpletest_cellular.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/minimqtt_adafruitio_cpython.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/cpython/minimqtt_adafruitio_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/minimqtt_simpletest_cpython.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/cpython/minimqtt_simpletest_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/cpython/user_data.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/cpython/user_data.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_adafruitio_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_adafruitio_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_certificate_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_certificate_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_pub_sub_blocking_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_pub_sub_blocking_topic_callbacks_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_pub_sub_nonblocking_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_pub_sub_pyportal_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/esp32spi/minimqtt_simpletest_esp32spi.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/esp32spi/minimqtt_simpletest_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/ethernet/minimqtt_adafruitio_eth.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/ethernet/minimqtt_adafruitio_eth.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/ethernet/minimqtt_simpletest_eth.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/ethernet/minimqtt_simpletest_eth.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/minimqtt_simpletest.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/minimqtt_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/minimqtt_adafruitio_native_networking.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/native_networking/minimqtt_adafruitio_native_networking.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/native_networking/minimqtt_pub_sub_blocking_native_networking.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py` & `adafruit_circuitpython_minimqtt-7.8.0/examples/native_networking/minimqtt_pub_sub_blocking_topic_callbacks_native_networking.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/pyproject.toml` & `adafruit_circuitpython_minimqtt-7.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-minimqtt"
 description = "MQTT client library for CircuitPython"
-version = "7.7.0"
+version = "7.8.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MiniMQTT"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/tests/mocket.py` & `adafruit_circuitpython_minimqtt-7.8.0/tests/mocket.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/tests/test_loop.py` & `adafruit_circuitpython_minimqtt-7.8.0/tests/test_loop.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/tests/test_port_ssl.py` & `adafruit_circuitpython_minimqtt-7.8.0/tests/test_port_ssl.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/tests/test_subscribe.py` & `adafruit_circuitpython_minimqtt-7.8.0/tests/test_subscribe.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/tests/test_unsubscribe.py` & `adafruit_circuitpython_minimqtt-7.8.0/tests/test_unsubscribe.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_minimqtt-7.7.0/tox.ini` & `adafruit_circuitpython_minimqtt-7.8.0/tox.ini`

 * *Files identical despite different names*

