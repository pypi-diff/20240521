# Comparing `tmp/vivarium_inputs-4.1.3.tar.gz` & `tmp/vivarium_inputs-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivarium_inputs-4.1.3.tar", last modified: Tue Jan  9 22:04:43 2024, max compression
+gzip compressed data, was "vivarium_inputs-5.0.0.tar", last modified: Mon May 20 22:07:29 2024, max compression
```

## Comparing `vivarium_inputs-4.1.3.tar` & `vivarium_inputs-5.0.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.082470 vivarium_inputs-4.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.070470 vivarium_inputs-4.1.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.070470 vivarium_inputs-4.1.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5623 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-01-09 22:04:43.082470 vivarium_inputs-4.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.070470 vivarium_inputs-4.1.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/docs/nitpick-exceptions
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.070470 vivarium_inputs-4.1.3/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.070470 vivarium_inputs-4.1.3/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.070470 vivarium_inputs-4.1.3/docs/source/api_reference/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/docs/source/api_reference/core.rst
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/docs/source/api_reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/docs/source/api_reference/interface.rst
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/docs/source/api_reference/mapping_extension.rst
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/docs/source/api_reference/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.070470 vivarium_inputs-4.1.3/docs/source/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/docs/source/tutorials/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    15588 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/docs/source/tutorials/pulling_data.rst
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-09 22:04:43.082470 vivarium_inputs-4.1.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1903 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.066470 vivarium_inputs-4.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.074470 vivarium_inputs-4.1.3/src/vivarium_inputs/
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-09 22:04:43.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    19727 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     9565 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7907 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.074470 vivarium_inputs-4.1.3/src/vivarium_inputs/mapping_extension/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/mapping_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/mapping_extension/alternative_risk_factor.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/mapping_extension/alternative_risk_factor_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/mapping_extension/health_technology.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/mapping_extension/health_technology_template.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/mapping_extension/healthcare_entity.py
--rw-r--r--   0 runner    (1001) docker     (127)      923 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/mapping_extension/healthcare_entity_template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.074470 vivarium_inputs-4.1.3/src/vivarium_inputs/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/testing/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)    18148 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/utility_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.078470 vivarium_inputs-4.1.3/src/vivarium_inputs/validation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    84465 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/validation/raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/validation/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)    57659 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/src/vivarium_inputs/validation/sim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.078470 vivarium_inputs-4.1.3/src/vivarium_inputs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-01-09 22:04:43.000000 vivarium_inputs-4.1.3/src/vivarium_inputs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-01-09 22:04:43.000000 vivarium_inputs-4.1.3/src/vivarium_inputs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 22:04:43.000000 vivarium_inputs-4.1.3/src/vivarium_inputs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-09 22:04:21.000000 vivarium_inputs-4.1.3/src/vivarium_inputs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-01-09 22:04:43.000000 vivarium_inputs-4.1.3/src/vivarium_inputs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-09 22:04:43.000000 vivarium_inputs-4.1.3/src/vivarium_inputs.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.078470 vivarium_inputs-4.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.078470 vivarium_inputs-4.1.3/tests/extract/
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/tests/extract/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     6345 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/tests/extract/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/tests/extract/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (127)     5067 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/tests/extract/test_get_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/tests/extract/test_utility_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/tests/test_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-09 22:04:43.078470 vivarium_inputs-4.1.3/tests/validation/
--rw-r--r--   0 runner    (1001) docker     (127)    15435 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/tests/validation/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/tests/validation/test_shared.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/tests/validation/test_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-01-09 22:04:11.000000 vivarium_inputs-4.1.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.633782 vivarium_inputs-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.621782 vivarium_inputs-5.0.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.621782 vivarium_inputs-5.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5804 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-20 22:07:29.633782 vivarium_inputs-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.625782 vivarium_inputs-5.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/docs/nitpick-exceptions
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.625782 vivarium_inputs-5.0.0/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.625782 vivarium_inputs-5.0.0/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.625782 vivarium_inputs-5.0.0/docs/source/api_reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/docs/source/api_reference/core.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/docs/source/api_reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/docs/source/api_reference/interface.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/docs/source/api_reference/mapping_extension.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/docs/source/api_reference/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7836 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.625782 vivarium_inputs-5.0.0/docs/source/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/docs/source/tutorials/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16002 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/docs/source/tutorials/pulling_data.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:07:29.633782 vivarium_inputs-5.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1901 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.621782 vivarium_inputs-5.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.625782 vivarium_inputs-5.0.0/src/vivarium_inputs/
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 22:07:29.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23714 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13418 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7043 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.629782 vivarium_inputs-5.0.0/src/vivarium_inputs/mapping_extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/mapping_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/mapping_extension/alternative_risk_factor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/mapping_extension/alternative_risk_factor_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/mapping_extension/health_technology.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/mapping_extension/health_technology_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/mapping_extension/healthcare_entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)      923 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/mapping_extension/healthcare_entity_template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.629782 vivarium_inputs-5.0.0/src/vivarium_inputs/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/testing/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19742 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/utility_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.629782 vivarium_inputs-5.0.0/src/vivarium_inputs/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84996 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/validation/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/validation/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59444 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/src/vivarium_inputs/validation/sim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.629782 vivarium_inputs-5.0.0/src/vivarium_inputs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-05-20 22:07:29.000000 vivarium_inputs-5.0.0/src/vivarium_inputs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-20 22:07:29.000000 vivarium_inputs-5.0.0/src/vivarium_inputs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:07:29.000000 vivarium_inputs-5.0.0/src/vivarium_inputs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:07:11.000000 vivarium_inputs-5.0.0/src/vivarium_inputs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-20 22:07:29.000000 vivarium_inputs-5.0.0/src/vivarium_inputs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 22:07:29.000000 vivarium_inputs-5.0.0/src/vivarium_inputs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.629782 vivarium_inputs-5.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.629782 vivarium_inputs-5.0.0/tests/extract/
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/tests/extract/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9888 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/tests/extract/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/tests/extract/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/tests/extract/test_get_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/tests/extract/test_utility_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/tests/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:07:29.629782 vivarium_inputs-5.0.0/tests/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)    15898 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/tests/validation/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/tests/validation/test_shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10700 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/tests/validation/test_sim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-20 22:07:01.000000 vivarium_inputs-5.0.0/tox.ini
```

### Comparing `vivarium_inputs-4.1.3/.github/pull_request_template.md` & `vivarium_inputs-5.0.0/.github/pull_request_template.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 ## Title: Summary, imperative, start upper case, don't end with a period
 <!-- Ideally, <=50 chars. 50 chars is here..: -->
 
 ### Description
 <!-- For use in commit message, wrap at 72 chars. 72 chars is here: -->
 - *Category*: <!-- one of bugfix, feature, refactor, POC, CI/infrastructure, documentation, 
                    revert, test, release, other/misc -->
-- *JIRA issue*: [MIC-XYZ](https://jira.ihme.washington.edu/browse/MIC-XYZ)
+- *JIRA issue*: https://jira.ihme.washington.edu/browse/MIC-XYZ
 
 ### Changes and notes
 <!-- 
 Change description – why, what, anything unexplained by the above.
 Include guidance to reviewers if changes are complex.
 -->
```

### Comparing `vivarium_inputs-4.1.3/.github/workflows/build.yml` & `vivarium_inputs-5.0.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/.github/workflows/deploy.yml` & `vivarium_inputs-5.0.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/.gitignore` & `vivarium_inputs-5.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/.readthedocs.yml` & `vivarium_inputs-5.0.0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/CHANGELOG.rst` & `vivarium_inputs-5.0.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+**5.0.0 - 05/20/24**
+
+ - Pull GBD 2021 data
+ - Add functionality to pull multiple locationals at once
+
+**4.1.4 - 01/11/24**
+
+ - Remove erroneously merged get_draws_kwargs argument
+
 **4.1.3 - 01/09/24**
 
  - Update PyPI to 2FA with trusted publisher
 
 **4.1.2 - 10/16/23**
 
  - Drop support for python 3.8
```

### Comparing `vivarium_inputs-4.1.3/CODE_OF_CONDUCT.rst` & `vivarium_inputs-5.0.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/CONTRIBUTING.rst` & `vivarium_inputs-5.0.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/LICENSE.txt` & `vivarium_inputs-5.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/PKG-INFO` & `vivarium_inputs-5.0.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: vivarium_inputs
-Version: 4.1.3
+Version: 5.0.0
 Summary: Transformations and artifact building for the vivarium microsimulation project.
 Home-page: https://github.com/ihmeuw/vivarium_inputs
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: click
 Requires-Dist: joblib
 Requires-Dist: tables
 Requires-Dist: vivarium>=1.2.1
-Requires-Dist: gbd_mapping<4.0.0,>=3.1.0
+Requires-Dist: gbd_mapping<5.0.0,>=4.0.0
 Requires-Dist: loguru
 Provides-Extra: docs
-Requires-Dist: sphinx<7.0,>=6.2.1; extra == "docs"
+Requires-Dist: sphinx<8.0,>=7.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
 Provides-Extra: data
-Requires-Dist: vivarium-gbd-access<4.0.0,>=3.0.7; extra == "data"
+Requires-Dist: vivarium-gbd-access<5.0.0,>=4.0.0; extra == "data"
 Requires-Dist: core-maths; extra == "data"
 Provides-Extra: dev
-Requires-Dist: sphinx<7.0,>=6.2.1; extra == "dev"
+Requires-Dist: sphinx<8.0,>=7.0; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: hypothesis; extra == "dev"
-Requires-Dist: vivarium-gbd-access<4.0.0,>=3.0.7; extra == "dev"
+Requires-Dist: vivarium-gbd-access<5.0.0,>=4.0.0; extra == "dev"
 Requires-Dist: core-maths; extra == "dev"
 
 Vivarium Inputs
 ===============
 
 .. image:: https://badge.fury.io/py/vivarium-inputs.svg
     :target: https://badge.fury.io/py/vivarium-inputs
@@ -50,7 +50,11 @@
     :alt: Latest Docs
 
 
 This package is used to transform Global Burden of Disease data and package it into data artifacts
 used as inputs into vivarium simulations.
 
 It requires access to the IHME cluster for use (but not for testing).
+
+
+`Check out the docs! <https://vivarium.readthedocs.io/projects/vivarium-inputs/en/latest/>`_
+--------------------------------------------------------------------------------------------
```

### Comparing `vivarium_inputs-4.1.3/README.rst` & `vivarium_inputs-5.0.0/README.rst`

 * *Files 27% similar despite different names*

```diff
@@ -13,7 +13,11 @@
     :alt: Latest Docs
 
 
 This package is used to transform Global Burden of Disease data and package it into data artifacts
 used as inputs into vivarium simulations.
 
 It requires access to the IHME cluster for use (but not for testing).
+
+
+`Check out the docs! <https://vivarium.readthedocs.io/projects/vivarium-inputs/en/latest/>`_
+--------------------------------------------------------------------------------------------
```

### Comparing `vivarium_inputs-4.1.3/docs/Makefile` & `vivarium_inputs-5.0.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/docs/source/conf.py` & `vivarium_inputs-5.0.0/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/docs/source/tutorials/pulling_data.rst` & `vivarium_inputs-5.0.0/docs/source/tutorials/pulling_data.rst`

 * *Files 4% similar despite different names*

```diff
@@ -362,45 +362,50 @@
     4  0.04        87.850727
 
 
 .. testcode::
     :hide:
 
     import inspect
-    from typing import Union
+    from typing import List, Optional, Union
 
     import pandas as pd
 
     from vivarium_inputs import (get_measure, get_population_structure,
                                  get_theoretical_minimum_risk_life_expectancy,
                                  get_age_bins, get_demographic_dimensions, get_raw_data)
     from gbd_mapping import ModelableEntity
 
     funcs = {get_measure: {
                 'parameters': {
                     'entity': ModelableEntity, 
                     'measure': str, 
-                    'location': str, 
-                    'get_draws_kwargs': inspect._empty,
+                    'location': Union[int, str, List[Union[int, str]]],
+                    'years': Optional[Union[int, str, List[int]]],
                         },
                 'return': pd.DataFrame, },
              get_population_structure: {
-                 'parameters': {'location': str},
+                 'parameters': {'location': Union[int, str, List[Union[int, str]]], 'years': Optional[Union[int, str, List[int]]]},
                  'return': pd.DataFrame, },
              get_theoretical_minimum_risk_life_expectancy: {
                  'parameters': {},
                  'return': pd.DataFrame, },
              get_age_bins: {
                  'parameters': {},
                  'return': pd.DataFrame, },
              get_demographic_dimensions: {
-                 'parameters': {'location': str},
+                 'parameters': {'location': Union[int, str, List[Union[int, str]]], 'years': Optional[Union[int, str, List[int]]]},
                  'return': pd.DataFrame, },
              get_raw_data: {
-                 'parameters': {'entity': ModelableEntity, 'measure': str, 'location': str},
+                 'parameters': {
+                    'entity': ModelableEntity,
+                    'measure': str,
+                    'location': Union[int, str, List[Union[int, str]]],
+                    'years': Optional[Union[int, str, List[int]]],
+                        },
                 'return': Union[pd.DataFrame, pd.Series], },
              }
     for func, spec in funcs.items():
         sig = inspect.signature(func)
         assert len(sig.parameters) == len(spec['parameters'])
         for name, annotation in spec['parameters'].items():
             assert name in sig.parameters
```

### Comparing `vivarium_inputs-4.1.3/setup.py` & `vivarium_inputs-5.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,30 +18,30 @@
         "numpy",
         "scipy",
         "pandas",
         "click",
         "joblib",
         "tables",
         "vivarium>=1.2.1",
-        "gbd_mapping>=3.1.0, <4.0.0",
+        "gbd_mapping>=4.0.0, <5.0.0",
         "loguru",
     ]
 
     setup_requires = ["setuptools_scm"]
 
