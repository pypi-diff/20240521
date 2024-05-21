# Comparing `tmp/datatrails-archivist-0.30.0.tar.gz` & `tmp/datatrails_archivist-0.30.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datatrails-archivist-0.30.0.tar", last modified: Mon Apr  8 15:11:19 2024, max compression
+gzip compressed data, was "datatrails_archivist-0.30.1.tar", last modified: Tue May 21 09:49:36 2024, max compression
```

## Comparing `datatrails-archivist-0.30.0.tar` & `datatrails_archivist-0.30.1.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12250 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/archivist/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-08 15:11:16.000000 datatrails-archivist-0.30.0/archivist/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/access_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/appidp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/applications.py
--rw-r--r--   0 runner    (1001) docker     (127)    11453 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/archivist.py
--rw-r--r--   0 runner    (1001) docker     (127)    12484 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/archivistpublic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/asset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/assetattachments.py
--rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/assets.py
--rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/attachments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/archivist/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/archivist/cmds/runner/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/runner/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/runner/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/runner/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/archivist/cmds/template/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/template/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/template/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/template/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/cmds/template/run.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/compliance_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/compliance_policy_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/compliance_policy_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/composite.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/confirmation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/confirmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/dictmerge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/events.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/or_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/proof_mechanism.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/retry429.py
--rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/sboms.py
--rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/subjects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/subjects_confirmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/tenancies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/archivist/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-04-08 15:11:19.000000 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-08 15:11:19.000000 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:11:19.000000 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 15:11:19.000000 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-08 15:11:19.000000 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 15:11:19.000000 datatrails-archivist-0.30.0/datatrails_archivist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-08 15:09:30.000000 datatrails-archivist-0.30.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-08 15:11:19.613119 datatrails-archivist-0.30.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12250 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/archivist/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-21 09:49:33.000000 datatrails_archivist-0.30.1/archivist/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8136 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/access_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/appidp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5926 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11226 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/archivist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12435 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/archivistpublic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/asset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/assetattachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12781 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/assets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6546 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/attachments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/archivist/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/archivist/cmds/runner/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/runner/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/runner/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/runner/run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/archivist/cmds/template/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/template/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/template/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/template/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/cmds/template/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/compliance_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/compliance_policy_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/compliance_policy_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/composite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/confirmation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/confirmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/dictmerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/or_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/proof_mechanism.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/retry429.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15897 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/sboms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9213 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/subjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/subjects_confirmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/tenancies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2720 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/archivist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13358 2024-05-21 09:49:36.000000 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-21 09:49:36.000000 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:49:36.000000 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-21 09:49:36.000000 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-21 09:49:36.000000 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 09:49:36.000000 datatrails_archivist-0.30.1/datatrails_archivist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21235 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-21 09:47:31.000000 datatrails_archivist-0.30.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-21 09:49:36.432689 datatrails_archivist-0.30.1/setup.cfg
```

### Comparing `datatrails-archivist-0.30.0/LICENSE` & `datatrails_archivist-0.30.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/PKG-INFO` & `datatrails_archivist-0.30.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrails-archivist
-Version: 0.30.0
+Version: 0.30.1
 Summary: DataTrails API
 Home-page: https://github.com/datatrails/datatrails-python
 Author: DataTrails Inc.
 Author-email: support@datatrails.ai
 License: MIT
 Project-URL: Documentation, https://python.datatrails.ai
 Project-URL: Source, https://github.com/datatrails/datatrails-python
@@ -21,15 +21,15 @@
 License-File: LICENSE
 Requires-Dist: backoff~=2.2.1
 Requires-Dist: certifi
 Requires-Dist: flatten-dict~=0.4
 Requires-Dist: iso8601~=2.1
 Requires-Dist: Jinja2~=3.1
 Requires-Dist: pyaml-env~=1.2
-Requires-Dist: requests~=2.31.0
+Requires-Dist: requests~=2.32.0
 Requires-Dist: requests-toolbelt~=1.0
 Requires-Dist: rfc3339~=6.2
 Requires-Dist: xmltodict~=0.13
 
 
 .. _readme:
