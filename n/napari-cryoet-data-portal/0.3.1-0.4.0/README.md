# Comparing `tmp/napari-cryoet-data-portal-0.3.1.tar.gz` & `tmp/napari_cryoet_data_portal-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-cryoet-data-portal-0.3.1.tar", last modified: Mon Apr  1 15:54:15 2024, max compression
+gzip compressed data, was "napari_cryoet_data_portal-0.4.0.tar", last modified: Tue May 21 20:08:32 2024, max compression
```

## Comparing `napari-cryoet-data-portal-0.3.1.tar` & `napari_cryoet_data_portal-0.4.0.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.169181 napari-cryoet-data-portal-0.3.1/
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.111757 napari-cryoet-data-portal-0.3.1/.github/
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.121126 napari-cryoet-data-portal-0.3.1/.github/workflows/
--rw-r--r--   0 asweet     (503) staff       (20)     1649 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/.github/workflows/test.yml
--rw-r--r--   0 asweet     (503) staff       (20)      992 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/.gitignore
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.123386 napari-cryoet-data-portal-0.3.1/.napari-hub/
--rw-r--r--   0 asweet     (503) staff       (20)      463 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 asweet     (503) staff       (20)      542 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/.napari-hub/config.yml
--rw-r--r--   0 asweet     (503) staff       (20)      815 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/.pre-commit-config.yaml
--rw-r--r--   0 asweet     (503) staff       (20)     1093 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/LICENSE
--rw-r--r--   0 asweet     (503) staff       (20)       96 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/MANIFEST.in
--rw-r--r--   0 asweet     (503) staff       (20)     8542 2024-04-01 15:54:15.168736 napari-cryoet-data-portal-0.3.1/PKG-INFO
--rw-r--r--   0 asweet     (503) staff       (20)     6693 2024-03-29 22:24:45.000000 napari-cryoet-data-portal-0.3.1/README.md
--rw-r--r--   0 asweet     (503) staff       (20)      329 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/SECURITY.md
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.125005 napari-cryoet-data-portal-0.3.1/examples/
--rw-r--r--   0 asweet     (503) staff       (20)      205 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/examples/demo-sample.py
--rw-r--r--   0 asweet     (503) staff       (20)      194 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/examples/demo.py
--rw-r--r--   0 asweet     (503) staff       (20)     1272 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/pyproject.toml
--rw-r--r--   0 asweet     (503) staff       (20)     1776 2024-04-01 15:54:15.170489 napari-cryoet-data-portal-0.3.1/setup.cfg
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.113549 napari-cryoet-data-portal-0.3.1/src/
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.143917 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/
--rw-r--r--   0 asweet     (503) staff       (20)      546 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/__init__.py
--rw-r--r--   0 asweet     (503) staff       (20)     3671 2023-12-15 22:27:55.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_filter.py
--rw-r--r--   0 asweet     (503) staff       (20)     1145 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_listing_tree_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     2835 2023-12-15 22:27:55.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_listing_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)      367 2023-11-14 01:00:32.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_logging.py
--rw-r--r--   0 asweet     (503) staff       (20)     2006 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_metadata_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     7095 2024-04-01 15:22:04.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_open_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     4178 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_progress_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     7256 2024-03-29 23:03:57.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_reader.py
--rw-r--r--   0 asweet     (503) staff       (20)     1779 2024-03-29 22:24:45.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_sample_data.py
--rw-r--r--   0 asweet     (503) staff       (20)     1605 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_task_worker.py
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.161445 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/
--rw-r--r--   0 asweet     (503) staff       (20)        0 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/__init__.py
--rw-r--r--   0 asweet     (503) staff       (20)      516 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/_utils.py
--rw-r--r--   0 asweet     (503) staff       (20)      489 2024-03-29 22:24:45.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/conftest.py
--rw-r--r--   0 asweet     (503) staff       (20)     3020 2023-12-15 21:36:22.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_listing_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     1081 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_metadata_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     1561 2024-03-29 22:23:36.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_open_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     1419 2024-03-29 22:24:45.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_reader.py
--rw-r--r--   0 asweet     (503) staff       (20)      962 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_sample.py
--rw-r--r--   0 asweet     (503) staff       (20)     2147 2023-12-15 21:36:22.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_uri_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     2349 2023-12-15 21:36:22.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     4670 2023-12-15 21:36:22.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_uri_widget.py
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.163442 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_vendored/
--rw-r--r--   0 asweet     (503) staff       (20)        0 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_vendored/__init__.py
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.164543 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_vendored/superqt/
--rw-r--r--   0 asweet     (503) staff       (20)        0 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_vendored/superqt/__init__.py
--rw-r--r--   0 asweet     (503) staff       (20)     6472 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_vendored/superqt/_searchable_tree_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)      411 2024-04-01 15:54:14.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_version.py
--rw-r--r--   0 asweet     (503) staff       (20)     3029 2023-12-15 22:27:55.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_widget.py
--rw-r--r--   0 asweet     (503) staff       (20)     1659 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/napari.yaml
-drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-04-01 15:54:15.166086 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/
--rw-r--r--   0 asweet     (503) staff       (20)     8542 2024-04-01 15:54:14.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/PKG-INFO
--rw-r--r--   0 asweet     (503) staff       (20)     1946 2024-04-01 15:54:15.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/SOURCES.txt
--rw-r--r--   0 asweet     (503) staff       (20)        1 2024-04-01 15:54:14.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/dependency_links.txt
--rw-r--r--   0 asweet     (503) staff       (20)       84 2024-04-01 15:54:15.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/entry_points.txt
--rw-r--r--   0 asweet     (503) staff       (20)      155 2024-04-01 15:54:15.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/requires.txt
--rw-r--r--   0 asweet     (503) staff       (20)       26 2024-04-01 15:54:15.000000 napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/top_level.txt
--rw-r--r--   0 asweet     (503) staff       (20)      624 2023-08-11 19:57:13.000000 napari-cryoet-data-portal-0.3.1/tox.ini
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-05-21 20:08:32.694780 napari_cryoet_data_portal-0.4.0/
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-05-21 20:08:32.686353 napari_cryoet_data_portal-0.4.0/.github/
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-05-21 20:08:32.688274 napari_cryoet_data_portal-0.4.0/.github/workflows/
+-rw-r--r--   0 asweet     (503) staff       (20)     1649 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/.github/workflows/test.yml
+-rw-r--r--   0 asweet     (503) staff       (20)      992 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/.gitignore
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-05-21 20:08:32.688697 napari_cryoet_data_portal-0.4.0/.napari-hub/
+-rw-r--r--   0 asweet     (503) staff       (20)      463 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 asweet     (503) staff       (20)      542 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/.napari-hub/config.yml
+-rw-r--r--   0 asweet     (503) staff       (20)      815 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/.pre-commit-config.yaml
+-rw-r--r--   0 asweet     (503) staff       (20)     1093 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/LICENSE
+-rw-r--r--   0 asweet     (503) staff       (20)       96 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/MANIFEST.in
+-rw-r--r--   0 asweet     (503) staff       (20)     8592 2024-05-21 20:08:32.694674 napari_cryoet_data_portal-0.4.0/PKG-INFO
+-rw-r--r--   0 asweet     (503) staff       (20)     6693 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/README.md
+-rw-r--r--   0 asweet     (503) staff       (20)      329 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/SECURITY.md
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-05-21 20:08:32.688973 napari_cryoet_data_portal-0.4.0/examples/
+-rw-r--r--   0 asweet     (503) staff       (20)      205 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/examples/demo-sample.py
+-rw-r--r--   0 asweet     (503) staff       (20)      194 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/examples/demo.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1272 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/pyproject.toml
+-rw-r--r--   0 asweet     (503) staff       (20)     1798 2024-05-21 20:08:32.695093 napari_cryoet_data_portal-0.4.0/setup.cfg
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-05-21 20:08:32.686745 napari_cryoet_data_portal-0.4.0/src/
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-05-21 20:08:32.691059 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/
+-rw-r--r--   0 asweet     (503) staff       (20)      546 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/__init__.py
+-rw-r--r--   0 asweet     (503) staff       (20)     3671 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_filter.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1145 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_listing_tree_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     2835 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_listing_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)      367 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_logging.py
+-rw-r--r--   0 asweet     (503) staff       (20)     2006 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_metadata_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     7512 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_open_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     4178 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_progress_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)    10824 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_reader.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1779 2024-05-21 18:35:12.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_sample_data.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1605 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_task_worker.py
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-05-21 20:08:32.693264 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/
+-rw-r--r--   0 asweet     (503) staff       (20)        0 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/__init__.py
+-rw-r--r--   0 asweet     (503) staff       (20)      516 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/_utils.py
+-rw-r--r--   0 asweet     (503) staff       (20)      718 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/conftest.py
+-rw-r--r--   0 asweet     (503) staff       (20)     3020 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/test_listing_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1081 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/test_metadata_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1559 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/test_open_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     2164 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/test_reader.py
+-rw-r--r--   0 asweet     (503) staff       (20)      962 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/test_sample.py
+-rw-r--r--   0 asweet     (503) staff       (20)     2147 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/test_uri_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     2349 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/test_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     4670 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_uri_widget.py
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-05-21 20:08:32.693400 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_vendored/
+-rw-r--r--   0 asweet     (503) staff       (20)        0 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_vendored/__init__.py
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-05-21 20:08:32.693638 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_vendored/superqt/
+-rw-r--r--   0 asweet     (503) staff       (20)        0 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_vendored/superqt/__init__.py
+-rw-r--r--   0 asweet     (503) staff       (20)     6472 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_vendored/superqt/_searchable_tree_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)      411 2024-05-21 20:08:32.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_version.py
+-rw-r--r--   0 asweet     (503) staff       (20)     3029 2024-05-21 20:03:13.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_widget.py
+-rw-r--r--   0 asweet     (503) staff       (20)     1659 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/napari.yaml
+drwxr-xr-x   0 asweet     (503) staff       (20)        0 2024-05-21 20:08:32.693998 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal.egg-info/
+-rw-r--r--   0 asweet     (503) staff       (20)     8592 2024-05-21 20:08:32.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal.egg-info/PKG-INFO
+-rw-r--r--   0 asweet     (503) staff       (20)     1946 2024-05-21 20:08:32.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal.egg-info/SOURCES.txt
+-rw-r--r--   0 asweet     (503) staff       (20)        1 2024-05-21 20:08:32.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal.egg-info/dependency_links.txt
+-rw-r--r--   0 asweet     (503) staff       (20)       84 2024-05-21 20:08:32.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal.egg-info/entry_points.txt
+-rw-r--r--   0 asweet     (503) staff       (20)      175 2024-05-21 20:08:32.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal.egg-info/requires.txt
+-rw-r--r--   0 asweet     (503) staff       (20)       26 2024-05-21 20:08:32.000000 napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal.egg-info/top_level.txt
+-rw-r--r--   0 asweet     (503) staff       (20)      624 2024-05-20 18:20:55.000000 napari_cryoet_data_portal-0.4.0/tox.ini
```

### Comparing `napari-cryoet-data-portal-0.3.1/.github/workflows/test.yml` & `napari_cryoet_data_portal-0.4.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/.gitignore` & `napari_cryoet_data_portal-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/.napari-hub/config.yml` & `napari_cryoet_data_portal-0.4.0/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/.pre-commit-config.yaml` & `napari_cryoet_data_portal-0.4.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/LICENSE` & `napari_cryoet_data_portal-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/PKG-INFO` & `napari_cryoet_data_portal-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-cryoet-data-portal
-Version: 0.3.1
+Version: 0.4.0
 Summary: List, preview, and open data from the CZII CryoET Data Portal
 Home-page: https://github.com/chanzuckerberg/napari-cryoet-data-portal
 Author: Andy Sweet
 Author-email: andrewdsweet@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/chanzuckerberg/napari-cryoet-data-portal/issues
 Project-URL: Documentation, https://github.com/chanzuckerberg/napari-cryoet-data-portal#README.md