-    data_requires = ["vivarium-gbd-access>=3.0.7, <4.0.0", "core-maths"]
+    data_requires = ["vivarium-gbd-access>=4.0.0, <5.0.0", "core-maths"]
 
     test_requirements = [
         "pytest",
         "pytest-mock",
         "hypothesis",
     ]
 
     doc_requirements = [
-        "sphinx>=6.2.1, <7.0",
+        "sphinx>=7.0, <8.0",
         "sphinx-rtd-theme",
     ]
 
     setup(
         name=about["__title__"],
         description=about["__summary__"],
         long_description=long_description,
```

### Comparing `vivarium_inputs-4.1.3/src/vivarium_inputs/core.py` & `vivarium_inputs-5.0.0/src/vivarium_inputs/core.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 from itertools import product
-from typing import Union
+from typing import List, Optional, Union
 
 import numpy as np
 import pandas as pd
-from gbd_mapping import Cause, Covariate, Etiology, RiskFactor, Sequela, causes
+from gbd_mapping import (
+    Cause,
+    Covariate,
+    Etiology,
+    ModelableEntity,
+    RiskFactor,
+    Sequela,
+    causes,
+)
 from loguru import logger
 
 from vivarium_inputs import extract, utilities, utility_data
 from vivarium_inputs.globals import (
     COVARIATE_VALUE_COLUMNS,
     DEMOGRAPHIC_COLUMNS,
     DISTRIBUTION_COLUMNS,
     DRAW_COLUMNS,
     EXTRA_RESIDUAL_CATEGORY,
     MEASURES,
     MINIMUM_EXPOSURE_VALUE,
     DataDoesNotExistError,
     InvalidQueryError,
     Population,
+    gbd,
 )
 from vivarium_inputs.mapping_extension import AlternativeRiskFactor, HealthcareEntity
 
 
-def get_data(entity, measure: str, location: Union[str, int], **get_draws_kwargs):
+def get_data(
+    entity: ModelableEntity,
+    measure: str,
+    location: Union[str, int, List[Union[str, int]]],
+    years: Optional[Union[int, str, List[int]]] = None,
+):
     measure_handlers = {
         # Cause-like measures
         "incidence_rate": (get_incidence_rate, ("cause", "sequela")),
         "raw_incidence_rate": (get_raw_incidence_rate, ("cause", "sequela")),
         "prevalence": (get_prevalence, ("cause", "sequela")),
         "birth_prevalence": (get_birth_prevalence, ("cause", "sequela")),
         "disability_weight": (get_disability_weight, ("cause", "sequela")),
@@ -71,18 +85,25 @@
         raise InvalidQueryError(f"No functions available to pull data for measure {measure}.")
 
     handler, entity_types = measure_handlers[measure]
 
     if entity.kind not in entity_types:
         raise InvalidQueryError(f"{measure.capitalize()} not available for {entity.kind}.")
 
-    location_id = (
-        utility_data.get_location_id(location) if isinstance(location, str) else location
-    )
-    data = handler(entity, location_id, **get_draws_kwargs)
+    if isinstance(location, list):
+        location_id = [
+            utility_data.get_location_id(loc) if isinstance(loc, str) else loc
+            for loc in location
+        ]
+    else:
+        location_id = [
+            utility_data.get_location_id(location) if isinstance(location, str) else location
+        ]
+
+    data = handler(entity, location_id, years)
 
     if measure in [
         "structure",
         "theoretical_minimum_risk_life_expectancy",
         "estimate",
         "exposure_distribution_weights",
     ]:
@@ -91,139 +112,241 @@
         value_cols = DRAW_COLUMNS
 
     data = utilities.reshape(data, value_cols=value_cols)
 
     return data
 
 
-def get_raw_incidence_rate(entity: Union[Cause, Sequela], location_id: int) -> pd.DataFrame:
-    data = extract.extract_data(entity, "incidence_rate", location_id)
+def get_raw_incidence_rate(
+    entity: Union[Cause, Sequela],
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
+    data = extract.extract_data(
+        entity,
+        "incidence_rate",
+        location_id,
+        validate=True,
+        years=years,
+    )
     if entity.kind == "cause":
         restrictions_entity = entity
     else:  # sequela
         cause = [c for c in causes if c.sequelae and entity in c.sequelae][0]
         restrictions_entity = cause
 
     data = utilities.filter_data_by_restrictions(
         data, restrictions_entity, "yld", utility_data.get_age_group_ids()
     )
     data = utilities.normalize(data, fill_value=0)
     data = data.filter(DEMOGRAPHIC_COLUMNS + DRAW_COLUMNS)
     return data
 
 
-def get_incidence_rate(entity: Union[Cause, Sequela], location_id: int) -> pd.DataFrame:
-    data = get_data(entity, "raw_incidence_rate", location_id)
-    prevalence = get_data(entity, "prevalence", location_id)
+def get_incidence_rate(
+    entity: Union[Cause, Sequela],
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
+    data = get_data(
+        entity,
+        "raw_incidence_rate",
+        location_id,
+        years=years,
+    )
+    prevalence = get_data(entity, "prevalence", location_id, years=years)
     # Convert from "True incidence" to the incidence rate among susceptibles
     data /= 1 - prevalence
     return data.fillna(0)
 
 
-def get_prevalence(entity: Union[Cause, Sequela], location_id: int) -> pd.DataFrame:
-    data = extract.extract_data(entity, "prevalence", location_id)
+def get_prevalence(
+    entity: Union[Cause, Sequela],
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
+    data = extract.extract_data(
+        entity,
+        "prevalence",
+        location_id,
+        validate=True,
+        years=years,
+    )
     if entity.kind == "cause":
         restrictions_entity = entity
     else:  # sequela
         cause = [c for c in causes if c.sequelae and entity in c.sequelae][0]
         restrictions_entity = cause
 
     data = utilities.filter_data_by_restrictions(
         data, restrictions_entity, "yld", utility_data.get_age_group_ids()
     )
     data = utilities.normalize(data, fill_value=0)
     data = data.filter(DEMOGRAPHIC_COLUMNS + DRAW_COLUMNS)
     return data
 
 
-def get_birth_prevalence(entity: Union[Cause, Sequela], location_id: int) -> pd.DataFrame:
-    data = extract.extract_data(entity, "birth_prevalence", location_id)
-    data = data.filter(["year_id", "sex_id", "location_id"] + DRAW_COLUMNS)
+def get_birth_prevalence(
+    entity: Union[Cause, Sequela],
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
+    data = extract.extract_data(
+        entity,
+        "birth_prevalence",
+        location_id,
+        validate=True,
+        years=years,
+    )
+    data = data.filter(["years", "sex_id", "location_id"] + DRAW_COLUMNS)
     data = utilities.normalize(data, fill_value=0)
     return data
 
 
-def get_disability_weight(entity: Union[Cause, Sequela], location_id: int) -> pd.DataFrame:
+def get_disability_weight(
+    entity: Union[Cause, Sequela],
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
     if entity.kind == "cause":
-        data = utility_data.get_demographic_dimensions(location_id, draws=True, value=0.0)
+        data = utility_data.get_demographic_dimensions(
+            location_id, draws=True, value=0.0, years=years
+        )
         data = data.set_index(
             utilities.get_ordered_index_cols(data.columns.difference(DRAW_COLUMNS))
         )
         if entity.sequelae:
             for sequela in entity.sequelae:
                 try:
-                    prevalence = get_data(sequela, "prevalence", location_id)
+                    prevalence = get_data(
+                        sequela,
+                        "prevalence",
+                        location_id,
+                        years=years,
+                    )
                 except DataDoesNotExistError:
                     # sequela prevalence does not exist so no point continuing with this sequela
                     continue
-                disability = get_data(sequela, "disability_weight", location_id)
-                disability.index = disability.index.set_levels(
-                    [location_id], level="location_id"
+                disability = get_data(
+                    sequela,
+                    "disability_weight",
+                    location_id,
+                    years=years,
                 )
                 data += prevalence * disability
-        cause_prevalence = get_data(entity, "prevalence", location_id)
+        cause_prevalence = get_data(entity, "prevalence", location_id, years=years)
         data = (data / cause_prevalence).fillna(0).reset_index()
     else:  # entity.kind == 'sequela'
         try:
-            data = extract.extract_data(entity, "disability_weight", location_id)
+            data = extract.extract_data(
+                entity,
+                "disability_weight",
+                location_id,
+                validate=True,
+                years=years,
+            )
             data = utilities.normalize(data)
+
             cause = [c for c in causes if c.sequelae and entity in c.sequelae][0]
             data = utilities.clear_disability_weight_outside_restrictions(
                 data, cause, 0.0, utility_data.get_age_group_ids()
             )
             data = data.filter(DEMOGRAPHIC_COLUMNS + DRAW_COLUMNS)
         except (IndexError, DataDoesNotExistError):
             logger.warning(
                 f"{entity.name.capitalize()} has no disability weight data. All values will be 0."
             )
-            data = utility_data.get_demographic_dimensions(location_id, draws=True, value=0.0)
+            data = utility_data.get_demographic_dimensions(
+                location_id, draws=True, value=0.0, years=years
+            )
     return data
 
 
-def get_remission_rate(entity: Cause, location_id: int) -> pd.DataFrame:
-    data = extract.extract_data(entity, "remission_rate", location_id)
-
+def get_remission_rate(
+    entity: Cause,
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
+    data = extract.extract_data(
+        entity,
+        "remission_rate",
+        location_id,
+        validate=True,
+        years=years,
+    )
     data = utilities.filter_data_by_restrictions(
         data, entity, "yld", utility_data.get_age_group_ids()
     )
     data = utilities.normalize(data, fill_value=0)
     data = data.filter(DEMOGRAPHIC_COLUMNS + DRAW_COLUMNS)
     return data
 
 
-def get_cause_specific_mortality_rate(entity: Cause, location_id: int) -> pd.DataFrame:
-    deaths = get_data(entity, "deaths", location_id)  # population isn't by draws
-    pop = get_data(Population(), "structure", location_id)
+def get_cause_specific_mortality_rate(
+    entity: Cause,
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
+    deaths = get_data(entity, "deaths", location_id, years=years)
+    # population isn't by draws
+    pop = get_data(Population(), "structure", location_id, years=years)
     data = deaths.join(pop, lsuffix="_deaths", rsuffix="_pop")
     data[DRAW_COLUMNS] = data[DRAW_COLUMNS].divide(data.value, axis=0)
     return data.drop(["value"], axis="columns")
 
 
-def get_excess_mortality_rate(entity: Cause, location_id: int) -> pd.DataFrame:
-    csmr = get_data(entity, "cause_specific_mortality_rate", location_id)
-    prevalence = get_data(entity, "prevalence", location_id)
+def get_excess_mortality_rate(
+    entity: Cause,
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
+    csmr = get_data(
+        entity,
+        "cause_specific_mortality_rate",
+        location_id,
+        years=years,
+    )
+    prevalence = get_data(entity, "prevalence", location_id, years=years)
     data = (csmr / prevalence).fillna(0)
     data = data.replace([np.inf, -np.inf], 0)
     return data
 
 
-def get_deaths(entity: Cause, location_id: int) -> pd.DataFrame:
-    data = extract.extract_data(entity, "deaths", location_id)
+def get_deaths(
+    entity: Cause,
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
+    data = extract.extract_data(
+        entity,
+        "deaths",
+        location_id,
+        validate=True,
+        years=years,
+    )
     data = utilities.filter_data_by_restrictions(
         data, entity, "yll", utility_data.get_age_group_ids()
     )
     data = utilities.normalize(data, fill_value=0)
     data = data.filter(DEMOGRAPHIC_COLUMNS + DRAW_COLUMNS)
     return data
 
 
 def get_exposure(
-    entity: Union[RiskFactor, AlternativeRiskFactor], location_id: int, **get_draws_kwargs
+    entity: Union[RiskFactor, AlternativeRiskFactor],
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
 ) -> pd.DataFrame:
-    data = extract.extract_data(entity, "exposure", location_id, **get_draws_kwargs)
+    data = extract.extract_data(
+        entity,
+        "exposure",
+        location_id,
+        validate=True,
+        years=years,
+    )
     data = data.drop("modelable_entity_id", "columns")
 
     if entity.name in EXTRA_RESIDUAL_CATEGORY:
         cat = EXTRA_RESIDUAL_CATEGORY[entity.name]
         data = data.drop(labels=data.query("parameter == @cat").index)
         data[DRAW_COLUMNS] = data[DRAW_COLUMNS].clip(lower=MINIMUM_EXPOSURE_VALUE)
 
@@ -257,100 +380,147 @@
     else:
         data = utilities.normalize(data, fill_value=0)
     data = data.filter(DEMOGRAPHIC_COLUMNS + DRAW_COLUMNS + ["parameter"])
     return data
 
 
 def get_exposure_standard_deviation(
-    entity: Union[RiskFactor, AlternativeRiskFactor], location_id: int
+    entity: Union[RiskFactor, AlternativeRiskFactor],
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
 ) -> pd.DataFrame:
-    data = extract.extract_data(entity, "exposure_standard_deviation", location_id)
+    data = extract.extract_data(
+        entity,
+        "exposure_standard_deviation",
+        location_id,
+        validate=True,
+        years=years,
+    )
     data = data.drop("modelable_entity_id", "columns")
 
-    exposure = extract.extract_data(entity, "exposure", location_id)
+    exposure = extract.extract_data(
+        entity,
+        "exposure",
+        location_id,
+        validate=True,
+        years=years,
+    )
     valid_age_groups = utilities.get_exposure_and_restriction_ages(exposure, entity)
     data = data[data.age_group_id.isin(valid_age_groups)]
 
     data = utilities.normalize(data, fill_value=0)
     data = data.filter(DEMOGRAPHIC_COLUMNS + DRAW_COLUMNS)
     return data
 
 
 def get_exposure_distribution_weights(
-    entity: Union[RiskFactor, AlternativeRiskFactor], location_id: int
+    entity: Union[RiskFactor, AlternativeRiskFactor],
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
 ) -> pd.DataFrame:
-    data = extract.extract_data(entity, "exposure_distribution_weights", location_id)
+    data = extract.extract_data(
+        entity,
+        "exposure_distribution_weights",
+        location_id,
+        validate=True,
+        years=years,
+    )
 
-    exposure = extract.extract_data(entity, "exposure", location_id)
+    exposure = extract.extract_data(
+        entity,
+        "exposure",
+        location_id,
+        validate=True,
+        years=years,
+    )
     valid_ages = utilities.get_exposure_and_restriction_ages(exposure, entity)
 
     data.drop("age_group_id", axis=1, inplace=True)
     df = []
     for age_id in valid_ages:
         copied = data.copy()
         copied["age_group_id"] = age_id
         df.append(copied)
     data = pd.concat(df)
     data = utilities.normalize(data, fill_value=0, cols_to_fill=DISTRIBUTION_COLUMNS)
+    if years != "all":
+        if years:
+            data = data.query(f"year_id=={years}")
+        else:
+            most_recent_year = gbd.get_most_recent_year()
+            data = data.query(f"year_id=={most_recent_year}")
     data = data.filter(DEMOGRAPHIC_COLUMNS + DISTRIBUTION_COLUMNS)
     data = utilities.wide_to_long(data, DISTRIBUTION_COLUMNS, var_name="parameter")
     return data
 
 
 def filter_relative_risk_to_cause_restrictions(data: pd.DataFrame) -> pd.DataFrame:
     """It applies age restrictions according to affected causes
     and affected measures. If affected measure is incidence_rate,
     it applies the yld_age_restrictions. If affected measure is
     excess_mortality_rate, it applies the yll_age_restrictions to filter
     the relative_risk data"""
 
+    age_bins = utility_data.get_age_bins()
+    ordered_age_ids = age_bins["age_group_id"].values
     causes_map = {c.name: c for c in causes}
     temp = []
     affected_entities = set(data.affected_entity)
     affected_measures = set(data.affected_measure)
     for cause, measure in product(affected_entities, affected_measures):
         df = data[(data.affected_entity == cause) & (data.affected_measure == measure)]
         cause = causes_map[cause]
-        if measure == "excess_mortality_rate":
+        if measure == "cause_specific_mortality_rate":
             start, end = utilities.get_age_group_ids_by_restriction(cause, "yll")
         else:  # incidence_rate
             start, end = utilities.get_age_group_ids_by_restriction(cause, "yld")
-        temp.append(df[df.age_group_id.isin(range(start, end + 1))])
+        start_index = list(ordered_age_ids).index(start)
+        end_index = list(ordered_age_ids).index(end)
+        allowed_ids = ordered_age_ids[start_index : (end_index + 1)]
+        temp.append(df[df.age_group_id.isin(allowed_ids)])
     data = pd.concat(temp)
     return data
 
 
-def get_relative_risk(entity: RiskFactor, location_id: int) -> pd.DataFrame:
-    data = extract.extract_data(entity, "relative_risk", location_id)
+def get_relative_risk(
+    entity: RiskFactor,
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
+    data = extract.extract_data(
+        entity,
+        "relative_risk",
+        location_id,
+        validate=True,
+        years=years,
+    )
 
     # FIXME: we don't currently support yll-only causes so I'm dropping them because the data in some cases is
     #  very messed up, with mort = morb = 1 (e.g., aortic aneurysm in the RR data for high systolic bp) -
     #  2/8/19 K.W.
     yll_only_causes = set([c.gbd_id for c in causes if c.restrictions.yll_only])
     data = data[~data.cause_id.isin(yll_only_causes)]
 
     data = utilities.convert_affected_entity(data, "cause_id")
     morbidity = data.morbidity == 1
     mortality = data.mortality == 1
     data.loc[morbidity & mortality, "affected_measure"] = "incidence_rate"
     data.loc[morbidity & ~mortality, "affected_measure"] = "incidence_rate"
-    data.loc[~morbidity & mortality, "affected_measure"] = "excess_mortality_rate"
+    data.loc[~morbidity & mortality, "affected_measure"] = "cause_specific_mortality_rate"
     data = filter_relative_risk_to_cause_restrictions(data)
-
     data = data.filter(
         DEMOGRAPHIC_COLUMNS
         + ["affected_entity", "affected_measure", "parameter"]
         + DRAW_COLUMNS
     )
     data = (
         data.groupby(["affected_entity", "parameter"])
         .apply(utilities.normalize, fill_value=1)
         .reset_index(drop=True)
     )
-
     if entity.distribution in ["dichotomous", "ordered_polytomous", "unordered_polytomous"]:
         tmrel_cat = utility_data.get_tmrel_category(entity)
         tmrel_mask = data.parameter == tmrel_cat
         data.loc[tmrel_mask, DRAW_COLUMNS] = data.loc[tmrel_mask, DRAW_COLUMNS].mask(
             np.isclose(data.loc[tmrel_mask, DRAW_COLUMNS], 1.0), 1.0
         )
 
@@ -363,20 +533,34 @@
     #  We presume all attributable mortality moves through incidence.
     if set(rr.mortality) == {1} and set(rr.morbidity) == {1}:
         df = df[df.measure_id == MEASURES["YLDs"]]
     return df
 
 
 def get_population_attributable_fraction(
-    entity: Union[RiskFactor, Etiology], location_id: int
+    entity: Union[RiskFactor, Etiology],
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
 ) -> pd.DataFrame:
     causes_map = {c.gbd_id: c for c in causes}
     if entity.kind == "risk_factor":
-        data = extract.extract_data(entity, "population_attributable_fraction", location_id)
-        relative_risk = extract.extract_data(entity, "relative_risk", location_id)
+        data = extract.extract_data(
+            entity,
+            "population_attributable_fraction",
+            location_id,
+            validate=True,
+            years=years,
+        )
+        relative_risk = extract.extract_data(
+            entity,
+            "relative_risk",
+            location_id,
+            validate=True,
+            years=years,
+        )
 
         # FIXME: we don't currently support yll-only causes so I'm dropping them because the data in some cases is
         #  very messed up, with mort = morb = 1 (e.g., aortic aneurysm in the RR data for high systolic bp) -
         #  2/8/19 K.W.
         yll_only_causes = set([c.gbd_id for c in causes if c.restrictions.yll_only])
         data = data[~data.cause_id.isin(yll_only_causes)]
         relative_risk = relative_risk[~relative_risk.cause_id.isin(yll_only_causes)]
@@ -396,15 +580,19 @@
                 df, cause, measure, utility_data.get_age_group_ids()
             )
             temp.append(df)
         data = pd.concat(temp, ignore_index=True)
 
     else:  # etiology
         data = extract.extract_data(
-            entity, "etiology_population_attributable_fraction", location_id
+            entity,
+            "etiology_population_attributable_fraction",
+            location_id,
+            validate=True,
+            years=years,
         )
         cause = [c for c in causes if entity in c.etiologies][0]
         data = utilities.filter_data_by_restrictions(
             data, cause, "inner", utility_data.get_age_group_ids()
         )
         if np.any(data[DRAW_COLUMNS] < 0):
             logger.warning(
@@ -426,56 +614,90 @@
     )
     data = data.filter(
         DEMOGRAPHIC_COLUMNS + ["affected_entity", "affected_measure"] + DRAW_COLUMNS
     )
     return data
 
 
-def get_estimate(entity: Covariate, location_id: int) -> pd.DataFrame:
-    data = extract.extract_data(entity, "estimate", location_id)
+def get_estimate(
+    entity: Covariate,
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
+    data = extract.extract_data(
+        entity,
+        "estimate",
+        location_id,
+        validate=True,
+        years=years,
+    )
 
     key_columns = ["location_id", "year_id"]
     if entity.by_age:
         key_columns.append("age_group_id")
     if entity.by_sex:
         key_columns.append("sex_id")
 
     data = data.filter(key_columns + COVARIATE_VALUE_COLUMNS)
     data = utilities.normalize(data)
     data = utilities.wide_to_long(data, COVARIATE_VALUE_COLUMNS, var_name="parameter")
     return data
 
 
-def get_utilization_rate(entity: HealthcareEntity, location_id: int) -> pd.DataFrame:
+def get_utilization_rate(entity: HealthcareEntity, location_id: List[int]) -> pd.DataFrame:
     data = extract.extract_data(entity, "utilization_rate", location_id)
     data = utilities.normalize(data, fill_value=0)
     data = data.filter(DEMOGRAPHIC_COLUMNS + DRAW_COLUMNS)
     return data
 
 
-def get_structure(entity: Population, location_id: int) -> pd.DataFrame:
-    data = extract.extract_data(entity, "structure", location_id)
+def get_structure(
+    entity: Population,
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
+    data = extract.extract_data(
+        entity,
+        "structure",
+        location_id,
+        validate=True,
+        years=years,
+    )
     data = data.drop("run_id", axis="columns").rename(columns={"population": "value"})
     data = utilities.normalize(data)
     return data
 
 
 def get_theoretical_minimum_risk_life_expectancy(
-    entity: Population, location_id: int
+    entity: Population,
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
 ) -> pd.DataFrame:
     data = extract.extract_data(
-        entity, "theoretical_minimum_risk_life_expectancy", location_id
+        entity,
+        "theoretical_minimum_risk_life_expectancy",
+        location_id,
+        validate=True,
+        years=years,
     )
     data = data.rename(columns={"age": "age_start", "life_expectancy": "value"})
     data["age_end"] = data.age_start.shift(-1).fillna(125.0)
     return data
 
 
-def get_age_bins(entity: Population, location_id: int) -> pd.DataFrame:
+def get_age_bins(
+    entity: Population,
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
     age_bins = utility_data.get_age_bins()[["age_group_name", "age_start", "age_end"]]
     return age_bins
 
 
-def get_demographic_dimensions(entity: Population, location_id: int) -> pd.DataFrame:
-    demographic_dimensions = utility_data.get_demographic_dimensions(location_id)
+def get_demographic_dimensions(
+    entity: Population,
+    location_id: List[int],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
+    demographic_dimensions = utility_data.get_demographic_dimensions(location_id, years=years)
     demographic_dimensions = utilities.normalize(demographic_dimensions)
     return demographic_dimensions
```

### Comparing `vivarium_inputs-4.1.3/src/vivarium_inputs/globals.py` & `vivarium_inputs-5.0.0/src/vivarium_inputs/globals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 """Global constants, errors, and module imports for inputs processing."""
+
 from gbd_mapping import ModelableEntity, causes, risk_factors
 
 # The purpose of this import block is to mask the dependency on internal
 # IHME data and allow CI and automated testing to work.
 try:
     from vivarium_gbd_access import gbd
 
     try:
-        from gbd_artifacts.exceptions import NoBestVersionError
         from get_draws.api import EmptyDataFrameException, InputsException
+        from get_draws.base.exceptions import NoBestVersionsException
     except ModuleNotFoundError:
-        raise RuntimeError("Problem importing gbd_artifacts.exceptions or get_draws.api.")
+        raise RuntimeError("Problem importing get_draws.base.exceptions or get_draws.api.")
 
 except ModuleNotFoundError:
 
     class GbdDummy:
         """Mock class to wrap internal dependency."""
 
         def __getattr__(self, item):
             raise ModuleNotFoundError("Required package vivarium_gbd_access not found.")
 
     gbd = GbdDummy()
 
-    class NoBestVersionError(Exception):
+    class NoBestVersionsException(Exception):
         """Mock class for gbd exception"""
 
         pass
 
     class EmptyDataFrameException(Exception):
         """Mock class for gbd exception"""
 
@@ -126,14 +127,17 @@
     "Susceptible incidence": 41,
     "Total incidence": 42,
     "HAQ Index (Healthcare Access and Quality Index)": 43,
     "Population": 44,
     "Fertility": 45,
 }
 
+# Number of draw columns
+NUM_DRAWS = 500
+
 # List of standard distribution columns
 DISTRIBUTION_COLUMNS = [
     "exp",
     "gamma",
     "invgamma",
     "llogis",
     "gumbel",
@@ -147,15 +151,15 @@
     "mgumbel",
 ]
 # List of standard covariate values
 COVARIATE_VALUE_COLUMNS = ["mean_value", "upper_value", "lower_value"]
 # List of standard demographic id column names.
 DEMOGRAPHIC_COLUMNS = ["location_id", "sex_id", "age_group_id", "year_id"]
 # List of standard GBD draw column names.
-DRAW_COLUMNS = [f"draw_{i}" for i in range(1000)]
+DRAW_COLUMNS = [f"draw_{i}" for i in range(NUM_DRAWS)]
 # Mapping of GBD sex ids
 SEXES = {"Male": 1, "Female": 2, "Combined": 3}
 # Mapping of non-standard age group ids sometimes found in GBD data
 SPECIAL_AGES = {"all_ages": 22, "age_standardized": 27}
 
 # Cause-risk pair where risk may have a protective effect on a certain cause with negative paf
 PROTECTIVE_CAUSE_RISK_PAIRS = {
```

### Comparing `vivarium_inputs-4.1.3/src/vivarium_inputs/interface.py` & `vivarium_inputs-5.0.0/src/vivarium_inputs/interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 """Access to vivarium simulation input data."""
-from typing import Union
+from typing import List, Optional, Union
 
 import pandas as pd
 from gbd_mapping import ModelableEntity
 
 import vivarium_inputs.validation.sim as validation
 from vivarium_inputs import core, extract, utilities, utility_data
 from vivarium_inputs.globals import Population
 
 
 def get_measure(
-    entity: ModelableEntity, measure: str, location: str, **get_draws_kwargs
+    entity: ModelableEntity,
+    measure: str,
+    location: Union[int, str, List[Union[int, str]]],
+    years: Optional[Union[int, str, List[int]]] = None,
 ) -> pd.DataFrame:
     """Pull GBD data for measure and entity and prep for simulation input,
     including scrubbing all GBD conventions to replace IDs with meaningful
     values or ranges and expanding over all demographic dimensions. To pull data
     using this function, please have at least 50GB of memory available.
 
     Available measures:
@@ -43,52 +46,62 @@
     ----------
     entity
         Entity for which to pull `measure`.
     measure
         Measure for which to pull data, should be a measure available for the
         kind of entity which `entity` is.
     location
-        Location for which to pull data.
+        Location for which to pull data. This can be a location id as an int, the location name
+        as a string, or a list of these two data types.
+    years
+        Years for which to extract data. If None, get most recent year. If 'all',
+        get all available data. Defaults to None.
 
     Returns
     -------
     pandas.DataFrame
         Dataframe standardized to the format expected by `vivarium` simulations.
 
     """
-    data = core.get_data(entity, measure, location, **get_draws_kwargs)
+    data = core.get_data(entity, measure, location, years)
     data = utilities.scrub_gbd_conventions(data, location)
-    validation.validate_for_simulation(data, entity, measure, location)
+    validation.validate_for_simulation(data, entity, measure, location, years)
     data = utilities.split_interval(data, interval_column="age", split_column_prefix="age")
     data = utilities.split_interval(data, interval_column="year", split_column_prefix="year")
     return utilities.sort_hierarchical_data(data)
 
 
-def get_population_structure(location: str) -> pd.DataFrame:
+def get_population_structure(
+    location: Union[int, str, List[Union[int, str]]],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
     """Pull GBD population data for the given location and standardize to the
     expected simulation input format, including scrubbing all GBD conventions
     to replace IDs with meaningful values or ranges and expanding over all
     demographic dimensions.
 
     Parameters
     ----------
     location
         Location for which to pull population data.
+    years
+        Years for which to extract data. If None, get most recent year. If 'all',
+        get all available data. Defaults to None.
 
     Returns
     -------
     pandas.DataFrame
         Dataframe of population data for `location`, standardized to the format
         expected by `vivarium` simulations.
 
     """
     pop = Population()
-    data = core.get_data(pop, "structure", location)
+    data = core.get_data(pop, "structure", location, years)
     data = utilities.scrub_gbd_conventions(data, location)
-    validation.validate_for_simulation(data, pop, "structure", location)
+    validation.validate_for_simulation(data, pop, "structure", location, years)
     data = utilities.split_interval(data, interval_column="age", split_column_prefix="age")
     data = utilities.split_interval(data, interval_column="year", split_column_prefix="year")
     return utilities.sort_hierarchical_data(data)
 
 
 def get_theoretical_minimum_risk_life_expectancy() -> pd.DataFrame:
     """Pull GBD theoretical minimum risk life expectancy data and standardize
@@ -129,41 +142,50 @@
     data = utilities.set_age_interval(data)
     validation.validate_for_simulation(data, pop, "age_bins", "Global")
     data = utilities.split_interval(data, interval_column="age", split_column_prefix="age")
     data = utilities.split_interval(data, interval_column="year", split_column_prefix="year")
     return utilities.sort_hierarchical_data(data)
 
 
-def get_demographic_dimensions(location: str) -> pd.DataFrame:
+def get_demographic_dimensions(
+    location: Union[int, str, List[Union[int, str]]],
+    years: Optional[Union[int, str, List[int]]] = None,
+) -> pd.DataFrame:
     """Pull the full demographic dimensions for GBD data, standardized to the
     expected simulation input format, including scrubbing all GBD conventions
-    to replace IDs with with meaningful values or ranges.
+    to replace IDs with meaningful values or ranges.
 
     Parameters
     ----------
     location
         Location for which to pull demographic dimension data.
+    years
+        Years for which to extract data. If None, get most recent year. If 'all',
+        get all available data. Defaults to None.
 
     Returns
     -------
     pandas.DataFrame
         Dataframe with age and year bins from GBD, sexes, and the given location.
 
     """
     pop = Population()
-    data = core.get_data(pop, "demographic_dimensions", location)
+    data = core.get_data(pop, "demographic_dimensions", location, years=years)
     data = utilities.scrub_gbd_conventions(data, location)
-    validation.validate_for_simulation(data, pop, "demographic_dimensions", location)
+    validation.validate_for_simulation(data, pop, "demographic_dimensions", location, years)
     data = utilities.split_interval(data, interval_column="age", split_column_prefix="age")
     data = utilities.split_interval(data, interval_column="year", split_column_prefix="year")
     return utilities.sort_hierarchical_data(data)
 
 
 def get_raw_data(
-    entity: ModelableEntity, measure: str, location: str
+    entity: ModelableEntity,
+    measure: str,
+    location: Union[int, str, List[Union[int, str]]],
+    years: Optional[Union[int, str, List[int]]] = None,
 ) -> Union[pd.Series, pd.DataFrame]:
     """Pull raw data from GBD for the requested entity, measure, and location.
     Skip standard raw validation checks in order to return data that can be
     investigated for oddities. The only filter that occurs is by applicable
     measure id, metric id, or to most detailed causes where relevant.
 
     Available measures:
@@ -195,17 +217,30 @@
     ----------
     entity
         Entity for which to extract data.
     measure
         Measure for which to extract data.
     location
         Location for which to extract data.
+    years
+        Years for which to extract data. If None, get most recent year. If 'all',
+        get all available data. Defaults to None.
 
     Returns
     -------
     Union[pandas.Series, pandas.DataFrame]
         Data for the entity-measure pair and specific location requested, with no
         formatting or reshaping.
     """
-    location_id = utility_data.get_location_id(location)
-    data = extract.extract_data(entity, measure, location_id, validate=False)
+    if not isinstance(location, list):
+        location = [location]
+    location_id = [
+        utility_data.get_location_id(loc) if isinstance(loc, str) else loc for loc in location
+    ]
+    data = extract.extract_data(
+        entity,
+        measure,
+        location_id,
+        validate=False,
+        years=years,
+    )
     return data
```

### Comparing `vivarium_inputs-4.1.3/src/vivarium_inputs/mapping_extension/alternative_risk_factor.py` & `vivarium_inputs-5.0.0/src/vivarium_inputs/mapping_extension/alternative_risk_factor.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/src/vivarium_inputs/mapping_extension/alternative_risk_factor_template.py` & `vivarium_inputs-5.0.0/src/vivarium_inputs/mapping_extension/alternative_risk_factor_template.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/src/vivarium_inputs/mapping_extension/healthcare_entity_template.py` & `vivarium_inputs-5.0.0/src/vivarium_inputs/mapping_extension/healthcare_entity_template.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/src/vivarium_inputs/utilities.py` & `vivarium_inputs-5.0.0/src/vivarium_inputs/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Errors and utility functions for input processing."""
+
 from numbers import Real
 from typing import List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 from gbd_mapping import Cause, RiskFactor, causes, risk_factors
 
@@ -26,21 +27,29 @@
     data = scrub_sex(data)
     data = scrub_age(data)
     data = scrub_year(data)
     data = scrub_affected_entity(data)
     return data
 
 
-def scrub_location(data, location):
+def scrub_location(data: pd.DataFrame, location: Union[int, List[str]]) -> pd.DataFrame:
+    # Coerce location names
+    if not isinstance(location, list):
+        location = [location]
+    location = [
+        utility_data.get_location_name(loc) if isinstance(loc, int) else loc
+        for loc in location
+    ]
+
     if "location_id" in data.index.names:
         data.index = data.index.rename("location", level="location_id").set_levels(
-            [location], level="location"
+            location, level="location"
         )
     else:
-        data = pd.concat([data], keys=[location], names=["location"])
+        data = pd.concat([data], keys=location, names=["location"])
     return data
 
 
 def scrub_sex(data):
     if "sex_id" in data.index.names:
         levels = list(
             data.index.levels[data.index.names.index("sex_id")].map(
@@ -304,14 +313,15 @@
     elif which_age == "outer":
         start = get_restriction_age_boundary(entity, "start")
         end = get_restriction_age_boundary(entity, "end")
     else:
         raise NotImplementedError(
             "The second argument of this function should be one of [yll, yld, inner, outer]."
         )
+
     return start, end
 
 
 def filter_data_by_restrictions(
     data: pd.DataFrame,
     entity: Union[RiskFactor, Cause],
     which_age: str,
@@ -428,15 +438,15 @@
     Returns
     -------
         The age group id corresponding to the minimum or maximum start or end
         age restriction, depending on `boundary`, if both 'yll' and 'yld'
         restrictions exist. Otherwise, returns whichever restriction exists.
     """
     yld_age = entity.restrictions[f"yld_age_group_id_{boundary}"]
-    yll_age = entity.restrictions[f"yld_age_group_id_{boundary}"]
+    yll_age = entity.restrictions[f"yll_age_group_id_{boundary}"]
     if yld_age is None:
         age = yll_age
     elif yll_age is None:
         age = yld_age
     else:
         start_op = max if reverse else min
         end_op = min if reverse else max
@@ -489,7 +499,36 @@
                 x.left for x in data.index.levels[data.index.names.index(interval_column)]
             ]
             data.index = data.index.rename(
                 f"{split_column_prefix}_start", level=interval_column
             ).set_levels(interval_starts, level=f"{split_column_prefix}_start")
             data = data.set_index(f"{split_column_prefix}_end", append=True)
     return data
+
+
+def process_kidney_dysfunction_exposure(
+    data: pd.DataFrame,
+) -> pd.DataFrame:
+    """Process kidney dysfunction exposure (rei ID 341) given GBD data. GBD data gives two measures
+    and an inaccurate cat5 category. cat1, cat2, and cat3 are defined for measure 5 and cat4 for
+    measure 18, but we will say they are all from measure 5 (this only makes a difference in validation
+    and not within a simulation). There are cat5 values (the residual category) but they are calculated
+    separately for each measure and so are not accurate. We will drop these values and recalculate cat5."""
+    # drop cat5 data
+    data = data.loc[data["parameter"] != "cat5"]
+    # re-define remaining data as measure ID 5
+    data["measure_id"] = 5
+    # recalculate cat5
+    draw_cols = [col for col in data.columns if col.startswith("draw_")]
+    groupby_cols = [
+        col
+        for col in data.columns
+        if col not in draw_cols + ["parameter", "modelable_entity_id"]
+    ]
+    # calculate residual values with 1-(sum of other categories)
+    cat5_data = 1 - data.groupby(groupby_cols).sum()
+    cat5_data = cat5_data.reset_index()
+    cat5_data["parameter"] = "cat5"
+    cat5_data["modelable_entity_id"] = np.nan
+    cat5_data = cat5_data[data.columns]
+    data = pd.concat([data, cat5_data])
+    return data
```

### Comparing `vivarium_inputs-4.1.3/src/vivarium_inputs/utility_data.py` & `vivarium_inputs-5.0.0/src/vivarium_inputs/utility_data.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import List
+from typing import Dict, List, Optional, Union
 
 import pandas as pd
 from gbd_mapping import RiskFactor
 
-from vivarium_inputs.globals import NON_MAX_TMREL, SEXES, gbd
+from vivarium_inputs.globals import NON_MAX_TMREL, NUM_DRAWS, SEXES, gbd
 
 
 def get_estimation_years(*_, **__) -> pd.Series:
     data = gbd.get_estimation_years()
     return data
 
 
@@ -25,45 +25,68 @@
     return data
 
 
 def get_age_bins(*_, **__) -> pd.DataFrame:
     age_bins = gbd.get_age_bins()[
         ["age_group_id", "age_group_name", "age_group_years_start", "age_group_years_end"]
     ].rename(columns={"age_group_years_start": "age_start", "age_group_years_end": "age_end"})
+    age_bins = age_bins.sort_values("age_start").reset_index(drop=True)
     return age_bins
 
 
-def get_location_id(location_name):
+def get_location_id(location_name: str) -> int:
     return {r.location_name: r.location_id for _, r in gbd.get_location_ids().iterrows()}[
         location_name
     ]
 
 
-def get_location_id_parents(location_id: int) -> List[int]:
-    location_metadata = gbd.get_location_path_to_global().set_index("location_id")
-    parent_ids = [
-        int(loc) for loc in location_metadata.at[location_id, "path_to_top_parent"].split(",")
-    ]
+def get_location_name(location_id: int) -> str:
+    return {
+        row.location_id: row.location_name for _, row in gbd.get_location_ids().iterrows()
+    }[location_id]
+
+
+def get_location_id_parents(location_id: Union[int, List[int]]) -> Dict[int, List]:
+    if isinstance(location_id, int):
+        location_id = [location_id]
+    location_metadata = gbd.get_location_path_to_global()
+    parent_ids = (
+        location_metadata.loc[location_metadata.location_id.isin(location_id)]
+        .set_index("location_id")["path_to_top_parent"]
+        .str.split(",")
+        .to_dict()
+    )
+    # Coerce list of parent ids to integers
+    parent_ids = {loc_id: list(map(int, parents)) for loc_id, parents in parent_ids.items()}
+
     return parent_ids
 
 
 def get_demographic_dimensions(
-    location_id: int, draws: bool = False, value: float = None
+    location_id: Union[int, List[int]],
+    draws: bool = False,
+    value: float = None,
+    years: Optional[Union[int, str, List[int]]] = None,
 ) -> pd.DataFrame:
     ages = get_age_group_ids()
     estimation_years = get_estimation_years()
-    years = range(min(estimation_years), max(estimation_years) + 1)
+    if years == "all":
+        years = range(min(estimation_years), max(estimation_years) + 1)
+    else:
+        if years and years not in estimation_years:
+            raise ValueError(f"years must be in {estimation_years}. You provided {years}.")
+        years = [years] if years else [gbd.get_most_recent_year()]
     sexes = [SEXES["Male"], SEXES["Female"]]
-    location = [location_id]
+    location = [location_id] if isinstance(location_id, int) else location_id
     values = [location, sexes, ages, years]
     names = ["location_id", "sex_id", "age_group_id", "year_id"]
 
     data = pd.MultiIndex.from_product(values, names=names).to_frame(index=False)
     if draws:
-        for i in range(1000):
+        for i in range(NUM_DRAWS):
             data[f"draw_{i}"] = value
     return data
 
 
 def get_tmrel_category(entity: RiskFactor) -> str:
     if entity.name in NON_MAX_TMREL:
         tmrel_cat = NON_MAX_TMREL[entity.name]
```

### Comparing `vivarium_inputs-4.1.3/src/vivarium_inputs/validation/raw.py` & `vivarium_inputs-5.0.0/src/vivarium_inputs/validation/raw.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,14 +27,15 @@
     RISKS_WITH_NEGATIVE_PAF,
     SEXES,
     SPECIAL_AGES,
     DataAbnormalError,
     DataDoesNotExistError,
     InvalidQueryError,
     Population,
+    gbd,
 )
 from vivarium_inputs.mapping_extension import (
     AlternativeRiskFactor,
     HealthcareEntity,
     HealthTechnology,
 )
 from vivarium_inputs.utilities import (
@@ -45,15 +46,15 @@
 
 MAX_INCIDENCE = 10
 MAX_REMISSION = 365 / 3
 MAX_CATEG_REL_RISK = 20
 MAX_CONT_REL_RISK = 10
 MAX_PAF = 1
 MIN_PAF = 0
-MAX_POP = 663_000_000  # Number pulled from GBD global population largest 5 year age bin.
+MAX_POP = 695_000_000  # Number pulled from GBD global population largest 5 year age bin.
 MIN_PROTECTIVE_PAF = -1
 MAX_UTILIZATION = 50
 MAX_LIFE_EXP = 90
 
 
 class RawValidationContext:
     def __init__(self, location_id, **additional_data):
@@ -127,15 +128,15 @@
     metadata_checkers[entity.kind](entity, measure)
 
 
 def validate_raw_data(
     data: pd.DataFrame,
     entity: ModelableEntity,
     measure: str,
-    location_id: int,
+    location_id: Union[int, List[int]],
     **additional_data,
 ) -> None:
     """Validate data conforms to the format expected from raw GBD data, that all
     values are within expected ranges,
 
     The following checks are performed for each entity-measure pair (some may
     be excluded for certain pairs if not applicable):
@@ -204,14 +205,17 @@
         "structure": validate_structure,
         "theoretical_minimum_risk_life_expectancy": validate_theoretical_minimum_risk_life_expectancy,
     }
 
     if measure not in validators:
         raise InvalidQueryError(f"No raw validator found for {measure}.")
 
+    # Make location_id a list if not already
+    if not isinstance(location_id, list):
+        location_id = [location_id]
     context = RawValidationContext(location_id, **additional_data)
 
     validators[measure](data, entity, context)
 
 
 ##############################################
 #   CHECK METADATA ENTITY SPECIFIC METHODS   #
@@ -1566,15 +1570,15 @@
 
     """
     check_data_exist(data, zeros_missing=True, value_columns=["life_expectancy"])
 
     expected_columns = ["age", "life_expectancy"]
     check_columns(expected_columns, data.columns)
 
-    min_age, max_age = 0, 105
+    min_age, max_age = 0, 110
     if data.age.min() != min_age or data.age.max() != max_age:
         raise DataAbnormalError(
             f"Data does not contain life expectancy values for ages [{min_age}, {max_age}]."
         )
 
     check_value_columns_boundary(
         data,
@@ -1770,23 +1774,28 @@
         "YLDs": (rr.morbidity == 1),
     }
 
     measure = "YLLs" if measure_id == MEASURES["YLLs"] else "YLDs"
     valid_rr = rr[(rr.cause_id == cause.gbd_id) & rr_measures[measure]]
 
     if entity.distribution in ["ensemble", "lognormal", "normal"]:
-        tmrel = (entity.tmred.max + entity.tmred.min) / 2
+        if entity.tmred.distribution == "draws":
+            ## TODO: [MIC-5049] handle iron deficiency TMREL in VPH
+            pass
+        else:
+            tmrel = (entity.tmred.max + entity.tmred.min) / 2
 
-        #  Non-trivial rr for continuous risk factors is where exposure is bigger(smaller) than tmrel.
-        e_othercols = [c for c in exposure.columns if c not in DRAW_COLUMNS]
-        df = exposure.set_index(e_othercols)
-        op = operator.lt if entity.tmred.inverted else operator.gt
-        exposed_age_groups = set(df[op(df, tmrel)].reset_index().age_group_id)
+            #  Non-trivial rr for continuous risk factors is where exposure is bigger(smaller) than tmrel.
+            e_othercols = [c for c in exposure.columns if c not in DRAW_COLUMNS]
+            df = exposure.set_index(e_othercols)
+            op = operator.lt if entity.tmred.inverted else operator.gt
+            exposed_age_groups = set(df[op(df, tmrel)].reset_index().age_group_id)
+
+            valid_rr = valid_rr[valid_rr.age_group_id.isin(exposed_age_groups)]
 
-        valid_rr = valid_rr[valid_rr.age_group_id.isin(exposed_age_groups)]
         rr_age_groups = set(valid_rr.age_group_id)
 
     else:  # categorical distribution
         #  Non-trivial rr for categorical risk factors is where relative risk is not equal to 1.
         #  Since non-trivial rr is determined by rr itself and rr age_group_id set is guaranteed to be
         #  a subset of exposure age_group_id set, we do not check exposure here.
         rr_othercols = [c for c in rr.columns if c not in DRAW_COLUMNS]
@@ -1950,24 +1959,25 @@
     Raises
     ------
     DataAbnormalError
         If data contains multiple location ids or a location id other than the
         global or requested location id.
 
     """
-    if len(data["location_id"].unique()) > 1:
-        raise DataAbnormalError(f"Data contains multiple location ids.")
-
-    data_location_id = data["location_id"].unique()[0]
 
-    if data_location_id not in context["parent_locations"] + [context["location_id"]]:
-        raise DataAbnormalError(
-            f'Data pulled for {context["location_id"]} actually has location '
-            f"id {data_location_id}, which is not in its hierarchy."
-        )
+    data_location_ids = data["location_id"].unique()
+    parent_locations = [
+        loc for value in context["parent_locations"].values() for loc in value
+    ]
+    for location_id in data_location_ids:
+        if location_id not in context["location_id"] + parent_locations:
+            raise DataAbnormalError(
+                f"Data pulled for '{data_location_ids}' actually has location "
+                f"id {location_id}, which is not in its hierarchy."
+            )
 
 
 def check_columns(expected_cols: List, existing_cols: List) -> None:
     """Verify that the passed lists of columns match.
 
     Parameters
     ----------
@@ -2045,16 +2055,18 @@
     return True
 
 
 def _check_continuity(data_ages: set, all_ages: set) -> None:
     """Make sure data_ages is contiguous block in all_ages."""
     data_ages = list(data_ages)
     all_ages = list(all_ages)
-    all_ages.sort()
-    data_ages.sort()
+    age_bins = utility_data.get_age_bins()
+    id_to_age_map = dict(zip(age_bins.age_group_id, age_bins.age_start))
+    all_ages.sort(key=lambda id: id_to_age_map[id])
+    data_ages.sort(key=lambda id: id_to_age_map[id])
     if (
         all_ages[all_ages.index(data_ages[0]) : all_ages.index(data_ages[-1]) + 1]
         != data_ages
     ):
         raise DataAbnormalError(f"Data contains a non-contiguous age groups: {data_ages}.")
```

### Comparing `vivarium_inputs-4.1.3/src/vivarium_inputs/validation/shared.py` & `vivarium_inputs-5.0.0/src/vivarium_inputs/validation/shared.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/src/vivarium_inputs/validation/sim.py` & `vivarium_inputs-5.0.0/src/vivarium_inputs/validation/sim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Union
+from typing import Dict, List, Optional, Union
 
 import numpy as np
 import pandas as pd
 from gbd_mapping import (
     Cause,
     Covariate,
     Etiology,
@@ -16,14 +16,15 @@
 from vivarium_inputs.globals import (
     BOUNDARY_SPECIAL_CASES,
     DRAW_COLUMNS,
     PROTECTIVE_CAUSE_RISK_PAIRS,
     RISKS_WITH_NEGATIVE_PAF,
     DataTransformationError,
     Population,
+    gbd,
 )
 from vivarium_inputs.mapping_extension import (
     AlternativeRiskFactor,
     HealthcareEntity,
     HealthTechnology,
 )
 from vivarium_inputs.validation.shared import check_value_columns_boundary
@@ -49,23 +50,23 @@
 VALID_PAF_RANGE = (0.0, 1.0)
 VALID_PROTECTIVE_PAF_MIN = -1.0
 VALID_COST_RANGE = (0, {"healthcare_entity": 30_000, "health_technology": 50})
 # FIXME: bumping for Mexico (max utilization ~422) 9/12/19 - K.W.
 VALID_UTILIZATION_RANGE = (0, 500)
 VALID_POPULATION_RANGE = (
     0,
-    345_000_000,
+    360_000_000_000,
 )  # Upper bound pulled from GBD global population largest sex-age bin.
 VALID_LIFE_EXP_RANGE = (0, 90)
 
 SCRUBBED_DEMOGRAPHIC_COLUMNS = ["location", "sex", "age", "year"]
 
 
 class SimulationValidationContext:
-    def __init__(self, location, **additional_data):
+    def __init__(self, location: List[str], **additional_data):
         self.context_data = {"location": location}
         self.context_data.update(additional_data)
 
         if "years" not in self.context_data:
             self.context_data["years"] = utility_data.get_year_block()
         if "age_bins" not in self.context_data:
             self.context_data["age_bins"] = utility_data.get_age_bins()
@@ -74,15 +75,20 @@
         return self.context_data[key]
 
     def __setitem__(self, key, value):
         self.context_data[key] = value
 
 
 def validate_for_simulation(
-    data: pd.DataFrame, entity: ModelableEntity, measure: str, location: str, **context_args
+    data: pd.DataFrame,
+    entity: ModelableEntity,
+    measure: str,
+    location: Union[int, str, List[Union[int, str]]],
+    years: Optional[int] = None,
+    **context_args,
 ) -> None:
     """Validate data conforms to the format that is expected by the simulation
     and conforms to normal expectations for a measure.
 
     Data coming in to the simulation is expected to have a full demographic set
     in most instances, as well non-missing, non-infinite, reasonable data. This
     function enforces column names, the demographic extents, and expected
@@ -104,15 +110,19 @@
     data
         Data to be validated.
     entity
         The GBD Entity to which the data pertain.
     measure
         The measure to which the data pertain.
     location
-        The location to which the data pertain.
+        The location(s) to which the data pertain.
+    check_all_years
+        Flag indicating whether to validate that we have all years.
+        Otherwise, validate that data has most recent year.
+        Defaults to False.
     context_args
         Any data or information needed to construct the SimulationContext used
         by the individual entity-measure validator functions.
 
     Raises
     -------
     DataTransformationError
@@ -143,14 +153,32 @@
         "age_bins": validate_age_bins,
         "demographic_dimensions": validate_demographic_dimensions,
     }
 
     if measure not in validators:
         raise NotImplementedError()
 
+    if years != "all":
+        if years:
+            context_args["years"] = pd.DataFrame(
+                {"year_start": years, "year_end": years + 1}, index=[0]
+            )
+        else:
+            most_recent_year = gbd.get_most_recent_year()
+            context_args["years"] = pd.DataFrame(
+                {"year_start": most_recent_year, "year_end": most_recent_year + 1}, index=[0]
+            )
+
+    # Coerce to location names
+    if not isinstance(location, list):
+        location = [location]
+    location = [
+        utility_data.get_location_name(loc) if isinstance(loc, int) else loc
+        for loc in location
+    ]
     context = SimulationValidationContext(location, **context_args)
     validators[measure](data, entity, context)
 
 
 #########################################################
 #   VALIDATE SIM DATA ENTITY-MEASURE SPECIFIC METHODS   #
 # ----------------------------------------------------- #
@@ -530,29 +558,28 @@
         data,
         boundary_value=VALID_EXCESS_MORT_RANGE[0],
         boundary_type="lower",
         value_columns=DRAW_COLUMNS,
         error=DataTransformationError,
     )
 
-    if entity.name in BOUNDARY_SPECIAL_CASES["excess_mortality_rate"].get(
-        context["location"], {}
-    ):
-        max_val = BOUNDARY_SPECIAL_CASES["excess_mortality_rate"][context["location"]][
-            entity.name
-        ]
-    else:
-        max_val = VALID_EXCESS_MORT_RANGE[1]
-    check_value_columns_boundary(
-        data,
-        boundary_value=max_val,
-        boundary_type="upper",
-        value_columns=DRAW_COLUMNS,
-        error=DataTransformationError,
-    )
+    for location in context["location"]:
+        if entity.name in BOUNDARY_SPECIAL_CASES["excess_mortality_rate"].get(location, {}):
+            max_val = BOUNDARY_SPECIAL_CASES["excess_mortality_rate"][context["location"]][
+                entity.name
+            ]
+        else:
+            max_val = VALID_EXCESS_MORT_RANGE[1]
+        check_value_columns_boundary(
+            data,
+            boundary_value=max_val,
+            boundary_type="upper",
+            value_columns=DRAW_COLUMNS,
+            error=DataTransformationError,
+        )
 
     check_age_restrictions(data, entity, rest_type="yll", fill_value=0.0, context=context)
     check_sex_restrictions(
         data, entity.restrictions.male_only, entity.restrictions.female_only, fill_value=0.0
     )
 
 
@@ -1193,32 +1220,30 @@
     data: pd.DataFrame, entity: Population, context: SimulationValidationContext
 ) -> None:
     """Because the structure of life expectancy data is somewhat different,
     containing a custom age column that doesn't match the standard GBD age
     groups, this validator doesn't use the standard column checks. Instead, it
     verifies that the data has the correct age columns and that ages range from
     0 to 110 years. It checks that all life expectancy values are within the
-    expected range and ensures that life expectancy is monotonically decreasing
-    by age.
+    expected range.
 
     Parameters
     ----------
     data
         Simulation-prepped theoretical minimum risk life expectancy data.
     entity
         Entity to which the data pertain.
     context
         Wrapper for additional data used in the validation process.
 
     Raises
     ------
     DataTransformationError
         If age columns are incorrectly named or contain invalid values or if
-        any life expectancy values are outside the expected range or not
-        monotonically decreasing over age.
+        any life expectancy values are outside the expected range.
 
     """
     expected_index_names = ["age"]
     validate_expected_index_and_columns(
         expected_index_names, data.index.names, ["value"], data.columns
     )
 
@@ -1244,19 +1269,14 @@
         VALID_LIFE_EXP_RANGE[1],
         "upper",
         value_columns=["value"],
         inclusive=False,
         error=DataTransformationError,
     )
 
-    if not data.sort_values(by="age", ascending=False).value.is_monotonic:
-        raise DataTransformationError(
-            "Life expectancy data is not monotonically decreasing over age."
-        )
-
 
 def validate_age_bins(
     data: pd.DataFrame, entity: Population, context: SimulationValidationContext
 ) -> None:
     """With only age columns in this data, the validator is an abbreviated
     version employing only the standard column check on ages.
 
@@ -1421,17 +1441,30 @@
     ------
     DataTransformationError
         If 'location' column does not contain only the single location given
         in `context`.
 
     """
     data_locations = data.index.unique("location")
-    if len(data_locations) != 1 or data_locations[0] != context["location"]:
+    if not set(data_locations) == (set(context["location"])):
+        # Locations requested for extraction not found in data
+        missing_locations_in_data = set(context["location"]).difference(data_locations)
+        if missing_locations_in_data:
+            missing_error_message = (
+                f"Locations missing in data include '{missing_locations_in_data}'. "
+            )
+        # Locations found in data but not requested for extraction
+        extra_locations_in_data = set(data_locations).difference(context["location"])
+        if extra_locations_in_data:
+            extra_error_message = (
+                f"Extra locations found in data include '{extra_locations_in_data}'. "
+            )
         raise DataTransformationError(
-            "Location must contain a single value that matches specified location."
+            "Location(s) must match between data and SimulationValidationContext. "
+            f"{missing_error_message} + {extra_error_message}"
         )
 
 
 def validate_sex_column(data: pd.DataFrame) -> None:
     """Validate that sex index column in the data has the expected values.
 
     Parameters
@@ -1500,16 +1533,18 @@
     expected_years = [
         pd.Interval(row.year_start, row.year_end, closed="left")
         for _, row in context["years"].iterrows()
     ]
     data_years = data.index.levels[data.index.names.index("year")]
 
     if not sorted(data_years) == sorted(expected_years):
+        formatted_expected_years = [interval.left for interval in sorted(expected_years)]
+        formatted_data_years = [interval.left for interval in sorted(data_years)]
         raise DataTransformationError(
-            "Year_start and year_end must cover [1990, 2017] in intervals of one year."
+            f"Data was expected to contain years {formatted_expected_years}. The data provided contains years {formatted_data_years}."
         )
 
 
 def validate_value_column(data: pd.DataFrame) -> None:
     """Validate that value columns (i.e., any non-index columns) in the data
     have no missing values.
 
@@ -1563,17 +1598,21 @@
     ------
     DataTransformationError
         If any values other than fill_value are found in any non-index columns
         in data outside the restrictions of entity.
 
     """
     start_id, end_id = utilities.get_age_group_ids_by_restriction(entity, rest_type)
+
     age_bins = context["age_bins"]
+    id_to_age_start_map = dict(zip(age_bins.age_group_id, age_bins.age_start))
+    age_range_start = id_to_age_start_map[start_id]
+    age_range_end = id_to_age_start_map[end_id]
     in_range_ages = age_bins.loc[
-        (age_bins.age_group_id >= start_id) & (age_bins.age_group_id <= end_id)
+        (age_bins.age_start >= age_range_start) & (age_bins.age_start <= age_range_end)
     ]
     in_range_age_intervals = [
         pd.Interval(row.age_start, row.age_end, closed="left")
         for _, row in in_range_ages.iterrows()
     ]
     outside = data.loc[~data.index.isin(in_range_age_intervals, "age")]
```

### Comparing `vivarium_inputs-4.1.3/src/vivarium_inputs.egg-info/PKG-INFO` & `vivarium_inputs-5.0.0/src/vivarium_inputs.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: vivarium_inputs
-Version: 4.1.3
+Version: 5.0.0
 Summary: Transformations and artifact building for the vivarium microsimulation project.
 Home-page: https://github.com/ihmeuw/vivarium_inputs
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: click
 Requires-Dist: joblib
 Requires-Dist: tables
 Requires-Dist: vivarium>=1.2.1
-Requires-Dist: gbd_mapping<4.0.0,>=3.1.0
+Requires-Dist: gbd_mapping<5.0.0,>=4.0.0
 Requires-Dist: loguru
 Provides-Extra: docs
-Requires-Dist: sphinx<7.0,>=6.2.1; extra == "docs"
+Requires-Dist: sphinx<8.0,>=7.0; extra == "docs"
 Requires-Dist: sphinx-rtd-theme; extra == "docs"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-mock; extra == "test"
 Requires-Dist: hypothesis; extra == "test"
 Provides-Extra: data
-Requires-Dist: vivarium-gbd-access<4.0.0,>=3.0.7; extra == "data"
+Requires-Dist: vivarium-gbd-access<5.0.0,>=4.0.0; extra == "data"
 Requires-Dist: core-maths; extra == "data"
 Provides-Extra: dev
-Requires-Dist: sphinx<7.0,>=6.2.1; extra == "dev"
+Requires-Dist: sphinx<8.0,>=7.0; extra == "dev"
 Requires-Dist: sphinx-rtd-theme; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: hypothesis; extra == "dev"
-Requires-Dist: vivarium-gbd-access<4.0.0,>=3.0.7; extra == "dev"
+Requires-Dist: vivarium-gbd-access<5.0.0,>=4.0.0; extra == "dev"
 Requires-Dist: core-maths; extra == "dev"
 
 Vivarium Inputs
 ===============
 
 .. image:: https://badge.fury.io/py/vivarium-inputs.svg
     :target: https://badge.fury.io/py/vivarium-inputs
@@ -50,7 +50,11 @@
     :alt: Latest Docs
 
 
 This package is used to transform Global Burden of Disease data and package it into data artifacts
 used as inputs into vivarium simulations.
 
 It requires access to the IHME cluster for use (but not for testing).
+
+
+`Check out the docs! <https://vivarium.readthedocs.io/projects/vivarium-inputs/en/latest/>`_
+--------------------------------------------------------------------------------------------
```

### Comparing `vivarium_inputs-4.1.3/src/vivarium_inputs.egg-info/SOURCES.txt` & `vivarium_inputs-5.0.0/src/vivarium_inputs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/tests/conftest.py` & `vivarium_inputs-5.0.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/tests/extract/test_core.py` & `vivarium_inputs-5.0.0/tests/extract/test_extract.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,104 +3,89 @@
 import gbd_mapping
 import numpy as np
 import pandas as pd
 import pytest
 from gbd_mapping import ModelableEntity, causes, covariates, risk_factors
 
 from tests.extract.check import RUNNING_ON_CI
-from vivarium_inputs import core, utility_data
-from vivarium_inputs.mapping_extension import healthcare_entities
+from vivarium_inputs import extract, utility_data
 
 pytestmark = pytest.mark.skipif(
     RUNNING_ON_CI, reason="Don't run these tests on the CI server"
 )
 
 
+VALIDATE_FLAG = False
+
+
 def success_expected(entity_name, measure_name, location):
-    df = core.get_data(entity_name, measure_name, location)
+    df = extract.extract_data(entity_name, measure_name, location, validate=VALIDATE_FLAG)
     return df
 
 
 def fail_expected(entity_name, measure_name, location):
     with pytest.raises(Exception):
-        df = core.get_data(entity_name, measure_name, location)
+        df = extract.extract_data(entity_name, measure_name, location, validate=VALIDATE_FLAG)
 
 
 class MCFlag(IntFlag):
     """
     Use the idea of a bit field with support from python's enum type IntFlag
     See here for general information on bit fields:
     https://en.wikipedia.org/wiki/Bit_field
 
     And here for python's enum type:
     https://docs.python.org/3.6/library/enum.html
     """
 
     INCIDENCE_RATE = 1
-    RAW_INCIDENCE_RATE = 2
-    PREVALENCE = 4
-    BIRTH_PREVALENCE = 8
-    DISABILITY_WEIGHT = 16
-    REMISSION_RATE = 32
-    CAUSE_SPECIFIC_MORTALITY_RATE = 64
-    EXCESS_MORTALITY_RATE = 128
-    DEATHS = 512
+    PREVALENCE = 2
+    BIRTH_PREVALENCE = 4
+    DISABILITY_WEIGHT = 8
+    REMISSION_RATE = 16
+    DEATHS = 32
+    ALL = (
+        INCIDENCE_RATE
+        | PREVALENCE
+        | BIRTH_PREVALENCE
+        | DISABILITY_WEIGHT
+        | REMISSION_RATE
+        | DEATHS
+    )
 
 
 entity = [
     (
-        causes.measles,
-        MCFlag.INCIDENCE_RATE
-        | MCFlag.RAW_INCIDENCE_RATE
-        | MCFlag.PREVALENCE
-        | MCFlag.DISABILITY_WEIGHT
-        | MCFlag.CAUSE_SPECIFIC_MORTALITY_RATE
-        | MCFlag.EXCESS_MORTALITY_RATE
-        | MCFlag.DEATHS,
-    ),
-    (
-        causes.diarrheal_diseases,
+        causes.hiv_aids,
         MCFlag.INCIDENCE_RATE
-        | MCFlag.RAW_INCIDENCE_RATE
         | MCFlag.PREVALENCE
-        | MCFlag.DISABILITY_WEIGHT
+        | MCFlag.BIRTH_PREVALENCE
         | MCFlag.REMISSION_RATE
-        | MCFlag.CAUSE_SPECIFIC_MORTALITY_RATE
-        | MCFlag.EXCESS_MORTALITY_RATE
         | MCFlag.DEATHS,
     ),
     (
-        causes.diabetes_mellitus_type_2,
-        MCFlag.INCIDENCE_RATE
-        | MCFlag.RAW_INCIDENCE_RATE
-        | MCFlag.PREVALENCE
-        | MCFlag.DISABILITY_WEIGHT
-        | MCFlag.CAUSE_SPECIFIC_MORTALITY_RATE
-        | MCFlag.EXCESS_MORTALITY_RATE
-        | MCFlag.DEATHS,
+        causes.neural_tube_defects,
+        MCFlag.INCIDENCE_RATE | MCFlag.PREVALENCE | MCFlag.BIRTH_PREVALENCE | MCFlag.DEATHS,
     ),
 ]
 measures = [
     ("incidence_rate", MCFlag.INCIDENCE_RATE),
-    ("raw_incidence_rate", MCFlag.RAW_INCIDENCE_RATE),
     ("prevalence", MCFlag.PREVALENCE),
     ("birth_prevalence", MCFlag.BIRTH_PREVALENCE),
     ("disability_weight", MCFlag.DISABILITY_WEIGHT),
     ("remission_rate", MCFlag.REMISSION_RATE),
-    ("cause_specific_mortality_rate", MCFlag.CAUSE_SPECIFIC_MORTALITY_RATE),
-    ("excess_mortality_rate", MCFlag.EXCESS_MORTALITY_RATE),
     ("deaths", MCFlag.DEATHS),
 ]
 locations = ["India"]
 
 
 @pytest.mark.parametrize("entity", entity, ids=lambda x: x[0].name)
 @pytest.mark.parametrize("measure", measures, ids=lambda x: x[0])
 @pytest.mark.parametrize("location", locations)
-def test_core_causelike(entity, measure, location):
+def test_extract_causelike(entity, measure, location):
     entity_name, entity_expected_measure_ids = entity
     measure_name, measure_id = measure
     tester = success_expected if (entity_expected_measure_ids & measure_id) else fail_expected
     df = tester(entity_name, measure_name, utility_data.get_location_id(location))
 
 
 class MRFlag(IntFlag):
@@ -114,88 +99,94 @@
     """
 
     EXPOSURE = 1
     EXPOSURE_SD = 2
     EXPOSURE_DIST_WEIGHTS = 4
     RELATIVE_RISK = 8
     PAF = 16
-    # not implemented
-    # MEDIATION_FACTORS = 32
-    ALL = EXPOSURE | EXPOSURE_SD | EXPOSURE_DIST_WEIGHTS | RELATIVE_RISK | PAF
+    ETIOLOGY_PAF = 32
+    MEDIATION_FACTORS = 64
+    ALL = (
+        EXPOSURE
+        | EXPOSURE_SD
+        | EXPOSURE_DIST_WEIGHTS
+        | RELATIVE_RISK
+        | PAF
+        | ETIOLOGY_PAF
+        | MEDIATION_FACTORS
+    )
 
 
 entity_r = [
     (
-        risk_factors.high_systolic_blood_pressure,
+        risk_factors.high_fasting_plasma_glucose,
         MRFlag.EXPOSURE
         | MRFlag.EXPOSURE_SD
         | MRFlag.EXPOSURE_DIST_WEIGHTS
         | MRFlag.RELATIVE_RISK
-        | MRFlag.PAF,
+        | MRFlag.PAF
+        | MRFlag.ETIOLOGY_PAF
+        | MRFlag.MEDIATION_FACTORS,
     ),
     (
         risk_factors.low_birth_weight_and_short_gestation,
-        MRFlag.EXPOSURE | MRFlag.RELATIVE_RISK | MRFlag.PAF,
+        MRFlag.EXPOSURE | MRFlag.RELATIVE_RISK | MRFlag.PAF | MRFlag.ETIOLOGY_PAF,
     ),
 ]
 measures_r = [
     ("exposure", MRFlag.EXPOSURE),
     ("exposure_standard_deviation", MRFlag.EXPOSURE_SD),
     ("exposure_distribution_weights", MRFlag.EXPOSURE_DIST_WEIGHTS),
-    ("relative_risk", MRFlag.RELATIVE_RISK),
+    # TODO: Add back in with Mic-4936
+    # ("relative_risk", MRFlag.RELATIVE_RISK),
     ("population_attributable_fraction", MRFlag.PAF),
+    ("etiology_population_attributable_fraction", MRFlag.ETIOLOGY_PAF),
+    ("mediation_factors", MRFlag.MEDIATION_FACTORS),
 ]
 locations_r = ["India"]
 
 
 @pytest.mark.parametrize("entity", entity_r, ids=lambda x: x[0].name)
 @pytest.mark.parametrize("measure", measures_r, ids=lambda x: x[0])
 @pytest.mark.parametrize("location", locations_r)
-def test_core_risklike(entity, measure, location):
+def test_extract_risklike(entity, measure, location):
     entity_name, entity_expected_measure_ids = entity
     measure_name, measure_id = measure
     tester = success_expected if (entity_expected_measure_ids & measure_id) else fail_expected
     df = tester(entity_name, measure_name, utility_data.get_location_id(location))
 
 
 entity_cov = [
     covariates.systolic_blood_pressure_mmhg,
 ]
 measures_cov = ["estimate"]
 locations_cov = ["India"]
 
 
-@pytest.mark.parametrize("entity", entity_cov, ids=lambda x: x.name)
-@pytest.mark.parametrize("measure", measures_cov, ids=lambda x: x)
+@pytest.mark.parametrize("entity", entity_cov)
+@pytest.mark.parametrize("measure", measures_cov)
 @pytest.mark.parametrize("location", locations_cov)
-def test_core_covariatelike(entity, measure, location):
-    df = core.get_data(entity, measure, utility_data.get_location_id(location))
+def test_extract_covariatelike(entity, measure, location):
+    df = extract.extract_data(
+        entity, measure, utility_data.get_location_id(location), validate=VALIDATE_FLAG
+    )
 
 
 @pytest.mark.parametrize(
-    "measures",
-    [
-        "structure",
-        "age_bins",
-        "demographic_dimensions",
-        "theoretical_minimum_risk_life_expectancy",
-    ],
+    "measures", ["structure", "theoretical_minimum_risk_life_expectancy"]
 )
-def test_core_population(measures):
+def test_extract_population(measures):
     pop = ModelableEntity("ignored", "population", None)
-    df = core.get_data(pop, measures, utility_data.get_location_id("India"))
-
-
-# TODO - Underlying problem with gbd access. Remove when corrected.
-entity_health_system = [
-    healthcare_entities.outpatient_visits,
-]
-measures_health_system = ["utilization_rate"]
-locations_health_system = ["India"]
+    df = extract.extract_data(
+        pop, measures, utility_data.get_location_id("India"), validate=VALIDATE_FLAG
+    )
 
 
-@pytest.mark.skip(reason="Underlying problem with gbd access. Remove when corrected.")
-@pytest.mark.parametrize("entity", entity_health_system, ids=lambda x: x.name)
-@pytest.mark.parametrize("measure", measures_health_system, ids=lambda x: x)
-@pytest.mark.parametrize("location", locations_health_system)
-def test_core_healthsystem(entity, measure, location):
-    df = core.get_data(entity, measure, utility_data.get_location_id(location))
+# TODO: Remove with Mic-4936
+@pytest.mark.parametrize("entity", entity_r, ids=lambda x: x[0].name)
+@pytest.mark.parametrize("location", locations_r)
+@pytest.mark.xfail(reason="New relative risk data is not set up for processing yet")
+def test_extract_relative_risk(entity, location):
+    measure_name = "relative_risk"
+    measure_id = MRFlag.RELATIVE_RISK
+    entity_name, entity_expected_measure_ids = entity
+    df = extract.extract_data(entity_name, measure_name, location)
```

### Comparing `vivarium_inputs-4.1.3/tests/extract/test_extract.py` & `vivarium_inputs-5.0.0/tests/extract/test_get_measure.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,89 +3,98 @@
 import gbd_mapping
 import numpy as np
 import pandas as pd
 import pytest
 from gbd_mapping import ModelableEntity, causes, covariates, risk_factors
 
 from tests.extract.check import RUNNING_ON_CI
-from vivarium_inputs import extract, utility_data
+from vivarium_inputs import utility_data
+from vivarium_inputs.globals import DataAbnormalError
+from vivarium_inputs.interface import get_measure
+from vivarium_inputs.mapping_extension import healthcare_entities
 
 pytestmark = pytest.mark.skipif(
     RUNNING_ON_CI, reason="Don't run these tests on the CI server"
 )
 
 
-VALIDATE_FLAG = False
-
-
 def success_expected(entity_name, measure_name, location):
-    df = extract.extract_data(entity_name, measure_name, location, validate=VALIDATE_FLAG)
+    df = get_measure(entity_name, measure_name, location)
     return df
 
 
 def fail_expected(entity_name, measure_name, location):
     with pytest.raises(Exception):
-        df = extract.extract_data(entity_name, measure_name, location, validate=VALIDATE_FLAG)
+        df = get_measure(entity_name, measure_name, location)
 
 
 class MCFlag(IntFlag):
     """
     Use the idea of a bit field with support from python's enum type IntFlag
     See here for general information on bit fields:
     https://en.wikipedia.org/wiki/Bit_field
 
     And here for python's enum type:
     https://docs.python.org/3.6/library/enum.html
     """
 
     INCIDENCE_RATE = 1
-    PREVALENCE = 2
-    BIRTH_PREVALENCE = 4
-    DISABILITY_WEIGHT = 8
-    REMISSION_RATE = 16
-    DEATHS = 32
-    ALL = (
-        INCIDENCE_RATE
-        | PREVALENCE
-        | BIRTH_PREVALENCE
-        | DISABILITY_WEIGHT
-        | REMISSION_RATE
-        | DEATHS
-    )
+    RAW_INCIDENCE_RATE = 2
+    PREVALENCE = 4
+    BIRTH_PREVALENCE = 8
+    DISABILITY_WEIGHT = 16
+    REMISSION_RATE = 32
+    CAUSE_SPECIFIC_MORTALITY_RATE = 64
+    EXCESS_MORTALITY_RATE = 128
+    DEATHS = 512
 
 
 entity = [
     (
         causes.measles,
         MCFlag.INCIDENCE_RATE
         | MCFlag.PREVALENCE
-        | MCFlag.BIRTH_PREVALENCE
+        | MCFlag.DISABILITY_WEIGHT
+        | MCFlag.CAUSE_SPECIFIC_MORTALITY_RATE
+        | MCFlag.EXCESS_MORTALITY_RATE,
+    ),
+    (
+        causes.diarrheal_diseases,
+        MCFlag.INCIDENCE_RATE
+        | MCFlag.PREVALENCE
+        | MCFlag.DISABILITY_WEIGHT
         | MCFlag.REMISSION_RATE
-        | MCFlag.DEATHS,
+        | MCFlag.CAUSE_SPECIFIC_MORTALITY_RATE
+        | MCFlag.EXCESS_MORTALITY_RATE,
     ),
     (
         causes.diabetes_mellitus_type_2,
-        MCFlag.INCIDENCE_RATE | MCFlag.PREVALENCE | MCFlag.BIRTH_PREVALENCE | MCFlag.DEATHS,
+        MCFlag.INCIDENCE_RATE
+        | MCFlag.PREVALENCE
+        | MCFlag.DISABILITY_WEIGHT
+        | MCFlag.CAUSE_SPECIFIC_MORTALITY_RATE
+        | MCFlag.EXCESS_MORTALITY_RATE,
     ),
 ]
 measures = [
     ("incidence_rate", MCFlag.INCIDENCE_RATE),
     ("prevalence", MCFlag.PREVALENCE),
     ("birth_prevalence", MCFlag.BIRTH_PREVALENCE),
     ("disability_weight", MCFlag.DISABILITY_WEIGHT),
     ("remission_rate", MCFlag.REMISSION_RATE),
-    ("deaths", MCFlag.DEATHS),
+    ("cause_specific_mortality_rate", MCFlag.CAUSE_SPECIFIC_MORTALITY_RATE),
+    ("excess_mortality_rate", MCFlag.EXCESS_MORTALITY_RATE),
 ]
 locations = ["India"]
 
 
 @pytest.mark.parametrize("entity", entity, ids=lambda x: x[0].name)
 @pytest.mark.parametrize("measure", measures, ids=lambda x: x[0])
 @pytest.mark.parametrize("location", locations)
-def test_extract_causelike(entity, measure, location):
+def test_get_measure_causelike(entity, measure, location):
     entity_name, entity_expected_measure_ids = entity
     measure_name, measure_id = measure
     tester = success_expected if (entity_expected_measure_ids & measure_id) else fail_expected
     df = tester(entity_name, measure_name, utility_data.get_location_id(location))
 
 
 class MRFlag(IntFlag):
@@ -99,82 +108,100 @@
     """
 
     EXPOSURE = 1
     EXPOSURE_SD = 2
     EXPOSURE_DIST_WEIGHTS = 4
     RELATIVE_RISK = 8
     PAF = 16
-    ETIOLOGY_PAF = 32
-    MEDIATION_FACTORS = 64
-    ALL = (
-        EXPOSURE
-        | EXPOSURE_SD
-        | EXPOSURE_DIST_WEIGHTS
-        | RELATIVE_RISK
-        | PAF
-        | ETIOLOGY_PAF
-        | MEDIATION_FACTORS
-    )
+    ALL = EXPOSURE | EXPOSURE_SD | EXPOSURE_DIST_WEIGHTS | RELATIVE_RISK | PAF
 
 
 entity_r = [
     (
         risk_factors.high_systolic_blood_pressure,
-        MRFlag.EXPOSURE
-        | MRFlag.EXPOSURE_SD
-        | MRFlag.EXPOSURE_DIST_WEIGHTS
-        | MRFlag.RELATIVE_RISK
-        | MRFlag.PAF
-        | MRFlag.ETIOLOGY_PAF
-        | MRFlag.MEDIATION_FACTORS,
+        MRFlag.EXPOSURE | MRFlag.EXPOSURE_SD | MRFlag.EXPOSURE_DIST_WEIGHTS
+        # TODO: Add back in once Mic-4936 is resolved
+        #        | MRFlag.RELATIVE_RISK
+        | MRFlag.PAF,
     ),
     (
         risk_factors.low_birth_weight_and_short_gestation,
-        MRFlag.EXPOSURE | MRFlag.RELATIVE_RISK | MRFlag.PAF | MRFlag.ETIOLOGY_PAF,
+        MRFlag.EXPOSURE | MRFlag.RELATIVE_RISK | MRFlag.PAF,
     ),
 ]
 measures_r = [
     ("exposure", MRFlag.EXPOSURE),
     ("exposure_standard_deviation", MRFlag.EXPOSURE_SD),
     ("exposure_distribution_weights", MRFlag.EXPOSURE_DIST_WEIGHTS),
-    ("relative_risk", MRFlag.RELATIVE_RISK),
+    # TODO: Add back in once Mic-4936 is resolved
+    #    ("relative_risk", MRFlag.RELATIVE_RISK),
     ("population_attributable_fraction", MRFlag.PAF),
-    ("etiology_population_attributable_fraction", MRFlag.ETIOLOGY_PAF),
-    ("mediation_factors", MRFlag.MEDIATION_FACTORS),
 ]
 locations_r = ["India"]
 
 
 @pytest.mark.parametrize("entity", entity_r, ids=lambda x: x[0].name)
 @pytest.mark.parametrize("measure", measures_r, ids=lambda x: x[0])
 @pytest.mark.parametrize("location", locations_r)
-def test_extract_risklike(entity, measure, location):
+def test_get_measure_risklike(entity, measure, location):
     entity_name, entity_expected_measure_ids = entity
     measure_name, measure_id = measure
     tester = success_expected if (entity_expected_measure_ids & measure_id) else fail_expected
     df = tester(entity_name, measure_name, utility_data.get_location_id(location))
 
 
 entity_cov = [
     covariates.systolic_blood_pressure_mmhg,
 ]
 measures_cov = ["estimate"]
 locations_cov = ["India"]
 
 
-@pytest.mark.parametrize("entity", entity_cov)
-@pytest.mark.parametrize("measure", measures_cov)
+@pytest.mark.parametrize("entity", entity_cov, ids=lambda x: x.name)
+@pytest.mark.parametrize("measure", measures_cov, ids=lambda x: x)
 @pytest.mark.parametrize("location", locations_cov)
-def test_extract_covariatelike(entity, measure, location):
-    df = extract.extract_data(
-        entity, measure, utility_data.get_location_id(location), validate=VALIDATE_FLAG
-    )
+def test_get_measure_covariatelike(entity, measure, location):
+    df = get_measure(entity, measure, utility_data.get_location_id(location))
 
 
-@pytest.mark.parametrize(
-    "measures", ["structure", "theoretical_minimum_risk_life_expectancy"]
-)
-def test_extract_population(measures):
-    pop = ModelableEntity("ignored", "population", None)
-    df = extract.extract_data(
-        pop, measures, utility_data.get_location_id("India"), validate=VALIDATE_FLAG
-    )
+# TODO: Remove with Mic-4936
+entity_r = [
+    (
+        risk_factors.high_systolic_blood_pressure,
+        MRFlag.RELATIVE_RISK,
+    ),
+]
+measures_r = [
+    ("relative_risk", MRFlag.RELATIVE_RISK),
+]
+locations_r = ["India"]
+
+
+@pytest.mark.parametrize("entity", entity_r, ids=lambda x: x[0].name)
+@pytest.mark.parametrize("measure", measures_r, ids=lambda x: x[0])
+@pytest.mark.parametrize("location", locations_r)
+def test_get_failing_relative_risk(entity, measure, location):
+    entity_name, entity_expected_measure_ids = entity
+    measure_name, measure_id = measure
+    with pytest.raises(DataAbnormalError):
+        df = get_measure(entity_name, measure_name, location)
+
+
+entity_r = [
+    (
+        risk_factors.iron_deficiency,
+        MRFlag.RELATIVE_RISK,
+    ),
+]
+measures_r = [
+    ("relative_risk", MRFlag.RELATIVE_RISK),
+]
+locations_r = ["India"]
+
+
+@pytest.mark.parametrize("entity", entity_r, ids=lambda x: x[0].name)
+@pytest.mark.parametrize("measure", measures_r, ids=lambda x: x[0])
+@pytest.mark.parametrize("location", locations_r)
+def test_get_working_relative_risk(entity, measure, location):
+    entity_name, entity_expected_measure_ids = entity
+    measure_name, measure_id = measure
+    df = success_expected(entity_name, measure_name, utility_data.get_location_id(location))
```

### Comparing `vivarium_inputs-4.1.3/tests/extract/test_utility_data.py` & `vivarium_inputs-5.0.0/tests/extract/test_utility_data.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,36 +8,43 @@
 pytestmark = pytest.mark.skipif(
     RUNNING_ON_CI, reason="Don't run these tests on the CI server"
 )
 
 
 def test_get_estimation_years():
     result = ud.get_estimation_years()
-    assert set([1990, 1995, 2000, 2005, 2010, 2015, 2017, 2019]) == set(result)
+    assert set([1990, 1995, 2000, 2005, 2010, 2015, 2019, 2020, 2021, 2022]) == set(result)
 
 
 def test_get_year_block():
     result = ud.get_year_block()
     assert result.year_start.iloc[0] == 1990
-    assert result.year_end.iloc[-1] == 2020
+    assert result.year_end.iloc[-1] == 2023
 
 
 def test_get_age_group_ids():
     result = ud.get_age_group_ids()
-    truth = list(range(2, 21)) + [30, 31, 32, 235]
+    truth = [2, 3, 388, 389, 238, 34] + list(range(6, 21)) + [30, 31, 32, 235]
     assert result == truth
 
 
 def test_get_location_id():
     result_india = ud.get_location_id("India")
     assert 163 == result_india
 
 
-def test_get_location_id_parents():
-    assert [1, 158, 159, 163] == ud.get_location_id_parents(163)
+@pytest.mark.parametrize(
+    "location_id, expected",
+    [
+        (163, {163: [1, 158, 159, 163]}),
+        ([163, 175], {163: [1, 158, 159, 163], 175: [1, 166, 174, 175]}),
+    ],
+)
+def test_get_location_id_parents(location_id, expected):
+    assert expected == ud.get_location_id_parents(location_id)
 
 
 def test_get_demographic_dimensions():
     result = ud.get_demographic_dimensions(163)
     assert len(result)
     assert set(["location_id", "sex_id", "age_group_id", "year_id"]) == set(result.columns)
```

### Comparing `vivarium_inputs-4.1.3/tests/test_utilities.py` & `vivarium_inputs-5.0.0/tests/test_utilities.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/tests/validation/test_raw.py` & `vivarium_inputs-5.0.0/tests/validation/test_raw.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 import numpy as np
 import pandas as pd
 import pytest
 
+from tests.extract.check import RUNNING_ON_CI
 from vivarium_inputs.globals import SEXES, DataAbnormalError, DataDoesNotExistError
 from vivarium_inputs.validation import raw
 
 LOCATION_ID = 100
-ESTIMATION_YEARS = tuple(list(range(1990, 2015, 5)) + [2017])
-AGE_GROUP_IDS = tuple(range(1, 6))
+ESTIMATION_YEARS = tuple(list(range(1990, 2015, 5)) + list(range(2019, 2022)))
+AGE_GROUP_IDS = tuple([2, 3, 388, 389, 238, 34])
 PARENT_LOCATIONS = (1, 5, 10)
 
 
 @pytest.fixture
 def mock_validation_context():
     context = raw.RawValidationContext(
-        location_id=LOCATION_ID,
+        location_id=[LOCATION_ID],
         estimation_years=list(ESTIMATION_YEARS),
         age_group_ids=list(AGE_GROUP_IDS),
         sexes=SEXES,
-        parent_locations=list(PARENT_LOCATIONS),
+        parent_locations={LOCATION_ID: list(PARENT_LOCATIONS)},
     )
     return context
 
 
 @pytest.fixture
 def measures_mock(mocker):
     return mocker.patch("vivarium_inputs.validation.raw.MEASURES", {"A": 1, "B": 2})
@@ -74,61 +75,57 @@
     data = pd.DataFrame({"mortality": mort, "morbidity": morb})
     raw.check_mort_morb_flags(data, yld_only, yll_only)
 
 
 @pytest.mark.parametrize(
     "years, bin_type",
     [
-        (range(1950, 2020), "annual"),
-        (range(1990, 2018), "annual"),
-        (list(range(1990, 2015, 5)) + [2017], "binned"),
+        (range(1950, 2023), "annual"),
+        (range(1990, 2022), "annual"),
+        (list(range(1990, 2015, 5)) + list(range(2019, 2022)), "binned"),
     ],
     ids=["annual with extra", "annual", "binned"],
 )
 def test_check_years_pass(mock_validation_context, years, bin_type):
     df = pd.DataFrame({"year_id": years})
     raw.check_years(df, mock_validation_context, bin_type)
 
 
 @pytest.mark.parametrize(
     "years, bin_type, match",
     [
         ([1990, 1992], "annual", "missing"),
         ([1990, 1995], "binned", "missing"),
-        (list(range(1990, 2015, 5)) + [2017, 2020], "binned", "extra"),
+        (list(range(1990, 2015, 5)) + list(range(2019, 2023)), "binned", "extra"),
     ],
     ids=["annual with gap", "binned with gap", "binned with extra"],
 )
 def test_check_years_fail(mock_validation_context, years, bin_type, match):
     df = pd.DataFrame({"year_id": years})
     with pytest.raises(DataAbnormalError, match=match):
         raw.check_years(df, mock_validation_context, bin_type)
 
 
 @pytest.mark.parametrize("location_id", list(range(2, 10)))
 def test_check_location_pass(mock_validation_context, location_id):
-    mock_validation_context["location_id"] = location_id
+    mock_validation_context["location_id"] = [location_id]
     df = pd.DataFrame({"location_id": [location_id] * 5})
     raw.check_location(df, mock_validation_context)
 
 
 @pytest.mark.parametrize("location_id", PARENT_LOCATIONS)
 def test_check_location_parent_pass(mock_validation_context, location_id):
     df = pd.DataFrame({"location_id": [location_id]})
     raw.check_location(df, mock_validation_context)
 
 
-@pytest.mark.parametrize(
-    "location_ids, match",
-    [([1, 2], "multiple"), ([2, 2], "actually has location id")],
-    ids=["multiple locations", "wrong location"],
-)
-def test_check_location_fail(mock_validation_context, location_ids, match):
-    df = pd.DataFrame({"location_id": location_ids})
-    with pytest.raises(DataAbnormalError, match=match):
+@pytest.mark.parametrize("location_id", list(range(20, 25)))
+def test_check_location_fail(mock_validation_context, location_id):
+    df = pd.DataFrame({"location_id": [location_id]})
+    with pytest.raises(DataAbnormalError, match="Data pulled for "):
         raw.check_location(df, mock_validation_context)
 
 
 @pytest.mark.parametrize("columns", [["a", "b"], ["c", "d", "e"], ["a"], []])
 def test_check_columns_pass(columns):
     raw.check_columns(columns, columns)
 
@@ -214,47 +211,50 @@
         data, zeros_missing=True, value_columns=data.columns, error=False
     )
 
 
 @pytest.mark.parametrize(
     "test_age_ids, start, end, match",
     [
-        ([1, 2, 3, 100], None, None, "invalid"),
-        ([1, 3, 4, 5], None, None, "non-contiguous"),
-        ([1, 2, 3, 100], 1, 3, "invalid"),
-        ([1, 2, 3, 5], 1, 3, "non-contiguous"),
+        ([2, 3, 388, 100], None, None, "invalid"),
+        ([2, 3, 388, 238], None, None, "non-contiguous"),
+        ([2, 3, 388, 100], 2, 388, "invalid"),
+        ([2, 3, 388, 238], 2, 388, "non-contiguous"),
     ],
 )
+@pytest.mark.skipif(RUNNING_ON_CI, reason="Don't run these tests on the CI server")
 def test_check_age_group_ids_fail(mock_validation_context, test_age_ids, start, end, match):
     df = pd.DataFrame({"age_group_id": test_age_ids})
     with pytest.raises(DataAbnormalError, match=match):
         raw.check_age_group_ids(df, mock_validation_context, start, end)
 
 
 @pytest.mark.parametrize(
     "test_age_ids, start, end, match",
     [
-        ([2, 3], 2, 4, "contain all age groups in restriction range"),
-        ([2, 3, 4], 2, 3, "additional age groups"),
-        ([1, 2, 3, 4, 5], 1, 3, "additional age groups"),
-        ([1, 2, 3], 1, 5, "contain all age groups in restriction range"),
+        ([2, 3], 2, 388, "contain all age groups in restriction range"),
+        ([2, 3, 388], 2, 3, "additional age groups"),
+        ([2, 3, 388, 389, 238], 2, 388, "additional age groups"),
+        ([2, 3, 388], 2, 238, "contain all age groups in restriction range"),
     ],
 )
+@pytest.mark.skipif(RUNNING_ON_CI, reason="Don't run these tests on the CI server")
 def test_check_age_group_ids_warn(
     mock_validation_context, caplog, test_age_ids, start, end, match
 ):
     df = pd.DataFrame({"age_group_id": test_age_ids})
     raw.check_age_group_ids(df, mock_validation_context, start, end)
     assert match in caplog.text
 
 
 @pytest.mark.parametrize(
     "test_age_ids, start, end",
-    [([2, 3, 4], 2, 4), ([2, 3, 4], None, None), ([1, 2, 3, 4, 5], 1, 5)],
+    [([2, 3, 388], 2, 388), ([2, 3, 388], None, None), ([2, 3, 388, 389, 238], 2, 238)],
 )
+@pytest.mark.skipif(RUNNING_ON_CI, reason="Don't run these tests on the CI server")
 def test_check_age_group_ids_pass(mock_validation_context, test_age_ids, start, end, recwarn):
     df = pd.DataFrame({"age_group_id": test_age_ids})
     raw.check_age_group_ids(df, mock_validation_context, start, end)
 
     assert len(recwarn) == 0, "An unexpected warning was raised."
 
 
@@ -306,19 +306,25 @@
     df = pd.DataFrame({"sex_id": sex_ids})
     raw.check_sex_ids(df, mock_validation_context, male, female, both)
 
     assert len(recwarn) == 0, "An unexpected warning was raised."
 
 
 test_data = [
-    (pd.DataFrame({"age_group_id": [1, 2, 3], "a": 1, "b": 0}), 1, 4, ["a", "b"], "missing"),
     (
-        pd.DataFrame({"age_group_id": [1, 2], "a": [0, 0], "b": [0, 0]}),
-        1,
+        pd.DataFrame({"age_group_id": [2, 3, 388], "a": 1, "b": 0}),
+        2,
+        389,
+        ["a", "b"],
+        "missing",
+    ),
+    (
+        pd.DataFrame({"age_group_id": [2, 3], "a": [0, 0], "b": [0, 0]}),
         2,
+        3,
         ["a", "b"],
         "missing for all age groups",
     ),
 ]
 
 
 @pytest.mark.parametrize("data, start, end, val_cols, match", test_data)
@@ -328,33 +334,43 @@
     with pytest.raises(DataAbnormalError, match=match):
         raw.check_age_restrictions(
             data, mock_validation_context, start, end, value_columns=val_cols
         )
 
 
 test_data = [
-    (pd.DataFrame({"age_group_id": [1, 2, 3, 4, 5], "a": 1, "b": 0}), 1, 4, ["a", "b"]),
-    (pd.DataFrame({"age_group_id": [1, 2, 3], "a": [1, 1, 1], "b": [2, 3, 0]}), 1, 2, ["a"]),
+    (
+        pd.DataFrame({"age_group_id": [2, 3, 388, 389, 238], "a": 1, "b": 0}),
+        2,
+        389,
+        ["a", "b"],
+    ),
+    (pd.DataFrame({"age_group_id": [2, 3, 4], "a": [1, 1, 1], "b": [2, 3, 0]}), 2, 3, ["a"]),
 ]
 
 
 @pytest.mark.parametrize("data, start, end, val_cols", test_data)
 def test_check_age_restrictions_warn(
     mock_validation_context, caplog, data, start, end, val_cols
 ):
     raw.check_age_restrictions(
         data, mock_validation_context, start, end, value_columns=val_cols
     )
     assert "also included" in caplog.text
 
 
 test_data = [
-    (pd.DataFrame({"age_group_id": [1, 2, 3], "a": 1, "b": 0}), 1, 3, ["a", "b"]),
-    (pd.DataFrame({"age_group_id": [1, 2], "a": [1, 0], "b": [1, 0.1]}), 1, 2, ["a", "b"]),
-    (pd.DataFrame({"age_group_id": [1, 2, 3], "a": [1, 1, 0], "b": [2, 3, 0]}), 1, 3, ["a"]),
+    (pd.DataFrame({"age_group_id": [2, 3, 388], "a": 1, "b": 0}), 2, 388, ["a", "b"]),
+    (pd.DataFrame({"age_group_id": [2, 3], "a": [1, 0], "b": [1, 0.1]}), 2, 3, ["a", "b"]),
+    (
+        pd.DataFrame({"age_group_id": [2, 3, 388], "a": [1, 1, 0], "b": [2, 3, 0]}),
+        2,
+        388,
+        ["a"],
+    ),
 ]
 
 
 @pytest.mark.parametrize("data, start, end, val_cols", test_data)
 def test_check_age_restrictions_pass(mock_validation_context, data, start, end, val_cols):
     raw.check_age_restrictions(
         data, mock_validation_context, start, end, value_columns=val_cols
```

### Comparing `vivarium_inputs-4.1.3/tests/validation/test_shared.py` & `vivarium_inputs-5.0.0/tests/validation/test_shared.py`

 * *Files identical despite different names*

### Comparing `vivarium_inputs-4.1.3/tests/validation/test_sim.py` & `vivarium_inputs-5.0.0/tests/validation/test_sim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import numpy as np
 import pandas as pd
 import pytest
 
+from tests.extract.check import RUNNING_ON_CI
 from vivarium_inputs.globals import DataTransformationError
 from vivarium_inputs.validation import sim
 
 
 @pytest.fixture
 def mock_validation_context():
     years = pd.DataFrame({"year_start": range(1990, 2017), "year_end": range(1991, 2018)})
@@ -22,15 +23,15 @@
     )
 
     return context
 
 
 @pytest.mark.parametrize("location", ("Kenya", "Papua New Guinea"))
 def test__validate_location_column_pass(mock_validation_context, location):
-    mock_validation_context["location"] = location
+    mock_validation_context["location"] = [location]
     df = pd.DataFrame({"location": [location], "other": [0]}).set_index(["location", "other"])
     sim.validate_location_column(df, mock_validation_context)
 
 
 @pytest.mark.parametrize(
     "locations,expected_location",
     ((["Kenya", "Kenya"], "Egypt"), (["Algeria", "Nigeria"], "Algeria")),
@@ -159,14 +160,15 @@
         ((0, 0, 1, 1, 1), (3, 5), "outer", 0.0),
         ((0, 1, 1, 1, 0), (2, 4), "outer", 0.0),
         ((1, 1, 1, 0, 0), (1, 3), "outer", 0.0),
         ((2, 2, 2, 1, 1), (1, 3), "outer", 1.0),
     ],
     ids=("no_restr", "left_restr", "outer_restr", "right_restr", "nonzero_fill"),
 )
+@pytest.mark.skipif(RUNNING_ON_CI, reason="Don't run these tests on the CI server")
 def test_check_age_restrictions(
     mocker, mock_validation_context, values, ids, restriction_type, fill
 ):
     entity = mocker.patch(
         "vivarium_inputs.validation.sim.utilities.get_age_group_ids_by_restriction"
     )
     entity.return_value = ids
@@ -184,14 +186,15 @@
         ((1, 1, 1, 1, 1), (1, 4), "outer", 0.0),
         ((0, 1, 1, 1, 1), (1, 3), "outer", 0.0),
         ((1, 1, 1, 1, 0), (1, 3), "outer", 0.0),
         ((2, 2, 2, 2, 1), (2, 5), "outer", 1.0),
     ],
     ids=("both_sides", "left_side", "right_side", "nonzero_fill"),
 )
+@pytest.mark.skipif(RUNNING_ON_CI, reason="Don't run these tests on the CI server")
 def test_check_age_restrictions_fail(
     mocker, mock_validation_context, values, ids, restriction_type, fill
 ):
     entity = mocker.patch(
         "vivarium_inputs.validation.sim.utilities.get_age_group_ids_by_restriction"
     )
     entity.return_value = ids
```

