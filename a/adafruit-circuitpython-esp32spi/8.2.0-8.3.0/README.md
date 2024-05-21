# Comparing `tmp/adafruit_circuitpython_esp32spi-8.2.0.tar.gz` & `tmp/adafruit_circuitpython_esp32spi-8.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit_circuitpython_esp32spi-8.2.0.tar", last modified: Wed May 15 18:24:50 2024, max compression
+gzip compressed data, was "adafruit_circuitpython_esp32spi-8.3.0.tar", last modified: Tue May 21 14:40:26 2024, max compression
```

## Comparing `adafruit_circuitpython_esp32spi-8.2.0.tar` & `adafruit_circuitpython_esp32spi-8.3.0.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:50.183754 adafruit_circuitpython_esp32spi-8.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:50.175754 adafruit_circuitpython_esp32spi-8.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:50.179754 adafruit_circuitpython_esp32spi-8.2.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:50.179754 adafruit_circuitpython_esp32spi-8.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:50.179754 adafruit_circuitpython_esp32spi-8.2.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-15 18:24:50.183754 adafruit_circuitpython_esp32spi-8.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:50.183754 adafruit_circuitpython_esp32spi-8.2.0/adafruit_circuitpython_esp32spi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-15 18:24:50.000000 adafruit_circuitpython_esp32spi-8.2.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-15 18:24:50.000000 adafruit_circuitpython_esp32spi-8.2.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:24:50.000000 adafruit_circuitpython_esp32spi-8.2.0/adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-15 18:24:50.000000 adafruit_circuitpython_esp32spi-8.2.0/adafruit_circuitpython_esp32spi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-15 18:24:50.000000 adafruit_circuitpython_esp32spi-8.2.0/adafruit_circuitpython_esp32spi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:50.179754 adafruit_circuitpython_esp32spi-8.2.0/adafruit_esp32spi/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3180 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/adafruit_esp32spi/PWMOut.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/adafruit_esp32spi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39665 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/adafruit_esp32spi/adafruit_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8441 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/adafruit_esp32spi/adafruit_esp32spi_socketpool.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13198 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6293 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/adafruit_esp32spi/digitalio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:50.183754 adafruit_circuitpython_esp32spi-8.2.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:50.183754 adafruit_circuitpython_esp32spi-8.2.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:50.183754 adafruit_circuitpython_esp32spi-8.2.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_cheerlights.py
--rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_ipconfig.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_localtime.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_settings.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_simpletest_rp2040.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_tcp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_udp_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_wpa2ent_aio_post.py
--rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_wpa2ent_simpletest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:50.183754 adafruit_circuitpython_esp32spi-8.2.0/examples/gpio/
--rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/gpio/esp32spi_gpio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/gpio/gpio.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:50.183754 adafruit_circuitpython_esp32spi-8.2.0/examples/server/
--rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/examples/server/esp32spi_wsgiserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-15 18:24:47.000000 adafruit_circuitpython_esp32spi-8.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-15 18:24:41.000000 adafruit_circuitpython_esp32spi-8.2.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:24:50.183754 adafruit_circuitpython_esp32spi-8.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:26.366692 adafruit_circuitpython_esp32spi-8.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:26.354693 adafruit_circuitpython_esp32spi-8.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:26.358693 adafruit_circuitpython_esp32spi-8.3.0/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:26.358693 adafruit_circuitpython_esp32spi-8.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:26.362692 adafruit_circuitpython_esp32spi-8.3.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    16814 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-21 14:40:26.366692 adafruit_circuitpython_esp32spi-8.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:26.366692 adafruit_circuitpython_esp32spi-8.3.0/adafruit_circuitpython_esp32spi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4228 2024-05-21 14:40:26.000000 adafruit_circuitpython_esp32spi-8.3.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-21 14:40:26.000000 adafruit_circuitpython_esp32spi-8.3.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:40:26.000000 adafruit_circuitpython_esp32spi-8.3.0/adafruit_circuitpython_esp32spi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-21 14:40:26.000000 adafruit_circuitpython_esp32spi-8.3.0/adafruit_circuitpython_esp32spi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 14:40:26.000000 adafruit_circuitpython_esp32spi-8.3.0/adafruit_circuitpython_esp32spi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:26.362692 adafruit_circuitpython_esp32spi-8.3.0/adafruit_esp32spi/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3180 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/adafruit_esp32spi/PWMOut.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/adafruit_esp32spi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39665 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/adafruit_esp32spi/adafruit_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7976 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/adafruit_esp32spi/adafruit_esp32spi_socketpool.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13198 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6293 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/adafruit_esp32spi/digitalio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:26.362692 adafruit_circuitpython_esp32spi-8.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:26.366692 adafruit_circuitpython_esp32spi-8.3.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:26.366692 adafruit_circuitpython_esp32spi-8.3.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     3104 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_cheerlights.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3178 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_ipconfig.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_localtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_settings.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_simpletest_rp2040.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_tcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_udp_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_wpa2ent_aio_post.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_wpa2ent_simpletest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:26.366692 adafruit_circuitpython_esp32spi-8.3.0/examples/gpio/
+-rw-r--r--   0 runner    (1001) docker     (127)     5220 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/gpio/esp32spi_gpio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6253 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/gpio/gpio.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:26.366692 adafruit_circuitpython_esp32spi-8.3.0/examples/server/
+-rwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/examples/server/esp32spi_wsgiserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-21 14:40:23.000000 adafruit_circuitpython_esp32spi-8.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      231 2024-05-21 14:40:17.000000 adafruit_circuitpython_esp32spi-8.3.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 14:40:26.366692 adafruit_circuitpython_esp32spi-8.3.0/setup.cfg
```

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit_circuitpython_esp32spi-8.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/.gitignore` & `adafruit_circuitpython_esp32spi-8.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/.pre-commit-config.yaml` & `adafruit_circuitpython_esp32spi-8.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/.pylintrc` & `adafruit_circuitpython_esp32spi-8.3.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/CODE_OF_CONDUCT.md` & `adafruit_circuitpython_esp32spi-8.3.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/LICENSE` & `adafruit_circuitpython_esp32spi-8.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/LICENSES/CC-BY-4.0.txt` & `adafruit_circuitpython_esp32spi-8.3.0/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/LICENSES/MIT.txt` & `adafruit_circuitpython_esp32spi-8.3.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/LICENSES/Unlicense.txt` & `adafruit_circuitpython_esp32spi-8.3.0/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/PKG-INFO` & `adafruit_circuitpython_esp32spi-8.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32spi
-Version: 8.2.0
+Version: 8.3.0
 Summary: CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
 Keywords: adafruit,blinka,circuitpython,micropython,esp32spi,wifi,esp32
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/README.rst` & `adafruit_circuitpython_esp32spi-8.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO` & `adafruit_circuitpython_esp32spi-8.3.0/adafruit_circuitpython_esp32spi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32spi
-Version: 8.2.0
+Version: 8.3.0
 Summary: CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI
 Keywords: adafruit,blinka,circuitpython,micropython,esp32spi,wifi,esp32
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt` & `adafruit_circuitpython_esp32spi-8.3.0/adafruit_circuitpython_esp32spi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/adafruit_esp32spi/PWMOut.py` & `adafruit_circuitpython_esp32spi-8.3.0/adafruit_esp32spi/PWMOut.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/adafruit_esp32spi/adafruit_esp32spi.py` & `adafruit_circuitpython_esp32spi-8.3.0/adafruit_esp32spi/adafruit_esp32spi.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 import struct
 import time
 from micropython import const
 from adafruit_bus_device.spi_device import SPIDevice
 from digitalio import Direction
 
-__version__ = "8.2.0"
+__version__ = "8.3.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI.git"
 
 _SET_NET_CMD = const(0x10)
 _SET_PASSPHRASE_CMD = const(0x11)
 _SET_IP_CONFIG = const(0x14)
 _SET_DNS_CONFIG = const(0x15)
 _SET_HOSTNAME = const(0x16)
```

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/adafruit_esp32spi/adafruit_esp32spi_socketpool.py` & `adafruit_circuitpython_esp32spi-8.3.0/adafruit_esp32spi/adafruit_esp32spi_socketpool.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,36 +17,33 @@
 
     if TYPE_CHECKING:
         from esp32spi.adafruit_esp32spi import ESP_SPIcontrol
 except ImportError:
     pass
 
 