```

### Comparing `datatrails-archivist-0.30.0/README.rst` & `datatrails_archivist-0.30.1/README.rst`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/access_policies.py` & `datatrails_archivist-0.30.1/archivist/access_policies.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/appidp.py` & `datatrails_archivist-0.30.1/archivist/appidp.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/applications.py` & `datatrails_archivist-0.30.1/archivist/applications.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/archivist.py` & `datatrails_archivist-0.30.1/archivist/archivist.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,39 @@
 # -*- coding: utf-8 -*-
 """Archivist connection interface
 
-   This module contains the base Archivist class which manages
-   the connection parameters to a DataTrails instance and
-   the basic REST verbs to GET, POST, PATCH and DELETE entities..
-
-   The REST methods in this class should only be used directly when
-   a CRUD endpoint for the specific type of entity is unavailable.
-   Current CRUD endpoints are assets, events, locations, attachments.
-   IAM subjects and IAM access policies.
-
-   Instantiation of this class encapsulates the URL and authentication
-   parameters (the max_time parameter is optional):
-
-   .. code-block:: python
-
-      with open(".auth_token", mode="r", encoding="utf-8") as tokenfile:
-          authtoken = tokenfile.read().strip()
-
-      # Initialize connection to Archivist
-      arch = Archivist(
-          "https://app.datatrails.ai",
-          authtoken,
-          max_time=300.0,
-      )
+This module contains the base Archivist class which manages
+the connection parameters to a DataTrails instance and
+the basic REST verbs to GET, POST, PATCH and DELETE entities..
+
+The REST methods in this class should only be used directly when
+a CRUD endpoint for the specific type of entity is unavailable.
+Current CRUD endpoints are assets, events, locations, attachments.
+IAM subjects and IAM access policies.
+
+Instantiation of this class encapsulates the URL and authentication
+parameters (the max_time parameter is optional):
+
+.. code-block:: python
+
+   with open(".auth_token", mode="r", encoding="utf-8") as tokenfile:
+       authtoken = tokenfile.read().strip()
+
+   # Initialize connection to Archivist
+   arch = Archivist(
+       "https://app.datatrails.ai",
+       authtoken,
+       max_time=300.0,
+   )
 
-    The arch variable now has additional endpoints assets,events,locations,
-    attachments, IAM subjects and IAM access policies documented elsewhere.
+ The arch variable now has additional endpoints assets,events,locations,
+ attachments, IAM subjects and IAM access policies documented elsewhere.
 
 """
+
 from copy import deepcopy
 from logging import getLogger
 from time import time
 from typing import Any, BinaryIO
 
 from requests_toolbelt.multipart.encoder import MultipartEncoder
 
@@ -249,22 +250,20 @@
         Returns:
             dict representing the response body (entity).
         """
         if data:
             response = self.session.post(
                 url,
                 data=request,
-                verify=self.verify,
             )
         else:
             response = self.session.post(
                 url,
                 json=request,
                 headers=self._add_headers(headers),
-                verify=self.verify,
             )
 
         error = _parse_response(response)
         if error is not None:
             raise error
 
         return response.json()
@@ -301,15 +300,14 @@
             "content-type": multipart.content_type,
         }
 
         response = self.session.post(
             url,
             data=multipart,  # pyright: ignore    https://github.com/requests/toolbelt/issues/312
             headers=self._add_headers(headers),
-            verify=self.verify,
             params=_dotdict(params),
         )
 
         self._response_ring_buffer.appendleft(response)
 
         error = _parse_response(response)
         if error is not None:
@@ -331,15 +329,14 @@
 
         Returns:
             dict representing the response body (entity).
         """
         response = self.session.delete(
             url,
             headers=self._add_headers(headers),
-            verify=self.verify,
         )
 
         self._response_ring_buffer.appendleft(response)
 
         error = _parse_response(response)
         if error is not None:
             raise error
@@ -367,15 +364,14 @@
             dict representing the response body (entity).
         """
 
         response = self.session.patch(
             url,
             json=request,
             headers=self._add_headers(headers),
-            verify=self.verify,
         )
 
         self._response_ring_buffer.appendleft(response)
 
         error = _parse_response(response)
         if error is not None:
             raise error
```

### Comparing `datatrails-archivist-0.30.0/archivist/archivistpublic.py` & `datatrails_archivist-0.30.1/archivist/archivistpublic.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,15 @@
         self.close()
 
     @property
     def session(self) -> requests.Session:
         """creates and returns session"""
         if self._session is None:
             self._session = requests.Session()
+            self._session.verify = self.verify
         return self._session
 
     def close(self):
         """closes current session if open"""
         if self._session is not None:
             self._session.close()
             self._session = None
@@ -193,15 +194,14 @@
         Returns:
             dict representing the response body (entity).
 
         """
         response = self.session.get(
             url,
             headers=self._add_headers(headers),
-            verify=self.verify,
             params=_dotdict(params),
         )
 
         self._response_ring_buffer.appendleft(response)
 
         error = _parse_response(response)
         if error is not None:
@@ -233,15 +233,14 @@
         Returns:
             REST response (not the response body)
 
         """
         response = self.session.get(
             url,
             headers=self._add_headers(headers),
-            verify=self.verify,
             stream=True,
             params=_dotdict(params),
         )
 
         self._response_ring_buffer.appendleft(response)
 
         error = _parse_response(response)