@@ -21,18 +21,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cmap
 Requires-Dist: cryoet_data_portal~=3.0
 Requires-Dist: fsspec[http,s3]
 Requires-Dist: npe2
 Requires-Dist: numpy
+Requires-Dist: napari>=0.4.19
 Requires-Dist: napari_ome_zarr
 Requires-Dist: ndjson
 Requires-Dist: qtpy
 Requires-Dist: superqt
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
```

### Comparing `napari-cryoet-data-portal-0.3.1/README.md` & `napari_cryoet_data_portal-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/pyproject.toml` & `napari_cryoet_data_portal-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/setup.cfg` & `napari_cryoet_data_portal-0.4.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -26,18 +26,20 @@
 	Documentation = https://github.com/chanzuckerberg/napari-cryoet-data-portal#README.md
 	Source Code = https://github.com/chanzuckerberg/napari-cryoet-data-portal
 	User Support = https://github.com/chanzuckerberg/napari-cryoet-data-portal/issues
 
 [options]
 packages = find:
 install_requires = 
+	cmap
 	cryoet_data_portal ~= 3.0
 	fsspec[http,s3]
 	npe2
 	numpy
+	napari>=0.4.19
 	napari_ome_zarr
 	ndjson
 	qtpy
 	superqt
 python_requires = >=3.8
 include_package_data = True
 package_dir =