+import errno
 import time
 import gc
 from micropython import const
 from adafruit_esp32spi import adafruit_esp32spi as esp32spi
 
 _global_socketpool = {}
 
 
-class SocketPoolContants:  # pylint: disable=too-few-public-methods
-    """Helper class for the constants that are needed everywhere"""
+class SocketPool:
+    """ESP32SPI SocketPool library"""
 
     SOCK_STREAM = const(0)
     SOCK_DGRAM = const(1)
     AF_INET = const(2)
     NO_SOCKET_AVAIL = const(255)
 
     MAX_PACKET = const(4000)
 
-
-class SocketPool(SocketPoolContants):
-    """ESP32SPI SocketPool library"""
-
     def __new__(cls, iface: ESP_SPIcontrol):
         # We want to make sure to return the same pool for the same interface
         if iface not in _global_socketpool:
             _global_socketpool[iface] = super().__new__(cls)
         return _global_socketpool[iface]
 
     def __init__(self, iface: ESP_SPIcontrol):
@@ -56,20 +53,20 @@
         self, host, port, family=0, socktype=0, proto=0, flags=0
     ):
         """Given a hostname and a port name, return a 'socket.getaddrinfo'
         compatible list of tuples. Honestly, we ignore anything but host & port"""
         if not isinstance(port, int):
             raise ValueError("Port must be an integer")
         ipaddr = self._interface.get_host_by_name(host)