@@ -268,15 +267,14 @@
                 params["page_size"] = page_size
             else:
                 params = {"page_size": page_size}
 
         response = self.session.get(
             url,
             headers=self._add_headers(headers),
-            verify=self.verify,
             params=_dotdict(params),
         )
 
         self._response_ring_buffer.appendleft(response)
 
         error = _parse_response(response)
         if error is not None:
```

### Comparing `datatrails-archivist-0.30.0/archivist/asset.py` & `datatrails_archivist-0.30.1/archivist/asset.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/assetattachments.py` & `datatrails_archivist-0.30.1/archivist/assetattachments.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/assets.py` & `datatrails_archivist-0.30.1/archivist/assets.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/attachments.py` & `datatrails_archivist-0.30.1/archivist/attachments.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/cmds/runner/main.py` & `datatrails_archivist-0.30.1/archivist/cmds/runner/main.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/cmds/runner/run.py` & `datatrails_archivist-0.30.1/archivist/cmds/runner/run.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/cmds/template/main.py` & `datatrails_archivist-0.30.1/archivist/cmds/template/main.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/cmds/template/run.py` & `datatrails_archivist-0.30.1/archivist/cmds/template/run.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/compliance.py` & `datatrails_archivist-0.30.1/archivist/compliance.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/compliance_policies.py` & `datatrails_archivist-0.30.1/archivist/compliance_policies.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/compliance_policy_requests.py` & `datatrails_archivist-0.30.1/archivist/compliance_policy_requests.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/compliance_policy_type.py` & `datatrails_archivist-0.30.1/archivist/compliance_policy_type.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/composite.py` & `datatrails_archivist-0.30.1/archivist/composite.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/confirmation_status.py` & `datatrails_archivist-0.30.1/archivist/confirmation_status.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/confirmer.py` & `datatrails_archivist-0.30.1/archivist/confirmer.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/constants.py` & `datatrails_archivist-0.30.1/archivist/constants.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/dictmerge.py` & `datatrails_archivist-0.30.1/archivist/dictmerge.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/errors.py` & `datatrails_archivist-0.30.1/archivist/errors.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/events.py` & `datatrails_archivist-0.30.1/archivist/events.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/locations.py` & `datatrails_archivist-0.30.1/archivist/locations.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/logger.py` & `datatrails_archivist-0.30.1/archivist/logger.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/parser.py` & `datatrails_archivist-0.30.1/archivist/parser.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/proof_mechanism.py` & `datatrails_archivist-0.30.1/archivist/proof_mechanism.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/retry429.py` & `datatrails_archivist-0.30.1/archivist/retry429.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/runner.py` & `datatrails_archivist-0.30.1/archivist/runner.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/sboms.py` & `datatrails_archivist-0.30.1/archivist/sboms.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/subjects.py` & `datatrails_archivist-0.30.1/archivist/subjects.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/subjects_confirmer.py` & `datatrails_archivist-0.30.1/archivist/subjects_confirmer.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/tenancies.py` & `datatrails_archivist-0.30.1/archivist/tenancies.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/timestamp.py` & `datatrails_archivist-0.30.1/archivist/timestamp.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/archivist/utils.py` & `datatrails_archivist-0.30.1/archivist/utils.py`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/datatrails_archivist.egg-info/PKG-INFO` & `datatrails_archivist-0.30.1/datatrails_archivist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datatrails-archivist
-Version: 0.30.0
+Version: 0.30.1
 Summary: DataTrails API
 Home-page: https://github.com/datatrails/datatrails-python
 Author: DataTrails Inc.
 Author-email: support@datatrails.ai
 License: MIT
 Project-URL: Documentation, https://python.datatrails.ai
 Project-URL: Source, https://github.com/datatrails/datatrails-python
@@ -21,15 +21,15 @@
 License-File: LICENSE
 Requires-Dist: backoff~=2.2.1
 Requires-Dist: certifi
 Requires-Dist: flatten-dict~=0.4
 Requires-Dist: iso8601~=2.1
 Requires-Dist: Jinja2~=3.1
 Requires-Dist: pyaml-env~=1.2
-Requires-Dist: requests~=2.31.0
+Requires-Dist: requests~=2.32.0
 Requires-Dist: requests-toolbelt~=1.0
 Requires-Dist: rfc3339~=6.2
 Requires-Dist: xmltodict~=0.13
 
 
 .. _readme:
```

### Comparing `datatrails-archivist-0.30.0/datatrails_archivist.egg-info/SOURCES.txt` & `datatrails_archivist-0.30.1/datatrails_archivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/pyproject.toml` & `datatrails_archivist-0.30.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datatrails-archivist-0.30.0/setup.cfg` & `datatrails_archivist-0.30.1/setup.cfg`

 * *Files identical despite different names*