```

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/__init__.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/__init__.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_filter.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_filter.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_listing_tree_widget.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_listing_tree_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_listing_widget.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_listing_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_metadata_widget.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_metadata_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_open_widget.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_open_widget.py`

 * *Files 24% similar despite different names*

```diff
@@ -15,39 +15,29 @@
     QWidget,
 )
 from cryoet_data_portal import Annotation, Client, Tomogram
 
 from napari_cryoet_data_portal._logging import logger
 from napari_cryoet_data_portal._progress_widget import ProgressWidget
 from napari_cryoet_data_portal._reader import (
-    read_annotation,
+    read_annotation_files,
     read_tomogram,
 )
 
 if TYPE_CHECKING:
     from napari.components import ViewerModel
 
 
 # TODO: read these from metadata instead of hard-coding them.
 @dataclass
 class Resolution:
     name: str
     indices: Tuple[int, ...]
     scale: float
 
-    @property
-    def offset(self) -> float:
-        """The offset due to a larger first pixel for lower resolutions.
-
-        When visualized in napari, this ensures that the different multi-scale
-        layers opened separately share the same visual extent in the canvas that
-        starts at (-0.5, -0.5, -0.5).
-        """
-        return (self.scale - 1) / 2
-
 
 MULTI_RESOLUTION = Resolution(name="Multi", indices=(0, 1, 2), scale=1)
 HIGH_RESOLUTION = Resolution(name="High", indices=(0,), scale=1)
 MID_RESOLUTION = Resolution(name="Mid", indices=(1,), scale=2)
 LOW_RESOLUTION = Resolution(name="Low", indices=(2,), scale=4)
 
 RESOLUTIONS: Tuple[Resolution, ...] = (
@@ -134,61 +124,78 @@
 
     def _loadTomogram(
         self,
         tomogram: Tomogram,
         resolution: Resolution,
     ) -> Generator[FullLayerData, None, None]:
         logger.debug("OpenWidget._loadTomogram: %s", tomogram.name)
-        image_data, image_attrs, _ = read_tomogram(tomogram)
-        # Skip indexing for multi-resolution to avoid adding any
-        # unnecessary nodes to the dask compute graph.
-        if resolution is not MULTI_RESOLUTION:
-            image_data = image_data[resolution.indices[0]]
-        # Materialize low resolution immediately on this thread to prevent napari blocking.
-        if resolution is LOW_RESOLUTION:
-            image_data = np.asarray(image_data)
-        # Get scale before resolution scaling for annotations.
-        image_scale = image_attrs["scale"]
-        image_attrs["scale"] = tuple(
-            resolution.scale * s for s in image_scale
-        )
-        image_translate = image_attrs.get("translate", (0,) * len(image_attrs["scale"]))
-        image_attrs["translate"] = tuple(
-            resolution.offset + t for t in image_translate
-        )
-        yield image_data, image_attrs, "image"
+        image_layer = read_tomogram(tomogram)
+        # Extract image_scale before the resolution is taken into account,
+        # so we can use it to align other annotations later.
+        image_scale = image_layer[1]["scale"]
+        yield _handle_image_at_resolution(image_layer, resolution)
 
         # Looking up tomogram.tomogram_voxel_spacing.annotations triggers a query
         # using the client from where the tomogram was found.
         # A single client is not thread safe, so we need a new instance for each query.
         client = Client(self._uri)
         annotations = Annotation.find(
             client, 
             [Annotation.tomogram_voxel_spacing_id == tomogram.tomogram_voxel_spacing_id],
         )
 
         for annotation in annotations:
-            point_paths = tuple(
-                f.https_path
-                for f in annotation.files
-                if f.shape_type == "Point"
-            )
-            if len(point_paths) > 0:
-                anno_data, anno_attrs, anno_type = read_annotation(annotation, tomogram=tomogram)
-                # Inherit scale from full resolution image so that we can pick up
-                # that scale when it changes.
-                anno_attrs["scale"] = image_scale
-                # Scaling points also changes the size, so adjust accordingly.
-                anno_attrs["size"] /= np.mean(image_scale)
-                yield anno_data, anno_attrs, anno_type
-            else:
-                logger.warn("Found no points annotations. Skipping.")
+            for layer in read_annotation_files(annotation, tomogram=tomogram):
+                if layer[2] == "labels":
+                    layer = _handle_image_at_resolution(layer, resolution)
+                elif layer[2] == "points":
+                    layer = _handle_points_at_scale(layer, image_scale)
+                yield layer
 
     def _onLayerLoaded(self, layer_data: FullLayerData) -> None:
         logger.debug("OpenWidget._onLayerLoaded")
         data, attrs, layer_type = layer_data
         if layer_type == "image":
             self._viewer.add_image(data, **attrs)
         elif layer_type == "points":
             self._viewer.add_points(data, **attrs)
+        elif layer_type == "labels":
+            self._viewer.add_labels(data, **attrs)
         else:
             raise AssertionError(f"Unexpected {layer_type=}")
+
+
+def _handle_image_at_resolution(layer_data: FullLayerData, resolution: Resolution) -> FullLayerData:
+    data, attrs, layer_type = layer_data
+    # Skip indexing for multi-resolution to avoid adding any
+    # unnecessary nodes to the dask compute graph.
+    if resolution is not MULTI_RESOLUTION:
+        data = data[resolution.indices[0]]
+
+    # Materialize low resolution immediately on this thread to prevent napari blocking.
+    # Once async loading is working on a stable napari release, we could remove this.
+    if resolution is LOW_RESOLUTION:
+        data = np.asarray(data)
+
+    # Adjust the scale and and translation based on the resolution.
+    image_scale = attrs["scale"]
+    attrs["scale"] = tuple(resolution.scale * s for s in image_scale)
+    # Offset the translation due to a larger first pixel for lower resolutions.
+    # When visualized in napari, this ensures that the different multi-scale
+    # layers opened separately share the same visual extent in the canvas that
+    # starts at some scaled version of (-0.5, -0.5, -0.5).
+    image_translate = attrs.get("translate", (0,) * len(image_scale))
+    attrs["translate"] = tuple(
+        (s * (resolution.scale - 1) / 2) + t
+        for s, t in zip(image_scale, image_translate)
+    )
+    return data, attrs, layer_type
+
+
+def _handle_points_at_scale(layer_data: FullLayerData, image_scale: Tuple[float, float, float]) -> FullLayerData:
+    data, attrs, layer_type = layer_data
+    # Inherit scale from full resolution image, so that points are visually
+    # aligned with the image.
+    attrs["scale"] = image_scale
+    # Scaling points also changes the size, so adjust accordingly.
+    attrs["size"] /= np.mean(image_scale)
+    return data, attrs, layer_type
```

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_progress_widget.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_progress_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_sample_data.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_sample_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -32,20 +32,20 @@
     tomogram_image = (np.asarray(tomogram_image[0][-1]), *tomogram_image[1:])
     tomogram_image[1]["scale"] = (4, 4, 4)
 
     annotations = tuple(tomogram_spacing.annotations)
     ribosome_annotations = [
         item
         for item in annotations
-        if item.object_name.lower() == "cytosolic ribosome"
+        if "cytosolic ribosome" in item.object_name.lower()
     ].pop()
     fas_annotations = [
         item
         for item in annotations
-        if item.object_name.lower() == "fatty acid synthase"
+        if "fatty acid synthase" in item.object_name.lower()
     ].pop()
     ribosome_points = read_annotation(ribosome_annotations, tomogram=tomogram)
     fatty_acid_points = read_annotation(fas_annotations, tomogram=tomogram)
 
     return [
         tomogram_image,
         ribosome_points,
```

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_task_worker.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_task_worker.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/_utils.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/_utils.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_listing_widget.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/test_listing_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_metadata_widget.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/test_metadata_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_open_widget.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/test_open_widget.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,21 +32,21 @@
     widget._viewer.layers.append(Points())
     assert len(widget._viewer.layers) == 1
     assert widget._clear_existing_layers.isChecked()
     
     with qtbot.waitSignal(widget._progress.finished, timeout=30000):
         widget.setTomogram(tomogram)
     
-    assert len(widget._viewer.layers) == 3
+    assert len(widget._viewer.layers) > 1
 
 
 def test_set_tomogram_adds_layers_to_viewer_without_clearing_existing(widget: OpenWidget, tomogram: Tomogram, qtbot: QtBot):
     assert len(widget._viewer.layers) == 0
     widget._viewer.layers.append(Points())
     assert len(widget._viewer.layers) == 1
     widget._clear_existing_layers.setChecked(False)
 
     with qtbot.waitSignal(widget._progress.finished, timeout=30000):
         widget.setTomogram(tomogram)
 
-    assert len(widget._viewer.layers) == 4
+    assert len(widget._viewer.layers) > 1
```

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_sample.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_uri_widget.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/test_uri_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_tests/test_widget.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_uri_widget.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_uri_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_vendored/superqt/_searchable_tree_widget.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_vendored/superqt/_searchable_tree_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/_widget.py` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal/napari.yaml` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/PKG-INFO` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-cryoet-data-portal
-Version: 0.3.1
+Version: 0.4.0
 Summary: List, preview, and open data from the CZII CryoET Data Portal
 Home-page: https://github.com/chanzuckerberg/napari-cryoet-data-portal
 Author: Andy Sweet
 Author-email: andrewdsweet@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/chanzuckerberg/napari-cryoet-data-portal/issues
 Project-URL: Documentation, https://github.com/chanzuckerberg/napari-cryoet-data-portal#README.md
@@ -21,18 +21,20 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Image Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cmap
 Requires-Dist: cryoet_data_portal~=3.0
 Requires-Dist: fsspec[http,s3]
 Requires-Dist: npe2
 Requires-Dist: numpy
+Requires-Dist: napari>=0.4.19
 Requires-Dist: napari_ome_zarr
 Requires-Dist: ndjson
 Requires-Dist: qtpy
 Requires-Dist: superqt
 Provides-Extra: testing
 Requires-Dist: tox; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
```

### Comparing `napari-cryoet-data-portal-0.3.1/src/napari_cryoet_data_portal.egg-info/SOURCES.txt` & `napari_cryoet_data_portal-0.4.0/src/napari_cryoet_data_portal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-cryoet-data-portal-0.3.1/tox.ini` & `napari_cryoet_data_portal-0.4.0/tox.ini`

 * *Files identical despite different names*