-        return [(SocketPoolContants.AF_INET, socktype, proto, "", (ipaddr, port))]
+        return [(SocketPool.AF_INET, socktype, proto, "", (ipaddr, port))]
 
     def socket(  # pylint: disable=redefined-builtin
         self,
-        family=SocketPoolContants.AF_INET,
-        type=SocketPoolContants.SOCK_STREAM,
+        family=AF_INET,
+        type=SOCK_STREAM,
         proto=0,
         fileno=None,
     ):
         """Create a new socket and return it"""
         return Socket(self, family, type, proto, fileno)
 
 
@@ -181,15 +178,15 @@
                 num_read += len(bytes_read)
                 num_to_read -= len(bytes_read)
             elif num_read > 0:
                 # We got a message, but there are no more bytes to read, so we can stop.
                 break
             # No bytes yet, or more bytes requested.
             if self._timeout > 0 and time.monotonic() - last_read_time > self._timeout:
-                raise timeout("timed out")
+                raise OSError(errno.ETIMEDOUT)
         return num_read
 
     def settimeout(self, value):
         """Set the read timeout for sockets.
         If value is 0 socket reads will block until a message is available.
         """
         self._timeout = value
@@ -223,15 +220,7 @@
             self.close()
             self._socknum = SocketPool.NO_SOCKET_AVAIL
         return result
 
     def close(self):
         """Close the socket, after reading whatever remains"""
         self._interface.socket_close(self._socknum)
-
-
-class timeout(TimeoutError):  # pylint: disable=invalid-name
-    """TimeoutError class. An instance of this error will be raised by recv_into() if
-    the timeout has elapsed and we haven't received any data yet."""
-
-    def __init__(self, msg):
-        super().__init__(msg)
```

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py` & `adafruit_circuitpython_esp32spi-8.3.0/adafruit_esp32spi/adafruit_esp32spi_wifimanager.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/adafruit_esp32spi/digitalio.py` & `adafruit_circuitpython_esp32spi-8.3.0/adafruit_esp32spi/digitalio.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/docs/_static/favicon.ico` & `adafruit_circuitpython_esp32spi-8.3.0/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/docs/api.rst` & `adafruit_circuitpython_esp32spi-8.3.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/docs/conf.py` & `adafruit_circuitpython_esp32spi-8.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/docs/index.rst` & `adafruit_circuitpython_esp32spi-8.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_aio_post.py` & `adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_cheerlights.py` & `adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_cheerlights.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_ipconfig.py` & `adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_ipconfig.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_localtime.py` & `adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_localtime.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_settings.toml` & `adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_settings.toml`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_simpletest.py` & `adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_simpletest_rp2040.py` & `adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_simpletest_rp2040.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_tcp_client.py` & `adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_tcp_client.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_udp_client.py` & `adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_udp_client.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_wpa2ent_aio_post.py` & `adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_wpa2ent_aio_post.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/examples/esp32spi_wpa2ent_simpletest.py` & `adafruit_circuitpython_esp32spi-8.3.0/examples/esp32spi_wpa2ent_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/examples/gpio/esp32spi_gpio.py` & `adafruit_circuitpython_esp32spi-8.3.0/examples/gpio/esp32spi_gpio.py`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/examples/gpio/gpio.md` & `adafruit_circuitpython_esp32spi-8.3.0/examples/gpio/gpio.md`

 * *Files identical despite different names*

### Comparing `adafruit_circuitpython_esp32spi-8.2.0/pyproject.toml` & `adafruit_circuitpython_esp32spi-8.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-esp32spi"
 description = "CircuitPython driver library for using ESP32 as WiFi  co-processor using SPI"
-version = "8.2.0"
+version = "8.3.0"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32SPI"}
 keywords = [
     "adafruit",
```

