# Comparing `tmp/osm2gmns-0.7.5.tar.gz` & `tmp/osm2gmns-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osm2gmns-0.7.5.tar", last modified: Fri Feb 23 21:11:18 2024, max compression
+gzip compressed data, was "osm2gmns-0.7.6.tar", last modified: Tue May 21 19:32:35 2024, max compression
```

## Comparing `osm2gmns-0.7.5.tar` & `osm2gmns-0.7.6.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2024-02-23 21:11:18.707685 osm2gmns-0.7.5/
--rw-rw-rw-   0        0        0    35821 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/LICENSE
--rw-rw-rw-   0        0        0     6523 2024-02-23 21:11:18.705686 osm2gmns-0.7.5/PKG-INFO
--rw-rw-rw-   0        0        0     5823 2024-02-05 19:19:30.000000 osm2gmns-0.7.5/README.rst
-drwxrwxrwx   0        0        0        0 2024-02-23 21:11:18.567626 osm2gmns-0.7.5/osm2gmns/
--rw-rw-rw-   0        0        0     1681 2024-02-23 21:10:41.000000 osm2gmns-0.7.5/osm2gmns/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-23 21:11:18.600989 osm2gmns-0.7.5/osm2gmns/func_lib/
--rw-rw-rw-   0        0        0      517 2024-02-05 02:06:31.000000 osm2gmns-0.7.5/osm2gmns/func_lib/__init__.py
--rw-rw-rw-   0        0        0    10900 2024-02-05 02:16:19.000000 osm2gmns-0.7.5/osm2gmns/func_lib/extract_relation_id.py
-drwxrwxrwx   0        0        0        0 2024-02-23 21:11:18.623795 osm2gmns-0.7.5/osm2gmns/io/
--rw-rw-rw-   0        0        0        0 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/io/__init__.py
--rw-rw-rw-   0        0        0     3822 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/io/downloader.py
--rw-rw-rw-   0        0        0    24925 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/io/load_from_csv.py
--rw-rw-rw-   0        0        0     5765 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/io/output_mrnet.py
--rw-rw-rw-   0        0        0    10388 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/io/read_from_osm.py
--rw-rw-rw-   0        0        0     4513 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/io/readfile_mp.py
--rw-rw-rw-   0        0        0      625 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/io/util_io.py
--rw-rw-rw-   0        0        0     8994 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/io/writefile.py
-drwxrwxrwx   0        0        0        0 2024-02-23 21:11:18.641970 osm2gmns-0.7.5/osm2gmns/movement/
--rw-rw-rw-   0        0        0        0 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/movement/__init__.py
--rw-rw-rw-   0        0        0     5982 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/movement/autoconintd.py
--rw-rw-rw-   0        0        0     1690 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/movement/autoconm.py
--rw-rw-rw-   0        0        0     2329 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/movement/exp_auto_connection.py
--rw-rw-rw-   0        0        0      107 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/movement/exp_connection_from_turns.py
--rw-rw-rw-   0        0        0      317 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/movement/exp_generate_movements.py
--rw-rw-rw-   0        0        0     9316 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/movement/generate_movements.py
--rw-rw-rw-   0        0        0     1747 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/movement/util_mvmt.py
-drwxrwxrwx   0        0        0        0 2024-02-23 21:11:18.650428 osm2gmns-0.7.5/osm2gmns/multiresolutionnet/
--rw-rw-rw-   0        0        0        0 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/multiresolutionnet/__init__.py
--rw-rw-rw-   0        0        0    12903 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/multiresolutionnet/build_mrnet.py
--rw-rw-rw-   0        0        0    31005 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/multiresolutionnet/netgen.py
-drwxrwxrwx   0        0        0        0 2024-02-23 21:11:18.660447 osm2gmns-0.7.5/osm2gmns/networkclass/
--rw-rw-rw-   0        0        0        0 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/networkclass/__init__.py
--rw-rw-rw-   0        0        0     1416 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/networkclass/basenet.py
--rw-rw-rw-   0        0        0    11127 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/networkclass/macronet.py
--rw-rw-rw-   0        0        0     3747 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/networkclass/mesonet.py
--rw-rw-rw-   0        0        0     1894 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/networkclass/micronet.py
-drwxrwxrwx   0        0        0        0 2024-02-23 21:11:18.688758 osm2gmns-0.7.5/osm2gmns/osmnet/
--rw-rw-rw-   0        0        0        0 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/osmnet/__init__.py
--rw-rw-rw-   0        0        0    21605 2024-02-04 21:18:53.000000 osm2gmns-0.7.5/osm2gmns/osmnet/build_net.py
--rw-rw-rw-   0        0        0     6004 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/osmnet/check_args.py
--rw-rw-rw-   0        0        0     3838 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/osmnet/combine_links.py
--rw-rw-rw-   0        0        0     9965 2024-02-04 21:18:53.000000 osm2gmns-0.7.5/osm2gmns/osmnet/complex_intersection.py
--rw-rw-rw-   0        0        0     4035 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/osmnet/enrich_net_info.py
--rw-rw-rw-   0        0        0     3617 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/osmnet/osmclasses.py
--rw-rw-rw-   0        0        0    11290 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/osmnet/pois.py
--rw-rw-rw-   0        0        0     2703 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/osmnet/visualization.py
--rw-rw-rw-   0        0        0     2691 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/osmnet/wayfilters.py
--rw-rw-rw-   0        0        0     3372 2023-05-30 20:33:52.000000 osm2gmns-0.7.5/osm2gmns/settings.py
-drwxrwxrwx   0        0        0        0 2024-02-23 21:11:18.698737 osm2gmns-0.7.5/osm2gmns/utils/
--rw-rw-rw-   0        0        0        0 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/utils/__init__.py
--rw-rw-rw-   0        0        0     2105 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/utils/util.py
--rw-rw-rw-   0        0        0     6162 2023-03-02 19:34:08.000000 osm2gmns-0.7.5/osm2gmns/utils/util_coord.py
--rw-rw-rw-   0        0        0     5245 2023-02-20 17:34:51.000000 osm2gmns-0.7.5/osm2gmns/utils/util_geo.py
-drwxrwxrwx   0        0        0        0 2024-02-23 21:11:18.596632 osm2gmns-0.7.5/osm2gmns.egg-info/
--rw-rw-rw-   0        0        0     6523 2024-02-23 21:11:18.000000 osm2gmns-0.7.5/osm2gmns.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2024-02-23 21:11:18.000000 osm2gmns-0.7.5/osm2gmns.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-23 21:11:18.000000 osm2gmns-0.7.5/osm2gmns.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       97 2024-02-23 21:11:18.000000 osm2gmns-0.7.5/osm2gmns.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-02-23 21:11:18.000000 osm2gmns-0.7.5/osm2gmns.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-23 21:11:18.708736 osm2gmns-0.7.5/setup.cfg
--rw-rw-rw-   0        0        0     1017 2024-02-23 21:10:47.000000 osm2gmns-0.7.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-02-23 21:11:18.703686 osm2gmns-0.7.5/tests/
--rw-rw-rw-   0        0        0      280 2024-02-05 00:16:37.000000 osm2gmns-0.7.5/tests/__init__.py
--rw-rw-rw-   0        0        0      747 2024-02-05 00:28:24.000000 osm2gmns-0.7.5/tests/test_relation_id_finder.py
+drwxr-xr-x   0 jlu486     (503) staff       (20)        0 2024-05-21 19:32:35.684394 osm2gmns-0.7.6/
+-rw-r--r--   0 jlu486     (503) staff       (20)    35147 2024-05-21 15:39:43.000000 osm2gmns-0.7.6/LICENSE
+-rw-r--r--   0 jlu486     (503) staff       (20)     6089 2024-05-21 19:32:35.684099 osm2gmns-0.7.6/PKG-INFO
+-rw-r--r--   0 jlu486     (503) staff       (20)     5228 2024-05-21 19:28:49.000000 osm2gmns-0.7.6/README.rst
+drwxr-xr-x   0 jlu486     (503) staff       (20)        0 2024-05-21 19:32:35.661018 osm2gmns-0.7.6/osm2gmns/
+-rw-r--r--   0 jlu486     (503) staff       (20)     1626 2024-05-21 19:10:06.000000 osm2gmns-0.7.6/osm2gmns/__init__.py
+drwxr-xr-x   0 jlu486     (503) staff       (20)        0 2024-05-21 19:32:35.663698 osm2gmns-0.7.6/osm2gmns/func_lib/
+-rw-r--r--   0 jlu486     (503) staff       (20)      506 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/func_lib/__init__.py
+-rw-r--r--   0 jlu486     (503) staff       (20)    10652 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/func_lib/extract_relation_id.py
+drwxr-xr-x   0 jlu486     (503) staff       (20)        0 2024-05-21 19:32:35.668115 osm2gmns-0.7.6/osm2gmns/io/
+-rw-r--r--   0 jlu486     (503) staff       (20)        0 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/io/__init__.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     3716 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/io/downloader.py
+-rw-r--r--   0 jlu486     (503) staff       (20)    24347 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/io/load_from_csv.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     5653 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/io/output_mrnet.py
+-rw-r--r--   0 jlu486     (503) staff       (20)    10094 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/io/read_from_osm.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     4366 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/io/readfile_mp.py
+-rw-r--r--   0 jlu486     (503) staff       (20)      607 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/io/util_io.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     8817 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/io/writefile.py
+drwxr-xr-x   0 jlu486     (503) staff       (20)        0 2024-05-21 19:32:35.672864 osm2gmns-0.7.6/osm2gmns/movement/
+-rw-r--r--   0 jlu486     (503) staff       (20)        0 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/movement/__init__.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     5873 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/movement/autoconintd.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     1647 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/movement/autoconm.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     2246 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/movement/exp_auto_connection.py
+-rw-r--r--   0 jlu486     (503) staff       (20)      101 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/movement/exp_connection_from_turns.py
+-rw-r--r--   0 jlu486     (503) staff       (20)      304 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/movement/exp_generate_movements.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     9137 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/movement/generate_movements.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     1690 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/movement/util_mvmt.py
+drwxr-xr-x   0 jlu486     (503) staff       (20)        0 2024-05-21 19:32:35.674227 osm2gmns-0.7.6/osm2gmns/multiresolutionnet/
+-rw-r--r--   0 jlu486     (503) staff       (20)        0 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/multiresolutionnet/__init__.py
+-rw-r--r--   0 jlu486     (503) staff       (20)    12622 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/multiresolutionnet/build_mrnet.py
+-rw-r--r--   0 jlu486     (503) staff       (20)    30482 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/multiresolutionnet/netgen.py
+drwxr-xr-x   0 jlu486     (503) staff       (20)        0 2024-05-21 19:32:35.676271 osm2gmns-0.7.6/osm2gmns/networkclass/
+-rw-r--r--   0 jlu486     (503) staff       (20)        0 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/networkclass/__init__.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     1353 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/networkclass/basenet.py
+-rw-r--r--   0 jlu486     (503) staff       (20)    10803 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/networkclass/macronet.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     3637 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/networkclass/mesonet.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     1835 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/networkclass/micronet.py
+drwxr-xr-x   0 jlu486     (503) staff       (20)        0 2024-05-21 19:32:35.680538 osm2gmns-0.7.6/osm2gmns/osmnet/
+-rw-r--r--   0 jlu486     (503) staff       (20)        0 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/osmnet/__init__.py
+-rw-r--r--   0 jlu486     (503) staff       (20)    21114 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/osmnet/build_net.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     5864 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/osmnet/check_args.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     3719 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/osmnet/combine_links.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     9743 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/osmnet/complex_intersection.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     5560 2024-05-21 18:58:22.000000 osm2gmns-0.7.6/osm2gmns/osmnet/enrich_net_info.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     3495 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/osmnet/osmclasses.py
+-rw-r--r--   0 jlu486     (503) staff       (20)    11017 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/osmnet/pois.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     2606 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/osmnet/visualization.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     2624 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/osmnet/wayfilters.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     3305 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/settings.py
+drwxr-xr-x   0 jlu486     (503) staff       (20)        0 2024-05-21 19:32:35.682242 osm2gmns-0.7.6/osm2gmns/utils/
+-rw-r--r--   0 jlu486     (503) staff       (20)        0 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/utils/__init__.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     2046 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/utils/util.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     5975 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/utils/util_coord.py
+-rw-r--r--   0 jlu486     (503) staff       (20)     5112 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/osm2gmns/utils/util_geo.py
+drwxr-xr-x   0 jlu486     (503) staff       (20)        0 2024-05-21 19:32:35.683617 osm2gmns-0.7.6/osm2gmns.egg-info/
+-rw-r--r--   0 jlu486     (503) staff       (20)     6089 2024-05-21 19:32:35.000000 osm2gmns-0.7.6/osm2gmns.egg-info/PKG-INFO
+-rw-r--r--   0 jlu486     (503) staff       (20)     1564 2024-05-21 19:32:35.000000 osm2gmns-0.7.6/osm2gmns.egg-info/SOURCES.txt
+-rw-r--r--   0 jlu486     (503) staff       (20)        1 2024-05-21 19:32:35.000000 osm2gmns-0.7.6/osm2gmns.egg-info/dependency_links.txt
+-rw-r--r--   0 jlu486     (503) staff       (20)      112 2024-05-21 19:32:35.000000 osm2gmns-0.7.6/osm2gmns.egg-info/requires.txt
+-rw-r--r--   0 jlu486     (503) staff       (20)       15 2024-05-21 19:32:35.000000 osm2gmns-0.7.6/osm2gmns.egg-info/top_level.txt
+-rw-r--r--   0 jlu486     (503) staff       (20)       38 2024-05-21 19:32:35.684461 osm2gmns-0.7.6/setup.cfg
+-rw-r--r--   0 jlu486     (503) staff       (20)     1183 2024-05-21 19:29:37.000000 osm2gmns-0.7.6/setup.py
+drwxr-xr-x   0 jlu486     (503) staff       (20)        0 2024-05-21 19:32:35.683104 osm2gmns-0.7.6/tests/
+-rw-r--r--   0 jlu486     (503) staff       (20)      272 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/tests/__init__.py
+-rw-r--r--   0 jlu486     (503) staff       (20)      717 2024-05-21 15:39:44.000000 osm2gmns-0.7.6/tests/test_relation_id_finder.py
```

### Comparing `osm2gmns-0.7.5/LICENSE` & `osm2gmns-0.7.6/LICENSE`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,674 +1,674 @@
-                    GNU GENERAL PUBLIC LICENSE
-                       Version 3, 29 June 2007
-
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
- Everyone is permitted to copy and distribute verbatim copies
- of this license document, but changing it is not allowed.
-
-                            Preamble
-
-  The GNU General Public License is a free, copyleft license for
-software and other kinds of works.
-
-  The licenses for most software and other practical works are designed
-to take away your freedom to share and change the works.  By contrast,
-the GNU General Public License is intended to guarantee your freedom to
-share and change all versions of a program--to make sure it remains free
-software for all its users.  We, the Free Software Foundation, use the
-GNU General Public License for most of our software; it applies also to
-any other work released this way by its authors.  You can apply it to
-your programs, too.
-
-  When we speak of free software, we are referring to freedom, not
-price.  Our General Public Licenses are designed to make sure that you
-have the freedom to distribute copies of free software (and charge for
-them if you wish), that you receive source code or can get it if you
-want it, that you can change the software or use pieces of it in new
-free programs, and that you know you can do these things.
-
-  To protect your rights, we need to prevent others from denying you
-these rights or asking you to surrender the rights.  Therefore, you have
-certain responsibilities if you distribute copies of the software, or if
-you modify it: responsibilities to respect the freedom of others.
-
-  For example, if you distribute copies of such a program, whether
-gratis or for a fee, you must pass on to the recipients the same
-freedoms that you received.  You must make sure that they, too, receive
-or can get the source code.  And you must show them these terms so they
-know their rights.
-
-  Developers that use the GNU GPL protect your rights with two steps:
-(1) assert copyright on the software, and (2) offer you this License
-giving you legal permission to copy, distribute and/or modify it.
-
-  For the developers' and authors' protection, the GPL clearly explains
-that there is no warranty for this free software.  For both users' and
-authors' sake, the GPL requires that modified versions be marked as
-changed, so that their problems will not be attributed erroneously to
-authors of previous versions.
-
-  Some devices are designed to deny users access to install or run
-modified versions of the software inside them, although the manufacturer
-can do so.  This is fundamentally incompatible with the aim of
-protecting users' freedom to change the software.  The systematic
-pattern of such abuse occurs in the area of products for individuals to
-use, which is precisely where it is most unacceptable.  Therefore, we
-have designed this version of the GPL to prohibit the practice for those
-products.  If such problems arise substantially in other domains, we
-stand ready to extend this provision to those domains in future versions
-of the GPL, as needed to protect the freedom of users.
-
-  Finally, every program is threatened constantly by software patents.
-States should not allow patents to restrict development and use of
-software on general-purpose computers, but in those that do, we wish to
-avoid the special danger that patents applied to a free program could
-make it effectively proprietary.  To prevent this, the GPL assures that
-patents cannot be used to render the program non-free.
-
-  The precise terms and conditions for copying, distribution and
-modification follow.
-
-                       TERMS AND CONDITIONS
-
-  0. Definitions.
-
-  "This License" refers to version 3 of the GNU General Public License.
-
-  "Copyright" also means copyright-like laws that apply to other kinds of
-works, such as semiconductor masks.
-
-  "The Program" refers to any copyrightable work licensed under this
-License.  Each licensee is addressed as "you".  "Licensees" and
-"recipients" may be individuals or organizations.
-
-  To "modify" a work means to copy from or adapt all or part of the work
-in a fashion requiring copyright permission, other than the making of an
-exact copy.  The resulting work is called a "modified version" of the
-earlier work or a work "based on" the earlier work.
-
-  A "covered work" means either the unmodified Program or a work based
-on the Program.
-
-  To "propagate" a work means to do anything with it that, without
-permission, would make you directly or secondarily liable for
-infringement under applicable copyright law, except executing it on a
-computer or modifying a private copy.  Propagation includes copying,
-distribution (with or without modification), making available to the
-public, and in some countries other activities as well.
-
-  To "convey" a work means any kind of propagation that enables other
-parties to make or receive copies.  Mere interaction with a user through
-a computer network, with no transfer of a copy, is not conveying.
-
-  An interactive user interface displays "Appropriate Legal Notices"
-to the extent that it includes a convenient and prominently visible
-feature that (1) displays an appropriate copyright notice, and (2)
-tells the user that there is no warranty for the work (except to the
-extent that warranties are provided), that licensees may convey the
-work under this License, and how to view a copy of this License.  If
-the interface presents a list of user commands or options, such as a
-menu, a prominent item in the list meets this criterion.
-
-  1. Source Code.
-
-  The "source code" for a work means the preferred form of the work
-for making modifications to it.  "Object code" means any non-source
-form of a work.
-
-  A "Standard Interface" means an interface that either is an official
-standard defined by a recognized standards body, or, in the case of
-interfaces specified for a particular programming language, one that
-is widely used among developers working in that language.
-
-  The "System Libraries" of an executable work include anything, other
-than the work as a whole, that (a) is included in the normal form of
-packaging a Major Component, but which is not part of that Major
-Component, and (b) serves only to enable use of the work with that
-Major Component, or to implement a Standard Interface for which an
-implementation is available to the public in source code form.  A
-"Major Component", in this context, means a major essential component
-(kernel, window system, and so on) of the specific operating system
-(if any) on which the executable work runs, or a compiler used to
-produce the work, or an object code interpreter used to run it.
-
-  The "Corresponding Source" for a work in object code form means all
-the source code needed to generate, install, and (for an executable
-work) run the object code and to modify the work, including scripts to
-control those activities.  However, it does not include the work's
-System Libraries, or general-purpose tools or generally available free
-programs which are used unmodified in performing those activities but
-which are not part of the work.  For example, Corresponding Source
-includes interface definition files associated with source files for
-the work, and the source code for shared libraries and dynamically
-linked subprograms that the work is specifically designed to require,
-such as by intimate data communication or control flow between those
-subprograms and other parts of the work.
-
-  The Corresponding Source need not include anything that users
-can regenerate automatically from other parts of the Corresponding
-Source.
-
-  The Corresponding Source for a work in source code form is that
-same work.
-
-  2. Basic Permissions.
-
-  All rights granted under this License are granted for the term of
-copyright on the Program, and are irrevocable provided the stated
-conditions are met.  This License explicitly affirms your unlimited
-permission to run the unmodified Program.  The output from running a
-covered work is covered by this License only if the output, given its
-content, constitutes a covered work.  This License acknowledges your
-rights of fair use or other equivalent, as provided by copyright law.
-
-  You may make, run and propagate covered works that you do not
-convey, without conditions so long as your license otherwise remains
-in force.  You may convey covered works to others for the sole purpose
-of having them make modifications exclusively for you, or provide you
-with facilities for running those works, provided that you comply with
-the terms of this License in conveying all material for which you do
-not control copyright.  Those thus making or running the covered works
-for you must do so exclusively on your behalf, under your direction
-and control, on terms that prohibit them from making any copies of
-your copyrighted material outside their relationship with you.
-
-  Conveying under any other circumstances is permitted solely under
-the conditions stated below.  Sublicensing is not allowed; section 10
-makes it unnecessary.
-
-  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
-
-  No covered work shall be deemed part of an effective technological
-measure under any applicable law fulfilling obligations under article
-11 of the WIPO copyright treaty adopted on 20 December 1996, or
-similar laws prohibiting or restricting circumvention of such
-measures.
-
-  When you convey a covered work, you waive any legal power to forbid
-circumvention of technological measures to the extent such circumvention
-is effected by exercising rights under this License with respect to
-the covered work, and you disclaim any intention to limit operation or
-modification of the work as a means of enforcing, against the work's
-users, your or third parties' legal rights to forbid circumvention of
-technological measures.
-
-  4. Conveying Verbatim Copies.
-
-  You may convey verbatim copies of the Program's source code as you
-receive it, in any medium, provided that you conspicuously and
-appropriately publish on each copy an appropriate copyright notice;
-keep intact all notices stating that this License and any
-non-permissive terms added in accord with section 7 apply to the code;
-keep intact all notices of the absence of any warranty; and give all
-recipients a copy of this License along with the Program.
-
-  You may charge any price or no price for each copy that you convey,
-and you may offer support or warranty protection for a fee.
-
-  5. Conveying Modified Source Versions.
-
-  You may convey a work based on the Program, or the modifications to
-produce it from the Program, in the form of source code under the
-terms of section 4, provided that you also meet all of these conditions:
-
-    a) The work must carry prominent notices stating that you modified
-    it, and giving a relevant date.
-
-    b) The work must carry prominent notices stating that it is
-    released under this License and any conditions added under section
-    7.  This requirement modifies the requirement in section 4 to
-    "keep intact all notices".
-
-    c) You must license the entire work, as a whole, under this
-    License to anyone who comes into possession of a copy.  This
-    License will therefore apply, along with any applicable section 7
-    additional terms, to the whole of the work, and all its parts,
-    regardless of how they are packaged.  This License gives no
-    permission to license the work in any other way, but it does not
-    invalidate such permission if you have separately received it.
-
-    d) If the work has interactive user interfaces, each must display
-    Appropriate Legal Notices; however, if the Program has interactive
-    interfaces that do not display Appropriate Legal Notices, your
-    work need not make them do so.
-
-  A compilation of a covered work with other separate and independent
-works, which are not by their nature extensions of the covered work,
-and which are not combined with it such as to form a larger program,
-in or on a volume of a storage or distribution medium, is called an
-"aggregate" if the compilation and its resulting copyright are not
-used to limit the access or legal rights of the compilation's users
-beyond what the individual works permit.  Inclusion of a covered work
-in an aggregate does not cause this License to apply to the other
-parts of the aggregate.
-
-  6. Conveying Non-Source Forms.
-
-  You may convey a covered work in object code form under the terms
-of sections 4 and 5, provided that you also convey the
-machine-readable Corresponding Source under the terms of this License,
-in one of these ways:
-
-    a) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by the
-    Corresponding Source fixed on a durable physical medium
-    customarily used for software interchange.
-
-    b) Convey the object code in, or embodied in, a physical product
-    (including a physical distribution medium), accompanied by a
-    written offer, valid for at least three years and valid for as
-    long as you offer spare parts or customer support for that product
-    model, to give anyone who possesses the object code either (1) a
-    copy of the Corresponding Source for all the software in the
-    product that is covered by this License, on a durable physical
-    medium customarily used for software interchange, for a price no
-    more than your reasonable cost of physically performing this
-    conveying of source, or (2) access to copy the
-    Corresponding Source from a network server at no charge.
-
-    c) Convey individual copies of the object code with a copy of the
-    written offer to provide the Corresponding Source.  This
-    alternative is allowed only occasionally and noncommercially, and
-    only if you received the object code with such an offer, in accord
-    with subsection 6b.
-
-    d) Convey the object code by offering access from a designated
-    place (gratis or for a charge), and offer equivalent access to the
-    Corresponding Source in the same way through the same place at no
-    further charge.  You need not require recipients to copy the
-    Corresponding Source along with the object code.  If the place to
-    copy the object code is a network server, the Corresponding Source
-    may be on a different server (operated by you or a third party)
-    that supports equivalent copying facilities, provided you maintain
-    clear directions next to the object code saying where to find the
-    Corresponding Source.  Regardless of what server hosts the
-    Corresponding Source, you remain obligated to ensure that it is
-    available for as long as needed to satisfy these requirements.
-
-    e) Convey the object code using peer-to-peer transmission, provided
-    you inform other peers where the object code and Corresponding
-    Source of the work are being offered to the general public at no
-    charge under subsection 6d.
-
-  A separable portion of the object code, whose source code is excluded
-from the Corresponding Source as a System Library, need not be
-included in conveying the object code work.
-
-  A "User Product" is either (1) a "consumer product", which means any
-tangible personal property which is normally used for personal, family,
-or household purposes, or (2) anything designed or sold for incorporation
-into a dwelling.  In determining whether a product is a consumer product,
-doubtful cases shall be resolved in favor of coverage.  For a particular
-product received by a particular user, "normally used" refers to a
-typical or common use of that class of product, regardless of the status
-of the particular user or of the way in which the particular user
-actually uses, or expects or is expected to use, the product.  A product
-is a consumer product regardless of whether the product has substantial
-commercial, industrial or non-consumer uses, unless such uses represent
-the only significant mode of use of the product.
-
-  "Installation Information" for a User Product means any methods,
-procedures, authorization keys, or other information required to install
-and execute modified versions of a covered work in that User Product from
-a modified version of its Corresponding Source.  The information must
-suffice to ensure that the continued functioning of the modified object
-code is in no case prevented or interfered with solely because
-modification has been made.
-
-  If you convey an object code work under this section in, or with, or
-specifically for use in, a User Product, and the conveying occurs as
-part of a transaction in which the right of possession and use of the
-User Product is transferred to the recipient in perpetuity or for a
-fixed term (regardless of how the transaction is characterized), the
-Corresponding Source conveyed under this section must be accompanied
-by the Installation Information.  But this requirement does not apply
-if neither you nor any third party retains the ability to install
-modified object code on the User Product (for example, the work has
-been installed in ROM).
-
-  The requirement to provide Installation Information does not include a
-requirement to continue to provide support service, warranty, or updates
-for a work that has been modified or installed by the recipient, or for
-the User Product in which it has been modified or installed.  Access to a
-network may be denied when the modification itself materially and
-adversely affects the operation of the network or violates the rules and
-protocols for communication across the network.
-
-  Corresponding Source conveyed, and Installation Information provided,
-in accord with this section must be in a format that is publicly
-documented (and with an implementation available to the public in
-source code form), and must require no special password or key for
-unpacking, reading or copying.
-
-  7. Additional Terms.
-
-  "Additional permissions" are terms that supplement the terms of this
-License by making exceptions from one or more of its conditions.
-Additional permissions that are applicable to the entire Program shall
-be treated as though they were included in this License, to the extent
-that they are valid under applicable law.  If additional permissions
-apply only to part of the Program, that part may be used separately
-under those permissions, but the entire Program remains governed by
-this License without regard to the additional permissions.
-
-  When you convey a copy of a covered work, you may at your option
-remove any additional permissions from that copy, or from any part of
-it.  (Additional permissions may be written to require their own
-removal in certain cases when you modify the work.)  You may place
-additional permissions on material, added by you to a covered work,
-for which you have or can give appropriate copyright permission.
-
-  Notwithstanding any other provision of this License, for material you
-add to a covered work, you may (if authorized by the copyright holders of
-that material) supplement the terms of this License with terms:
-
-    a) Disclaiming warranty or limiting liability differently from the
-    terms of sections 15 and 16 of this License; or
-
-    b) Requiring preservation of specified reasonable legal notices or
-    author attributions in that material or in the Appropriate Legal
-    Notices displayed by works containing it; or
-
-    c) Prohibiting misrepresentation of the origin of that material, or
-    requiring that modified versions of such material be marked in
-    reasonable ways as different from the original version; or
-
-    d) Limiting the use for publicity purposes of names of licensors or
-    authors of the material; or
-
-    e) Declining to grant rights under trademark law for use of some
-    trade names, trademarks, or service marks; or
-
-    f) Requiring indemnification of licensors and authors of that
-    material by anyone who conveys the material (or modified versions of
-    it) with contractual assumptions of liability to the recipient, for
-    any liability that these contractual assumptions directly impose on
-    those licensors and authors.
-
-  All other non-permissive additional terms are considered "further
-restrictions" within the meaning of section 10.  If the Program as you
-received it, or any part of it, contains a notice stating that it is
-governed by this License along with a term that is a further
-restriction, you may remove that term.  If a license document contains
-a further restriction but permits relicensing or conveying under this
-License, you may add to a covered work material governed by the terms
-of that license document, provided that the further restriction does
-not survive such relicensing or conveying.
-
-  If you add terms to a covered work in accord with this section, you
-must place, in the relevant source files, a statement of the
-additional terms that apply to those files, or a notice indicating
-where to find the applicable terms.
-
-  Additional terms, permissive or non-permissive, may be stated in the
-form of a separately written license, or stated as exceptions;
-the above requirements apply either way.
-
-  8. Termination.
-
-  You may not propagate or modify a covered work except as expressly
-provided under this License.  Any attempt otherwise to propagate or
-modify it is void, and will automatically terminate your rights under
-this License (including any patent licenses granted under the third
-paragraph of section 11).
-
-  However, if you cease all violation of this License, then your
-license from a particular copyright holder is reinstated (a)
-provisionally, unless and until the copyright holder explicitly and
-finally terminates your license, and (b) permanently, if the copyright
-holder fails to notify you of the violation by some reasonable means
-prior to 60 days after the cessation.
-
-  Moreover, your license from a particular copyright holder is
-reinstated permanently if the copyright holder notifies you of the
-violation by some reasonable means, this is the first time you have
-received notice of violation of this License (for any work) from that
-copyright holder, and you cure the violation prior to 30 days after
-your receipt of the notice.
-
-  Termination of your rights under this section does not terminate the
-licenses of parties who have received copies or rights from you under
-this License.  If your rights have been terminated and not permanently
-reinstated, you do not qualify to receive new licenses for the same
-material under section 10.
-
-  9. Acceptance Not Required for Having Copies.
-
-  You are not required to accept this License in order to receive or
-run a copy of the Program.  Ancillary propagation of a covered work
-occurring solely as a consequence of using peer-to-peer transmission
-to receive a copy likewise does not require acceptance.  However,
-nothing other than this License grants you permission to propagate or
-modify any covered work.  These actions infringe copyright if you do
-not accept this License.  Therefore, by modifying or propagating a
-covered work, you indicate your acceptance of this License to do so.
-
-  10. Automatic Licensing of Downstream Recipients.
-
-  Each time you convey a covered work, the recipient automatically
-receives a license from the original licensors, to run, modify and
-propagate that work, subject to this License.  You are not responsible
-for enforcing compliance by third parties with this License.
-
-  An "entity transaction" is a transaction transferring control of an
-organization, or substantially all assets of one, or subdividing an
-organization, or merging organizations.  If propagation of a covered
-work results from an entity transaction, each party to that
-transaction who receives a copy of the work also receives whatever
-licenses to the work the party's predecessor in interest had or could
-give under the previous paragraph, plus a right to possession of the
-Corresponding Source of the work from the predecessor in interest, if
-the predecessor has it or can get it with reasonable efforts.
-
-  You may not impose any further restrictions on the exercise of the
-rights granted or affirmed under this License.  For example, you may
-not impose a license fee, royalty, or other charge for exercise of
-rights granted under this License, and you may not initiate litigation
-(including a cross-claim or counterclaim in a lawsuit) alleging that
-any patent claim is infringed by making, using, selling, offering for
-sale, or importing the Program or any portion of it.
-
-  11. Patents.
-
-  A "contributor" is a copyright holder who authorizes use under this
-License of the Program or a work on which the Program is based.  The
-work thus licensed is called the contributor's "contributor version".
-
-  A contributor's "essential patent claims" are all patent claims
-owned or controlled by the contributor, whether already acquired or
-hereafter acquired, that would be infringed by some manner, permitted
-by this License, of making, using, or selling its contributor version,
-but do not include claims that would be infringed only as a
-consequence of further modification of the contributor version.  For
-purposes of this definition, "control" includes the right to grant
-patent sublicenses in a manner consistent with the requirements of
-this License.
-
-  Each contributor grants you a non-exclusive, worldwide, royalty-free
-patent license under the contributor's essential patent claims, to
-make, use, sell, offer for sale, import and otherwise run, modify and
-propagate the contents of its contributor version.
-
-  In the following three paragraphs, a "patent license" is any express
-agreement or commitment, however denominated, not to enforce a patent
-(such as an express permission to practice a patent or covenant not to
-sue for patent infringement).  To "grant" such a patent license to a
-party means to make such an agreement or commitment not to enforce a
-patent against the party.
-
-  If you convey a covered work, knowingly relying on a patent license,
-and the Corresponding Source of the work is not available for anyone
-to copy, free of charge and under the terms of this License, through a
-publicly available network server or other readily accessible means,
-then you must either (1) cause the Corresponding Source to be so
-available, or (2) arrange to deprive yourself of the benefit of the
-patent license for this particular work, or (3) arrange, in a manner
-consistent with the requirements of this License, to extend the patent
-license to downstream recipients.  "Knowingly relying" means you have
-actual knowledge that, but for the patent license, your conveying the
-covered work in a country, or your recipient's use of the covered work
-in a country, would infringe one or more identifiable patents in that
-country that you have reason to believe are valid.
-
-  If, pursuant to or in connection with a single transaction or
-arrangement, you convey, or propagate by procuring conveyance of, a
-covered work, and grant a patent license to some of the parties
-receiving the covered work authorizing them to use, propagate, modify
-or convey a specific copy of the covered work, then the patent license
-you grant is automatically extended to all recipients of the covered
-work and works based on it.
-
-  A patent license is "discriminatory" if it does not include within
-the scope of its coverage, prohibits the exercise of, or is
-conditioned on the non-exercise of one or more of the rights that are
-specifically granted under this License.  You may not convey a covered
-work if you are a party to an arrangement with a third party that is
-in the business of distributing software, under which you make payment
-to the third party based on the extent of your activity of conveying
-the work, and under which the third party grants, to any of the
-parties who would receive the covered work from you, a discriminatory
-patent license (a) in connection with copies of the covered work
-conveyed by you (or copies made from those copies), or (b) primarily
-for and in connection with specific products or compilations that
-contain the covered work, unless you entered into that arrangement,
-or that patent license was granted, prior to 28 March 2007.
-
-  Nothing in this License shall be construed as excluding or limiting
-any implied license or other defenses to infringement that may
-otherwise be available to you under applicable patent law.
-
-  12. No Surrender of Others' Freedom.
-
-  If conditions are imposed on you (whether by court order, agreement or
-otherwise) that contradict the conditions of this License, they do not
-excuse you from the conditions of this License.  If you cannot convey a
-covered work so as to satisfy simultaneously your obligations under this
-License and any other pertinent obligations, then as a consequence you may
-not convey it at all.  For example, if you agree to terms that obligate you
-to collect a royalty for further conveying from those to whom you convey
-the Program, the only way you could satisfy both those terms and this
-License would be to refrain entirely from conveying the Program.
-
-  13. Use with the GNU Affero General Public License.
-
-  Notwithstanding any other provision of this License, you have
-permission to link or combine any covered work with a work licensed
-under version 3 of the GNU Affero General Public License into a single
-combined work, and to convey the resulting work.  The terms of this
-License will continue to apply to the part which is the covered work,
-but the special requirements of the GNU Affero General Public License,
-section 13, concerning interaction through a network will apply to the
-combination as such.
-
-  14. Revised Versions of this License.
-
-  The Free Software Foundation may publish revised and/or new versions of
-the GNU General Public License from time to time.  Such new versions will
-be similar in spirit to the present version, but may differ in detail to
-address new problems or concerns.
-
-  Each version is given a distinguishing version number.  If the
-Program specifies that a certain numbered version of the GNU General
-Public License "or any later version" applies to it, you have the
-option of following the terms and conditions either of that numbered
-version or of any later version published by the Free Software
-Foundation.  If the Program does not specify a version number of the
-GNU General Public License, you may choose any version ever published
-by the Free Software Foundation.
-
-  If the Program specifies that a proxy can decide which future
-versions of the GNU General Public License can be used, that proxy's
-public statement of acceptance of a version permanently authorizes you
-to choose that version for the Program.
-
-  Later license versions may give you additional or different
-permissions.  However, no additional obligations are imposed on any
-author or copyright holder as a result of your choosing to follow a
-later version.
-
-  15. Disclaimer of Warranty.
-
-  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
-APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
-HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
-OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
-THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
-PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
-IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
-ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
-
-  16. Limitation of Liability.
-
-  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
-WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
-THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
-GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
-USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
-DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
-PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
-EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
-SUCH DAMAGES.
-
-  17. Interpretation of Sections 15 and 16.
-
-  If the disclaimer of warranty and limitation of liability provided
-above cannot be given local legal effect according to their terms,
-reviewing courts shall apply local law that most closely approximates
-an absolute waiver of all civil liability in connection with the
-Program, unless a warranty or assumption of liability accompanies a
-copy of the Program in return for a fee.
-
-                     END OF TERMS AND CONDITIONS
-
-            How to Apply These Terms to Your New Programs
-
-  If you develop a new program, and you want it to be of the greatest
-possible use to the public, the best way to achieve this is to make it
-free software which everyone can redistribute and change under these terms.
-
-  To do so, attach the following notices to the program.  It is safest
-to attach them to the start of each source file to most effectively
-state the exclusion of warranty; and each file should have at least
-the "copyright" line and a pointer to where the full notice is found.
-
-    <one line to give the program's name and a brief idea of what it does.>
-    Copyright (C) <year>  <name of author>
-
-    This program is free software: you can redistribute it and/or modify
-    it under the terms of the GNU General Public License as published by
-    the Free Software Foundation, either version 3 of the License, or
-    (at your option) any later version.
-
-    This program is distributed in the hope that it will be useful,
-    but WITHOUT ANY WARRANTY; without even the implied warranty of
-    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
-    GNU General Public License for more details.
-
-    You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
-Also add information on how to contact you by electronic and paper mail.
-
-  If the program does terminal interaction, make it output a short
-notice like this when it starts in an interactive mode:
-
-    <program>  Copyright (C) <year>  <name of author>
-    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
-    This is free software, and you are welcome to redistribute it
-    under certain conditions; type `show c' for details.
-
-The hypothetical commands `show w' and `show c' should show the appropriate
-parts of the General Public License.  Of course, your program's commands
-might be different; for a GUI interface, you would use an "about box".
-
-  You should also get your employer (if you work as a programmer) or school,
-if any, to sign a "copyright disclaimer" for the program, if necessary.
-For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
-
-  The GNU General Public License does not permit incorporating your program
-into proprietary programs.  If your program is a subroutine library, you
-may consider it more useful to permit linking proprietary applications with
-the library.  If this is what you want to do, use the GNU Lesser General
-Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+                    GNU GENERAL PUBLIC LICENSE
+                       Version 3, 29 June 2007
+
+ Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Everyone is permitted to copy and distribute verbatim copies
+ of this license document, but changing it is not allowed.
+
+                            Preamble
+
+  The GNU General Public License is a free, copyleft license for
+software and other kinds of works.
+
+  The licenses for most software and other practical works are designed
+to take away your freedom to share and change the works.  By contrast,
+the GNU General Public License is intended to guarantee your freedom to
+share and change all versions of a program--to make sure it remains free
+software for all its users.  We, the Free Software Foundation, use the
+GNU General Public License for most of our software; it applies also to
+any other work released this way by its authors.  You can apply it to
+your programs, too.
+
+  When we speak of free software, we are referring to freedom, not
+price.  Our General Public Licenses are designed to make sure that you
+have the freedom to distribute copies of free software (and charge for
+them if you wish), that you receive source code or can get it if you
+want it, that you can change the software or use pieces of it in new
+free programs, and that you know you can do these things.
+
+  To protect your rights, we need to prevent others from denying you
+these rights or asking you to surrender the rights.  Therefore, you have
+certain responsibilities if you distribute copies of the software, or if
+you modify it: responsibilities to respect the freedom of others.
+
+  For example, if you distribute copies of such a program, whether
+gratis or for a fee, you must pass on to the recipients the same
+freedoms that you received.  You must make sure that they, too, receive
+or can get the source code.  And you must show them these terms so they
+know their rights.
+
+  Developers that use the GNU GPL protect your rights with two steps:
+(1) assert copyright on the software, and (2) offer you this License
+giving you legal permission to copy, distribute and/or modify it.
+
+  For the developers' and authors' protection, the GPL clearly explains
+that there is no warranty for this free software.  For both users' and
+authors' sake, the GPL requires that modified versions be marked as
+changed, so that their problems will not be attributed erroneously to
+authors of previous versions.
+
+  Some devices are designed to deny users access to install or run
+modified versions of the software inside them, although the manufacturer
+can do so.  This is fundamentally incompatible with the aim of
+protecting users' freedom to change the software.  The systematic
+pattern of such abuse occurs in the area of products for individuals to
+use, which is precisely where it is most unacceptable.  Therefore, we
+have designed this version of the GPL to prohibit the practice for those
+products.  If such problems arise substantially in other domains, we
+stand ready to extend this provision to those domains in future versions
+of the GPL, as needed to protect the freedom of users.
+
+  Finally, every program is threatened constantly by software patents.
+States should not allow patents to restrict development and use of
+software on general-purpose computers, but in those that do, we wish to
+avoid the special danger that patents applied to a free program could
+make it effectively proprietary.  To prevent this, the GPL assures that
+patents cannot be used to render the program non-free.
+
+  The precise terms and conditions for copying, distribution and
+modification follow.
+
+                       TERMS AND CONDITIONS
+
+  0. Definitions.
+
+  "This License" refers to version 3 of the GNU General Public License.
+
+  "Copyright" also means copyright-like laws that apply to other kinds of
+works, such as semiconductor masks.
+
+  "The Program" refers to any copyrightable work licensed under this
+License.  Each licensee is addressed as "you".  "Licensees" and
+"recipients" may be individuals or organizations.
+
+  To "modify" a work means to copy from or adapt all or part of the work
+in a fashion requiring copyright permission, other than the making of an
+exact copy.  The resulting work is called a "modified version" of the
+earlier work or a work "based on" the earlier work.
+
+  A "covered work" means either the unmodified Program or a work based
+on the Program.
+
+  To "propagate" a work means to do anything with it that, without
+permission, would make you directly or secondarily liable for
+infringement under applicable copyright law, except executing it on a
+computer or modifying a private copy.  Propagation includes copying,
+distribution (with or without modification), making available to the
+public, and in some countries other activities as well.
+
+  To "convey" a work means any kind of propagation that enables other
+parties to make or receive copies.  Mere interaction with a user through
+a computer network, with no transfer of a copy, is not conveying.
+
+  An interactive user interface displays "Appropriate Legal Notices"
+to the extent that it includes a convenient and prominently visible
+feature that (1) displays an appropriate copyright notice, and (2)
+tells the user that there is no warranty for the work (except to the
+extent that warranties are provided), that licensees may convey the
+work under this License, and how to view a copy of this License.  If
+the interface presents a list of user commands or options, such as a
+menu, a prominent item in the list meets this criterion.
+
+  1. Source Code.
+
+  The "source code" for a work means the preferred form of the work
+for making modifications to it.  "Object code" means any non-source
+form of a work.
+
+  A "Standard Interface" means an interface that either is an official
+standard defined by a recognized standards body, or, in the case of
+interfaces specified for a particular programming language, one that
+is widely used among developers working in that language.
+
+  The "System Libraries" of an executable work include anything, other
+than the work as a whole, that (a) is included in the normal form of
+packaging a Major Component, but which is not part of that Major
+Component, and (b) serves only to enable use of the work with that
+Major Component, or to implement a Standard Interface for which an
+implementation is available to the public in source code form.  A
+"Major Component", in this context, means a major essential component
+(kernel, window system, and so on) of the specific operating system
+(if any) on which the executable work runs, or a compiler used to
+produce the work, or an object code interpreter used to run it.
+
+  The "Corresponding Source" for a work in object code form means all
+the source code needed to generate, install, and (for an executable
+work) run the object code and to modify the work, including scripts to
+control those activities.  However, it does not include the work's
+System Libraries, or general-purpose tools or generally available free
+programs which are used unmodified in performing those activities but
+which are not part of the work.  For example, Corresponding Source
+includes interface definition files associated with source files for
+the work, and the source code for shared libraries and dynamically
+linked subprograms that the work is specifically designed to require,
+such as by intimate data communication or control flow between those
+subprograms and other parts of the work.
+
+  The Corresponding Source need not include anything that users
+can regenerate automatically from other parts of the Corresponding
+Source.
+
+  The Corresponding Source for a work in source code form is that
+same work.
+
+  2. Basic Permissions.
+
+  All rights granted under this License are granted for the term of
+copyright on the Program, and are irrevocable provided the stated
+conditions are met.  This License explicitly affirms your unlimited
+permission to run the unmodified Program.  The output from running a
+covered work is covered by this License only if the output, given its
+content, constitutes a covered work.  This License acknowledges your
+rights of fair use or other equivalent, as provided by copyright law.
+
+  You may make, run and propagate covered works that you do not
+convey, without conditions so long as your license otherwise remains
+in force.  You may convey covered works to others for the sole purpose
+of having them make modifications exclusively for you, or provide you
+with facilities for running those works, provided that you comply with
+the terms of this License in conveying all material for which you do
+not control copyright.  Those thus making or running the covered works
+for you must do so exclusively on your behalf, under your direction
+and control, on terms that prohibit them from making any copies of
+your copyrighted material outside their relationship with you.
+
+  Conveying under any other circumstances is permitted solely under
+the conditions stated below.  Sublicensing is not allowed; section 10
+makes it unnecessary.
+
+  3. Protecting Users' Legal Rights From Anti-Circumvention Law.
+
+  No covered work shall be deemed part of an effective technological
+measure under any applicable law fulfilling obligations under article
+11 of the WIPO copyright treaty adopted on 20 December 1996, or
+similar laws prohibiting or restricting circumvention of such
+measures.
+
+  When you convey a covered work, you waive any legal power to forbid
+circumvention of technological measures to the extent such circumvention
+is effected by exercising rights under this License with respect to
+the covered work, and you disclaim any intention to limit operation or
+modification of the work as a means of enforcing, against the work's
+users, your or third parties' legal rights to forbid circumvention of
+technological measures.
+
+  4. Conveying Verbatim Copies.
+
+  You may convey verbatim copies of the Program's source code as you
+receive it, in any medium, provided that you conspicuously and
+appropriately publish on each copy an appropriate copyright notice;
+keep intact all notices stating that this License and any
+non-permissive terms added in accord with section 7 apply to the code;
+keep intact all notices of the absence of any warranty; and give all
+recipients a copy of this License along with the Program.
+
+  You may charge any price or no price for each copy that you convey,
+and you may offer support or warranty protection for a fee.
+
+  5. Conveying Modified Source Versions.
+
+  You may convey a work based on the Program, or the modifications to
+produce it from the Program, in the form of source code under the
+terms of section 4, provided that you also meet all of these conditions:
+
+    a) The work must carry prominent notices stating that you modified
+    it, and giving a relevant date.
+
+    b) The work must carry prominent notices stating that it is
+    released under this License and any conditions added under section
+    7.  This requirement modifies the requirement in section 4 to
+    "keep intact all notices".
+
+    c) You must license the entire work, as a whole, under this
+    License to anyone who comes into possession of a copy.  This
+    License will therefore apply, along with any applicable section 7
+    additional terms, to the whole of the work, and all its parts,
+    regardless of how they are packaged.  This License gives no
+    permission to license the work in any other way, but it does not
+    invalidate such permission if you have separately received it.
+
+    d) If the work has interactive user interfaces, each must display
+    Appropriate Legal Notices; however, if the Program has interactive
+    interfaces that do not display Appropriate Legal Notices, your
+    work need not make them do so.
+
+  A compilation of a covered work with other separate and independent
+works, which are not by their nature extensions of the covered work,
+and which are not combined with it such as to form a larger program,
+in or on a volume of a storage or distribution medium, is called an
+"aggregate" if the compilation and its resulting copyright are not
+used to limit the access or legal rights of the compilation's users
+beyond what the individual works permit.  Inclusion of a covered work
+in an aggregate does not cause this License to apply to the other
+parts of the aggregate.
+
+  6. Conveying Non-Source Forms.
+
+  You may convey a covered work in object code form under the terms
+of sections 4 and 5, provided that you also convey the
+machine-readable Corresponding Source under the terms of this License,
+in one of these ways:
+
+    a) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by the
+    Corresponding Source fixed on a durable physical medium
+    customarily used for software interchange.
+
+    b) Convey the object code in, or embodied in, a physical product
+    (including a physical distribution medium), accompanied by a
+    written offer, valid for at least three years and valid for as
+    long as you offer spare parts or customer support for that product
+    model, to give anyone who possesses the object code either (1) a
+    copy of the Corresponding Source for all the software in the
+    product that is covered by this License, on a durable physical
+    medium customarily used for software interchange, for a price no
+    more than your reasonable cost of physically performing this
+    conveying of source, or (2) access to copy the
+    Corresponding Source from a network server at no charge.
+
+    c) Convey individual copies of the object code with a copy of the
+    written offer to provide the Corresponding Source.  This
+    alternative is allowed only occasionally and noncommercially, and
+    only if you received the object code with such an offer, in accord
+    with subsection 6b.
+
+    d) Convey the object code by offering access from a designated
+    place (gratis or for a charge), and offer equivalent access to the
+    Corresponding Source in the same way through the same place at no
+    further charge.  You need not require recipients to copy the
+    Corresponding Source along with the object code.  If the place to
+    copy the object code is a network server, the Corresponding Source
+    may be on a different server (operated by you or a third party)
+    that supports equivalent copying facilities, provided you maintain
+    clear directions next to the object code saying where to find the
+    Corresponding Source.  Regardless of what server hosts the
+    Corresponding Source, you remain obligated to ensure that it is
+    available for as long as needed to satisfy these requirements.
+
+    e) Convey the object code using peer-to-peer transmission, provided
+    you inform other peers where the object code and Corresponding
+    Source of the work are being offered to the general public at no
+    charge under subsection 6d.
+
+  A separable portion of the object code, whose source code is excluded
+from the Corresponding Source as a System Library, need not be
+included in conveying the object code work.
+
+  A "User Product" is either (1) a "consumer product", which means any
+tangible personal property which is normally used for personal, family,
+or household purposes, or (2) anything designed or sold for incorporation
+into a dwelling.  In determining whether a product is a consumer product,
+doubtful cases shall be resolved in favor of coverage.  For a particular
+product received by a particular user, "normally used" refers to a
+typical or common use of that class of product, regardless of the status
+of the particular user or of the way in which the particular user
+actually uses, or expects or is expected to use, the product.  A product
+is a consumer product regardless of whether the product has substantial
+commercial, industrial or non-consumer uses, unless such uses represent
+the only significant mode of use of the product.
+
+  "Installation Information" for a User Product means any methods,
+procedures, authorization keys, or other information required to install
+and execute modified versions of a covered work in that User Product from
+a modified version of its Corresponding Source.  The information must
+suffice to ensure that the continued functioning of the modified object
+code is in no case prevented or interfered with solely because
+modification has been made.
+
+  If you convey an object code work under this section in, or with, or
+specifically for use in, a User Product, and the conveying occurs as
+part of a transaction in which the right of possession and use of the
+User Product is transferred to the recipient in perpetuity or for a
+fixed term (regardless of how the transaction is characterized), the
+Corresponding Source conveyed under this section must be accompanied
+by the Installation Information.  But this requirement does not apply
+if neither you nor any third party retains the ability to install
+modified object code on the User Product (for example, the work has
+been installed in ROM).
+
+  The requirement to provide Installation Information does not include a
+requirement to continue to provide support service, warranty, or updates
+for a work that has been modified or installed by the recipient, or for
+the User Product in which it has been modified or installed.  Access to a
+network may be denied when the modification itself materially and
+adversely affects the operation of the network or violates the rules and
+protocols for communication across the network.
+
+  Corresponding Source conveyed, and Installation Information provided,
+in accord with this section must be in a format that is publicly
+documented (and with an implementation available to the public in
+source code form), and must require no special password or key for
+unpacking, reading or copying.
+
+  7. Additional Terms.
+
+  "Additional permissions" are terms that supplement the terms of this
+License by making exceptions from one or more of its conditions.
+Additional permissions that are applicable to the entire Program shall
+be treated as though they were included in this License, to the extent
+that they are valid under applicable law.  If additional permissions
+apply only to part of the Program, that part may be used separately
+under those permissions, but the entire Program remains governed by
+this License without regard to the additional permissions.
+
+  When you convey a copy of a covered work, you may at your option
+remove any additional permissions from that copy, or from any part of
+it.  (Additional permissions may be written to require their own
+removal in certain cases when you modify the work.)  You may place
+additional permissions on material, added by you to a covered work,
+for which you have or can give appropriate copyright permission.
+
+  Notwithstanding any other provision of this License, for material you
+add to a covered work, you may (if authorized by the copyright holders of
+that material) supplement the terms of this License with terms:
+
+    a) Disclaiming warranty or limiting liability differently from the
+    terms of sections 15 and 16 of this License; or
+
+    b) Requiring preservation of specified reasonable legal notices or
+    author attributions in that material or in the Appropriate Legal
+    Notices displayed by works containing it; or
+
+    c) Prohibiting misrepresentation of the origin of that material, or
+    requiring that modified versions of such material be marked in
+    reasonable ways as different from the original version; or
+
+    d) Limiting the use for publicity purposes of names of licensors or
+    authors of the material; or
+
+    e) Declining to grant rights under trademark law for use of some
+    trade names, trademarks, or service marks; or
+
+    f) Requiring indemnification of licensors and authors of that
+    material by anyone who conveys the material (or modified versions of
+    it) with contractual assumptions of liability to the recipient, for
+    any liability that these contractual assumptions directly impose on
+    those licensors and authors.
+
+  All other non-permissive additional terms are considered "further
+restrictions" within the meaning of section 10.  If the Program as you
+received it, or any part of it, contains a notice stating that it is
+governed by this License along with a term that is a further
+restriction, you may remove that term.  If a license document contains
+a further restriction but permits relicensing or conveying under this
+License, you may add to a covered work material governed by the terms
+of that license document, provided that the further restriction does
+not survive such relicensing or conveying.
+
+  If you add terms to a covered work in accord with this section, you
+must place, in the relevant source files, a statement of the
+additional terms that apply to those files, or a notice indicating
+where to find the applicable terms.
+
+  Additional terms, permissive or non-permissive, may be stated in the
+form of a separately written license, or stated as exceptions;
+the above requirements apply either way.
+
+  8. Termination.
+
+  You may not propagate or modify a covered work except as expressly
+provided under this License.  Any attempt otherwise to propagate or
+modify it is void, and will automatically terminate your rights under
+this License (including any patent licenses granted under the third
+paragraph of section 11).
+
+  However, if you cease all violation of this License, then your
+license from a particular copyright holder is reinstated (a)
+provisionally, unless and until the copyright holder explicitly and
+finally terminates your license, and (b) permanently, if the copyright
+holder fails to notify you of the violation by some reasonable means
+prior to 60 days after the cessation.
+
+  Moreover, your license from a particular copyright holder is
+reinstated permanently if the copyright holder notifies you of the
+violation by some reasonable means, this is the first time you have
+received notice of violation of this License (for any work) from that
+copyright holder, and you cure the violation prior to 30 days after
+your receipt of the notice.
+
+  Termination of your rights under this section does not terminate the
+licenses of parties who have received copies or rights from you under
+this License.  If your rights have been terminated and not permanently
+reinstated, you do not qualify to receive new licenses for the same
+material under section 10.
+
+  9. Acceptance Not Required for Having Copies.
+
+  You are not required to accept this License in order to receive or
+run a copy of the Program.  Ancillary propagation of a covered work
+occurring solely as a consequence of using peer-to-peer transmission
+to receive a copy likewise does not require acceptance.  However,
+nothing other than this License grants you permission to propagate or
+modify any covered work.  These actions infringe copyright if you do
+not accept this License.  Therefore, by modifying or propagating a
+covered work, you indicate your acceptance of this License to do so.
+
+  10. Automatic Licensing of Downstream Recipients.
+
+  Each time you convey a covered work, the recipient automatically
+receives a license from the original licensors, to run, modify and
+propagate that work, subject to this License.  You are not responsible
+for enforcing compliance by third parties with this License.
+
+  An "entity transaction" is a transaction transferring control of an
+organization, or substantially all assets of one, or subdividing an
+organization, or merging organizations.  If propagation of a covered
+work results from an entity transaction, each party to that
+transaction who receives a copy of the work also receives whatever
+licenses to the work the party's predecessor in interest had or could
+give under the previous paragraph, plus a right to possession of the
+Corresponding Source of the work from the predecessor in interest, if
+the predecessor has it or can get it with reasonable efforts.
+
+  You may not impose any further restrictions on the exercise of the
+rights granted or affirmed under this License.  For example, you may
+not impose a license fee, royalty, or other charge for exercise of
+rights granted under this License, and you may not initiate litigation
+(including a cross-claim or counterclaim in a lawsuit) alleging that
+any patent claim is infringed by making, using, selling, offering for
+sale, or importing the Program or any portion of it.
+
+  11. Patents.
+
+  A "contributor" is a copyright holder who authorizes use under this
+License of the Program or a work on which the Program is based.  The
+work thus licensed is called the contributor's "contributor version".
+
+  A contributor's "essential patent claims" are all patent claims
+owned or controlled by the contributor, whether already acquired or
+hereafter acquired, that would be infringed by some manner, permitted
+by this License, of making, using, or selling its contributor version,
+but do not include claims that would be infringed only as a
+consequence of further modification of the contributor version.  For
+purposes of this definition, "control" includes the right to grant
+patent sublicenses in a manner consistent with the requirements of
+this License.
+
+  Each contributor grants you a non-exclusive, worldwide, royalty-free
+patent license under the contributor's essential patent claims, to
+make, use, sell, offer for sale, import and otherwise run, modify and
+propagate the contents of its contributor version.
+
+  In the following three paragraphs, a "patent license" is any express
+agreement or commitment, however denominated, not to enforce a patent
+(such as an express permission to practice a patent or covenant not to
+sue for patent infringement).  To "grant" such a patent license to a
+party means to make such an agreement or commitment not to enforce a
+patent against the party.
+
+  If you convey a covered work, knowingly relying on a patent license,
+and the Corresponding Source of the work is not available for anyone
+to copy, free of charge and under the terms of this License, through a
+publicly available network server or other readily accessible means,
+then you must either (1) cause the Corresponding Source to be so
+available, or (2) arrange to deprive yourself of the benefit of the
+patent license for this particular work, or (3) arrange, in a manner
+consistent with the requirements of this License, to extend the patent
+license to downstream recipients.  "Knowingly relying" means you have
+actual knowledge that, but for the patent license, your conveying the
+covered work in a country, or your recipient's use of the covered work
+in a country, would infringe one or more identifiable patents in that
+country that you have reason to believe are valid.
+
+  If, pursuant to or in connection with a single transaction or
+arrangement, you convey, or propagate by procuring conveyance of, a
+covered work, and grant a patent license to some of the parties
+receiving the covered work authorizing them to use, propagate, modify
+or convey a specific copy of the covered work, then the patent license
+you grant is automatically extended to all recipients of the covered
+work and works based on it.
+
+  A patent license is "discriminatory" if it does not include within
+the scope of its coverage, prohibits the exercise of, or is
+conditioned on the non-exercise of one or more of the rights that are
+specifically granted under this License.  You may not convey a covered
+work if you are a party to an arrangement with a third party that is
+in the business of distributing software, under which you make payment
+to the third party based on the extent of your activity of conveying
+the work, and under which the third party grants, to any of the
+parties who would receive the covered work from you, a discriminatory
+patent license (a) in connection with copies of the covered work
+conveyed by you (or copies made from those copies), or (b) primarily
+for and in connection with specific products or compilations that
+contain the covered work, unless you entered into that arrangement,
+or that patent license was granted, prior to 28 March 2007.
+
+  Nothing in this License shall be construed as excluding or limiting
+any implied license or other defenses to infringement that may
+otherwise be available to you under applicable patent law.
+
+  12. No Surrender of Others' Freedom.
+
+  If conditions are imposed on you (whether by court order, agreement or
+otherwise) that contradict the conditions of this License, they do not
+excuse you from the conditions of this License.  If you cannot convey a
+covered work so as to satisfy simultaneously your obligations under this
+License and any other pertinent obligations, then as a consequence you may
+not convey it at all.  For example, if you agree to terms that obligate you
+to collect a royalty for further conveying from those to whom you convey
+the Program, the only way you could satisfy both those terms and this
+License would be to refrain entirely from conveying the Program.
+
+  13. Use with the GNU Affero General Public License.
+
+  Notwithstanding any other provision of this License, you have
+permission to link or combine any covered work with a work licensed
+under version 3 of the GNU Affero General Public License into a single
+combined work, and to convey the resulting work.  The terms of this
+License will continue to apply to the part which is the covered work,
+but the special requirements of the GNU Affero General Public License,
+section 13, concerning interaction through a network will apply to the
+combination as such.
+
+  14. Revised Versions of this License.
+
+  The Free Software Foundation may publish revised and/or new versions of
+the GNU General Public License from time to time.  Such new versions will
+be similar in spirit to the present version, but may differ in detail to
+address new problems or concerns.
+
+  Each version is given a distinguishing version number.  If the
+Program specifies that a certain numbered version of the GNU General
+Public License "or any later version" applies to it, you have the
+option of following the terms and conditions either of that numbered
+version or of any later version published by the Free Software
+Foundation.  If the Program does not specify a version number of the
+GNU General Public License, you may choose any version ever published
+by the Free Software Foundation.
+
+  If the Program specifies that a proxy can decide which future
+versions of the GNU General Public License can be used, that proxy's
+public statement of acceptance of a version permanently authorizes you
+to choose that version for the Program.
+
+  Later license versions may give you additional or different
+permissions.  However, no additional obligations are imposed on any
+author or copyright holder as a result of your choosing to follow a
+later version.
+
+  15. Disclaimer of Warranty.
+
+  THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY
+APPLICABLE LAW.  EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT
+HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY
+OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO,
+THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE.  THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM
+IS WITH YOU.  SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF
+ALL NECESSARY SERVICING, REPAIR OR CORRECTION.
+
+  16. Limitation of Liability.
+
+  IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING
+WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS
+THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY
+GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE
+USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF
+DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD
+PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS),
+EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF
+SUCH DAMAGES.
+
+  17. Interpretation of Sections 15 and 16.
+
+  If the disclaimer of warranty and limitation of liability provided
+above cannot be given local legal effect according to their terms,
+reviewing courts shall apply local law that most closely approximates
+an absolute waiver of all civil liability in connection with the
+Program, unless a warranty or assumption of liability accompanies a
+copy of the Program in return for a fee.
+
+                     END OF TERMS AND CONDITIONS
+
+            How to Apply These Terms to Your New Programs
+
+  If you develop a new program, and you want it to be of the greatest
+possible use to the public, the best way to achieve this is to make it
+free software which everyone can redistribute and change under these terms.
+
+  To do so, attach the following notices to the program.  It is safest
+to attach them to the start of each source file to most effectively
+state the exclusion of warranty; and each file should have at least
+the "copyright" line and a pointer to where the full notice is found.
+
+    <one line to give the program's name and a brief idea of what it does.>
+    Copyright (C) <year>  <name of author>
+
+    This program is free software: you can redistribute it and/or modify
+    it under the terms of the GNU General Public License as published by
+    the Free Software Foundation, either version 3 of the License, or
+    (at your option) any later version.
+
+    This program is distributed in the hope that it will be useful,
+    but WITHOUT ANY WARRANTY; without even the implied warranty of
+    MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
+    GNU General Public License for more details.
+
+    You should have received a copy of the GNU General Public License
+    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+
+Also add information on how to contact you by electronic and paper mail.
+
+  If the program does terminal interaction, make it output a short
+notice like this when it starts in an interactive mode:
+
+    <program>  Copyright (C) <year>  <name of author>
+    This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
+    This is free software, and you are welcome to redistribute it
+    under certain conditions; type `show c' for details.
+
+The hypothetical commands `show w' and `show c' should show the appropriate
+parts of the General Public License.  Of course, your program's commands
+might be different; for a GUI interface, you would use an "about box".
+
+  You should also get your employer (if you work as a programmer) or school,
+if any, to sign a "copyright disclaimer" for the program, if necessary.
+For more information on this, and how to apply and follow the GNU GPL, see
+<http://www.gnu.org/licenses/>.
+
+  The GNU General Public License does not permit incorporating your program
+into proprietary programs.  If your program is a subroutine library, you
+may consider it more useful to permit linking proprietary applications with
+the library.  If this is what you want to do, use the GNU Lesser General
+Public License instead of this License.  But first, please read
+<http://www.gnu.org/philosophy/why-not-lgpl.html>.
```

### Comparing `osm2gmns-0.7.5/PKG-INFO` & `osm2gmns-0.7.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,165 +1,154 @@
-Metadata-Version: 2.1
-Name: osm2gmns
-Version: 0.7.5
-Summary: convert map data from OpenStreetMap to network files in GMNS format
-Home-page: https://github.com/jiawlu/OSM2GMNS
-Author: Jiawei Lu, Xuesong Zhou
-Author-email: jiaweil9@asu.edu, xzhou74@asu.edu
-License: GPLv3+
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9.0
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: numpy>=1.26.4
-Requires-Dist: osmium>=3.7.0
-Requires-Dist: Requests>=2.31.0
-Requires-Dist: setuptools>=68.2.2
-Requires-Dist: Shapely>=2.0.3
-Requires-Dist: matplotlib>=3.8.2
-
-osm2gmns
-====================================
-| **Authors**: Jiawei Lu, Xuesong (Simon) Zhou
-| **Email**: jiaweil9@asu.edu, xzhou74@asu.edu
-
-
-osm2gmns is an open-source Python package that enables users to conveniently obtain and
-manipulate any networks from `OpenStreetMap`_ (OSM). With a single line of Python code,
-users can obtian and model drivable, bikeable, walkable, railway, and aeroway networks
-for any region in the world, and output networks to csv files in `GMNS`_ format for seamless
-data sharing and research collaboration. osm2gmns mainly focus on providing researchers and
-practitioners with flexible, standard and ready-to-use multi-module transportation networks,
-as well as a bunch of customized and practical functions to facilitate various reseaches
-and applications on traffic modeling.
-
-
-Publication
-====================================
-
-Lu, J., & Zhou, X.S. (2023). Virtual track networks: A hierarchical modeling framework and
-open-source tools for simplified and efficient connected and automated mobility (CAM) system
-design based on general modeling network specification (GMNS). Transportation Research
-Part C: Emerging Technologies, 153, 104223. `paper link`_
-
-
-Main Features
-====================================
-
-- Obtain any networks from OSM. osm2gmns parses map data from OSM and output networks to
-  csv files in GMNS format.
-- Standard network format. osm2gmns adopts GMNS as the network format for seamless data
-  sharing and research collaboration.
-- Ready-to-use network. osm2gmns cleans erroneous information from osm map data and is able
-  to fill up critical missing values, i.e., lanes, speed and capacity, to quickly provide
-  ready-to-use networks.
-- Directed network. two directed road links are generated for each bi-directional osm ways identified by osm2gmns
-- Multi-module support. five different network types are supported, including auto, bike, walk, railway, and aeroway
-- Customized and practical functions to facilitate traffic modeling. functions include
-  complex intersection consolidation, moevement generation, traffic zone creation, short link combination,
-  network visualization.
-- Multi-Resolution modeling. osm2gmns automatically construct the corresponding mesoscopic and microscopic
-  networks for any macroscopic network in GMNS format.
-
-
-Installation
-====================================
-
-.. code-block:: bash
-
-    pip install osm2gmns
-
-If you meet installation issues, please refer to the `user's guide`_ for solutions.
-
-
-Simple examples
-====================================
-
-You can find the osm map file used in the examples below at 'sample networks/Arizona State University, Tempe Campus'
-
-Quickly get the network with point of interest (POI) information from an osm file
-
-.. code:: python
-
-    >>> import osm2gmns as og
-    >>> net = og.getNetFromFile('asu.osm', POI=True)
-    >>> og.outputNetToCSV(net)
-
-Generate multi-resolution networks from an osm file
-
-.. code:: python
-
-    >>> import osm2gmns as og
-    >>> net = og.getNetFromFile('asu.osm')
-    >>> og.consolidateComplexIntersections(net, auto_identify=True)
-    >>> og.buildMultiResolutionNets(net)
-    >>> og.outputNetToCSV(net)
-
-
-Get relation id of a place of interest and download the corresponding osm file
-=====================================================================================================================
-You can use the following code to get the relation id of a place of interest and download the corresponding osm file.
-
-.. code:: python
-
-    >>> import osm2gmns as og
-    # get relation id of a place of interest
-    # For the place of interest, e.g. Arizona State University
-    # e.g. "Tempe, Arizona, United States"
-    # e.g. "Arizona, US"
-    # e.g. "Beijing Jiaotong University, Beijing, China"
-    >>> rel_id = og.getOSMRelationID('Arizona State University')
-    >>> rel_id
-        Info: Found relation id 3444656 from web
-        Info: location of the place of interest:
-        {
-            "place_id": 318528634,
-            "licence": "Data \u00a9 OpenStreetMap contributors, ODbL 1.0. http://osm.org/copyright",
-            "osm_type": "relation",
-            "osm_id": 3444656,
-            "lat": "33.4213174",
-            "lon": "-111.93316305413154",
-            "class": "amenity",
-            "type": "university",
-            "place_rank": 30,
-            "importance": 0.5547365758311374,
-            "addresstype": "amenity",
-            "name": "Arizona State University",
-            "display_name": "Arizona State University, 1151, South Forest Avenue, Tempe Junction, Tempe, Maricopa County, Arizona, 85281, United States",
-            "boundingbox": [
-                "33.4102062",
-                "33.4329786",
-                "-111.9411651",
-                "-111.9092447"
-            ]
-        }
-    3444656
-
-    # download the corresponding osm file
-    >>> og.downloadOSMData(rel_id, 'asu.osm')
-
-
-Visualization
-====================================
-
-You can visualize generated networks using `NeXTA`_ or `QGIS`_.
-
-.. figure:: https://github.com/jiawlu/OSM2GMNS/blob/master/sample%20networks/Arizona%20State%20University%2C%20Tempe%20Campus/net_asu.png
-    :name: case_asu
-    :align: center
-    :width: 80%
-
-    Arizona State Unversity, Tempe Campus
-
-
-User's guide
-====================================
-You can check the `user's guide`_ for a detailed introduction of osm2gmns.
-
-
-.. _`OpenStreetMap`: https://www.openstreetmap.org
-.. _`GMNS`: https://github.com/zephyr-data-specs/GMNS
-.. _`paper link`: https://doi.org/10.1016/j.trc.2023.104223
-.. _`NeXTA`: https://github.com/asu-trans-ai-lab/NeXTA4GMNS
-.. _`QGIS`: https://qgis.org
-.. _`user's guide`: https://osm2gmns.readthedocs.io
+Metadata-Version: 2.1
+Name: osm2gmns
+Version: 0.7.6
+Summary: convert map data from OpenStreetMap to network files in GMNS format
+Home-page: https://github.com/jiawlu/OSM2GMNS
+Author: Jiawei Lu, Xuesong Zhou
+Author-email: jiaweil9@asu.edu, xzhou74@asu.edu
+License: GPLv3+
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: osmium>=3.7.0
+Requires-Dist: pyufunc>=0.2.1
+Requires-Dist: Requests>=2.31.0
+Requires-Dist: setuptools>=68.2.2
+Requires-Dist: Shapely>=2.0.3
+Requires-Dist: matplotlib>=3.8.2
+
+osm2gmns
+====================================
+| **Authors**: Jiawei Lu, Xuesong (Simon) Zhou
+| **Email**: jiaweil9@asu.edu, xzhou74@asu.edu
+
+
+osm2gmns is an open-source Python package that enables users to conveniently obtain and
+manipulate any networks from OpenStreetMap (OSM). With a single line of Python code,
+users can obtain and model drivable, bikeable, walkable, railway, and aeroway networks
+for any region in the world and output networks to CSV files in GMNS format for seamless
+data sharing and research collaboration. osm2gmns mainly focuses on providing researchers and
+practitioners with flexible, standard and ready-to-use multi-modal transportation networks,
+as well as a bunch of customized and practical functions to facilitate various research
+and applications on traffic modeling.
+
+
+Publication
+====================================
+
+Lu, J., & Zhou, X.S. (2023). Virtual track networks: A hierarchical modeling framework and
+open-source tools for simplified and efficient connected and automated mobility (CAM) system
+design based on general modeling network specification (GMNS). Transportation Research
+Part C: Emerging Technologies, 153, 104223. `paper link`_
+
+
+Main Features
+====================================
+
+- Obtain any networks from OSM. osm2gmns parses map data from OSM and output networks to
+  csv files in GMNS format.
+- Standard network format. osm2gmns adopts GMNS as the network format for seamless data
+  sharing and research collaboration.
+- Ready-to-use network. osm2gmns cleans erroneous information from osm map data and is able
+  to fill up critical missing values, i.e., lanes, speed and capacity, to quickly provide
+  ready-to-use networks.
+- Directed network. two directed road links are generated for each bi-directional osm ways identified by osm2gmns
+- Multi-module support. five different network types are supported, including auto, bike, walk, railway, and aeroway
+- Customized and practical functions to facilitate traffic modeling. functions include
+  complex intersection consolidation, moevement generation, traffic zone creation, short link combination,
+  network visualization.
+- Multi-Resolution modeling. osm2gmns automatically construct the corresponding mesoscopic and microscopic
+  networks for any macroscopic network in GMNS format.
+
+
+Installation
+====================================
+
+.. code-block:: bash
+
+    pip install osm2gmns
+
+If you meet installation issues, please refer to the `user's guide`_ for solutions.
+
+
+Simple examples
+====================================
+
+You can find the osm map file used in the examples below at 'sample networks/Arizona State University, Tempe Campus'
+
+Quickly get the network with point of interest (POI) information from an osm file
+
+.. code:: python
+
+    >>> import osm2gmns as og
+    >>> net = og.getNetFromFile('asu.osm', POI=True)
+    >>> og.outputNetToCSV(net)
+
+Generate multi-resolution networks from an osm file
+
+.. code:: python
+
+    >>> import osm2gmns as og
+    >>> net = og.getNetFromFile('asu.osm')
+    >>> og.consolidateComplexIntersections(net, auto_identify=True)
+    >>> og.buildMultiResolutionNets(net)
+    >>> og.outputNetToCSV(net)
+
+
+Get relation id of a place of interest and download the corresponding osm file
+=====================================================================================================================
+You can use the following code to get the relation id of a place of interest and download the corresponding osm file.
+
+.. code:: python
+
+    >>> import osm2gmns as og
+    # get relation id of a place of interest
+    # For the place of interest, e.g. Arizona State University
+    # e.g. "Tempe, Arizona, United States"
+    # e.g. "Arizona, US"
+    # e.g. "Beijing Jiaotong University, Beijing, China"
+    >>> rel_id = og.getOSMRelationID('Arizona State University')
+    >>> rel_id
+        Info: Found relation id 3444656 from web
+        Info: location of the place of interest:
+        {
+            "place_id": 318528634,
+            "licence": "Data \u00a9 OpenStreetMap contributors, ODbL 1.0. http://osm.org/copyright",
+            "osm_type": "relation",
+            "osm_id": 3444656,
+            "lat": "33.4213174",
+            "lon": "-111.93316305413154",
+            "class": "amenity",
+            "type": "university",
+            "place_rank": 30,
+            "importance": 0.5547365758311374,
+            "addresstype": "amenity",
+            "name": "Arizona State University",
+            "display_name": "Arizona State University, 1151, South Forest Avenue, Tempe Junction, Tempe, Maricopa County, Arizona, 85281, United States",
+            "boundingbox": [
+                "33.4102062",
+                "33.4329786",
+                "-111.9411651",
+                "-111.9092447"
+            ]
+        }
+    3444656
+
+    # download the corresponding osm file
+    >>> og.downloadOSMData(rel_id, 'asu.osm')
+
+
+User's guide
+====================================
+You can check the `user's guide`_ for a detailed introduction of osm2gmns.
+
+
+.. _`OpenStreetMap`: https://www.openstreetmap.org
+.. _`GMNS`: https://github.com/zephyr-data-specs/GMNS
+.. _`paper link`: https://doi.org/10.1016/j.trc.2023.104223
+.. _`user's guide`: https://osm2gmns.readthedocs.io
```

### Comparing `osm2gmns-0.7.5/README.rst` & `osm2gmns-0.7.6/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,145 +1,130 @@
-osm2gmns
-====================================
-| **Authors**: Jiawei Lu, Xuesong (Simon) Zhou
-| **Email**: jiaweil9@asu.edu, xzhou74@asu.edu
-
-
-osm2gmns is an open-source Python package that enables users to conveniently obtain and
-manipulate any networks from `OpenStreetMap`_ (OSM). With a single line of Python code,
-users can obtian and model drivable, bikeable, walkable, railway, and aeroway networks
-for any region in the world, and output networks to csv files in `GMNS`_ format for seamless
-data sharing and research collaboration. osm2gmns mainly focus on providing researchers and
-practitioners with flexible, standard and ready-to-use multi-module transportation networks,
-as well as a bunch of customized and practical functions to facilitate various reseaches
-and applications on traffic modeling.
-
-
-Publication
-====================================
-
-Lu, J., & Zhou, X.S. (2023). Virtual track networks: A hierarchical modeling framework and
-open-source tools for simplified and efficient connected and automated mobility (CAM) system
-design based on general modeling network specification (GMNS). Transportation Research
-Part C: Emerging Technologies, 153, 104223. `paper link`_
-
-
-Main Features
-====================================
-
-- Obtain any networks from OSM. osm2gmns parses map data from OSM and output networks to
-  csv files in GMNS format.
-- Standard network format. osm2gmns adopts GMNS as the network format for seamless data
-  sharing and research collaboration.
-- Ready-to-use network. osm2gmns cleans erroneous information from osm map data and is able
-  to fill up critical missing values, i.e., lanes, speed and capacity, to quickly provide
-  ready-to-use networks.
-- Directed network. two directed road links are generated for each bi-directional osm ways identified by osm2gmns
-- Multi-module support. five different network types are supported, including auto, bike, walk, railway, and aeroway
-- Customized and practical functions to facilitate traffic modeling. functions include
-  complex intersection consolidation, moevement generation, traffic zone creation, short link combination,
-  network visualization.
-- Multi-Resolution modeling. osm2gmns automatically construct the corresponding mesoscopic and microscopic
-  networks for any macroscopic network in GMNS format.
-
-
-Installation
-====================================
-
-.. code-block:: bash
-
-    pip install osm2gmns
-
-If you meet installation issues, please refer to the `user's guide`_ for solutions.
-
-
-Simple examples
-====================================
-
-You can find the osm map file used in the examples below at 'sample networks/Arizona State University, Tempe Campus'
-
-Quickly get the network with point of interest (POI) information from an osm file
-
-.. code:: python
-
-    >>> import osm2gmns as og
-    >>> net = og.getNetFromFile('asu.osm', POI=True)
-    >>> og.outputNetToCSV(net)
-
-Generate multi-resolution networks from an osm file
-
-.. code:: python
-
-    >>> import osm2gmns as og
-    >>> net = og.getNetFromFile('asu.osm')
-    >>> og.consolidateComplexIntersections(net, auto_identify=True)
-    >>> og.buildMultiResolutionNets(net)
-    >>> og.outputNetToCSV(net)
-
-
-Get relation id of a place of interest and download the corresponding osm file
-=====================================================================================================================
-You can use the following code to get the relation id of a place of interest and download the corresponding osm file.
-
-.. code:: python
-
-    >>> import osm2gmns as og
-    # get relation id of a place of interest
-    # For the place of interest, e.g. Arizona State University
-    # e.g. "Tempe, Arizona, United States"
-    # e.g. "Arizona, US"
-    # e.g. "Beijing Jiaotong University, Beijing, China"
-    >>> rel_id = og.getOSMRelationID('Arizona State University')
-    >>> rel_id
-        Info: Found relation id 3444656 from web
-        Info: location of the place of interest:
-        {
-            "place_id": 318528634,
-            "licence": "Data \u00a9 OpenStreetMap contributors, ODbL 1.0. http://osm.org/copyright",
-            "osm_type": "relation",
-            "osm_id": 3444656,
-            "lat": "33.4213174",
-            "lon": "-111.93316305413154",
-            "class": "amenity",
-            "type": "university",
-            "place_rank": 30,
-            "importance": 0.5547365758311374,
-            "addresstype": "amenity",
-            "name": "Arizona State University",
-            "display_name": "Arizona State University, 1151, South Forest Avenue, Tempe Junction, Tempe, Maricopa County, Arizona, 85281, United States",
-            "boundingbox": [
-                "33.4102062",
-                "33.4329786",
-                "-111.9411651",
-                "-111.9092447"
-            ]
-        }
-    3444656
-
-    # download the corresponding osm file
-    >>> og.downloadOSMData(rel_id, 'asu.osm')
-
-
-Visualization
-====================================
-
-You can visualize generated networks using `NeXTA`_ or `QGIS`_.
-
-.. figure:: https://github.com/jiawlu/OSM2GMNS/blob/master/sample%20networks/Arizona%20State%20University%2C%20Tempe%20Campus/net_asu.png
-    :name: case_asu
-    :align: center
-    :width: 80%
-
-    Arizona State Unversity, Tempe Campus
-
-
-User's guide
-====================================
-You can check the `user's guide`_ for a detailed introduction of osm2gmns.
-
-
-.. _`OpenStreetMap`: https://www.openstreetmap.org
-.. _`GMNS`: https://github.com/zephyr-data-specs/GMNS
-.. _`paper link`: https://doi.org/10.1016/j.trc.2023.104223
-.. _`NeXTA`: https://github.com/asu-trans-ai-lab/NeXTA4GMNS
-.. _`QGIS`: https://qgis.org
+osm2gmns
+====================================
+| **Authors**: Jiawei Lu, Xuesong (Simon) Zhou
+| **Email**: jiaweil9@asu.edu, xzhou74@asu.edu
+
+
+osm2gmns is an open-source Python package that enables users to conveniently obtain and
+manipulate any networks from OpenStreetMap (OSM). With a single line of Python code,
+users can obtain and model drivable, bikeable, walkable, railway, and aeroway networks
+for any region in the world and output networks to CSV files in GMNS format for seamless
+data sharing and research collaboration. osm2gmns mainly focuses on providing researchers and
+practitioners with flexible, standard and ready-to-use multi-modal transportation networks,
+as well as a bunch of customized and practical functions to facilitate various research
+and applications on traffic modeling.
+
+
+Publication
+====================================
+
+Lu, J., & Zhou, X.S. (2023). Virtual track networks: A hierarchical modeling framework and
+open-source tools for simplified and efficient connected and automated mobility (CAM) system
+design based on general modeling network specification (GMNS). Transportation Research
+Part C: Emerging Technologies, 153, 104223. `paper link`_
+
+
+Main Features
+====================================
+
+- Obtain any networks from OSM. osm2gmns parses map data from OSM and output networks to
+  csv files in GMNS format.
+- Standard network format. osm2gmns adopts GMNS as the network format for seamless data
+  sharing and research collaboration.
+- Ready-to-use network. osm2gmns cleans erroneous information from osm map data and is able
+  to fill up critical missing values, i.e., lanes, speed and capacity, to quickly provide
+  ready-to-use networks.
+- Directed network. two directed road links are generated for each bi-directional osm ways identified by osm2gmns
+- Multi-module support. five different network types are supported, including auto, bike, walk, railway, and aeroway
+- Customized and practical functions to facilitate traffic modeling. functions include
+  complex intersection consolidation, moevement generation, traffic zone creation, short link combination,
+  network visualization.
+- Multi-Resolution modeling. osm2gmns automatically construct the corresponding mesoscopic and microscopic
+  networks for any macroscopic network in GMNS format.
+
+
+Installation
+====================================
+
+.. code-block:: bash
+
+    pip install osm2gmns
+
+If you meet installation issues, please refer to the `user's guide`_ for solutions.
+
+
+Simple examples
+====================================
+
+You can find the osm map file used in the examples below at 'sample networks/Arizona State University, Tempe Campus'
+
+Quickly get the network with point of interest (POI) information from an osm file
+
+.. code:: python
+
+    >>> import osm2gmns as og
+    >>> net = og.getNetFromFile('asu.osm', POI=True)
+    >>> og.outputNetToCSV(net)
+
+Generate multi-resolution networks from an osm file
+
+.. code:: python
+
+    >>> import osm2gmns as og
+    >>> net = og.getNetFromFile('asu.osm')
+    >>> og.consolidateComplexIntersections(net, auto_identify=True)
+    >>> og.buildMultiResolutionNets(net)
+    >>> og.outputNetToCSV(net)
+
+
+Get relation id of a place of interest and download the corresponding osm file
+=====================================================================================================================
+You can use the following code to get the relation id of a place of interest and download the corresponding osm file.
+
+.. code:: python
+
+    >>> import osm2gmns as og
+    # get relation id of a place of interest
+    # For the place of interest, e.g. Arizona State University
+    # e.g. "Tempe, Arizona, United States"
+    # e.g. "Arizona, US"
+    # e.g. "Beijing Jiaotong University, Beijing, China"
+    >>> rel_id = og.getOSMRelationID('Arizona State University')
+    >>> rel_id
+        Info: Found relation id 3444656 from web
+        Info: location of the place of interest:
+        {
+            "place_id": 318528634,
+            "licence": "Data \u00a9 OpenStreetMap contributors, ODbL 1.0. http://osm.org/copyright",
+            "osm_type": "relation",
+            "osm_id": 3444656,
+            "lat": "33.4213174",
+            "lon": "-111.93316305413154",
+            "class": "amenity",
+            "type": "university",
+            "place_rank": 30,
+            "importance": 0.5547365758311374,
+            "addresstype": "amenity",
+            "name": "Arizona State University",
+            "display_name": "Arizona State University, 1151, South Forest Avenue, Tempe Junction, Tempe, Maricopa County, Arizona, 85281, United States",
+            "boundingbox": [
+                "33.4102062",
+                "33.4329786",
+                "-111.9411651",
+                "-111.9092447"
+            ]
+        }
+    3444656
+
+    # download the corresponding osm file
+    >>> og.downloadOSMData(rel_id, 'asu.osm')
+
+
+User's guide
+====================================
+You can check the `user's guide`_ for a detailed introduction of osm2gmns.
+
+
+.. _`OpenStreetMap`: https://www.openstreetmap.org
+.. _`GMNS`: https://github.com/zephyr-data-specs/GMNS
+.. _`paper link`: https://doi.org/10.1016/j.trc.2023.104223
 .. _`user's guide`: https://osm2gmns.readthedocs.io
```

### Comparing `osm2gmns-0.7.5/osm2gmns/func_lib/extract_relation_id.py` & `osm2gmns-0.7.6/osm2gmns/func_lib/extract_relation_id.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,249 +1,249 @@
-# -*- coding:utf-8 -*-
-##############################################################
-# Created Date: Monday, May 29th 2023
-# Contact Info: luoxiangyong01@gmail.com
-# Author/Copyright: Mr. Xiangyong Luo
-##############################################################
-
-
-import requests
-import json
-import urllib
-import os
-from typing import Union
-from pathlib import Path
-
-
-class OSMRelationIDFinder:
-    """A class to find the osm relation id of a place of interest globally
-       Use the Nominatim API to find the relation id of a place of interest
-
-    Args:
-        poi_name (str): the name of the place of interest,
-            e.g., "Arizona State University"
-            e.g., "Tempe, Arizona, USA"
-            e.g., "Arizona, USA"
-
-    Example:
-    >>> import osm2gmns as og
-    >>> rel = og.OSM_RelationID_Finder("Arizona State University")
-    >>> rel.rel_id
-        Info: Found relation id 3444656 from web
-        Info: location of the place of interest:
-        {
-            "place_id": 318528634,
-            "licence": "Data \u00a9 OpenStreetMap contributors, ODbL 1.0. http://osm.org/copyright",
-            "osm_type": "relation",
-            "osm_id": 3444656,
-            "lat": "33.4213174",
-            "lon": "-111.93316305413154",
-            "class": "amenity",
-            "type": "university",
-            "place_rank": 30,
-            "importance": 0.5547365758311374,
-            "addresstype": "amenity",
-            "name": "Arizona State University",
-            "display_name": "Arizona State University, 1151, South Forest Avenue, Tempe Junction, Tempe, Maricopa County, Arizona, 85281, United States",
-            "boundingbox": [
-                "33.4102062",
-                "33.4329786",
-                "-111.9411651",
-                "-111.9092447"
-            ]
-        }
-    3444656
-
-    # download the corresponding osm file
-    >>> og.downloadOSMData(rel.rel_id, 'asu.osm')
-
-    """
-
-    def __init__(self, poi_name: str) -> None:
-
-        self.poi_name = poi_name
-        self.__url_json = self.__get_url_data()
-
-        # maximum number of results to show
-        # if parameter will applied in function rel_id_info
-        # if the number of results is greater than _max_show, only show the first _max_show results
-        self._max_show = 5
-
-        # TODO: Unable to find the relation id locally, search from the web
-        # the default path to save/load global country, state, and city information
-        self._path_global_rel_id = self.__path2linux(os.path.join(
-            Path(__file__).resolve().parent.parent.parent, "dependencies/global_rel_id.json"))
-
-    def __get_url_data(self) -> dict:
-        # prepare url
-        base_url = 'https://nominatim.openstreetmap.org/search?'
-        params = {"q": self.poi_name, "format": "json"}
-        url = base_url + urllib.parse.urlencode(params)
-
-        # get data from url using requests
-        url_res = requests.get(url)
-        url_json = json.loads(url_res.text)
-        return url_json
-
-    @property
-    def rel_id(self) -> Union[float, None]:
-        # Three logic to find the relation id
-        # 1. Search from web, if relation id exist, return the relation id
-        # 2. If relation id does not exist
-        #    check whether url_json (result from web) is empty,
-        #    if not, return relation id of the first element
-        # 3. If url_json is empty, Search locally, return None if not found locally
-
-        for i in self.__url_json:
-            if i["osm_type"] == "relation":
-                print(f"  Info: Found relation id {i['osm_id']} from web")
-                print("  Info: location of the place of interest:")
-                print(json.dumps(i, indent=4))
-                return i["osm_id"]
-
-        if len(self.rel_id_info) > 0:
-            print("  Info: Could not find relation id directly from web")
-            print(f"  but there is a possible relation id {self.rel_id_info[0]['osm_id']} from web")
-            print("  or you can find more related ids: rel.rel_id_info")
-            print(f"Detailed info for {self.rel_id_info[0]['osm_id']}: {json.dumps(self.rel_id_info[0], indent=4)}\n")
-            return self.rel_id_info[0]["osm_id"]
-
-        print("  Info: Could not find relation id from web: https://nominatim.openstreetmap.org/ui/search.html \n")
-        return self.__find_local_rel_id()
-
-    @property
-    def rel_id_info(self) -> dict:
-        # show detailed information of the relation id
-        return self.__url_json if len(self.__url_json) < self._max_show else self.__url_json[:self._max_show]
-
-    # convert OS path to standard linux path
-    def __path2linux(self, path: Union[str, Path]) -> str:
-        """Convert a path to a linux path, linux path can run in windows, linux and mac"""
-        try:
-            return path.replace("\\", "/")
-        except Exception:
-            return str(path).replace("\\", "/")
-
-    def __find_local_rel_id(self) -> str:
-        # sourcery skip: extract-duplicate-method
-
-        # Step 0 load the global country, state, and city information from github
-        try:
-            print("  Info: Try to load global_rel_id.json from GitHub\n")
-            github_url = "https://raw.githubusercontent.com/xyluo25/OSM2GMNS/master/dependencies/global_rel_id.json"
-            global_rel_id_dict = json.loads(requests.get(github_url).text)
-        except Exception:
-            # if user can not access the internet, load the local file instead
-            # please make sure the file exists in the local path
-            # path: dependencies/global_rel_id.json
-            print("  Info: Can not load global_rel_id.json from GitHub")
-            print(f"  try to load local file: {self._path_global_rel_id}.\n")
-            try:
-                with open(self._path_global_rel_id, "r") as f:
-                    global_rel_id_dict = json.load(f)
-            except Exception:
-                print("  Error: Can not load global_rel_id.json from local file\n \
-                      please make sure the file exists in dependencies/global_rel_id.json \n \
-                      Please search from https://www.openstreetmap.org/#map=5/40.298/-102.500  \n")
-                return None
-
-        # if we can not load dictionary, return None
-        if not isinstance(global_rel_id_dict, dict):
-            print("  Info: Could not load global_rel_id.json from GitHub.")
-            print("  Please search from https://www.openstreetmap.org/#map=5/40.298/-102.500  \n")
-            return None
-
-        search_name = self.poi_name.split(",")[0].strip()
-        if search_name == self.poi_name:
-            search_name = self.poi_name.split(" ")[0].strip()
-
-        # Step 1 Find the country start with the input characters
-        start_with_country = [country_name for country_name in global_rel_id_dict["country"].keys(
-        ) if country_name.lower().startswith(search_name.lower())][:self._max_show]
-
-        # Step 2 Find the state start with the input characters
-        start_with_state = [state_name for state_name in global_rel_id_dict["state"].keys(
-        ) if state_name.lower().startswith(search_name.lower())][:self._max_show]
-
-        # Step 3 Find the city start with the input characters
-        start_with_city = [city_name for city_name in global_rel_id_dict["city"].keys(
-        ) if city_name.lower().startswith(search_name.lower())][:self._max_show]
-
-        # Step 4 Format the results
-        formatted_str = ""
-        if start_with_city:
-            formatted_str += "City:\n"
-            for city_name in start_with_city:
-                formatted_str += f"""{city_name},
-                {global_rel_id_dict["city"][city_name]["state"]},
-                {global_rel_id_dict["city"][city_name]["country"]},
-                rel_id: {global_rel_id_dict["city"][city_name]["osm_id"]} \n"""
-
-        if start_with_state:
-            formatted_str += "State:\n"
-            for state_name in start_with_state:
-                formatted_str += f"""{state_name},
-                {global_rel_id_dict["state"][state_name]["country"]},
-                rel_id: {global_rel_id_dict["state"][state_name]["osm_id"]} \n"""
-
-        if start_with_country:
-            formatted_str += "Country:\n"
-            for country_name in start_with_country:
-                formatted_str += f"""{country_name},
-                rel_id: {global_rel_id_dict["country"][country_name]["osm_id"]} \n"""
-
-        if formatted_str:
-
-            formatted_str = f"""Info:\nWe can not search rel_id from web with place of interest: {self.poi_name} \n \
-            Search locally with country, state and city startswith {search_name}:\n""" + formatted_str
-
-            formatted_str += "You can replace your place of interest with local results above to get the rel_id\n"
-            print(formatted_str)
-
-        print("  Info: Could not load global_rel_id.json locally")
-        print("  Please search from https://www.openstreetmap.org/#map=5/40.298/-102.500  \n")
-        return None
-
-
-def getOSMRelationID(poi_name: str) -> Union[float, None]:
-    """Get the relation id of a place of interest globally
-
-    Args:
-        poi_name (str): the name of the place of interest,
-            e.g., "Arizona State University"
-            e.g., "Tempe, Arizona, USA"
-            e.g., "Arizona, USA"
-
-    Returns:
-        Union[float, None]: the relation id of the place of interest, if not found, return None
-
-    Example:
-        >>> import osm2gmns as og
-        >>> rel = og.getOSMRelationID("Arizona State University")
-        >>> rel
-            Info: Found relation id 3444656 from web
-            Info: location of the place of interest:
-            {
-                "place_id": 318528634,
-                "licence": "Data \u00a9 OpenStreetMap contributors, ODbL 1.0. http://osm.org/copyright",
-                "osm_type": "relation",
-                "osm_id": 3444656,
-                "lat": "33.4213174",
-                "lon": "-111.93316305413154",
-                "class": "amenity",
-                "type": "university",
-                "place_rank": 30,
-                "importance": 0.5547365758311374,
-                "addresstype": "amenity",
-                "name": "Arizona State University",
-                "display_name": "Arizona State University, 1151, South Forest Avenue, Tempe Junction, Tempe, Maricopa County, Arizona, 85281, United States",
-                "boundingbox": [
-                    "33.4102062",
-                    "33.4329786",
-                    "-111.9411651",
-                    "-111.9092447"
-                ]
-            }
-        3444656
-    """
-    rel = OSMRelationIDFinder(poi_name)
+# -*- coding:utf-8 -*-
+##############################################################
+# Created Date: Monday, May 29th 2023
+# Contact Info: luoxiangyong01@gmail.com
+# Author/Copyright: Mr. Xiangyong Luo
+##############################################################
+
+
+import requests
+import json
+import urllib
+import os
+from typing import Union
+from pathlib import Path
+
+
+class OSMRelationIDFinder:
+    """A class to find the osm relation id of a place of interest globally
+       Use the Nominatim API to find the relation id of a place of interest
+
+    Args:
+        poi_name (str): the name of the place of interest,
+            e.g., "Arizona State University"
+            e.g., "Tempe, Arizona, USA"
+            e.g., "Arizona, USA"
+
+    Example:
+    >>> import osm2gmns as og
+    >>> rel = og.OSM_RelationID_Finder("Arizona State University")
+    >>> rel.rel_id
+        Info: Found relation id 3444656 from web
+        Info: location of the place of interest:
+        {
+            "place_id": 318528634,
+            "licence": "Data \u00a9 OpenStreetMap contributors, ODbL 1.0. http://osm.org/copyright",
+            "osm_type": "relation",
+            "osm_id": 3444656,
+            "lat": "33.4213174",
+            "lon": "-111.93316305413154",
+            "class": "amenity",
+            "type": "university",
+            "place_rank": 30,
+            "importance": 0.5547365758311374,
+            "addresstype": "amenity",
+            "name": "Arizona State University",
+            "display_name": "Arizona State University, 1151, South Forest Avenue, Tempe Junction, Tempe, Maricopa County, Arizona, 85281, United States",
+            "boundingbox": [
+                "33.4102062",
+                "33.4329786",
+                "-111.9411651",
+                "-111.9092447"
+            ]
+        }
+    3444656
+
+    # download the corresponding osm file
+    >>> og.downloadOSMData(rel.rel_id, 'asu.osm')
+
+    """
+
+    def __init__(self, poi_name: str) -> None:
+
+        self.poi_name = poi_name
+        self.__url_json = self.__get_url_data()
+
+        # maximum number of results to show
+        # if parameter will applied in function rel_id_info
+        # if the number of results is greater than _max_show, only show the first _max_show results
+        self._max_show = 5
+
+        # TODO: Unable to find the relation id locally, search from the web
+        # the default path to save/load global country, state, and city information
+        self._path_global_rel_id = self.__path2linux(os.path.join(
+            Path(__file__).resolve().parent.parent.parent, "dependencies/global_rel_id.json"))
+
+    def __get_url_data(self) -> dict:
+        # prepare url
+        base_url = 'https://nominatim.openstreetmap.org/search?'
+        params = {"q": self.poi_name, "format": "json"}
+        url = base_url + urllib.parse.urlencode(params)
+
+        # get data from url using requests
+        url_res = requests.get(url)
+        url_json = json.loads(url_res.text)
+        return url_json
+
+    @property
+    def rel_id(self) -> Union[float, None]:
+        # Three logic to find the relation id
+        # 1. Search from web, if relation id exist, return the relation id
+        # 2. If relation id does not exist
+        #    check whether url_json (result from web) is empty,
+        #    if not, return relation id of the first element
+        # 3. If url_json is empty, Search locally, return None if not found locally
+
+        for i in self.__url_json:
+            if i["osm_type"] == "relation":
+                print(f"  Info: Found relation id {i['osm_id']} from web")
+                print("  Info: location of the place of interest:")
+                print(json.dumps(i, indent=4))
+                return i["osm_id"]
+
+        if len(self.rel_id_info) > 0:
+            print("  Info: Could not find relation id directly from web")
+            print(f"  but there is a possible relation id {self.rel_id_info[0]['osm_id']} from web")
+            print("  or you can find more related ids: rel.rel_id_info")
+            print(f"Detailed info for {self.rel_id_info[0]['osm_id']}: {json.dumps(self.rel_id_info[0], indent=4)}\n")
+            return self.rel_id_info[0]["osm_id"]
+
+        print("  Info: Could not find relation id from web: https://nominatim.openstreetmap.org/ui/search.html \n")
+        return self.__find_local_rel_id()
+
+    @property
+    def rel_id_info(self) -> dict:
+        # show detailed information of the relation id
+        return self.__url_json if len(self.__url_json) < self._max_show else self.__url_json[:self._max_show]
+
+    # convert OS path to standard linux path
+    def __path2linux(self, path: Union[str, Path]) -> str:
+        """Convert a path to a linux path, linux path can run in windows, linux and mac"""
+        try:
+            return path.replace("\\", "/")
+        except Exception:
+            return str(path).replace("\\", "/")
+
+    def __find_local_rel_id(self) -> str:
+        # sourcery skip: extract-duplicate-method
+
+        # Step 0 load the global country, state, and city information from github
+        try:
+            print("  Info: Try to load global_rel_id.json from GitHub\n")
+            github_url = "https://raw.githubusercontent.com/xyluo25/OSM2GMNS/master/dependencies/global_rel_id.json"
+            global_rel_id_dict = json.loads(requests.get(github_url).text)
+        except Exception:
+            # if user can not access the internet, load the local file instead
+            # please make sure the file exists in the local path
+            # path: dependencies/global_rel_id.json
+            print("  Info: Can not load global_rel_id.json from GitHub")
+            print(f"  try to load local file: {self._path_global_rel_id}.\n")
+            try:
+                with open(self._path_global_rel_id, "r") as f:
+                    global_rel_id_dict = json.load(f)
+            except Exception:
+                print("  Error: Can not load global_rel_id.json from local file\n \
+                      please make sure the file exists in dependencies/global_rel_id.json \n \
+                      Please search from https://www.openstreetmap.org/#map=5/40.298/-102.500  \n")
+                return None
+
+        # if we can not load dictionary, return None
+        if not isinstance(global_rel_id_dict, dict):
+            print("  Info: Could not load global_rel_id.json from GitHub.")
+            print("  Please search from https://www.openstreetmap.org/#map=5/40.298/-102.500  \n")
+            return None
+
+        search_name = self.poi_name.split(",")[0].strip()
+        if search_name == self.poi_name:
+            search_name = self.poi_name.split(" ")[0].strip()
+
+        # Step 1 Find the country start with the input characters
+        start_with_country = [country_name for country_name in global_rel_id_dict["country"].keys(
+        ) if country_name.lower().startswith(search_name.lower())][:self._max_show]
+
+        # Step 2 Find the state start with the input characters
+        start_with_state = [state_name for state_name in global_rel_id_dict["state"].keys(
+        ) if state_name.lower().startswith(search_name.lower())][:self._max_show]
+
+        # Step 3 Find the city start with the input characters
+        start_with_city = [city_name for city_name in global_rel_id_dict["city"].keys(
+        ) if city_name.lower().startswith(search_name.lower())][:self._max_show]
+
+        # Step 4 Format the results
+        formatted_str = ""
+        if start_with_city:
+            formatted_str += "City:\n"
+            for city_name in start_with_city:
+                formatted_str += f"""{city_name},
+                {global_rel_id_dict["city"][city_name]["state"]},
+                {global_rel_id_dict["city"][city_name]["country"]},
+                rel_id: {global_rel_id_dict["city"][city_name]["osm_id"]} \n"""
+
+        if start_with_state:
+            formatted_str += "State:\n"
+            for state_name in start_with_state:
+                formatted_str += f"""{state_name},
+                {global_rel_id_dict["state"][state_name]["country"]},
+                rel_id: {global_rel_id_dict["state"][state_name]["osm_id"]} \n"""
+
+        if start_with_country:
+            formatted_str += "Country:\n"
+            for country_name in start_with_country:
+                formatted_str += f"""{country_name},
+                rel_id: {global_rel_id_dict["country"][country_name]["osm_id"]} \n"""
+
+        if formatted_str:
+
+            formatted_str = f"""Info:\nWe can not search rel_id from web with place of interest: {self.poi_name} \n \
+            Search locally with country, state and city startswith {search_name}:\n""" + formatted_str
+
+            formatted_str += "You can replace your place of interest with local results above to get the rel_id\n"
+            print(formatted_str)
+
+        print("  Info: Could not load global_rel_id.json locally")
+        print("  Please search from https://www.openstreetmap.org/#map=5/40.298/-102.500  \n")
+        return None
+
+
+def getOSMRelationID(poi_name: str) -> Union[float, None]:
+    """Get the relation id of a place of interest globally
+
+    Args:
+        poi_name (str): the name of the place of interest,
+            e.g., "Arizona State University"
+            e.g., "Tempe, Arizona, USA"
+            e.g., "Arizona, USA"
+
+    Returns:
+        Union[float, None]: the relation id of the place of interest, if not found, return None
+
+    Example:
+        >>> import osm2gmns as og
+        >>> rel = og.getOSMRelationID("Arizona State University")
+        >>> rel
+            Info: Found relation id 3444656 from web
+            Info: location of the place of interest:
+            {
+                "place_id": 318528634,
+                "licence": "Data \u00a9 OpenStreetMap contributors, ODbL 1.0. http://osm.org/copyright",
+                "osm_type": "relation",
+                "osm_id": 3444656,
+                "lat": "33.4213174",
+                "lon": "-111.93316305413154",
+                "class": "amenity",
+                "type": "university",
+                "place_rank": 30,
+                "importance": 0.5547365758311374,
+                "addresstype": "amenity",
+                "name": "Arizona State University",
+                "display_name": "Arizona State University, 1151, South Forest Avenue, Tempe Junction, Tempe, Maricopa County, Arizona, 85281, United States",
+                "boundingbox": [
+                    "33.4102062",
+                    "33.4329786",
+                    "-111.9411651",
+                    "-111.9092447"
+                ]
+            }
+        3444656
+    """
+    rel = OSMRelationIDFinder(poi_name)
     return rel.rel_id
```

### Comparing `osm2gmns-0.7.5/osm2gmns/io/downloader.py` & `osm2gmns-0.7.6/osm2gmns/io/downloader.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-#!/usr/bin/env python
-# Eclipse SUMO, Simulation of Urban MObility; see https://eclipse.org/sumo
-# Copyright (C) 2009-2020 German Aerospace Center (DLR) and others.
-# This program and the accompanying materials are made available under the
-# terms of the Eclipse Public License 2.0 which is available at
-# https://www.eclipse.org/legal/epl-2.0/
-# This Source Code may also be made available under the following Secondary
-# Licenses when the conditions for such availability set forth in the Eclipse
-# Public License 2.0 are satisfied: GNU General Public License, version 2
-# or later which is available at
-# https://www.gnu.org/licenses/old-licenses/gpl-2.0-standalone.html
-# SPDX-License-Identifier: EPL-2.0 OR GPL-2.0-or-later
-
-# @file    osmGet.py
-# @author  Daniel Krajzewicz
-# @author  Jakob Erdmann
-# @author  Michael Behrisch
-# @date    2009-08-01
-
-
-import os
-import http.client as httplib
-import urllib.parse as urlparse
-import base64
-
-
-
-_url = "www.overpass-api.de/api/interpreter"
-# alternatives: overpass.kumi.systems/api/interpreter, sumo.dlr.de/osm/api/interpreter
-
-
-def _readCompressed(conn, urlpath, query, filename):
-    conn.request("POST", "/" + urlpath, """
-    <osm-script timeout="240" element-limit="1073741824">
-    <union>
-       %s
-       <recurse type="node-relation" into="rels"/>
-       <recurse type="node-way"/>
-       <recurse type="way-relation"/>
-    </union>
-    <union>
-       <item/>
-       <recurse type="way-node"/>
-    </union>
-    <print mode="body"/>
-    </osm-script>""" % query)
-    response = conn.getresponse()
-    # print(response.status, response.reason)
-    if response.status == 200:
-        print('valid reponses got from API server.')
-        print('receving data...')
-        out = open(filename, "wb")
-        out.write(response.read())
-        out.close()
-        print(f'map data has been written to {filename}')
-
-
-def downloadOSMData(area_id, output_filename='map.osm', url=_url):
-    """
-    Download OpenStreetMap data via overpass API
-
-    Parameters
-    ----------
-    area_id: int
-        relation_id of the area of interest
-    output_filename: int
-        full path where the downloaded network will be stored
-    url: int
-        OpenStreetMap API url
-
-    Returns
-    -------
-    None
-    """
-
-    file_name, file_extension = os.path.splitext(output_filename)
-    if not file_extension:
-        print(f'WARNING: no file extension in output_filename {output_filename}, output_filename is changed to {file_name}.osm')
-        output_filename = f'{file_name}.osm'
-    elif file_extension not in ['.osm', '.xml']:
-        print(f'WARNING:  the file extension in output_filename {output_filename} is not supported, output_filename is changed to {file_name}.osm')
-        output_filename = f'{file_name}.osm'
-
-    if "http" in url:
-        url = urlparse.urlparse(url)
-    else:
-        url = urlparse.urlparse("https://" + url)
-    if os.environ.get("https_proxy") is not None:
-        headers = {}
-        proxy_url = urlparse.urlparse(os.environ.get("https_proxy"))
-        if proxy_url.username and proxy_url.password:
-            auth = '%s:%s' % (proxy_url.username, proxy_url.password)
-            headers['Proxy-Authorization'] = 'Basic ' + base64.b64encode(auth)
-        conn = httplib.HTTPSConnection(proxy_url.hostname, proxy_url.port)
-        conn.set_tunnel(url.hostname, 443, headers)
-    else:
-        if url.scheme == "https":
-            conn = httplib.HTTPSConnection(url.hostname, url.port)
-        else:
-            conn = httplib.HTTPConnection(url.hostname, url.port)
-
-    if area_id < 3600000000:
-        area_id += 3600000000
-    _readCompressed(conn, url.path, '<area-query ref="%s"/>' % area_id, output_filename)
-
-    conn.close()
+#!/usr/bin/env python
+# Eclipse SUMO, Simulation of Urban MObility; see https://eclipse.org/sumo
+# Copyright (C) 2009-2020 German Aerospace Center (DLR) and others.
+# This program and the accompanying materials are made available under the
+# terms of the Eclipse Public License 2.0 which is available at
+# https://www.eclipse.org/legal/epl-2.0/
+# This Source Code may also be made available under the following Secondary
+# Licenses when the conditions for such availability set forth in the Eclipse
+# Public License 2.0 are satisfied: GNU General Public License, version 2
+# or later which is available at
+# https://www.gnu.org/licenses/old-licenses/gpl-2.0-standalone.html
+# SPDX-License-Identifier: EPL-2.0 OR GPL-2.0-or-later
+
+# @file    osmGet.py
+# @author  Daniel Krajzewicz
+# @author  Jakob Erdmann
+# @author  Michael Behrisch
+# @date    2009-08-01
+
+
+import os
+import http.client as httplib
+import urllib.parse as urlparse
+import base64
+
+
+
+_url = "www.overpass-api.de/api/interpreter"
+# alternatives: overpass.kumi.systems/api/interpreter, sumo.dlr.de/osm/api/interpreter
+
+
+def _readCompressed(conn, urlpath, query, filename):
+    conn.request("POST", "/" + urlpath, """
+    <osm-script timeout="240" element-limit="1073741824">
+    <union>
+       %s
+       <recurse type="node-relation" into="rels"/>
+       <recurse type="node-way"/>
+       <recurse type="way-relation"/>
+    </union>
+    <union>
+       <item/>
+       <recurse type="way-node"/>
+    </union>
+    <print mode="body"/>
+    </osm-script>""" % query)
+    response = conn.getresponse()
+    # print(response.status, response.reason)
+    if response.status == 200:
+        print('valid reponses got from API server.')
+        print('receving data...')
+        out = open(filename, "wb")
+        out.write(response.read())
+        out.close()
+        print(f'map data has been written to {filename}')
+
+
+def downloadOSMData(area_id, output_filename='map.osm', url=_url):
+    """
+    Download OpenStreetMap data via overpass API
+
+    Parameters
+    ----------
+    area_id: int
+        relation_id of the area of interest
+    output_filename: int
+        full path where the downloaded network will be stored
+    url: int
+        OpenStreetMap API url
+
+    Returns
+    -------
+    None
+    """
+
+    file_name, file_extension = os.path.splitext(output_filename)
+    if not file_extension:
+        print(f'WARNING: no file extension in output_filename {output_filename}, output_filename is changed to {file_name}.osm')
+        output_filename = f'{file_name}.osm'
+    elif file_extension not in ['.osm', '.xml']:
+        print(f'WARNING:  the file extension in output_filename {output_filename} is not supported, output_filename is changed to {file_name}.osm')
+        output_filename = f'{file_name}.osm'
+
+    if "http" in url:
+        url = urlparse.urlparse(url)
+    else:
+        url = urlparse.urlparse("https://" + url)
+    if os.environ.get("https_proxy") is not None:
+        headers = {}
+        proxy_url = urlparse.urlparse(os.environ.get("https_proxy"))
+        if proxy_url.username and proxy_url.password:
+            auth = '%s:%s' % (proxy_url.username, proxy_url.password)
+            headers['Proxy-Authorization'] = 'Basic ' + base64.b64encode(auth)
+        conn = httplib.HTTPSConnection(proxy_url.hostname, proxy_url.port)
+        conn.set_tunnel(url.hostname, 443, headers)
+    else:
+        if url.scheme == "https":
+            conn = httplib.HTTPSConnection(url.hostname, url.port)
+        else:
+            conn = httplib.HTTPConnection(url.hostname, url.port)
+
+    if area_id < 3600000000:
+        area_id += 3600000000
+    _readCompressed(conn, url.path, '<area-query ref="%s"/>' % area_id, output_filename)
+
+    conn.close()
```

### Comparing `osm2gmns-0.7.5/osm2gmns/io/load_from_csv.py` & `osm2gmns-0.7.6/osm2gmns/io/load_from_csv.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,579 +1,579 @@
-from osm2gmns.networkclass.macronet import Node, Link, Movement, Segment, POI, Network
-from osm2gmns.movement.util_mvmt import getMovementDescription, getMovementGeometry
-from osm2gmns.utils.util_coord import from_latlon
-from osm2gmns.utils.util_geo import GeoTransformer
-import osm2gmns.settings as og_settings
-import os
-import csv
-import sys
-import numpy as np
-from shapely import wkt, geometry
-
-
-_node_required_fields = {'node_id', 'x_coord', 'y_coord'}
-_node_optional_fields = {'name', 'osm_node_id', 'osm_highway', 'zone_id', 'ctrl_type', 'node_type', 'activity_type', 'is_boundary', 'intersection_id', 'poi_id', 'notes'}
-_link_required_fields = {'link_id', 'from_node_id', 'to_node_id', 'lanes'}
-_link_optional_fields = {'name', 'osm_way_id', 'dir_flag', 'length', 'free_speed', 'capacity', 'link_type_name', 'link_type', 'geometry', 'allowed_uses', 'from_biway', 'is_link', 'VDF_fftt1', 'VDF_cap1'}
-_mvmt_required_fields = {'mvmt_id', 'node_id', 'ib_link_id', 'start_ib_lane', 'end_ib_lane', 'ob_link_id', 'start_ob_lane', 'end_ob_lane'}
-_mvmt_optional_fields = {'osm_node_id', 'name', 'lanes', 'ib_osm_node_id', 'ob_osm_node_id', 'type', 'penalty', 'capacity', 'ctrl_type', 'mvmt_txt_id', 'geometry', 'volume', 'free_speed', 'allowed_uses','generated_by_osm2gmns'}
-_segment_required_fields = {'segment_id', 'link_id', 'ref_node_id', 'start_lr', 'end_lr', 'l_lanes_added', 'r_lanes_added'}
-_segment_optional_fields = {'grade', 'capacity', 'free_speed', 'lanes', 'bike_facility', 'ped_facility', 'parking', 'allowed_uses', 'toll', 'jurisdiction', 'row_width', 'opt_comment'}
-
-
-def _loadNodes(network, node_filepath, coordinate_type, encoding):
-    if encoding is None:
-        fin = open(node_filepath, 'r')
-    else:
-        fin = open(node_filepath, 'r', encoding=encoding)
-    reader = csv.DictReader(fin)
-
-    fieldnames = reader.fieldnames.copy()
-    if '' in fieldnames:
-        print('WARNING: columns with an empty header are detected in the node file. these columns will be skipped')
-        fieldnames = [fieldname for fieldname in fieldnames if fieldname]
-    
-    fieldnames_set = set(fieldnames)
-    if len(fieldnames) > len(fieldnames_set):
-        print('WARNING: columns with duplicate header names are detected in the node file. please check')
-
-    for field in _node_required_fields:
-        if field not in fieldnames_set:
-            sys.exit(f'ERROR: required field ({field}) does not exist in the node file')
-    other_fields = list(fieldnames_set.difference(_node_required_fields.union(_node_optional_fields)))
-
-    max_node_id = network.max_node_id
-    max_intersection_id = network.max_intersection_id
-    node_id_list = []
-    node_coord_list = []
-    node_dict = {}
-    for node_info in reader:
-        # required
-        node = Node(int(node_info['node_id']))
-        if node.node_id > max_node_id: max_node_id = node.node_id
-
-        x_coord, y_coord = float(node_info['x_coord']), float(node_info['y_coord'])
-        if coordinate_type == 'lonlat':
-            node.geometry = geometry.Point(round(x_coord, og_settings.lonlat_coord_precision), round(y_coord, og_settings.lonlat_coord_precision))
-            node_id_list.append(node.node_id)
-            node_coord_list.append((x_coord, y_coord))
-        elif coordinate_type == 'meter':
-            node.geometry_xy = geometry.Point(round(x_coord, og_settings.local_coord_precision), round(y_coord, og_settings.local_coord_precision))
-        elif coordinate_type == 'feet':
-            node.geometry_xy = geometry.Point(round(x_coord*0.3048, og_settings.local_coord_precision), round(y_coord*0.3048, og_settings.local_coord_precision))
-
-        # optional
-        name = node_info['name'] if 'name' in reader.fieldnames else None
-        if name: node.name = name
-        osm_node_id = node_info['osm_node_id'] if 'osm_node_id' in reader.fieldnames else None
-        if osm_node_id: node.osm_node_id = osm_node_id
-        osm_highway = node_info['osm_highway'] if 'osm_highway' in reader.fieldnames else None
-        if osm_highway: node.osm_highway = osm_highway
-        zone_id = node_info['zone_id'] if 'zone_id' in reader.fieldnames else None
-        if zone_id: node.zone_id = int(zone_id)
-
-        ctrl_type = node_info['ctrl_type'] if 'ctrl_type' in reader.fieldnames else None
-        if ctrl_type: node.ctrl_type = ctrl_type
-        node_type = node_info['node_type'] if 'node_type' in reader.fieldnames else None
-        if node_type: node.node_type = node_type
-        activity_type = node_info['activity_type'] if 'activity_type' in reader.fieldnames else None
-        if activity_type: node.activity_type = activity_type
-        is_boundary = node_info['is_boundary'] if 'is_boundary' in reader.fieldnames else None
-        if is_boundary: node.is_boundary = int(is_boundary)
-
-        intersection_id = node_info['intersection_id'] if 'intersection_id' in reader.fieldnames else None
-        if intersection_id:
-            node.intersection_id = int(intersection_id)
-            if node.intersection_id > max_intersection_id:
-                max_intersection_id = node.intersection_id
-
-        poi_id = node_info['poi_id'] if 'poi_id' in reader.fieldnames else None
-        if poi_id: node.poi_id = poi_id
-        notes = node_info['notes'] if 'notes' in reader.fieldnames else None
-        if notes: node.notes = notes
-
-        # others
-        for field in other_fields:
-            node.other_attrs[field] = node_info[field]
-
-        node_dict[node.node_id] = node
-    fin.close()
-
-    max_node_id += 1
-    max_intersection_id += 1
-
-    if coordinate_type == 'lonlat':
-        coord_array = np.array(node_coord_list)
-        central_lon = coord_array[:,0].mean()
-        central_lat = coord_array[:,1].mean()
-        northern = True if central_lat >= 0 else False
-
-        xs, ys = from_latlon(coord_array[:,0], coord_array[:,1], central_lon)
-        xs, ys = np.round(xs, og_settings.local_coord_precision), np.round(ys, og_settings.local_coord_precision)
-
-        for node_no, node_id in enumerate(node_id_list):
-            node = node_dict[node_id]
-            node.geometry_xy = geometry.Point((xs[node_no],ys[node_no]))
-
-        network.GT = GeoTransformer(central_lon, central_lat, northern)
-
-    network.node_dict = node_dict
-    network.max_node_id = max_node_id
-    network.max_intersection_id = max_intersection_id
-    network.node_other_attrs = other_fields
-
-
-def _loadLinks(network, link_filepath, coordinate_type, encoding):
-    if encoding is None:
-        fin = open(link_filepath, 'r')
-    else:
-        fin = open(link_filepath, 'r', encoding=encoding)
-    reader = csv.DictReader(fin)
-
-    fieldnames = reader.fieldnames.copy()
-    if '' in fieldnames:
-        print('WARNING: columns with an empty header are detected in the link file. these columns will be skipped')
-        fieldnames = [fieldname for fieldname in fieldnames if fieldname]
-    
-    fieldnames_set = set(fieldnames)
-    if len(fieldnames) > len(fieldnames_set):
-        print('WARNING: columns with duplicate header names are detected in the link file. please check')
-
-    for field in _link_required_fields:
-        if field not in fieldnames_set:
-            sys.exit(f'ERROR: required field ({field}) does not exist in the link file')
-    other_fields = list(fieldnames_set.difference(_link_required_fields.union(_link_optional_fields)))
-
-    node_dict = network.node_dict
-    GT = network.GT
-
-    max_link_id = network.max_link_id
-    link_dict = {}
-    for link_info in reader:
-        # required
-        link = Link(int(link_info['link_id']))
-        if link.link_id > max_link_id: max_link_id = link.link_id
-
-        from_node_id, to_node_id = int(link_info['from_node_id']), int(link_info['to_node_id'])
-        if from_node_id == to_node_id:
-            print(f'WARNING: from_node and to_node of link {link.link_id} are the same')
-            continue
-
-        try:
-            link.from_node = node_dict[from_node_id]
-        except KeyError:
-            print(f'WARNING: from_node {from_node_id} of link {link.link_id} does not exist in the node file')
-            continue
-        try:
-            link.to_node = node_dict[to_node_id]
-        except KeyError:
-            print(f'WARNING: to_node {to_node_id} of link {link.link_id} does not exist in the node file')
-            continue
-
-        lanes = link_info['lanes']
-        if lanes:
-            link.lanes = int(float(lanes))
-
-        # optional
-        name = link_info['name'] if 'name' in reader.fieldnames else None
-        if name: link.name = name
-        osm_way_id = link_info['osm_way_id'] if 'osm_way_id' in reader.fieldnames else None
-        if osm_way_id: link.osm_way_id = osm_way_id
-        dir_flag = link_info['dir_flag'] if 'dir_flag' in reader.fieldnames else None
-        if dir_flag: link.dir_flag = int(dir_flag)
-
-        free_speed = link_info['free_speed'] if 'free_speed' in reader.fieldnames else None
-        if free_speed: link.free_speed = float(free_speed)
-        capacity = link_info['capacity'] if 'capacity' in reader.fieldnames else None
-        if capacity: link.capacity = float(capacity)
-
-        link_type_name = link_info['link_type_name'] if 'link_type_name' in reader.fieldnames else None
-        if link_type_name: link.link_type_name = link_type_name
-        link_type = link_info['link_type'] if 'link_type' in reader.fieldnames else None
-        if link_type:
-            try:
-                link.link_type = int(link_type)
-            except ValueError:
-                print(f'WARNING: link_type {link_type} of link {link.link_id} is not an integer')
-
-        geometry_str = link_info['geometry'] if 'geometry' in reader.fieldnames else None
-        if geometry_str:
-            if coordinate_type == 'lonlat':
-                link.geometry = wkt.loads(geometry_str)
-                if not link.geometry.is_valid:
-                    print(f'WARNING: link {link.link_id} geometry is not a valid LineString')
-                    continue
-                link.geometry_xy = GT.geo_from_latlon(link.geometry)
-            elif coordinate_type == 'meter':        # todo
-                pass
-            elif coordinate_type == 'feet':         # todo
-                pass
-
-        allowed_uses = link_info['allowed_uses'] if 'allowed_uses' in reader.fieldnames else None
-        if allowed_uses: link.allowed_uses = allowed_uses.split(';')
-
-        from_biway = link_info['from_biway'] if 'from_biway' in reader.fieldnames else None
-        if from_biway:
-            if from_biway == '1':
-                link.from_bidirectional_way = True
-            elif from_biway == '0':
-                link.from_bidirectional_way = False
-
-        is_link = link_info['is_link'] if 'is_link' in reader.fieldnames else None
-        if is_link:
-            if is_link == '1':
-                link.is_link = True
-            elif is_link == '0':
-                link.is_link = False
-
-        VDF_fftt1 = link_info['VDF_fftt1'] if 'VDF_fftt1' in reader.fieldnames else None
-        if VDF_fftt1: link.VDF_fftt1 = float(VDF_fftt1)
-        VDF_cap1 = link_info['VDF_cap1'] if 'VDF_cap1' in reader.fieldnames else None
-        if VDF_cap1: link.VDF_cap1 = float(VDF_cap1)
-
-        # others
-        for field in other_fields:
-            link.other_attrs[field] = link_info[field]
-
-        link_dict[link.link_id] = link
-        link.from_node.outgoing_link_list.append(link)
-        link.to_node.incoming_link_list.append(link)
-
-    fin.close()
-    max_link_id += 1
-
-    network.max_link_id = max_link_id
-    network.link_dict = link_dict
-    network.link_other_attrs = other_fields
-
-
-
-def _loadSegments(network, segment_filepath, encoding):
-    if encoding is None:
-        fin = open(segment_filepath, 'r')
-    else:
-        fin = open(segment_filepath, 'r', encoding=encoding)
-    reader = csv.DictReader(fin)
-
-    for field in _segment_required_fields:
-        if field not in reader.fieldnames:
-            sys.exit(f'ERROR: required field ({field}) does not exist in the segment file')
-    other_fields = list(set(reader.fieldnames).difference(_segment_required_fields.union(_segment_optional_fields)))
-
-    node_dict = network.node_dict
-    link_dict = network.link_dict
-
-    max_segment_id = network.max_segment_id
-
-    for segment_info in reader:
-        # required
-        segment = Segment(int(segment_info['segment_id']))
-        if segment.segment_id > max_segment_id: max_segment_id = segment.segment_id
-
-        link_id = int(segment_info['link_id'])
-        try:
-            link = link_dict[link_id]
-        except KeyError:
-            print(f'WARNING: link {link_id} of segment {segment.segment_id} does not exist in the link file')
-            continue
-
-        if link.lanes is None:
-            print(f'WARNING: link {link_id} of segment {segment.segment_id} does not have lanes information')
-            continue
-
-        segment.link = link
-
-        ref_node_id = int(segment_info['ref_node_id'])
-        try:
-            ref_node = node_dict[ref_node_id]
-        except KeyError:
-            print(f'WARNING: ref_node {ref_node_id} of segment {segment.segment_id} does not exist in the node file')
-            continue
-
-        if ref_node is not link.from_node:
-            print(f'WARNING: osm2gmns only supports sgements with from_node_id of the corresponding link as the ref_node_id. segment {segment.segment_id} will be skipped')
-            continue
-
-        segment.ref_node = ref_node
-
-        segment.start_lr = float(segment_info['start_lr'])
-        segment.end_lr = float(segment_info['end_lr'])
-        segment.l_lanes_added = int(segment_info['l_lanes_added'])
-        segment.r_lanes_added = int(segment_info['r_lanes_added'])
-
-        # optional
-
-        # others
-        for field in other_fields:
-            segment.other_attrs[field] = segment_info[field]
-
-        link.segment_list.append(segment)
-
-    fin.close()
-    max_segment_id += 1
-
-    network.max_segment_id = max_segment_id
-    network.segment_other_attrs = other_fields
-
-
-def _loadMovements(network, movement_filepath, coordinate_type, encoding):
-    if encoding is None:
-        fin = open(movement_filepath, 'r')
-    else:
-        fin = open(movement_filepath, 'r', encoding=encoding)
-    reader = csv.DictReader(fin)
-
-    for field in _mvmt_required_fields:
-        if field not in reader.fieldnames:
-            sys.exit(f'ERROR: required field ({field}) does not exist in the movement file')
-    other_fields = list(set(reader.fieldnames).difference(_mvmt_required_fields.union(_mvmt_optional_fields)))
-
-    node_dict = network.node_dict
-    link_dict = network.link_dict
-    GT = network.GT
-
-    max_movement_id = network.max_movement_id
-
-    for movement_info in reader:
-        # required
-        movement = Movement(int(movement_info['mvmt_id']))
-        if movement.movement_id > max_movement_id: max_movement_id = movement.movement_id
-
-        node_id = int(movement_info['node_id'])
-        try:
-            node = node_dict[node_id]
-        except KeyError:
-            print(f'WARNING: node {node_id} of movement {movement.movement_id} does not exist in the node file')
-            continue
-        movement.node = node
-
-        ib_link_id = int(movement_info['ib_link_id'])
-        try:
-            ib_link = link_dict[ib_link_id]
-        except KeyError:
-            print(f'WARNING: ib_link {ib_link_id} of movement {movement.movement_id} does not exist in the link file')
-            continue
-
-        start_ib_lane = int(float(movement_info['start_ib_lane']))
-        end_ib_lane_str = movement_info['end_ib_lane']
-        end_ib_lane = int(float(end_ib_lane_str)) if end_ib_lane_str else start_ib_lane
-
-        ob_link_id = int(movement_info['ob_link_id'])
-        try:
-            ob_link = link_dict[ob_link_id]
-        except KeyError:
-            print(f'WARNING: ob_link {ob_link_id} of movement {movement.movement_id} does not exist in the link file')
-            continue
-
-        start_ob_lane = int(float(movement_info['start_ob_lane']))
-        end_ob_lane_str = movement_info['end_ob_lane']
-        end_ob_lane = int(float(end_ob_lane_str)) if end_ob_lane_str else start_ob_lane
-
-        movement.ib_link, movement.start_ib_lane, movement.end_ib_lane = ib_link, start_ib_lane, end_ib_lane
-        movement.ob_link, movement.start_ob_lane, movement.end_ob_lane = ob_link, start_ob_lane, end_ob_lane
-
-        # optional
-        type_file = movement_info['type'] if 'type' in reader.fieldnames else None
-        mvmt_txt_id_file = movement_info['mvmt_txt_id'] if 'mvmt_txt_id' in reader.fieldnames else None
-        if type_file and mvmt_txt_id_file:
-            movement.type, movement.mvmt_txt_id = type_file, mvmt_txt_id_file
-        else:
-            mvmt_txt_id, mvmt_type = getMovementDescription(ib_link, ob_link)
-            movement.type = type_file if type_file else mvmt_type
-            movement.mvmt_txt_id = mvmt_txt_id_file if mvmt_txt_id_file else mvmt_txt_id
-
-        penalty = movement_info['penalty'] if 'penalty' in reader.fieldnames else None
-        if penalty: movement.penalty = float(penalty)
-        capacity = movement_info['capacity'] if 'capacity' in reader.fieldnames else None
-        if capacity: movement.capacity = float(capacity)
-        ctrl_type = movement_info['ctrl_type'] if 'ctrl_type' in reader.fieldnames else None
-        if ctrl_type: movement.ctrl_type = ctrl_type
-        volume = movement_info['volume'] if 'volume' in reader.fieldnames else None
-        if volume: movement.volume = float(volume)
-        free_speed = movement_info['free_speed'] if 'free_speed' in reader.fieldnames else None
-        if free_speed: movement.free_speed = float(free_speed)
-        allowed_uses = movement_info['allowed_uses'] if 'allowed_uses' in reader.fieldnames else None
-        if allowed_uses: movement.allowed_uses = allowed_uses.split(';')
-        generated_by_osm2gmns = movement_info['generated_by_osm2gmns'] if 'generated_by_osm2gmns' in reader.fieldnames else None
-        if generated_by_osm2gmns:
-            if generated_by_osm2gmns == '1':
-                movement.generated_by_osm2gmns = True
-            elif generated_by_osm2gmns == '0':
-                movement.generated_by_osm2gmns = False
-
-        geometry_str = movement_info['geometry'] if 'geometry' in reader.fieldnames else None
-        if geometry_str:
-            if coordinate_type == 'lonlat':
-                movement.geometry = wkt.loads(geometry_str)
-                movement.geometry_xy = GT.geo_from_latlon(movement.geometry)
-            elif coordinate_type == 'meter':        # todo
-                pass
-            elif coordinate_type == 'feet':         # todo
-                pass
-        else:
-            if coordinate_type == 'lonlat':
-                movement.geometry_xy = getMovementGeometry(ib_link, ob_link)
-                movement.geometry = GT.geo_to_latlon(movement.geometry_xy)
-            elif coordinate_type == 'meter':        # todo
-                pass
-            elif coordinate_type == 'feet':         # todo
-                pass
-
-        # others
-        for field in other_fields:
-            movement.other_attrs[field] = movement_info[field]
-
-        network.user_input_movement_list.append(movement)
-
-    fin.close()
-    max_movement_id += 1
-
-    network.max_movement_id = max_movement_id
-    network.movement_other_attrs = other_fields
-
-
-def _loadGeometries(network, geometry_filepath, encoding):
-    pass
-
-
-def _loadPOIs(network, poi_filepath, encoding):
-    if encoding is None:
-        fin = open(poi_filepath, 'r')
-    else:
-        fin = open(poi_filepath, 'r', encoding=encoding)
-    reader = csv.DictReader(fin)
-
-    max_poi_id = network.max_poi_id
-    GT = network.GT
-
-    POI_list = []
-    for poi_info in reader:
-        poi = POI()
-        name = poi_info['name']
-        if name: poi.name = name
-        poi.poi_id = int(poi_info['poi_id'])
-        if poi.poi_id > max_poi_id: max_poi_id = poi.poi_id
-        osm_way_id = poi_info['osm_way_id']
-        if osm_way_id: poi.osm_way_id = osm_way_id
-        osm_relation_id = poi_info['osm_relation_id']
-        if osm_relation_id: poi.osm_relation_id = osm_relation_id
-        building = poi_info['building']
-        if building: poi.building = building
-        amenity = poi_info['amenity']
-        if amenity: poi.amenity = amenity
-        leisure = poi_info['leisure']
-        if leisure: poi.leisure = leisure
-        way = poi_info['way']
-        if way: poi.way = way
-
-        poi.geometry = wkt.loads(poi_info['geometry'])
-        lon, lat = poi.geometry.centroid.x, poi.geometry.centroid.y
-        poi.centroid = geometry.Point((round(lon,og_settings.lonlat_coord_precision),round(lat,og_settings.lonlat_coord_precision)))
-
-        poi.geometry_xy = GT.geo_from_latlon(poi.geometry)
-        x, y = poi.geometry_xy.centroid.x, poi.geometry_xy.centroid.y
-        poi.centroid_xy = geometry.Point((round(x,og_settings.local_coord_precision),round(y,og_settings.local_coord_precision)))
-
-        POI_list.append(poi)
-
-    fin.close()
-    max_poi_id += 1
-
-    network.max_poi_id = max_poi_id
-
-
-def loadNetFromCSV(folder='', node_file=None, link_file=None, movement_file=None,
-                   segment_file=None, geometry_file=None, POI_file=None,
-                   coordinate_type='lonlat', enconding=None):
-    """
-    Load a network from csv files in GMNS format
-
-    Parameters
-    ----------
-    folder: str
-        the folder where network files are stored
-    node_file: str
-        filename of the node file. required
-    link_file: str
-        filename of the link file. required
-    movement_file: str, None
-        filename of the movement file. optional
-    segment_file: str, None
-        filename of the segment file. optional
-    geometry_file: str, None
-        filename of the geometry file. optional
-    POI_file: str, None
-        filename of the POI file. optional
-    coordinate_type: str
-        the coordinate system used by the network to be loaded. can be lonlat, meter, feet
-    enconding: str, None
-        the encoding used by the network files. if None, osm2gmns will use the default encoding of the local operating system
-
-    Returns
-    -------
-    network: Network
-        an osm2gmns Network object
-
-    """
-
-    if node_file is None:
-        sys.exit('ERROR: node_file is not specified')
-    node_filepath = os.path.join(folder, node_file)
-    if not os.path.isfile(node_filepath):
-        sys.exit(f'ERROR: cannot open node_file {node_filepath}')
-
-    if link_file is None:
-        sys.exit('ERROR: link_file is not specified')
-    link_filepath = os.path.join(folder, link_file)
-    if not os.path.isfile(link_filepath):
-        sys.exit(f'ERROR: cannot open link_file {link_filepath}')
-
-    if movement_file is not None:
-        movement_filepath = os.path.join(folder, movement_file)
-        if not os.path.isfile(movement_filepath):
-            sys.exit(f'ERROR: cannot open movement_file {movement_filepath}')
-    else:
-        movement_filepath = None
-
-    if segment_file is not None:
-        segment_filepath = os.path.join(folder, segment_file)
-        if not os.path.isfile(segment_filepath):
-            sys.exit(f'ERROR: cannot open segment_file {segment_filepath}')
-    else:
-        segment_filepath = None
-
-    if geometry_file is not None:
-        geometry_filepath = os.path.join(folder, geometry_file)
-        if not os.path.isfile(geometry_filepath):
-            sys.exit(f'ERROR: cannot open geometry_file {geometry_filepath}')
-    else:
-        geometry_filepath = None
-
-    if POI_file is not None:
-        POI_filepath = os.path.join(folder, POI_file)
-        if not os.path.isfile(POI_filepath):
-            sys.exit(f'ERROR: cannot open POI_file {POI_filepath}')
-    else:
-        POI_filepath = None
-
-    network = Network()
-
-    if og_settings.verbose:
-        print('Loading Network From CSV Files')
-
-    _loadNodes(network, node_filepath, coordinate_type, enconding)
-
-    _loadLinks(network, link_filepath, coordinate_type, enconding)
-
-    if segment_file is not None:
-        _loadSegments(network, segment_filepath, enconding)
-
-    if movement_file is not None:
-        _loadMovements(network, movement_filepath, coordinate_type, enconding)
-
-    if geometry_file is not None:
-        _loadGeometries(network, geometry_filepath, enconding)
-
-    if POI_file is not None:
-        _loadPOIs(network, POI_filepath, enconding)
-
+from osm2gmns.networkclass.macronet import Node, Link, Movement, Segment, POI, Network
+from osm2gmns.movement.util_mvmt import getMovementDescription, getMovementGeometry
+from osm2gmns.utils.util_coord import from_latlon
+from osm2gmns.utils.util_geo import GeoTransformer
+import osm2gmns.settings as og_settings
+import os
+import csv
+import sys
+import numpy as np
+from shapely import wkt, geometry
+
+
+_node_required_fields = {'node_id', 'x_coord', 'y_coord'}
+_node_optional_fields = {'name', 'osm_node_id', 'osm_highway', 'zone_id', 'ctrl_type', 'node_type', 'activity_type', 'is_boundary', 'intersection_id', 'poi_id', 'notes'}
+_link_required_fields = {'link_id', 'from_node_id', 'to_node_id', 'lanes'}
+_link_optional_fields = {'name', 'osm_way_id', 'dir_flag', 'length', 'free_speed', 'capacity', 'link_type_name', 'link_type', 'geometry', 'allowed_uses', 'from_biway', 'is_link', 'VDF_fftt1', 'VDF_cap1'}
+_mvmt_required_fields = {'mvmt_id', 'node_id', 'ib_link_id', 'start_ib_lane', 'end_ib_lane', 'ob_link_id', 'start_ob_lane', 'end_ob_lane'}
+_mvmt_optional_fields = {'osm_node_id', 'name', 'lanes', 'ib_osm_node_id', 'ob_osm_node_id', 'type', 'penalty', 'capacity', 'ctrl_type', 'mvmt_txt_id', 'geometry', 'volume', 'free_speed', 'allowed_uses','generated_by_osm2gmns'}
+_segment_required_fields = {'segment_id', 'link_id', 'ref_node_id', 'start_lr', 'end_lr', 'l_lanes_added', 'r_lanes_added'}
+_segment_optional_fields = {'grade', 'capacity', 'free_speed', 'lanes', 'bike_facility', 'ped_facility', 'parking', 'allowed_uses', 'toll', 'jurisdiction', 'row_width', 'opt_comment'}
+
+
+def _loadNodes(network, node_filepath, coordinate_type, encoding):
+    if encoding is None:
+        fin = open(node_filepath, 'r')
+    else:
+        fin = open(node_filepath, 'r', encoding=encoding)
+    reader = csv.DictReader(fin)
+
+    fieldnames = reader.fieldnames.copy()
+    if '' in fieldnames:
+        print('WARNING: columns with an empty header are detected in the node file. these columns will be skipped')
+        fieldnames = [fieldname for fieldname in fieldnames if fieldname]
+    
+    fieldnames_set = set(fieldnames)
+    if len(fieldnames) > len(fieldnames_set):
+        print('WARNING: columns with duplicate header names are detected in the node file. please check')
+
+    for field in _node_required_fields:
+        if field not in fieldnames_set:
+            sys.exit(f'ERROR: required field ({field}) does not exist in the node file')
+    other_fields = list(fieldnames_set.difference(_node_required_fields.union(_node_optional_fields)))
+
+    max_node_id = network.max_node_id
+    max_intersection_id = network.max_intersection_id
+    node_id_list = []
+    node_coord_list = []
+    node_dict = {}
+    for node_info in reader:
+        # required
+        node = Node(int(node_info['node_id']))
+        if node.node_id > max_node_id: max_node_id = node.node_id
+
+        x_coord, y_coord = float(node_info['x_coord']), float(node_info['y_coord'])
+        if coordinate_type == 'lonlat':
+            node.geometry = geometry.Point(round(x_coord, og_settings.lonlat_coord_precision), round(y_coord, og_settings.lonlat_coord_precision))
+            node_id_list.append(node.node_id)
+            node_coord_list.append((x_coord, y_coord))
+        elif coordinate_type == 'meter':
+            node.geometry_xy = geometry.Point(round(x_coord, og_settings.local_coord_precision), round(y_coord, og_settings.local_coord_precision))
+        elif coordinate_type == 'feet':
+            node.geometry_xy = geometry.Point(round(x_coord*0.3048, og_settings.local_coord_precision), round(y_coord*0.3048, og_settings.local_coord_precision))
+
+        # optional
+        name = node_info['name'] if 'name' in reader.fieldnames else None
+        if name: node.name = name
+        osm_node_id = node_info['osm_node_id'] if 'osm_node_id' in reader.fieldnames else None
+        if osm_node_id: node.osm_node_id = osm_node_id
+        osm_highway = node_info['osm_highway'] if 'osm_highway' in reader.fieldnames else None
+        if osm_highway: node.osm_highway = osm_highway
+        zone_id = node_info['zone_id'] if 'zone_id' in reader.fieldnames else None
+        if zone_id: node.zone_id = int(zone_id)
+
+        ctrl_type = node_info['ctrl_type'] if 'ctrl_type' in reader.fieldnames else None
+        if ctrl_type: node.ctrl_type = ctrl_type
+        node_type = node_info['node_type'] if 'node_type' in reader.fieldnames else None
+        if node_type: node.node_type = node_type
+        activity_type = node_info['activity_type'] if 'activity_type' in reader.fieldnames else None
+        if activity_type: node.activity_type = activity_type
+        is_boundary = node_info['is_boundary'] if 'is_boundary' in reader.fieldnames else None
+        if is_boundary: node.is_boundary = int(is_boundary)
+
+        intersection_id = node_info['intersection_id'] if 'intersection_id' in reader.fieldnames else None
+        if intersection_id:
+            node.intersection_id = int(intersection_id)
+            if node.intersection_id > max_intersection_id:
+                max_intersection_id = node.intersection_id
+
+        poi_id = node_info['poi_id'] if 'poi_id' in reader.fieldnames else None
+        if poi_id: node.poi_id = poi_id
+        notes = node_info['notes'] if 'notes' in reader.fieldnames else None
+        if notes: node.notes = notes
+
+        # others
+        for field in other_fields:
+            node.other_attrs[field] = node_info[field]
+
+        node_dict[node.node_id] = node
+    fin.close()
+
+    max_node_id += 1
+    max_intersection_id += 1
+
+    if coordinate_type == 'lonlat':
+        coord_array = np.array(node_coord_list)
+        central_lon = coord_array[:,0].mean()
+        central_lat = coord_array[:,1].mean()
+        northern = True if central_lat >= 0 else False
+
+        xs, ys = from_latlon(coord_array[:,0], coord_array[:,1], central_lon)
+        xs, ys = np.round(xs, og_settings.local_coord_precision), np.round(ys, og_settings.local_coord_precision)
+
+        for node_no, node_id in enumerate(node_id_list):
+            node = node_dict[node_id]
+            node.geometry_xy = geometry.Point((xs[node_no],ys[node_no]))
+
+        network.GT = GeoTransformer(central_lon, central_lat, northern)
+
+    network.node_dict = node_dict
+    network.max_node_id = max_node_id
+    network.max_intersection_id = max_intersection_id
+    network.node_other_attrs = other_fields
+
+
+def _loadLinks(network, link_filepath, coordinate_type, encoding):
+    if encoding is None:
+        fin = open(link_filepath, 'r')
+    else:
+        fin = open(link_filepath, 'r', encoding=encoding)
+    reader = csv.DictReader(fin)
+
+    fieldnames = reader.fieldnames.copy()
+    if '' in fieldnames:
+        print('WARNING: columns with an empty header are detected in the link file. these columns will be skipped')
+        fieldnames = [fieldname for fieldname in fieldnames if fieldname]
+    
+    fieldnames_set = set(fieldnames)
+    if len(fieldnames) > len(fieldnames_set):
+        print('WARNING: columns with duplicate header names are detected in the link file. please check')
+
+    for field in _link_required_fields:
+        if field not in fieldnames_set:
+            sys.exit(f'ERROR: required field ({field}) does not exist in the link file')
+    other_fields = list(fieldnames_set.difference(_link_required_fields.union(_link_optional_fields)))
+
+    node_dict = network.node_dict
+    GT = network.GT
+
+    max_link_id = network.max_link_id
+    link_dict = {}
+    for link_info in reader:
+        # required
+        link = Link(int(link_info['link_id']))
+        if link.link_id > max_link_id: max_link_id = link.link_id
+
+        from_node_id, to_node_id = int(link_info['from_node_id']), int(link_info['to_node_id'])
+        if from_node_id == to_node_id:
+            print(f'WARNING: from_node and to_node of link {link.link_id} are the same')
+            continue
+
+        try:
+            link.from_node = node_dict[from_node_id]
+        except KeyError:
+            print(f'WARNING: from_node {from_node_id} of link {link.link_id} does not exist in the node file')
+            continue
+        try:
+            link.to_node = node_dict[to_node_id]
+        except KeyError:
+            print(f'WARNING: to_node {to_node_id} of link {link.link_id} does not exist in the node file')
+            continue
+
+        lanes = link_info['lanes']
+        if lanes:
+            link.lanes = int(float(lanes))
+
+        # optional
+        name = link_info['name'] if 'name' in reader.fieldnames else None
+        if name: link.name = name
+        osm_way_id = link_info['osm_way_id'] if 'osm_way_id' in reader.fieldnames else None
+        if osm_way_id: link.osm_way_id = osm_way_id
+        dir_flag = link_info['dir_flag'] if 'dir_flag' in reader.fieldnames else None
+        if dir_flag: link.dir_flag = int(dir_flag)
+
+        free_speed = link_info['free_speed'] if 'free_speed' in reader.fieldnames else None
+        if free_speed: link.free_speed = float(free_speed)
+        capacity = link_info['capacity'] if 'capacity' in reader.fieldnames else None
+        if capacity: link.capacity = float(capacity)
+
+        link_type_name = link_info['link_type_name'] if 'link_type_name' in reader.fieldnames else None
+        if link_type_name: link.link_type_name = link_type_name
+        link_type = link_info['link_type'] if 'link_type' in reader.fieldnames else None
+        if link_type:
+            try:
+                link.link_type = int(link_type)
+            except ValueError:
+                print(f'WARNING: link_type {link_type} of link {link.link_id} is not an integer')
+
+        geometry_str = link_info['geometry'] if 'geometry' in reader.fieldnames else None
+        if geometry_str:
+            if coordinate_type == 'lonlat':
+                link.geometry = wkt.loads(geometry_str)
+                if not link.geometry.is_valid:
+                    print(f'WARNING: link {link.link_id} geometry is not a valid LineString')
+                    continue
+                link.geometry_xy = GT.geo_from_latlon(link.geometry)
+            elif coordinate_type == 'meter':        # todo
+                pass
+            elif coordinate_type == 'feet':         # todo
+                pass
+
+        allowed_uses = link_info['allowed_uses'] if 'allowed_uses' in reader.fieldnames else None
+        if allowed_uses: link.allowed_uses = allowed_uses.split(';')
+
+        from_biway = link_info['from_biway'] if 'from_biway' in reader.fieldnames else None
+        if from_biway:
+            if from_biway == '1':
+                link.from_bidirectional_way = True
+            elif from_biway == '0':
+                link.from_bidirectional_way = False
+
+        is_link = link_info['is_link'] if 'is_link' in reader.fieldnames else None
+        if is_link:
+            if is_link == '1':
+                link.is_link = True
+            elif is_link == '0':
+                link.is_link = False
+
+        VDF_fftt1 = link_info['VDF_fftt1'] if 'VDF_fftt1' in reader.fieldnames else None
+        if VDF_fftt1: link.VDF_fftt1 = float(VDF_fftt1)
+        VDF_cap1 = link_info['VDF_cap1'] if 'VDF_cap1' in reader.fieldnames else None
+        if VDF_cap1: link.VDF_cap1 = float(VDF_cap1)
+
+        # others
+        for field in other_fields:
+            link.other_attrs[field] = link_info[field]
+
+        link_dict[link.link_id] = link
+        link.from_node.outgoing_link_list.append(link)
+        link.to_node.incoming_link_list.append(link)
+
+    fin.close()
+    max_link_id += 1
+
+    network.max_link_id = max_link_id
+    network.link_dict = link_dict
+    network.link_other_attrs = other_fields
+
+
+
+def _loadSegments(network, segment_filepath, encoding):
+    if encoding is None:
+        fin = open(segment_filepath, 'r')
+    else:
+        fin = open(segment_filepath, 'r', encoding=encoding)
+    reader = csv.DictReader(fin)
+
+    for field in _segment_required_fields:
+        if field not in reader.fieldnames:
+            sys.exit(f'ERROR: required field ({field}) does not exist in the segment file')
+    other_fields = list(set(reader.fieldnames).difference(_segment_required_fields.union(_segment_optional_fields)))
+
+    node_dict = network.node_dict
+    link_dict = network.link_dict
+
+    max_segment_id = network.max_segment_id
+
+    for segment_info in reader:
+        # required
+        segment = Segment(int(segment_info['segment_id']))
+        if segment.segment_id > max_segment_id: max_segment_id = segment.segment_id
+
+        link_id = int(segment_info['link_id'])
+        try:
+            link = link_dict[link_id]
+        except KeyError:
+            print(f'WARNING: link {link_id} of segment {segment.segment_id} does not exist in the link file')
+            continue
+
+        if link.lanes is None:
+            print(f'WARNING: link {link_id} of segment {segment.segment_id} does not have lanes information')
+            continue
+
+        segment.link = link
+
+        ref_node_id = int(segment_info['ref_node_id'])
+        try:
+            ref_node = node_dict[ref_node_id]
+        except KeyError:
+            print(f'WARNING: ref_node {ref_node_id} of segment {segment.segment_id} does not exist in the node file')
+            continue
+
+        if ref_node is not link.from_node:
+            print(f'WARNING: osm2gmns only supports sgements with from_node_id of the corresponding link as the ref_node_id. segment {segment.segment_id} will be skipped')
+            continue
+
+        segment.ref_node = ref_node
+
+        segment.start_lr = float(segment_info['start_lr'])
+        segment.end_lr = float(segment_info['end_lr'])
+        segment.l_lanes_added = int(segment_info['l_lanes_added'])
+        segment.r_lanes_added = int(segment_info['r_lanes_added'])
+
+        # optional
+
+        # others
+        for field in other_fields:
+            segment.other_attrs[field] = segment_info[field]
+
+        link.segment_list.append(segment)
+
+    fin.close()
+    max_segment_id += 1
+
+    network.max_segment_id = max_segment_id
+    network.segment_other_attrs = other_fields
+
+
+def _loadMovements(network, movement_filepath, coordinate_type, encoding):
+    if encoding is None:
+        fin = open(movement_filepath, 'r')
+    else:
+        fin = open(movement_filepath, 'r', encoding=encoding)
+    reader = csv.DictReader(fin)
+
+    for field in _mvmt_required_fields:
+        if field not in reader.fieldnames:
+            sys.exit(f'ERROR: required field ({field}) does not exist in the movement file')
+    other_fields = list(set(reader.fieldnames).difference(_mvmt_required_fields.union(_mvmt_optional_fields)))
+
+    node_dict = network.node_dict
+    link_dict = network.link_dict
+    GT = network.GT
+
+    max_movement_id = network.max_movement_id
+
+    for movement_info in reader:
+        # required
+        movement = Movement(int(movement_info['mvmt_id']))
+        if movement.movement_id > max_movement_id: max_movement_id = movement.movement_id
+
+        node_id = int(movement_info['node_id'])
+        try:
+            node = node_dict[node_id]
+        except KeyError:
+            print(f'WARNING: node {node_id} of movement {movement.movement_id} does not exist in the node file')
+            continue
+        movement.node = node
+
+        ib_link_id = int(movement_info['ib_link_id'])
+        try:
+            ib_link = link_dict[ib_link_id]
+        except KeyError:
+            print(f'WARNING: ib_link {ib_link_id} of movement {movement.movement_id} does not exist in the link file')
+            continue
+
+        start_ib_lane = int(float(movement_info['start_ib_lane']))
+        end_ib_lane_str = movement_info['end_ib_lane']
+        end_ib_lane = int(float(end_ib_lane_str)) if end_ib_lane_str else start_ib_lane
+
+        ob_link_id = int(movement_info['ob_link_id'])
+        try:
+            ob_link = link_dict[ob_link_id]
+        except KeyError:
+            print(f'WARNING: ob_link {ob_link_id} of movement {movement.movement_id} does not exist in the link file')
+            continue
+
+        start_ob_lane = int(float(movement_info['start_ob_lane']))
+        end_ob_lane_str = movement_info['end_ob_lane']
+        end_ob_lane = int(float(end_ob_lane_str)) if end_ob_lane_str else start_ob_lane
+
+        movement.ib_link, movement.start_ib_lane, movement.end_ib_lane = ib_link, start_ib_lane, end_ib_lane
+        movement.ob_link, movement.start_ob_lane, movement.end_ob_lane = ob_link, start_ob_lane, end_ob_lane
+
+        # optional
+        type_file = movement_info['type'] if 'type' in reader.fieldnames else None
+        mvmt_txt_id_file = movement_info['mvmt_txt_id'] if 'mvmt_txt_id' in reader.fieldnames else None
+        if type_file and mvmt_txt_id_file:
+            movement.type, movement.mvmt_txt_id = type_file, mvmt_txt_id_file
+        else:
+            mvmt_txt_id, mvmt_type = getMovementDescription(ib_link, ob_link)
+            movement.type = type_file if type_file else mvmt_type
+            movement.mvmt_txt_id = mvmt_txt_id_file if mvmt_txt_id_file else mvmt_txt_id
+
+        penalty = movement_info['penalty'] if 'penalty' in reader.fieldnames else None
+        if penalty: movement.penalty = float(penalty)
+        capacity = movement_info['capacity'] if 'capacity' in reader.fieldnames else None
+        if capacity: movement.capacity = float(capacity)
+        ctrl_type = movement_info['ctrl_type'] if 'ctrl_type' in reader.fieldnames else None
+        if ctrl_type: movement.ctrl_type = ctrl_type
+        volume = movement_info['volume'] if 'volume' in reader.fieldnames else None
+        if volume: movement.volume = float(volume)
+        free_speed = movement_info['free_speed'] if 'free_speed' in reader.fieldnames else None
+        if free_speed: movement.free_speed = float(free_speed)
+        allowed_uses = movement_info['allowed_uses'] if 'allowed_uses' in reader.fieldnames else None
+        if allowed_uses: movement.allowed_uses = allowed_uses.split(';')
+        generated_by_osm2gmns = movement_info['generated_by_osm2gmns'] if 'generated_by_osm2gmns' in reader.fieldnames else None
+        if generated_by_osm2gmns:
+            if generated_by_osm2gmns == '1':
+                movement.generated_by_osm2gmns = True
+            elif generated_by_osm2gmns == '0':
+                movement.generated_by_osm2gmns = False
+
+        geometry_str = movement_info['geometry'] if 'geometry' in reader.fieldnames else None
+        if geometry_str:
+            if coordinate_type == 'lonlat':
+                movement.geometry = wkt.loads(geometry_str)
+                movement.geometry_xy = GT.geo_from_latlon(movement.geometry)
+            elif coordinate_type == 'meter':        # todo
+                pass
+            elif coordinate_type == 'feet':         # todo
+                pass
+        else:
+            if coordinate_type == 'lonlat':
+                movement.geometry_xy = getMovementGeometry(ib_link, ob_link)
+                movement.geometry = GT.geo_to_latlon(movement.geometry_xy)
+            elif coordinate_type == 'meter':        # todo
+                pass
+            elif coordinate_type == 'feet':         # todo
+                pass
+
+        # others
+        for field in other_fields:
+            movement.other_attrs[field] = movement_info[field]
+
+        network.user_input_movement_list.append(movement)
+
+    fin.close()
+    max_movement_id += 1
+
+    network.max_movement_id = max_movement_id
+    network.movement_other_attrs = other_fields
+
+
+def _loadGeometries(network, geometry_filepath, encoding):
+    pass
+
+
+def _loadPOIs(network, poi_filepath, encoding):
+    if encoding is None:
+        fin = open(poi_filepath, 'r')
+    else:
+        fin = open(poi_filepath, 'r', encoding=encoding)
+    reader = csv.DictReader(fin)
+
+    max_poi_id = network.max_poi_id
+    GT = network.GT
+
+    POI_list = []
+    for poi_info in reader:
+        poi = POI()
+        name = poi_info['name']
+        if name: poi.name = name
+        poi.poi_id = int(poi_info['poi_id'])
+        if poi.poi_id > max_poi_id: max_poi_id = poi.poi_id
+        osm_way_id = poi_info['osm_way_id']
+        if osm_way_id: poi.osm_way_id = osm_way_id
+        osm_relation_id = poi_info['osm_relation_id']
+        if osm_relation_id: poi.osm_relation_id = osm_relation_id
+        building = poi_info['building']
+        if building: poi.building = building
+        amenity = poi_info['amenity']
+        if amenity: poi.amenity = amenity
+        leisure = poi_info['leisure']
+        if leisure: poi.leisure = leisure
+        way = poi_info['way']
+        if way: poi.way = way
+
+        poi.geometry = wkt.loads(poi_info['geometry'])
+        lon, lat = poi.geometry.centroid.x, poi.geometry.centroid.y
+        poi.centroid = geometry.Point((round(lon,og_settings.lonlat_coord_precision),round(lat,og_settings.lonlat_coord_precision)))
+
+        poi.geometry_xy = GT.geo_from_latlon(poi.geometry)
+        x, y = poi.geometry_xy.centroid.x, poi.geometry_xy.centroid.y
+        poi.centroid_xy = geometry.Point((round(x,og_settings.local_coord_precision),round(y,og_settings.local_coord_precision)))
+
+        POI_list.append(poi)
+
+    fin.close()
+    max_poi_id += 1
+
+    network.max_poi_id = max_poi_id
+
+
+def loadNetFromCSV(folder='', node_file=None, link_file=None, movement_file=None,
+                   segment_file=None, geometry_file=None, POI_file=None,
+                   coordinate_type='lonlat', enconding=None):
+    """
+    Load a network from csv files in GMNS format
+
+    Parameters
+    ----------
+    folder: str
+        the folder where network files are stored
+    node_file: str
+        filename of the node file. required
+    link_file: str
+        filename of the link file. required
+    movement_file: str, None
+        filename of the movement file. optional
+    segment_file: str, None
+        filename of the segment file. optional
+    geometry_file: str, None
+        filename of the geometry file. optional
+    POI_file: str, None
+        filename of the POI file. optional
+    coordinate_type: str
+        the coordinate system used by the network to be loaded. can be lonlat, meter, feet
+    enconding: str, None
+        the encoding used by the network files. if None, osm2gmns will use the default encoding of the local operating system
+
+    Returns
+    -------
+    network: Network
+        an osm2gmns Network object
+
+    """
+
+    if node_file is None:
+        sys.exit('ERROR: node_file is not specified')
+    node_filepath = os.path.join(folder, node_file)
+    if not os.path.isfile(node_filepath):
+        sys.exit(f'ERROR: cannot open node_file {node_filepath}')
+
+    if link_file is None:
+        sys.exit('ERROR: link_file is not specified')
+    link_filepath = os.path.join(folder, link_file)
+    if not os.path.isfile(link_filepath):
+        sys.exit(f'ERROR: cannot open link_file {link_filepath}')
+
+    if movement_file is not None:
+        movement_filepath = os.path.join(folder, movement_file)
+        if not os.path.isfile(movement_filepath):
+            sys.exit(f'ERROR: cannot open movement_file {movement_filepath}')
+    else:
+        movement_filepath = None
+
+    if segment_file is not None:
+        segment_filepath = os.path.join(folder, segment_file)
+        if not os.path.isfile(segment_filepath):
+            sys.exit(f'ERROR: cannot open segment_file {segment_filepath}')
+    else:
+        segment_filepath = None
+
+    if geometry_file is not None:
+        geometry_filepath = os.path.join(folder, geometry_file)
+        if not os.path.isfile(geometry_filepath):
+            sys.exit(f'ERROR: cannot open geometry_file {geometry_filepath}')
+    else:
+        geometry_filepath = None
+
+    if POI_file is not None:
+        POI_filepath = os.path.join(folder, POI_file)
+        if not os.path.isfile(POI_filepath):
+            sys.exit(f'ERROR: cannot open POI_file {POI_filepath}')
+    else:
+        POI_filepath = None
+
+    network = Network()
+
+    if og_settings.verbose:
+        print('Loading Network From CSV Files')
+
+    _loadNodes(network, node_filepath, coordinate_type, enconding)
+
+    _loadLinks(network, link_filepath, coordinate_type, enconding)
+
+    if segment_file is not None:
+        _loadSegments(network, segment_filepath, enconding)
+
+    if movement_file is not None:
+        _loadMovements(network, movement_filepath, coordinate_type, enconding)
+
+    if geometry_file is not None:
+        _loadGeometries(network, geometry_filepath, enconding)
+
+    if POI_file is not None:
+        _loadPOIs(network, POI_filepath, enconding)
+
     return network
```

### Comparing `osm2gmns-0.7.5/osm2gmns/io/output_mrnet.py` & `osm2gmns-0.7.6/osm2gmns/io/output_mrnet.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,112 +1,112 @@
-from osm2gmns.io.util_io import getFileHandle
-import osm2gmns.settings as og_settings
-from shapely import wkt
-import os
-import csv
-
-
-def _outputMesoNodes(mesonet, mesonode_filepath, projection, encoding):
-    outfile = getFileHandle(mesonode_filepath, encoding)
-    writer = csv.writer(outfile)
-
-    writer.writerow(['node_id', 'zone_id', 'x_coord', 'y_coord', 'macro_node_id', 'macro_link_id', 'activity_type', 'is_boundary'])
-    for _, mesonode in mesonet.node_dict.items():
-        if projection:
-            x_coord = round(mesonode.geometry_xy.x, og_settings.local_coord_precision)
-            y_coord = round(mesonode.geometry_xy.y, og_settings.local_coord_precision)
-        else:
-            x_coord = round(mesonode.geometry.x, og_settings.lonlat_coord_precision)
-            y_coord = round(mesonode.geometry.y, og_settings.lonlat_coord_precision)
-
-        line = [mesonode.node_id, mesonode.zone_id, x_coord, y_coord, mesonode.macro_node_id, mesonode.macro_link_id,
-                mesonode.activity_type, mesonode.is_boundary]
-        writer.writerow(line)
-
-    outfile.close()
-
-
-def _outputMesoLinks(mesonet, mesolink_filepath, projection, encoding):
-    outfile = getFileHandle(mesolink_filepath, encoding)
-    writer = csv.writer(outfile)
-
-    writer.writerow(['link_id', 'from_node_id', 'to_node_id', 'dir_flag', 'length', 'lanes', 'capacity',
-                     'free_speed', 'link_type_name', 'link_type', 'geometry', 'macro_link_id', 'macro_node_id',
-                     'movement_id', 'mvmt_txt_id', 'ctrl_type', 'allowed_uses'])
-    for _, mesolink in mesonet.link_dict.items():
-        if projection:
-            geometry_ = wkt.dumps(mesolink.geometry_xy, rounding_precision=og_settings.local_coord_precision)
-        else:
-            geometry_ = wkt.dumps(mesolink.geometry, rounding_precision=og_settings.lonlat_coord_precision)
-
-        line = [mesolink.link_id, mesolink.from_node.node_id, mesolink.to_node.node_id, mesolink.dir_flag, mesolink.length,
-                mesolink.lanes, mesolink.capacity, mesolink.free_speed, mesolink.link_type_name,mesolink.link_type,
-                geometry_, mesolink.macro_link_id, mesolink.macro_node_id,  mesolink.movement_id, mesolink.mvmt_txt_id, mesolink.ctrl_type,
-                ';'.join(mesolink.allowed_uses)]
-        writer.writerow(line)
-
-    outfile.close()
-
-
-def _outputMicroNodes(micronet, micronode_filepath, projection, encoding):
-    outfile = getFileHandle(micronode_filepath, encoding)
-    writer = csv.writer(outfile)
-
-    writer.writerow(['node_id', 'zone_id', 'x_coord', 'y_coord', 'meso_link_id', 'lane_no', 'is_boundary'])
-    for _, micronode in micronet.node_dict.items():
-        if projection:
-            x_coord = round(micronode.geometry_xy.x, og_settings.local_coord_precision)
-            y_coord = round(micronode.geometry_xy.y, og_settings.local_coord_precision)
-        else:
-            x_coord = round(micronode.geometry.x, og_settings.lonlat_coord_precision)
-            y_coord = round(micronode.geometry.y, og_settings.lonlat_coord_precision)
-
-        line = [micronode.node_id, micronode.zone_id, x_coord, y_coord, micronode.mesolink.link_id, micronode.lane_no, micronode.is_boundary]
-        writer.writerow(line)
-
-    outfile.close()
-
-
-def _outputMicroLinks(micronet, microlink_filepath, projection, encoding):
-    outfile = getFileHandle(microlink_filepath, encoding)
-    writer = csv.writer(outfile)
-
-    writer.writerow(['link_id', 'from_node_id', 'to_node_id', 'dir_flag', 'length', 'lanes', 'capacity',
-                     'free_speed', 'link_type_name', 'link_type', 'geometry', 'macro_node_id', 'macro_link_id',
-                     'meso_link_id', 'cell_type', 'additional_cost', 'lane_no', 'mvmt_txt_id', 'ctrl_type', 'allowed_uses'])
-    for _, microlink in micronet.link_dict.items():
-        if projection:
-            geometry_ = wkt.dumps(microlink.geometry_xy, rounding_precision=og_settings.local_coord_precision)
-        else:
-            geometry_ = wkt.dumps(microlink.geometry, rounding_precision=og_settings.lonlat_coord_precision)
-
-        line = [microlink.link_id, microlink.from_node.node_id, microlink.to_node.node_id, microlink.dir_flag,
-                microlink.length, 1, microlink.mesolink.capacity, microlink.mesolink.free_speed,
-                microlink.mesolink.link_type_name, microlink.mesolink.link_type, geometry_,
-                microlink.mesolink.macro_node_id, microlink.mesolink.macro_link_id, microlink.mesolink.link_id,
-                microlink.cell_type, 0, microlink.lane_no, microlink.mvmt_txt_id, ';'.join(microlink.allowed_uses)]
-        writer.writerow(line)
-
-    outfile.close()
-
-
-
-def outputMesoNet(mesonet, output_folder, prefix, projection, encoding):
-    mesonet_folder = os.path.join(output_folder, 'mesonet')
-    if not os.path.isdir(mesonet_folder): os.mkdir(mesonet_folder)
-
-    mesonode_filepath = os.path.join(mesonet_folder, f'{prefix}node.csv')
-    _outputMesoNodes(mesonet, mesonode_filepath, projection, encoding)
-
-    mesolink_filepath = os.path.join(mesonet_folder, f'{prefix}link.csv')
-    _outputMesoLinks(mesonet, mesolink_filepath, projection, encoding)
-
-
-def outputMicroNet(micronet, output_folder, prefix, projection, encoding):
-    micronet_folder = os.path.join(output_folder, 'micronet')
-    if not os.path.isdir(micronet_folder): os.mkdir(micronet_folder)
-
-    micronode_filepath = os.path.join(micronet_folder, f'{prefix}node.csv')
-    _outputMicroNodes(micronet, micronode_filepath, projection, encoding)
-
-    microlink_filepath = os.path.join(micronet_folder, f'{prefix}link.csv')
-    _outputMicroLinks(micronet, microlink_filepath, projection, encoding)
+from osm2gmns.io.util_io import getFileHandle
+import osm2gmns.settings as og_settings
+from shapely import wkt
+import os
+import csv
+
+
+def _outputMesoNodes(mesonet, mesonode_filepath, projection, encoding):
+    outfile = getFileHandle(mesonode_filepath, encoding)
+    writer = csv.writer(outfile)
+
+    writer.writerow(['node_id', 'zone_id', 'x_coord', 'y_coord', 'macro_node_id', 'macro_link_id', 'activity_type', 'is_boundary'])
+    for _, mesonode in mesonet.node_dict.items():
+        if projection:
+            x_coord = round(mesonode.geometry_xy.x, og_settings.local_coord_precision)
+            y_coord = round(mesonode.geometry_xy.y, og_settings.local_coord_precision)
+        else:
+            x_coord = round(mesonode.geometry.x, og_settings.lonlat_coord_precision)
+            y_coord = round(mesonode.geometry.y, og_settings.lonlat_coord_precision)
+
+        line = [mesonode.node_id, mesonode.zone_id, x_coord, y_coord, mesonode.macro_node_id, mesonode.macro_link_id,
+                mesonode.activity_type, mesonode.is_boundary]
+        writer.writerow(line)
+
+    outfile.close()
+
+
+def _outputMesoLinks(mesonet, mesolink_filepath, projection, encoding):
+    outfile = getFileHandle(mesolink_filepath, encoding)
+    writer = csv.writer(outfile)
+
+    writer.writerow(['link_id', 'from_node_id', 'to_node_id', 'dir_flag', 'length', 'lanes', 'capacity',
+                     'free_speed', 'link_type_name', 'link_type', 'geometry', 'macro_link_id', 'macro_node_id',
+                     'movement_id', 'mvmt_txt_id', 'ctrl_type', 'allowed_uses'])
+    for _, mesolink in mesonet.link_dict.items():
+        if projection:
+            geometry_ = wkt.dumps(mesolink.geometry_xy, rounding_precision=og_settings.local_coord_precision)
+        else:
+            geometry_ = wkt.dumps(mesolink.geometry, rounding_precision=og_settings.lonlat_coord_precision)
+
+        line = [mesolink.link_id, mesolink.from_node.node_id, mesolink.to_node.node_id, mesolink.dir_flag, mesolink.length,
+                mesolink.lanes, mesolink.capacity, mesolink.free_speed, mesolink.link_type_name,mesolink.link_type,
+                geometry_, mesolink.macro_link_id, mesolink.macro_node_id,  mesolink.movement_id, mesolink.mvmt_txt_id, mesolink.ctrl_type,
+                ';'.join(mesolink.allowed_uses)]
+        writer.writerow(line)
+
+    outfile.close()
+
+
+def _outputMicroNodes(micronet, micronode_filepath, projection, encoding):
+    outfile = getFileHandle(micronode_filepath, encoding)
+    writer = csv.writer(outfile)
+
+    writer.writerow(['node_id', 'zone_id', 'x_coord', 'y_coord', 'meso_link_id', 'lane_no', 'is_boundary'])
+    for _, micronode in micronet.node_dict.items():
+        if projection:
+            x_coord = round(micronode.geometry_xy.x, og_settings.local_coord_precision)
+            y_coord = round(micronode.geometry_xy.y, og_settings.local_coord_precision)
+        else:
+            x_coord = round(micronode.geometry.x, og_settings.lonlat_coord_precision)
+            y_coord = round(micronode.geometry.y, og_settings.lonlat_coord_precision)
+
+        line = [micronode.node_id, micronode.zone_id, x_coord, y_coord, micronode.mesolink.link_id, micronode.lane_no, micronode.is_boundary]
+        writer.writerow(line)
+
+    outfile.close()
+
+
+def _outputMicroLinks(micronet, microlink_filepath, projection, encoding):
+    outfile = getFileHandle(microlink_filepath, encoding)
+    writer = csv.writer(outfile)
+
+    writer.writerow(['link_id', 'from_node_id', 'to_node_id', 'dir_flag', 'length', 'lanes', 'capacity',
+                     'free_speed', 'link_type_name', 'link_type', 'geometry', 'macro_node_id', 'macro_link_id',
+                     'meso_link_id', 'cell_type', 'additional_cost', 'lane_no', 'mvmt_txt_id', 'ctrl_type', 'allowed_uses'])
+    for _, microlink in micronet.link_dict.items():
+        if projection:
+            geometry_ = wkt.dumps(microlink.geometry_xy, rounding_precision=og_settings.local_coord_precision)
+        else:
+            geometry_ = wkt.dumps(microlink.geometry, rounding_precision=og_settings.lonlat_coord_precision)
+
+        line = [microlink.link_id, microlink.from_node.node_id, microlink.to_node.node_id, microlink.dir_flag,
+                microlink.length, 1, microlink.mesolink.capacity, microlink.mesolink.free_speed,
+                microlink.mesolink.link_type_name, microlink.mesolink.link_type, geometry_,
+                microlink.mesolink.macro_node_id, microlink.mesolink.macro_link_id, microlink.mesolink.link_id,
+                microlink.cell_type, 0, microlink.lane_no, microlink.mvmt_txt_id, ';'.join(microlink.allowed_uses)]
+        writer.writerow(line)
+
+    outfile.close()
+
+
+
+def outputMesoNet(mesonet, output_folder, prefix, projection, encoding):
+    mesonet_folder = os.path.join(output_folder, 'mesonet')
+    if not os.path.isdir(mesonet_folder): os.mkdir(mesonet_folder)
+
+    mesonode_filepath = os.path.join(mesonet_folder, f'{prefix}node.csv')
+    _outputMesoNodes(mesonet, mesonode_filepath, projection, encoding)
+
+    mesolink_filepath = os.path.join(mesonet_folder, f'{prefix}link.csv')
+    _outputMesoLinks(mesonet, mesolink_filepath, projection, encoding)
+
+
+def outputMicroNet(micronet, output_folder, prefix, projection, encoding):
+    micronet_folder = os.path.join(output_folder, 'micronet')
+    if not os.path.isdir(micronet_folder): os.mkdir(micronet_folder)
+
+    micronode_filepath = os.path.join(micronet_folder, f'{prefix}node.csv')
+    _outputMicroNodes(micronet, micronode_filepath, projection, encoding)
+
+    microlink_filepath = os.path.join(micronet_folder, f'{prefix}link.csv')
+    _outputMicroLinks(micronet, microlink_filepath, projection, encoding)
```

### Comparing `osm2gmns-0.7.5/osm2gmns/io/read_from_osm.py` & `osm2gmns-0.7.6/osm2gmns/io/read_from_osm.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,294 +1,294 @@
-from osm2gmns.osmnet.osmclasses import OSMNode, Way, Relation, OSMNetwork
-from osm2gmns.utils.util_coord import from_latlon
-from osm2gmns.utils.util_geo import GeoTransformer
-from osm2gmns.utils.util import getLogger
-import osm2gmns.settings as og_settings
-from shapely import geometry
-import numpy as np
-import sys
-import osmium
-import re
-
-
-class NWRHandler(osmium.SimpleHandler):
-    def __init__(self):
-        osmium.SimpleHandler.__init__(self)
-
-        self.strict_mode = True
-        self.bounds = None
-        self.POI = False
-
-        self.osm_node_dict = {}
-        self.osm_node_id_list = []
-        self.osm_node_coord_list = []
-
-        self.osm_way_dict = {}
-        self.relation_list = []
-
-    def node(self, n):
-        osm_node_id = str(n.id)
-        lon, lat = n.location.lon, n.location.lat
-        node_geometry = geometry.Point(lon, lat)
-        in_region = False if self.strict_mode and (not node_geometry.within(self.bounds)) else True
-
-        osm_node_name = n.tags.get('name')
-        osm_highway = n.tags.get('highway')
-        ctrl_type = 'signal' if (osm_highway is not None) and 'signal' in osm_highway else None
-
-        node = OSMNode(osm_node_name, osm_node_id, node_geometry, in_region, osm_highway, ctrl_type)
-        self.osm_node_dict[node.osm_node_id] = node
-
-        self.osm_node_id_list.append(osm_node_id)
-        self.osm_node_coord_list.append((lon, lat))
-        del n
-
-    def way(self, w):
-        way = Way()
-        way.osm_way_id = str(w.id)
-        way.ref_node_id_list = [str(node.ref) for node in w.nodes]
-
-        way.highway = w.tags.get('highway')
-        way.railway = w.tags.get('railway')
-        way.aeroway = w.tags.get('aeroway')
-
-        lane_info = w.tags.get('lanes')
-        if lane_info is not None:
-            lanes = re.findall(r'\d+\.?\d*', lane_info)
-            if len(lanes) > 0:
-                way.lanes = int(float(lanes[0]))  # in case of decimals
-            else:
-                logger = getLogger()
-                if logger: logger.warning(f'new lanes type detected at way {way.osm_way_id}, {lane_info}')
-        lane_info = w.tags.get('lanes:forward')
-        if lane_info is not None:
-            try:
-                way.forward_lanes = int(lane_info)
-            except:
-                pass
-        lane_info = w.tags.get('lanes:backward')
-        if lane_info is not None:
-            try:
-                way.backward_lanes = int(lane_info)
-            except:
-                pass
-
-        way.turn_lanes = w.tags.get('turn:lanes')
-        way.turn_lanes_forward = w.tags.get('turn:lanes:forward')
-        way.turn_lanes_backward = w.tags.get('turn:lanes:backward')
-
-        way.name = w.tags.get('name')
-
-        maxspeed_info = w.tags.get('maxspeed')
-        if maxspeed_info is not None:
-            try:
-                way.maxspeed = int(float(maxspeed_info))
-            except ValueError:
-                speeds = re.findall(r'\d+\.?\d* mph', maxspeed_info)
-                if len(speeds) > 0:
-                    way.maxspeed = int(float(speeds[0][:-4]) * 1.6)
-                else:
-                    speeds = re.findall(r'\d+\.?\d* km/h', maxspeed_info)
-                    if len(speeds) > 0:
-                        way.maxspeed = int(float(speeds[0][:-5]))
-                    else:
-                        logger = getLogger()
-                        if logger: logger.warning(f'new maxspeed type detected at way {way.osm_way_id}, {maxspeed_info}')
-
-        oneway_info = w.tags.get('oneway')
-        if oneway_info is not None:
-            if oneway_info == 'yes' or oneway_info == '1':
-                way.oneway = True
-            elif oneway_info == 'no' or oneway_info == '0':
-                way.oneway = False
-            elif oneway_info == '-1':
-                way.oneway = True
-                way.is_reversed = True
-            elif oneway_info in ['reversible', 'alternating']:
-                # todo: reversible, alternating: https://wiki.openstreetmap.org/wiki/Tag:oneway%3Dreversible
-                way.oneway = False
-            else:
-                logger = getLogger()
-                if logger: logger.warning(f'new lane type detected at way {way.osm_way_id}, {oneway_info}')
-
-        way.junction = w.tags.get('junction')
-        way.area = w.tags.get('area')
-        way.motor_vehicle = w.tags.get('motor_vehicle')
-        way.motorcar = w.tags.get('motorcar')
-        way.service = w.tags.get('service')
-        way.foot = w.tags.get('foot')
-        way.bicycle = w.tags.get('bicycle')
-        way.building = w.tags.get('building')
-        way.amenity = w.tags.get('amenity')
-        way.leisure = w.tags.get('leisure')
-
-        self.osm_way_dict[way.osm_way_id] = way
-        del w
-
-
-    def relation(self, r):
-        if not self.POI: return
-
-        relation = Relation()
-        relation.osm_relation_id = str(r.id)
-
-        relation.building = r.tags.get('building')
-        relation.amenity = r.tags.get('amenity')
-        relation.leisure = r.tags.get('leisure')
-        if (relation.building is None) and (relation.amenity is None):
-            return
-        relation.name = r.tags.get('name')
-
-        for member in r.members:
-            member_id, member_type, member_role = member.ref, member.type, member.role
-            member_id_str = str(member_id)
-            member_type_lc = member_type.lower()
-            if member_type_lc == 'n':
-                relation.member_id_list.append(member_id_str)
-            elif member_type_lc == 'w':
-                relation.member_id_list.append(member_id_str)
-            elif member_type_lc == 'r':
-                pass
-            else:
-                logger = getLogger()
-                if logger: logger.warning(f'new member type at relation {relation.osm_relation_id}, {member_type}')
-            relation.member_type_list.append(member_type_lc)
-            relation.member_role_list.append(member_role)
-
-        self.relation_list.append(relation)
-        del r
-
-
-def _processNodes(net, h):
-    coord_array = np.array(h.osm_node_coord_list)
-    central_lon, central_lat = np.mean(coord_array, axis=0)
-    central_lon, central_lat = float(central_lon), float(central_lat)
-    northern = True if central_lat >= 0 else False
-
-    xs, ys = from_latlon(coord_array[:, 0], coord_array[:, 1], central_lon)
-    for node_no, node_id in enumerate(h.osm_node_id_list):
-        node = h.osm_node_dict[node_id]
-        node.geometry_xy = geometry.Point((xs[node_no], ys[node_no]))
-
-    net.osm_node_dict = h.osm_node_dict
-    net.GT = GeoTransformer(central_lon, central_lat, northern)
-
-
-def _processWays(net, h):
-    for osm_way_id, osm_way in h.osm_way_dict.items():
-        try:
-            osm_way.ref_node_list = [net.osm_node_dict[ref_node_id] for ref_node_id in osm_way.ref_node_id_list]
-            net.osm_way_dict[osm_way_id] = osm_way
-        except KeyError as e:
-            print(f'WARNING: ref node {e} in way {osm_way_id} is not defined, way {osm_way_id} will not be imported')
-
-
-def _processRelations(net, h):
-    for relation in h.relation_list:
-        valid = True
-        for member_no, member_id in enumerate(relation.member_id_list):
-            member_type = relation.member_type_list[member_no]
-            if member_type == 'n':
-                try:
-                    relation.member_list.append(net.osm_node_dict[member_id])
-                except KeyError as e:
-                    print(f'WARNING: ref node {e} in relation {relation.osm_relation_id} is not defined, relation {relation.osm_relation_id} will not be imported')
-                    valid = False
-                    break
-            elif member_type == 'w':
-                try:
-                    relation.member_list.append(net.osm_way_dict[member_id])
-                except KeyError as e:
-                    print(f'WARNING: ref way {e} in relation {relation.osm_relation_id} is not defined, relation {relation.osm_relation_id} will not be imported')
-                    valid = False
-                    break
-            else:
-                pass
-
-        if valid:
-            net.osm_relation_list.append(relation)
-
-
-def _getBounds(filename, bbox):
-    """
-    Get network bounds from osm file or user given bbox
-
-    Parameters
-    ----------
-    filename: str
-        filename of the osm file
-    bbox: tuple
-        user given bound box
-
-    Returns
-    -------
-    bounds: geometry.Polygon
-        network boundary
-    """
-
-    try:
-        f = osmium.io.Reader(filename)
-    except:
-        sys.exit(f'Error: filepath {filename} contains invalid characters. Please use english characters only')
-
-    if bbox is None:
-        header = f.header()
-        box = header.box()
-        bottom_left = box.bottom_left
-        top_right = box.top_right
-        try:
-            minlat, minlon = bottom_left.lat, bottom_left.lon
-            maxlat, maxlon = top_right.lat, top_right.lon
-        except:
-            minlat, minlon = og_settings.default_bounds['minlat'], og_settings.default_bounds['minlon']
-            maxlat, maxlon = og_settings.default_bounds['maxlat'], og_settings.default_bounds['maxlon']
-    else:
-        minlat, minlon, maxlat, maxlon = bbox
-
-    bounds = geometry.Polygon([(minlon, maxlat), (maxlon, maxlat), (maxlon, minlat), (minlon, minlat)])
-    return bounds
-
-
-def readOSMFile(filename, POI, strict_mode, bbox):
-    """
-    Get nodes, ways and relations from osm file
-
-    Parameters
-    ----------
-    filename: str
-        filename of the osm file
-    POI: bool
-        get POI information or not
-    strict_mode: bool
-        use strcit_mode or not.
-    bbox: tuple
-        user given network boundary
-
-    Returns
-    -------
-    osmnet: OSMNetwork
-        OSMNetwork from the osm file
-    """
-
-    if og_settings.verbose:
-        print('  reading osm file')
-
-    osmnet = OSMNetwork()
-
-    osmnet.bounds = _getBounds(filename, bbox)
-
-    h = NWRHandler()
-    h.strict_mode = strict_mode
-    h.bounds = osmnet.bounds
-    h.POI = POI
-    h.apply_file(filename)
-
-    _processNodes(osmnet,h)
-    _processWays(osmnet,h)
-    _processRelations(osmnet, h)
-
-    return osmnet
-
-
-
-
-
+from osm2gmns.osmnet.osmclasses import OSMNode, Way, Relation, OSMNetwork
+from osm2gmns.utils.util_coord import from_latlon
+from osm2gmns.utils.util_geo import GeoTransformer
+from osm2gmns.utils.util import getLogger
+import osm2gmns.settings as og_settings
+from shapely import geometry
+import numpy as np
+import sys
+import osmium
+import re
+
+
+class NWRHandler(osmium.SimpleHandler):
+    def __init__(self):
+        osmium.SimpleHandler.__init__(self)
+
+        self.strict_mode = True
+        self.bounds = None
+        self.POI = False
+
+        self.osm_node_dict = {}
+        self.osm_node_id_list = []
+        self.osm_node_coord_list = []
+
+        self.osm_way_dict = {}
+        self.relation_list = []
+
+    def node(self, n):
+        osm_node_id = str(n.id)
+        lon, lat = n.location.lon, n.location.lat
+        node_geometry = geometry.Point(lon, lat)
+        in_region = False if self.strict_mode and (not node_geometry.within(self.bounds)) else True
+
+        osm_node_name = n.tags.get('name')
+        osm_highway = n.tags.get('highway')
+        ctrl_type = 'signal' if (osm_highway is not None) and 'signal' in osm_highway else None
+
+        node = OSMNode(osm_node_name, osm_node_id, node_geometry, in_region, osm_highway, ctrl_type)
+        self.osm_node_dict[node.osm_node_id] = node
+
+        self.osm_node_id_list.append(osm_node_id)
+        self.osm_node_coord_list.append((lon, lat))
+        del n
+
+    def way(self, w):
+        way = Way()
+        way.osm_way_id = str(w.id)
+        way.ref_node_id_list = [str(node.ref) for node in w.nodes]
+
+        way.highway = w.tags.get('highway')
+        way.railway = w.tags.get('railway')
+        way.aeroway = w.tags.get('aeroway')
+
+        lane_info = w.tags.get('lanes')
+        if lane_info is not None:
+            lanes = re.findall(r'\d+\.?\d*', lane_info)
+            if len(lanes) > 0:
+                way.lanes = int(float(lanes[0]))  # in case of decimals
+            else:
+                logger = getLogger()
+                if logger: logger.warning(f'new lanes type detected at way {way.osm_way_id}, {lane_info}')
+        lane_info = w.tags.get('lanes:forward')
+        if lane_info is not None:
+            try:
+                way.forward_lanes = int(lane_info)
+            except:
+                pass
+        lane_info = w.tags.get('lanes:backward')
+        if lane_info is not None:
+            try:
+                way.backward_lanes = int(lane_info)
+            except:
+                pass
+
+        way.turn_lanes = w.tags.get('turn:lanes')
+        way.turn_lanes_forward = w.tags.get('turn:lanes:forward')
+        way.turn_lanes_backward = w.tags.get('turn:lanes:backward')
+
+        way.name = w.tags.get('name')
+
+        maxspeed_info = w.tags.get('maxspeed')
+        if maxspeed_info is not None:
+            try:
+                way.maxspeed = int(float(maxspeed_info))
+            except ValueError:
+                speeds = re.findall(r'\d+\.?\d* mph', maxspeed_info)
+                if len(speeds) > 0:
+                    way.maxspeed = int(float(speeds[0][:-4]) * 1.6)
+                else:
+                    speeds = re.findall(r'\d+\.?\d* km/h', maxspeed_info)
+                    if len(speeds) > 0:
+                        way.maxspeed = int(float(speeds[0][:-5]))
+                    else:
+                        logger = getLogger()
+                        if logger: logger.warning(f'new maxspeed type detected at way {way.osm_way_id}, {maxspeed_info}')
+
+        oneway_info = w.tags.get('oneway')
+        if oneway_info is not None:
+            if oneway_info == 'yes' or oneway_info == '1':
+                way.oneway = True
+            elif oneway_info == 'no' or oneway_info == '0':
+                way.oneway = False
+            elif oneway_info == '-1':
+                way.oneway = True
+                way.is_reversed = True
+            elif oneway_info in ['reversible', 'alternating']:
+                # todo: reversible, alternating: https://wiki.openstreetmap.org/wiki/Tag:oneway%3Dreversible
+                way.oneway = False
+            else:
+                logger = getLogger()
+                if logger: logger.warning(f'new lane type detected at way {way.osm_way_id}, {oneway_info}')
+
+        way.junction = w.tags.get('junction')
+        way.area = w.tags.get('area')
+        way.motor_vehicle = w.tags.get('motor_vehicle')
+        way.motorcar = w.tags.get('motorcar')
+        way.service = w.tags.get('service')
+        way.foot = w.tags.get('foot')
+        way.bicycle = w.tags.get('bicycle')
+        way.building = w.tags.get('building')
+        way.amenity = w.tags.get('amenity')
+        way.leisure = w.tags.get('leisure')
+
+        self.osm_way_dict[way.osm_way_id] = way
+        del w
+
+
+    def relation(self, r):
+        if not self.POI: return
+
+        relation = Relation()
+        relation.osm_relation_id = str(r.id)
+
+        relation.building = r.tags.get('building')
+        relation.amenity = r.tags.get('amenity')
+        relation.leisure = r.tags.get('leisure')
+        if (relation.building is None) and (relation.amenity is None):
+            return
+        relation.name = r.tags.get('name')
+
+        for member in r.members:
+            member_id, member_type, member_role = member.ref, member.type, member.role
+            member_id_str = str(member_id)
+            member_type_lc = member_type.lower()
+            if member_type_lc == 'n':
+                relation.member_id_list.append(member_id_str)
+            elif member_type_lc == 'w':
+                relation.member_id_list.append(member_id_str)
+            elif member_type_lc == 'r':
+                pass
+            else:
+                logger = getLogger()
+                if logger: logger.warning(f'new member type at relation {relation.osm_relation_id}, {member_type}')
+            relation.member_type_list.append(member_type_lc)
+            relation.member_role_list.append(member_role)
+
+        self.relation_list.append(relation)
+        del r
+
+
+def _processNodes(net, h):
+    coord_array = np.array(h.osm_node_coord_list)
+    central_lon, central_lat = np.mean(coord_array, axis=0)
+    central_lon, central_lat = float(central_lon), float(central_lat)
+    northern = True if central_lat >= 0 else False
+
+    xs, ys = from_latlon(coord_array[:, 0], coord_array[:, 1], central_lon)
+    for node_no, node_id in enumerate(h.osm_node_id_list):
+        node = h.osm_node_dict[node_id]
+        node.geometry_xy = geometry.Point((xs[node_no], ys[node_no]))
+
+    net.osm_node_dict = h.osm_node_dict
+    net.GT = GeoTransformer(central_lon, central_lat, northern)
+
+
+def _processWays(net, h):
+    for osm_way_id, osm_way in h.osm_way_dict.items():
+        try:
+            osm_way.ref_node_list = [net.osm_node_dict[ref_node_id] for ref_node_id in osm_way.ref_node_id_list]
+            net.osm_way_dict[osm_way_id] = osm_way
+        except KeyError as e:
+            print(f'WARNING: ref node {e} in way {osm_way_id} is not defined, way {osm_way_id} will not be imported')
+
+
+def _processRelations(net, h):
+    for relation in h.relation_list:
+        valid = True
+        for member_no, member_id in enumerate(relation.member_id_list):
+            member_type = relation.member_type_list[member_no]
+            if member_type == 'n':
+                try:
+                    relation.member_list.append(net.osm_node_dict[member_id])
+                except KeyError as e:
+                    print(f'WARNING: ref node {e} in relation {relation.osm_relation_id} is not defined, relation {relation.osm_relation_id} will not be imported')
+                    valid = False
+                    break
+            elif member_type == 'w':
+                try:
+                    relation.member_list.append(net.osm_way_dict[member_id])
+                except KeyError as e:
+                    print(f'WARNING: ref way {e} in relation {relation.osm_relation_id} is not defined, relation {relation.osm_relation_id} will not be imported')
+                    valid = False
+                    break
+            else:
+                pass
+
+        if valid:
+            net.osm_relation_list.append(relation)
+
+
+def _getBounds(filename, bbox):
+    """
+    Get network bounds from osm file or user given bbox
+
+    Parameters
+    ----------
+    filename: str
+        filename of the osm file
+    bbox: tuple
+        user given bound box
+
+    Returns
+    -------
+    bounds: geometry.Polygon
+        network boundary
+    """
+
+    try:
+        f = osmium.io.Reader(filename)
+    except:
+        sys.exit(f'Error: filepath {filename} contains invalid characters. Please use english characters only')
+
+    if bbox is None:
+        header = f.header()
+        box = header.box()
+        bottom_left = box.bottom_left
+        top_right = box.top_right
+        try:
+            minlat, minlon = bottom_left.lat, bottom_left.lon
+            maxlat, maxlon = top_right.lat, top_right.lon
+        except:
+            minlat, minlon = og_settings.default_bounds['minlat'], og_settings.default_bounds['minlon']
+            maxlat, maxlon = og_settings.default_bounds['maxlat'], og_settings.default_bounds['maxlon']
+    else:
+        minlat, minlon, maxlat, maxlon = bbox
+
+    bounds = geometry.Polygon([(minlon, maxlat), (maxlon, maxlat), (maxlon, minlat), (minlon, minlat)])
+    return bounds
+
+
+def readOSMFile(filename, POI, strict_mode, bbox):
+    """
+    Get nodes, ways and relations from osm file
+
+    Parameters
+    ----------
+    filename: str
+        filename of the osm file
+    POI: bool
+        get POI information or not
+    strict_mode: bool
+        use strcit_mode or not.
+    bbox: tuple
+        user given network boundary
+
+    Returns
+    -------
+    osmnet: OSMNetwork
+        OSMNetwork from the osm file
+    """
+
+    if og_settings.verbose:
+        print('  reading osm file')
+
+    osmnet = OSMNetwork()
+
+    osmnet.bounds = _getBounds(filename, bbox)
+
+    h = NWRHandler()
+    h.strict_mode = strict_mode
+    h.bounds = osmnet.bounds
+    h.POI = POI
+    h.apply_file(filename)
+
+    _processNodes(osmnet,h)
+    _processWays(osmnet,h)
+    _processRelations(osmnet, h)
+
+    return osmnet
+
+
+
+
+
```

### Comparing `osm2gmns-0.7.5/osm2gmns/io/readfile_mp.py` & `osm2gmns-0.7.6/osm2gmns/io/readfile_mp.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,147 +1,147 @@
-import csv
-import os
-from osm2gmns.utils.util import *
-import osmium
-from collections import namedtuple
-import multiprocessing as mp
-
-
-Node = namedtuple('Node', ('id', 'tags', 'lonlat'))
-Way = namedtuple('Way', ('id', 'tags', 'refs'))
-Relation = namedtuple('Relation', ('id', 'tags', 'members'))
-
-
-def collectNodes1(filename):
-    class NodeHandler(osmium.SimpleHandler):
-        def __init__(self):
-            osmium.SimpleHandler.__init__(self)
-            self.nodes = []
-
-        def node(self, n):
-            node_id = n.id
-            if node_id % 3 == 1:
-                lonlat = (n.location.lon, n.location.lat)
-                tags = {tag.k: tag.v for tag in n.tags}
-                node = Node(node_id, tags, lonlat)
-                self.nodes.append(node)
-
-    node_handler = NodeHandler()
-    node_handler.apply_file(filename)
-    return 'n', node_handler.nodes
-
-
-def collectNodes2(filename):
-    class NodeHandler(osmium.SimpleHandler):
-        def __init__(self):
-            osmium.SimpleHandler.__init__(self)
-            self.nodes = []
-
-        def node(self, n):
-            node_id = n.id
-            if node_id % 3 == 2:
-                lonlat = (n.location.lon, n.location.lat)
-                tags = {tag.k: tag.v for tag in n.tags}
-                node = Node(node_id, tags, lonlat)
-                self.nodes.append(node)
-
-    node_handler = NodeHandler()
-    node_handler.apply_file(filename)
-    return 'n', node_handler.nodes
-
-
-def collectNodes3(filename):
-    class NodeHandler(osmium.SimpleHandler):
-        def __init__(self):
-            osmium.SimpleHandler.__init__(self)
-            self.nodes = []
-
-        def node(self, n):
-            node_id = n.id
-            if node_id % 3 == 0:
-                lonlat = (n.location.lon, n.location.lat)
-                tags = {tag.k: tag.v for tag in n.tags}
-                node = Node(node_id, tags, lonlat)
-                self.nodes.append(node)
-
-    node_handler = NodeHandler()
-    node_handler.apply_file(filename)
-    return 'n', node_handler.nodes
-
-
-def collectWaysRelations(filename):
-    class WayRelationHandler(osmium.SimpleHandler):
-        def __init__(self):
-            osmium.SimpleHandler.__init__(self)
-            self.ways = []
-            self.relations = []
-
-        def way(self, w):
-            way_id = w.id
-            refs = [node.ref for node in w.nodes]
-            tags = {tag.k: tag.v for tag in w.tags}
-            way = Way(way_id, tags, refs)
-            self.ways.append(way)
-
-        def relation(self, r):
-            relation_id = r.id
-            members = [(member.ref, member.type, member.role) for member in r.members]
-            tags = {tag.k: tag.v for tag in r.tags}
-            relation = Relation(relation_id, tags, members)
-            self.relations.append(relation)
-
-    wr_handler = WayRelationHandler()
-    wr_handler.apply_file(filename)
-    return 'wr', wr_handler.ways, wr_handler.relations
-
-
-def readOSMFile(filename):
-
-    bounds = default_bounds
-
-    f = osmium.io.Reader(filename)
-    header = f.header()
-    print('Bbox:', header.box())
-
-    results = []
-    p = mp.Pool(4)
-    results.append(p.apply_async(collectNodes1, (filename,)))
-    results.append(p.apply_async(collectNodes2, (filename,)))
-    results.append(p.apply_async(collectNodes3, (filename,)))
-    results.append(p.apply_async(collectWaysRelations, (filename,)))
-    p.close()
-    p.join()
-
-    nodes, ways, relations = [], [], []
-    for result in results:
-        result_tuple = result.get()
-        if result_tuple[0] == 'n':
-            nodes += result_tuple[1]
-        elif result_tuple[0] == 'wr':
-            ways = result_tuple[1]
-            relations = result_tuple[2]
-
-    return {'bounds':bounds, 'nodes':nodes, 'ways':ways, 'relations':relations}
-
-
-
-def readCSVFile(folder, encoding):
-    node_filepath = os.path.join(folder,'node.csv')
-    link_filepath = os.path.join(folder,'link.csv')
-
-    if encoding is None:
-        nfin = open(node_filepath, 'r')
-        lfin = open(link_filepath, 'r')
-    else:
-        nfin = open(node_filepath, 'r', encoding=encoding)
-        lfin = open(link_filepath, 'r', encoding=encoding)
-
-    reader = csv.DictReader(nfin)
-    node_data = [line for line in reader]
-    nfin.close()
-
-    reader = csv.DictReader(lfin)
-    link_data = [line for line in reader]
-    lfin.close()
-
-    return node_data, link_data
-
+import csv
+import os
+from osm2gmns.utils.util import *
+import osmium
+from collections import namedtuple
+import multiprocessing as mp
+
+
+Node = namedtuple('Node', ('id', 'tags', 'lonlat'))
+Way = namedtuple('Way', ('id', 'tags', 'refs'))
+Relation = namedtuple('Relation', ('id', 'tags', 'members'))
+
+
+def collectNodes1(filename):
+    class NodeHandler(osmium.SimpleHandler):
+        def __init__(self):
+            osmium.SimpleHandler.__init__(self)
+            self.nodes = []
+
+        def node(self, n):
+            node_id = n.id
+            if node_id % 3 == 1:
+                lonlat = (n.location.lon, n.location.lat)
+                tags = {tag.k: tag.v for tag in n.tags}
+                node = Node(node_id, tags, lonlat)
+                self.nodes.append(node)
+
+    node_handler = NodeHandler()
+    node_handler.apply_file(filename)
+    return 'n', node_handler.nodes
+
+
+def collectNodes2(filename):
+    class NodeHandler(osmium.SimpleHandler):
+        def __init__(self):
+            osmium.SimpleHandler.__init__(self)
+            self.nodes = []
+
+        def node(self, n):
+            node_id = n.id
+            if node_id % 3 == 2:
+                lonlat = (n.location.lon, n.location.lat)
+                tags = {tag.k: tag.v for tag in n.tags}
+                node = Node(node_id, tags, lonlat)
+                self.nodes.append(node)
+
+    node_handler = NodeHandler()
+    node_handler.apply_file(filename)
+    return 'n', node_handler.nodes
+
+
+def collectNodes3(filename):
+    class NodeHandler(osmium.SimpleHandler):
+        def __init__(self):
+            osmium.SimpleHandler.__init__(self)
+            self.nodes = []
+
+        def node(self, n):
+            node_id = n.id
+            if node_id % 3 == 0:
+                lonlat = (n.location.lon, n.location.lat)
+                tags = {tag.k: tag.v for tag in n.tags}
+                node = Node(node_id, tags, lonlat)
+                self.nodes.append(node)
+
+    node_handler = NodeHandler()
+    node_handler.apply_file(filename)
+    return 'n', node_handler.nodes
+
+
+def collectWaysRelations(filename):
+    class WayRelationHandler(osmium.SimpleHandler):
+        def __init__(self):
+            osmium.SimpleHandler.__init__(self)
+            self.ways = []
+            self.relations = []
+
+        def way(self, w):
+            way_id = w.id
+            refs = [node.ref for node in w.nodes]
+            tags = {tag.k: tag.v for tag in w.tags}
+            way = Way(way_id, tags, refs)
+            self.ways.append(way)
+
+        def relation(self, r):
+            relation_id = r.id
+            members = [(member.ref, member.type, member.role) for member in r.members]
+            tags = {tag.k: tag.v for tag in r.tags}
+            relation = Relation(relation_id, tags, members)
+            self.relations.append(relation)
+
+    wr_handler = WayRelationHandler()
+    wr_handler.apply_file(filename)
+    return 'wr', wr_handler.ways, wr_handler.relations
+
+
+def readOSMFile(filename):
+
+    bounds = default_bounds
+
+    f = osmium.io.Reader(filename)
+    header = f.header()
+    print('Bbox:', header.box())
+
+    results = []
+    p = mp.Pool(4)
+    results.append(p.apply_async(collectNodes1, (filename,)))
+    results.append(p.apply_async(collectNodes2, (filename,)))
+    results.append(p.apply_async(collectNodes3, (filename,)))
+    results.append(p.apply_async(collectWaysRelations, (filename,)))
+    p.close()
+    p.join()
+
+    nodes, ways, relations = [], [], []
+    for result in results:
+        result_tuple = result.get()
+        if result_tuple[0] == 'n':
+            nodes += result_tuple[1]
+        elif result_tuple[0] == 'wr':
+            ways = result_tuple[1]
+            relations = result_tuple[2]
+
+    return {'bounds':bounds, 'nodes':nodes, 'ways':ways, 'relations':relations}
+
+
+
+def readCSVFile(folder, encoding):
+    node_filepath = os.path.join(folder,'node.csv')
+    link_filepath = os.path.join(folder,'link.csv')
+
+    if encoding is None:
+        nfin = open(node_filepath, 'r')
+        lfin = open(link_filepath, 'r')
+    else:
+        nfin = open(node_filepath, 'r', encoding=encoding)
+        lfin = open(link_filepath, 'r', encoding=encoding)
+
+    reader = csv.DictReader(nfin)
+    node_data = [line for line in reader]
+    nfin.close()
+
+    reader = csv.DictReader(lfin)
+    link_data = [line for line in reader]
+    lfin.close()
+
+    return node_data, link_data
+
```

### Comparing `osm2gmns-0.7.5/osm2gmns/io/util_io.py` & `osm2gmns-0.7.6/osm2gmns/io/util_io.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-# @author       Jiawei Lu (jiaweil9@asu.edu)
-# @time         2021/12/8 12:21
-# @desc         [script description]
-
-
-def getFileHandle(filepath, encoding):
-
-    while True:
-        try:
-            if encoding is None:
-                outfile = open(filepath, 'w', newline='',errors='ignore')
-            else:
-                outfile = open(filepath, 'w', newline='', errors='ignore', encoding=encoding)
-            break
-        except PermissionError:
-            print(f'{filepath} may be locked by other programs. please release it then press Enter to try again')
-            input()
-
+# @author       Jiawei Lu (jiaweil9@asu.edu)
+# @time         2021/12/8 12:21
+# @desc         [script description]
+
+
+def getFileHandle(filepath, encoding):
+
+    while True:
+        try:
+            if encoding is None:
+                outfile = open(filepath, 'w', newline='',errors='ignore')
+            else:
+                outfile = open(filepath, 'w', newline='', errors='ignore', encoding=encoding)
+            break
+        except PermissionError:
+            print(f'{filepath} may be locked by other programs. please release it then press Enter to try again')
+            input()
+
     return outfile
```

### Comparing `osm2gmns-0.7.5/osm2gmns/io/writefile.py` & `osm2gmns-0.7.6/osm2gmns/io/writefile.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,177 +1,177 @@
-from osm2gmns.io.output_mrnet import outputMesoNet, outputMicroNet
-import osm2gmns.settings as og_settings
-from shapely import wkt
-import csv
-import os
-
-
-# we use errors='ignore' to make our program compatible with some characters that cannot be encoded by the local encoding,
-# these characters will be discarded
-
-def _outputNode(network, output_folder, node_filename, projection, encoding):
-    node_filepath = os.path.join(output_folder, node_filename)
-    while True:
-        try:
-            if encoding is None:
-                outfile = open(node_filepath, 'w', newline='',errors='ignore')
-            else:
-                outfile = open(node_filepath, 'w', newline='', errors='ignore', encoding=encoding)
-            break
-        except PermissionError:
-            print(f'{node_filename} may be locked by other programs. please release it then press Enter to try again')
-            input()
-    writer = csv.writer(outfile)
-    writer.writerow(['name', 'node_id', 'osm_node_id', 'osm_highway', 'zone_id', 'ctrl_type', 'node_type', 'activity_type',
-                     'is_boundary', 'x_coord', 'y_coord', 'intersection_id','poi_id','notes'])
-    for node_id,node in network.node_dict.items():
-        if projection:
-            x_coord = round(node.geometry_xy.x, og_settings.local_coord_precision)
-            y_coord = round(node.geometry_xy.y, og_settings.local_coord_precision)
-        else:
-            x_coord = round(node.geometry.x, og_settings.lonlat_coord_precision)
-            y_coord = round(node.geometry.y, og_settings.lonlat_coord_precision)
-        line = [node.name, node.node_id, node.osm_node_id, node.osm_highway, node.zone_id, node.ctrl_type, '', node.activity_type,
-                node.is_boundary, x_coord, y_coord,node.intersection_id,node.poi_id,node.notes]
-        writer.writerow(line)
-    outfile.close()
-
-
-def _outputLink(network, output_folder, link_filename, projection, encoding):
-    link_filepath = os.path.join(output_folder, link_filename)
-    while True:
-        try:
-            if encoding is None:
-                outfile = open(link_filepath, 'w', newline='',errors='ignore')
-            else:
-                outfile = open(link_filepath, 'w', newline='', errors='ignore', encoding=encoding)
-            break
-        except PermissionError:
-            print(f'{link_filename} may be locked by other programs. please release it then press Enter to try again')
-            input()
-    writer = csv.writer(outfile)
-    writer.writerow(['name', 'link_id', 'osm_way_id', 'from_node_id', 'to_node_id', 'dir_flag', 'length', 'lanes',
-                     'free_speed', 'capacity', 'link_type_name', 'link_type', 'geometry','allowed_uses','from_biway',
-                     'is_link', 'VDF_fftt1', 'VDF_cap1'])
-    for link_id, link in network.link_dict.items():
-        from_biway = 1 if link.from_bidirectional_way else 0
-        is_link = 1 if link.is_link else 0
-        if projection:
-            geometry_ = wkt.dumps(link.geometry_xy, rounding_precision=og_settings.local_coord_precision)
-        else:
-            geometry_ = wkt.dumps(link.geometry, rounding_precision=og_settings.lonlat_coord_precision)
-        line = [link.name, link.link_id, link.osm_way_id, link.from_node.node_id, link.to_node.node_id, link.dir_flag, link.length,
-                link.lanes, link.free_speed, link.capacity, link.link_type_name, link.link_type, geometry_, ';'.join(link.allowed_uses),
-                from_biway, is_link, link.VDF_fftt1, link.VDF_cap1]
-        writer.writerow(line)
-    outfile.close()
-
-
-def _outputMovement(network, output_folder, movement_filename, projection, encoding):
-    movement_filepath = os.path.join(output_folder, movement_filename)
-    if network.max_movement_id > 0:
-        while True:
-            try:
-                if encoding is None:
-                    outfile = open(movement_filepath, 'w', newline='', errors='ignore')  # ,errors='ignore'
-                else:
-                    outfile = open(movement_filepath, 'w', newline='', errors='ignore',
-                                   encoding=encoding)  # ,errors='ignore'
-                break
-            except PermissionError:
-                print(
-                    f'{movement_filename} may be locked by other programs. please release it then press Enter to try again')
-                input()
-        writer = csv.writer(outfile)
-        writer.writerow(['mvmt_id', 'node_id', 'osm_node_id', 'name', 'ib_link_id', 'start_ib_lane', 'end_ib_lane',
-                         'ob_link_id', 'start_ob_lane', 'end_ob_lane', 'lanes', 'ib_osm_node_id', 'ob_osm_node_id',
-                         'type', 'penalty', 'capacity', 'ctrl_type', 'mvmt_txt_id', 'geometry', 'volume', 'free_speed',
-                         'allowed_uses', 'generated_by_osm2gmns'])
-
-        for node_id, node in network.node_dict.items():
-            for mvmt in node.movement_list:
-                from_node = mvmt.ib_link.from_node
-                to_node = mvmt.ob_link.to_node
-                if projection:
-                    geometry_ = wkt.dumps(mvmt.geometry_xy, rounding_precision=og_settings.local_coord_precision)
-                else:
-                    geometry_ = wkt.dumps(mvmt.geometry, rounding_precision=og_settings.lonlat_coord_precision)
-
-                generated_by_osm2gmns = 1 if mvmt.generated_by_osm2gmns else 0
-
-                line = [mvmt.movement_id, node.node_id, node.osm_node_id, '', mvmt.ib_link.link_id, mvmt.start_ib_lane,
-                        mvmt.end_ib_lane, mvmt.ob_link.link_id, mvmt.start_ob_lane, mvmt.end_ob_lane, mvmt.lanes,
-                        from_node.osm_node_id, to_node.osm_node_id, mvmt.type, '', '', mvmt.ctrl_type, mvmt.mvmt_txt_id,
-                        geometry_, '', '', ';'.join(mvmt.allowed_uses), generated_by_osm2gmns]
-                writer.writerow(line)
-        outfile.close()
-
-
-def _outputPOI(network, output_folder, poi_filename, projection, encoding):
-    poi_filepath = os.path.join(output_folder, poi_filename)
-    if network.POI_list:
-        while True:
-            try:
-                if encoding is None:
-                    outfile = open(poi_filepath, 'w', newline='',errors='ignore')     # ,errors='ignore'
-                else:
-                    outfile = open(poi_filepath, 'w', newline='', errors='ignore', encoding=encoding)  # ,errors='ignore'
-                break
-            except PermissionError:
-                print(f'{poi_filename} may be locked by other programs. please release it then press Enter to try again')
-                input()
-        writer = csv.writer(outfile)
-        writer.writerow(['name', 'poi_id', 'osm_way_id', 'osm_relation_id','building','amenity','leisure','way','geometry','centroid',
-                         'area', 'area_ft2'])
-        for poi in network.POI_list:
-            geometry_ = poi.geometry_xy if projection else poi.geometry
-            centroid = poi.centroid_xy if projection else poi.centroid
-            area = poi.geometry_xy.area
-            area_ft2 = area * 10.7639
-            line = [poi.name, poi.poi_id, poi.osm_way_id, poi.osm_relation_id, poi.building, poi.amenity, poi.leisure, poi.way, geometry_,
-                    centroid, round(area,1), round(area_ft2,1)]
-            writer.writerow(line)
-
-
-def outputNetToCSV(network, output_folder='', prefix='', projection=False, encoding=None):
-    """
-    Output an osm2gmns network object to csv files in GMNS format
-
-    Parameters
-    ----------
-    network: Network
-        an osm2gmns network object
-    output_folder: str
-        path of the folder to store network files. can be an absolute or a relative path
-    prefix: str
-        prefix of output csv files
-    projection: bool
-        if True, osm2gmns will project the network to a local coordinate system when ouptting a network
-    encoding: str
-        the file encoding used to output a network
-
-    Returns
-    -------
-    None
-    """
-    if og_settings.verbose:
-        print('Outputting Network Files')
-
-    if output_folder:
-        if not os.path.isdir(output_folder): os.mkdir(output_folder)
-
-    node_filename = f'{prefix}node.csv'
-    _outputNode(network, output_folder, node_filename, projection, encoding)
-
-    link_filename = f'{prefix}link.csv'
-    _outputLink(network, output_folder, link_filename, projection, encoding)
-
-    movement_filename = f'{prefix}movement.csv'
-    _outputMovement(network, output_folder, movement_filename, projection, encoding)
-
-    poi_filename = f'{prefix}poi.csv'
-    _outputPOI(network, output_folder, poi_filename, projection, encoding)
-
-    if network.mesonet is not None:
-        outputMesoNet(network.mesonet, output_folder, prefix, projection, encoding)
-    if network.micronet is not None:
-        outputMicroNet(network.micronet, output_folder, prefix, projection, encoding)
+from osm2gmns.io.output_mrnet import outputMesoNet, outputMicroNet
+import osm2gmns.settings as og_settings
+from shapely import wkt
+import csv
+import os
+
+
+# we use errors='ignore' to make our program compatible with some characters that cannot be encoded by the local encoding,
+# these characters will be discarded
+
+def _outputNode(network, output_folder, node_filename, projection, encoding):
+    node_filepath = os.path.join(output_folder, node_filename)
+    while True:
+        try:
+            if encoding is None:
+                outfile = open(node_filepath, 'w', newline='',errors='ignore')
+            else:
+                outfile = open(node_filepath, 'w', newline='', errors='ignore', encoding=encoding)
+            break
+        except PermissionError:
+            print(f'{node_filename} may be locked by other programs. please release it then press Enter to try again')
+            input()
+    writer = csv.writer(outfile)
+    writer.writerow(['name', 'node_id', 'osm_node_id', 'osm_highway', 'zone_id', 'ctrl_type', 'node_type', 'activity_type',
+                     'is_boundary', 'x_coord', 'y_coord', 'intersection_id','poi_id','notes'])
+    for node_id,node in network.node_dict.items():
+        if projection:
+            x_coord = round(node.geometry_xy.x, og_settings.local_coord_precision)
+            y_coord = round(node.geometry_xy.y, og_settings.local_coord_precision)
+        else:
+            x_coord = round(node.geometry.x, og_settings.lonlat_coord_precision)
+            y_coord = round(node.geometry.y, og_settings.lonlat_coord_precision)
+        line = [node.name, node.node_id, node.osm_node_id, node.osm_highway, node.zone_id, node.ctrl_type, '', node.activity_type,
+                node.is_boundary, x_coord, y_coord,node.intersection_id,node.poi_id,node.notes]
+        writer.writerow(line)
+    outfile.close()
+
+
+def _outputLink(network, output_folder, link_filename, projection, encoding):
+    link_filepath = os.path.join(output_folder, link_filename)
+    while True:
+        try:
+            if encoding is None:
+                outfile = open(link_filepath, 'w', newline='',errors='ignore')
+            else:
+                outfile = open(link_filepath, 'w', newline='', errors='ignore', encoding=encoding)
+            break
+        except PermissionError:
+            print(f'{link_filename} may be locked by other programs. please release it then press Enter to try again')
+            input()
+    writer = csv.writer(outfile)
+    writer.writerow(['name', 'link_id', 'osm_way_id', 'from_node_id', 'to_node_id', 'dir_flag', 'length', 'lanes',
+                     'free_speed', 'capacity', 'link_type_name', 'link_type', 'geometry','allowed_uses','from_biway',
+                     'is_link', 'VDF_fftt1', 'VDF_cap1'])
+    for link_id, link in network.link_dict.items():
+        from_biway = 1 if link.from_bidirectional_way else 0
+        is_link = 1 if link.is_link else 0
+        if projection:
+            geometry_ = wkt.dumps(link.geometry_xy, rounding_precision=og_settings.local_coord_precision)
+        else:
+            geometry_ = wkt.dumps(link.geometry, rounding_precision=og_settings.lonlat_coord_precision)
+        line = [link.name, link.link_id, link.osm_way_id, link.from_node.node_id, link.to_node.node_id, link.dir_flag, link.length,
+                link.lanes, link.free_speed, link.capacity, link.link_type_name, link.link_type, geometry_, ';'.join(link.allowed_uses),
+                from_biway, is_link, link.VDF_fftt1, link.VDF_cap1]
+        writer.writerow(line)
+    outfile.close()
+
+
+def _outputMovement(network, output_folder, movement_filename, projection, encoding):
+    movement_filepath = os.path.join(output_folder, movement_filename)
+    if network.max_movement_id > 0:
+        while True:
+            try:
+                if encoding is None:
+                    outfile = open(movement_filepath, 'w', newline='', errors='ignore')  # ,errors='ignore'
+                else:
+                    outfile = open(movement_filepath, 'w', newline='', errors='ignore',
+                                   encoding=encoding)  # ,errors='ignore'
+                break
+            except PermissionError:
+                print(
+                    f'{movement_filename} may be locked by other programs. please release it then press Enter to try again')
+                input()
+        writer = csv.writer(outfile)
+        writer.writerow(['mvmt_id', 'node_id', 'osm_node_id', 'name', 'ib_link_id', 'start_ib_lane', 'end_ib_lane',
+                         'ob_link_id', 'start_ob_lane', 'end_ob_lane', 'lanes', 'ib_osm_node_id', 'ob_osm_node_id',
+                         'type', 'penalty', 'capacity', 'ctrl_type', 'mvmt_txt_id', 'geometry', 'volume', 'free_speed',
+                         'allowed_uses', 'generated_by_osm2gmns'])
+
+        for node_id, node in network.node_dict.items():
+            for mvmt in node.movement_list:
+                from_node = mvmt.ib_link.from_node
+                to_node = mvmt.ob_link.to_node
+                if projection:
+                    geometry_ = wkt.dumps(mvmt.geometry_xy, rounding_precision=og_settings.local_coord_precision)
+                else:
+                    geometry_ = wkt.dumps(mvmt.geometry, rounding_precision=og_settings.lonlat_coord_precision)
+
+                generated_by_osm2gmns = 1 if mvmt.generated_by_osm2gmns else 0
+
+                line = [mvmt.movement_id, node.node_id, node.osm_node_id, '', mvmt.ib_link.link_id, mvmt.start_ib_lane,
+                        mvmt.end_ib_lane, mvmt.ob_link.link_id, mvmt.start_ob_lane, mvmt.end_ob_lane, mvmt.lanes,
+                        from_node.osm_node_id, to_node.osm_node_id, mvmt.type, '', '', mvmt.ctrl_type, mvmt.mvmt_txt_id,
+                        geometry_, '', '', ';'.join(mvmt.allowed_uses), generated_by_osm2gmns]
+                writer.writerow(line)
+        outfile.close()
+
+
+def _outputPOI(network, output_folder, poi_filename, projection, encoding):
+    poi_filepath = os.path.join(output_folder, poi_filename)
+    if network.POI_list:
+        while True:
+            try:
+                if encoding is None:
+                    outfile = open(poi_filepath, 'w', newline='',errors='ignore')     # ,errors='ignore'
+                else:
+                    outfile = open(poi_filepath, 'w', newline='', errors='ignore', encoding=encoding)  # ,errors='ignore'
+                break
+            except PermissionError:
+                print(f'{poi_filename} may be locked by other programs. please release it then press Enter to try again')
+                input()
+        writer = csv.writer(outfile)
+        writer.writerow(['name', 'poi_id', 'osm_way_id', 'osm_relation_id','building','amenity','leisure','way','geometry','centroid',
+                         'area', 'area_ft2'])
+        for poi in network.POI_list:
+            geometry_ = poi.geometry_xy if projection else poi.geometry
+            centroid = poi.centroid_xy if projection else poi.centroid
+            area = poi.geometry_xy.area
+            area_ft2 = area * 10.7639
+            line = [poi.name, poi.poi_id, poi.osm_way_id, poi.osm_relation_id, poi.building, poi.amenity, poi.leisure, poi.way, geometry_,
+                    centroid, round(area,1), round(area_ft2,1)]
+            writer.writerow(line)
+
+
+def outputNetToCSV(network, output_folder='', prefix='', projection=False, encoding=None):
+    """
+    Output an osm2gmns network object to csv files in GMNS format
+
+    Parameters
+    ----------
+    network: Network
+        an osm2gmns network object
+    output_folder: str
+        path of the folder to store network files. can be an absolute or a relative path
+    prefix: str
+        prefix of output csv files
+    projection: bool
+        if True, osm2gmns will project the network to a local coordinate system when ouptting a network
+    encoding: str
+        the file encoding used to output a network
+
+    Returns
+    -------
+    None
+    """
+    if og_settings.verbose:
+        print('Outputting Network Files')
+
+    if output_folder:
+        if not os.path.isdir(output_folder): os.mkdir(output_folder)
+
+    node_filename = f'{prefix}node.csv'
+    _outputNode(network, output_folder, node_filename, projection, encoding)
+
+    link_filename = f'{prefix}link.csv'
+    _outputLink(network, output_folder, link_filename, projection, encoding)
+
+    movement_filename = f'{prefix}movement.csv'
+    _outputMovement(network, output_folder, movement_filename, projection, encoding)
+
+    poi_filename = f'{prefix}poi.csv'
+    _outputPOI(network, output_folder, poi_filename, projection, encoding)
+
+    if network.mesonet is not None:
+        outputMesoNet(network.mesonet, output_folder, prefix, projection, encoding)
+    if network.micronet is not None:
+        outputMicroNet(network.micronet, output_folder, prefix, projection, encoding)
```

### Comparing `osm2gmns-0.7.5/osm2gmns/movement/autoconintd.py` & `osm2gmns-0.7.6/osm2gmns/movement/autoconintd.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,109 +1,109 @@
-from osm2gmns.utils.util_geo import getLineAngle
-
-
-class CAutoConnectorIntD:
-    default_right_most_lanes = 1        # do not change
-    default_left_most_lanes = 1         # do not change
-
-    ib_link = None
-    ob_link_list = []
-    ob_link_list_sorted = []
-    connection_list = []
-
-    @classmethod
-    def getSequence(cls):       # order outbound links from left to right
-        angle_list = []
-
-        for ob_link in cls.ob_link_list:
-            angle = getLineAngle(cls.ib_link.geometry_xy, ob_link.geometry_xy)
-            angle_list.append(angle)
-
-        cls.ob_link_list_sorted = sorted(cls.ob_link_list, key=lambda x:angle_list[cls.ob_link_list.index(x)],reverse=True)
-
-
-    @classmethod
-    def getLaneConnection(cls):
-        cls.connection_list = [[] for _ in range(len(cls.ob_link_list_sorted))]
-        ib_lanes = cls.ib_link.outgoing_lanes
-
-        if ib_lanes == 1:
-            left_ob_link = cls.ob_link_list_sorted[0]
-            cls.connection_list[cls.ob_link_list.index(left_ob_link)] = [(0, 0),(0, 0)]
-            for ob_link in cls.ob_link_list_sorted[1:]:
-                cls.connection_list[cls.ob_link_list.index(ob_link)] = [(0, 0), (ob_link.incoming_lanes-1, ob_link.incoming_lanes-1)]
-            return
-
-        if len(cls.ob_link_list_sorted) == 1:
-            # only one ob_link, full connection
-            ob_link = cls.ob_link_list_sorted[0]
-            connection_lanes = min(ib_lanes, ob_link.incoming_lanes)
-            cls.connection_list[cls.ob_link_list.index(ob_link)] = [(0, connection_lanes - 1), (0, connection_lanes - 1)]
-
-        elif len(cls.ob_link_list_sorted) == 2:
-            # two ob_link, default right, remaining left
-            left_ob_link = cls.ob_link_list_sorted[0]
-            lanes_ib_link_left = ib_lanes - cls.default_left_most_lanes
-            lanes_ob_has = left_ob_link.incoming_lanes
-            connection_lanes = min(lanes_ib_link_left,lanes_ob_has)
-            cls.connection_list[cls.ob_link_list.index(left_ob_link)] = [(0, connection_lanes - 1), (0, connection_lanes - 1)]
-
-            right_ob_link = cls.ob_link_list_sorted[-1]
-            cls.connection_list[cls.ob_link_list.index(right_ob_link)] = [
-                (ib_lanes - cls.default_right_most_lanes, ib_lanes - 1),
-                (right_ob_link.incoming_lanes - cls.default_right_most_lanes, right_ob_link.incoming_lanes - 1)]
-
-        else:
-            # >= 3, default left, default right, remaining mid
-            left_ob_link = cls.ob_link_list_sorted[0]
-            cls.connection_list[cls.ob_link_list.index(left_ob_link)] = [(0,cls.default_left_most_lanes-1), (0,cls.default_left_most_lanes-1)]
-
-            mid_ob_link_list = cls.ob_link_list_sorted[1:-1]
-            lanes_assgined_to_each_mid_ob_link = [0] * len(mid_ob_link_list)
-            lanes_each_mid_ob_link_left = [link.incoming_lanes for link in mid_ob_link_list]
-
-            if ib_lanes - cls.default_left_most_lanes - cls.default_right_most_lanes >= len(mid_ob_link_list):
-                lanes_ib_link_left = ib_lanes - cls.default_left_most_lanes - cls.default_right_most_lanes
-                start_lane_no = cls.default_left_most_lanes
-                while (lanes_ib_link_left > 0) and (sum(lanes_each_mid_ob_link_left) > 0):
-                    for ob_link_no, ob_link in enumerate(mid_ob_link_list):
-                        if lanes_each_mid_ob_link_left[ob_link_no] == 0: continue
-                        if lanes_ib_link_left == 0: break
-                        lanes_each_mid_ob_link_left[ob_link_no] -= 1
-                        lanes_assgined_to_each_mid_ob_link[ob_link_no] += 1
-                        lanes_ib_link_left -= 1
-                for ob_link_no, ob_link in enumerate(mid_ob_link_list):
-                    cls.connection_list[cls.ob_link_list.index(ob_link)] = [
-                        (start_lane_no, start_lane_no + lanes_assgined_to_each_mid_ob_link[ob_link_no] - 1),
-                        (ob_link.incoming_lanes - lanes_assgined_to_each_mid_ob_link[ob_link_no], ob_link.incoming_lanes - 1)]
-                    start_lane_no += lanes_assgined_to_each_mid_ob_link[ob_link_no]
-            elif ib_lanes < len(mid_ob_link_list):
-                lane_no, link_no = -1, -1
-                for lane_no in range(ib_lanes-1):
-                    link_no = lane_no
-                    ob_link = mid_ob_link_list[link_no]
-                    cls.connection_list[cls.ob_link_list.index(ob_link)] = [(lane_no, lane_no), (ob_link.incoming_lanes - 1, ob_link.incoming_lanes - 1)]
-                lane_no += 1
-                start_link_no = link_no + 1
-                for link_no in range(start_link_no, len(mid_ob_link_list)):
-                    ob_link = mid_ob_link_list[link_no]
-                    cls.connection_list[cls.ob_link_list.index(ob_link)] = [(lane_no, lane_no), (ob_link.incoming_lanes - 1, ob_link.incoming_lanes - 1)]
-            else:
-                if ib_lanes - cls.default_left_most_lanes == len(mid_ob_link_list):
-                    start_lane_no = cls.default_left_most_lanes
-                else:
-                    # ib_lanes == len(mid_ob_link_list)
-                    start_lane_no = 0
-                for ob_link in mid_ob_link_list:
-                    cls.connection_list[cls.ob_link_list.index(ob_link)] = [(start_lane_no, start_lane_no), (ob_link.incoming_lanes - 1, ob_link.incoming_lanes - 1)]
-                    start_lane_no += 1
-
-            right_ob_link = cls.ob_link_list_sorted[-1]
-            cls.connection_list[cls.ob_link_list.index(right_ob_link)] = [
-                (ib_lanes - cls.default_right_most_lanes, ib_lanes - 1),
-                (right_ob_link.incoming_lanes - cls.default_right_most_lanes, right_ob_link.incoming_lanes - 1)]
-
-    @classmethod
-    def buildConnector(cls):
-        cls.getSequence()
-        cls.getLaneConnection()
-        return cls.connection_list
+from osm2gmns.utils.util_geo import getLineAngle
+
+
+class CAutoConnectorIntD:
+    default_right_most_lanes = 1        # do not change
+    default_left_most_lanes = 1         # do not change
+
+    ib_link = None
+    ob_link_list = []
+    ob_link_list_sorted = []
+    connection_list = []
+
+    @classmethod
+    def getSequence(cls):       # order outbound links from left to right
+        angle_list = []
+
+        for ob_link in cls.ob_link_list:
+            angle = getLineAngle(cls.ib_link.geometry_xy, ob_link.geometry_xy)
+            angle_list.append(angle)
+
+        cls.ob_link_list_sorted = sorted(cls.ob_link_list, key=lambda x:angle_list[cls.ob_link_list.index(x)],reverse=True)
+
+
+    @classmethod
+    def getLaneConnection(cls):
+        cls.connection_list = [[] for _ in range(len(cls.ob_link_list_sorted))]
+        ib_lanes = cls.ib_link.outgoing_lanes
+
+        if ib_lanes == 1:
+            left_ob_link = cls.ob_link_list_sorted[0]
+            cls.connection_list[cls.ob_link_list.index(left_ob_link)] = [(0, 0),(0, 0)]
+            for ob_link in cls.ob_link_list_sorted[1:]:
+                cls.connection_list[cls.ob_link_list.index(ob_link)] = [(0, 0), (ob_link.incoming_lanes-1, ob_link.incoming_lanes-1)]
+            return
+
+        if len(cls.ob_link_list_sorted) == 1:
+            # only one ob_link, full connection
+            ob_link = cls.ob_link_list_sorted[0]
+            connection_lanes = min(ib_lanes, ob_link.incoming_lanes)
+            cls.connection_list[cls.ob_link_list.index(ob_link)] = [(0, connection_lanes - 1), (0, connection_lanes - 1)]
+
+        elif len(cls.ob_link_list_sorted) == 2:
+            # two ob_link, default right, remaining left
+            left_ob_link = cls.ob_link_list_sorted[0]
+            lanes_ib_link_left = ib_lanes - cls.default_left_most_lanes
+            lanes_ob_has = left_ob_link.incoming_lanes
+            connection_lanes = min(lanes_ib_link_left,lanes_ob_has)
+            cls.connection_list[cls.ob_link_list.index(left_ob_link)] = [(0, connection_lanes - 1), (0, connection_lanes - 1)]
+
+            right_ob_link = cls.ob_link_list_sorted[-1]
+            cls.connection_list[cls.ob_link_list.index(right_ob_link)] = [
+                (ib_lanes - cls.default_right_most_lanes, ib_lanes - 1),
+                (right_ob_link.incoming_lanes - cls.default_right_most_lanes, right_ob_link.incoming_lanes - 1)]
+
+        else:
+            # >= 3, default left, default right, remaining mid
+            left_ob_link = cls.ob_link_list_sorted[0]
+            cls.connection_list[cls.ob_link_list.index(left_ob_link)] = [(0,cls.default_left_most_lanes-1), (0,cls.default_left_most_lanes-1)]
+
+            mid_ob_link_list = cls.ob_link_list_sorted[1:-1]
+            lanes_assgined_to_each_mid_ob_link = [0] * len(mid_ob_link_list)
+            lanes_each_mid_ob_link_left = [link.incoming_lanes for link in mid_ob_link_list]
+
+            if ib_lanes - cls.default_left_most_lanes - cls.default_right_most_lanes >= len(mid_ob_link_list):
+                lanes_ib_link_left = ib_lanes - cls.default_left_most_lanes - cls.default_right_most_lanes
+                start_lane_no = cls.default_left_most_lanes
+                while (lanes_ib_link_left > 0) and (sum(lanes_each_mid_ob_link_left) > 0):
+                    for ob_link_no, ob_link in enumerate(mid_ob_link_list):
+                        if lanes_each_mid_ob_link_left[ob_link_no] == 0: continue
+                        if lanes_ib_link_left == 0: break
+                        lanes_each_mid_ob_link_left[ob_link_no] -= 1
+                        lanes_assgined_to_each_mid_ob_link[ob_link_no] += 1
+                        lanes_ib_link_left -= 1
+                for ob_link_no, ob_link in enumerate(mid_ob_link_list):
+                    cls.connection_list[cls.ob_link_list.index(ob_link)] = [
+                        (start_lane_no, start_lane_no + lanes_assgined_to_each_mid_ob_link[ob_link_no] - 1),
+                        (ob_link.incoming_lanes - lanes_assgined_to_each_mid_ob_link[ob_link_no], ob_link.incoming_lanes - 1)]
+                    start_lane_no += lanes_assgined_to_each_mid_ob_link[ob_link_no]
+            elif ib_lanes < len(mid_ob_link_list):
+                lane_no, link_no = -1, -1
+                for lane_no in range(ib_lanes-1):
+                    link_no = lane_no
+                    ob_link = mid_ob_link_list[link_no]
+                    cls.connection_list[cls.ob_link_list.index(ob_link)] = [(lane_no, lane_no), (ob_link.incoming_lanes - 1, ob_link.incoming_lanes - 1)]
+                lane_no += 1
+                start_link_no = link_no + 1
+                for link_no in range(start_link_no, len(mid_ob_link_list)):
+                    ob_link = mid_ob_link_list[link_no]
+                    cls.connection_list[cls.ob_link_list.index(ob_link)] = [(lane_no, lane_no), (ob_link.incoming_lanes - 1, ob_link.incoming_lanes - 1)]
+            else:
+                if ib_lanes - cls.default_left_most_lanes == len(mid_ob_link_list):
+                    start_lane_no = cls.default_left_most_lanes
+                else:
+                    # ib_lanes == len(mid_ob_link_list)
+                    start_lane_no = 0
+                for ob_link in mid_ob_link_list:
+                    cls.connection_list[cls.ob_link_list.index(ob_link)] = [(start_lane_no, start_lane_no), (ob_link.incoming_lanes - 1, ob_link.incoming_lanes - 1)]
+                    start_lane_no += 1
+
+            right_ob_link = cls.ob_link_list_sorted[-1]
+            cls.connection_list[cls.ob_link_list.index(right_ob_link)] = [
+                (ib_lanes - cls.default_right_most_lanes, ib_lanes - 1),
+                (right_ob_link.incoming_lanes - cls.default_right_most_lanes, right_ob_link.incoming_lanes - 1)]
+
+    @classmethod
+    def buildConnector(cls):
+        cls.getSequence()
+        cls.getLaneConnection()
+        return cls.connection_list
```

### Comparing `osm2gmns-0.7.5/osm2gmns/movement/autoconm.py` & `osm2gmns-0.7.6/osm2gmns/movement/autoconm.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-from osm2gmns.utils.util_geo import getLineAngle
-
-class CAutoConnectorM:
-    default_right_most_lanes = 1        # do not change
-    default_left_most_lanes = 1         # do not change
-
-    ib_link_list = []
-    ob_link = None
-    ib_link_list_sorted = []
-    connection_list = []
-
-
-    @classmethod
-    def getSequence(cls):       # order inbound links from left to right
-        angle_list = []
-
-        for ib_link in cls.ib_link_list:
-            angle = getLineAngle(ib_link.geometry_xy, cls.ob_link.geometry_xy)
-            angle_list.append(angle)
-
-        cls.ib_link_list_sorted = sorted(cls.ib_link_list, key=lambda x:angle_list[cls.ib_link_list.index(x)],reverse=True)
-
-
-    @classmethod
-    def getLaneConnection(cls):
-        cls.connection_list = [[] for _ in range(len(cls.ib_link_list_sorted))]
-        ob_lanes = cls.ob_link.incoming_lanes
-
-        left_ib_link = cls.ib_link_list_sorted[0]
-        connection_lanes = min(ob_lanes, left_ib_link.outgoing_lanes)
-        cls.connection_list[cls.ib_link_list.index(left_ib_link)] = [(left_ib_link.outgoing_lanes-connection_lanes, left_ib_link.outgoing_lanes-1),
-                                                                     (0, connection_lanes-1)]        # in, out
-
-        for ib_link in cls.ib_link_list_sorted[1:]:
-            connection_lanes = min(ob_lanes, ib_link.outgoing_lanes)
-            cls.connection_list[cls.ib_link_list.index(ib_link)] = [(0, connection_lanes - 1), (ob_lanes-connection_lanes, ob_lanes-1)]  # in, out
-
-
-    @classmethod
-    def buildConnector(cls):
-        cls.getSequence()
-        cls.getLaneConnection()
-        return cls.connection_list
+from osm2gmns.utils.util_geo import getLineAngle
+
+class CAutoConnectorM:
+    default_right_most_lanes = 1        # do not change
+    default_left_most_lanes = 1         # do not change
+
+    ib_link_list = []
+    ob_link = None
+    ib_link_list_sorted = []
+    connection_list = []
+
+
+    @classmethod
+    def getSequence(cls):       # order inbound links from left to right
+        angle_list = []
+
+        for ib_link in cls.ib_link_list:
+            angle = getLineAngle(ib_link.geometry_xy, cls.ob_link.geometry_xy)
+            angle_list.append(angle)
+
+        cls.ib_link_list_sorted = sorted(cls.ib_link_list, key=lambda x:angle_list[cls.ib_link_list.index(x)],reverse=True)
+
+
+    @classmethod
+    def getLaneConnection(cls):
+        cls.connection_list = [[] for _ in range(len(cls.ib_link_list_sorted))]
+        ob_lanes = cls.ob_link.incoming_lanes
+
+        left_ib_link = cls.ib_link_list_sorted[0]
+        connection_lanes = min(ob_lanes, left_ib_link.outgoing_lanes)
+        cls.connection_list[cls.ib_link_list.index(left_ib_link)] = [(left_ib_link.outgoing_lanes-connection_lanes, left_ib_link.outgoing_lanes-1),
+                                                                     (0, connection_lanes-1)]        # in, out
+
+        for ib_link in cls.ib_link_list_sorted[1:]:
+            connection_lanes = min(ob_lanes, ib_link.outgoing_lanes)
+            cls.connection_list[cls.ib_link_list.index(ib_link)] = [(0, connection_lanes - 1), (ob_lanes-connection_lanes, ob_lanes-1)]  # in, out
+
+
+    @classmethod
+    def buildConnector(cls):
+        cls.getSequence()
+        cls.getLaneConnection()
+        return cls.connection_list
```

### Comparing `osm2gmns-0.7.5/osm2gmns/movement/exp_auto_connection.py` & `osm2gmns-0.7.6/osm2gmns/movement/exp_auto_connection.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,84 +1,84 @@
-# from osm2gmns.movement.util_mvmt import getLinkAngle
-from osm2gmns.utils.util_geo import getLineAngle
-from enum import Enum
-
-Direction = Enum('Direction', ('RIGHTMOST', 'LEFTMOST', 'FORWARD'))
-
-class MainDirections:
-    def __init__(self, parent, outgoing, available_lanes):
-        pass
-
-    def getStraightest(self):
-        return 0
-
-    def empty(self):
-        pass
-
-    def includes(self, d):
-        pass
-
-
-
-def _prepareLinkPriorities(current_link, outgoing, available_lanes):
-    priorities = []
-    main_directions = MainDirections(current_link, outgoing, available_lanes)
-    dist = main_directions.getStraightest()
-    if dist == -1:
-        return priorities
-
-
-
-
-
-    return 0
-
-
-def _divideOnEdges(current_link, connected_links):
-    available_lanes = list(range(current_link.lanes))
-    priorities = _prepareLinkPriorities(current_link, connected_links, available_lanes)
-
-
-
-
-def _getConnectedSorted(link):
-    connected_link_list = []
-    for outgoing_link in link.to_node.outgoing_link_list:
-        # if outgoing_link in link.forbidden_outgoing_link_list:
-        #     continue
-        if outgoing_link.to_node is link.from_node:
-            continue
-        connected_link_list.append(outgoing_link)
-
-    # no need to sort if empty or only with one element
-    if len(connected_link_list) <= 1:
-        return connected_link_list
-
-    angle_dict = {}
-    for connected_link in connected_link_list:
-        angle_dict[connected_link] = getLineAngle(link.geometry_xy,connected_link.geometry_xy)
-
-    # direction: clockwise
-    connected_link_list_sorted = sorted(connected_link_list, key=lambda x: angle_dict[x], reverse=True)
-    return connected_link_list_sorted
-
-
-def _computeLanes2Edges_(current_link):
-    connected_links = _getConnectedSorted(current_link)
-    if connected_links:
-        _divideOnEdges(current_link, connected_links)
-
-
-def _computeLanes2Edges(link_dict, processed_node_set):
-    for link_id, link in link_dict.items():
-        if link.to_node.node_id in processed_node_set:
-            continue
-        _computeLanes2Edges_(link)
-
-
-def _computeLanes2Lanes(net):
-    pass
-
-
-def guessMovements(net, processed_node_set):
-    _computeLanes2Edges(net.link_dict, processed_node_set)
+# from osm2gmns.movement.util_mvmt import getLinkAngle
+from osm2gmns.utils.util_geo import getLineAngle
+from enum import Enum
+
+Direction = Enum('Direction', ('RIGHTMOST', 'LEFTMOST', 'FORWARD'))
+
+class MainDirections:
+    def __init__(self, parent, outgoing, available_lanes):
+        pass
+
+    def getStraightest(self):
+        return 0
+
+    def empty(self):
+        pass
+
+    def includes(self, d):
+        pass
+
+
+
+def _prepareLinkPriorities(current_link, outgoing, available_lanes):
+    priorities = []
+    main_directions = MainDirections(current_link, outgoing, available_lanes)
+    dist = main_directions.getStraightest()
+    if dist == -1:
+        return priorities
+
+
+
+
+
+    return 0
+
+
+def _divideOnEdges(current_link, connected_links):
+    available_lanes = list(range(current_link.lanes))
+    priorities = _prepareLinkPriorities(current_link, connected_links, available_lanes)
+
+
+
+
+def _getConnectedSorted(link):
+    connected_link_list = []
+    for outgoing_link in link.to_node.outgoing_link_list:
+        # if outgoing_link in link.forbidden_outgoing_link_list:
+        #     continue
+        if outgoing_link.to_node is link.from_node:
+            continue
+        connected_link_list.append(outgoing_link)
+
+    # no need to sort if empty or only with one element
+    if len(connected_link_list) <= 1:
+        return connected_link_list
+
+    angle_dict = {}
+    for connected_link in connected_link_list:
+        angle_dict[connected_link] = getLineAngle(link.geometry_xy,connected_link.geometry_xy)
+
+    # direction: clockwise
+    connected_link_list_sorted = sorted(connected_link_list, key=lambda x: angle_dict[x], reverse=True)
+    return connected_link_list_sorted
+
+
+def _computeLanes2Edges_(current_link):
+    connected_links = _getConnectedSorted(current_link)
+    if connected_links:
+        _divideOnEdges(current_link, connected_links)
+
+
+def _computeLanes2Edges(link_dict, processed_node_set):
+    for link_id, link in link_dict.items():
+        if link.to_node.node_id in processed_node_set:
+            continue
+        _computeLanes2Edges_(link)
+
+
+def _computeLanes2Lanes(net):
+    pass
+
+
+def guessMovements(net, processed_node_set):
+    _computeLanes2Edges(net.link_dict, processed_node_set)
     _computeLanes2Lanes(net)
```

### Comparing `osm2gmns-0.7.5/osm2gmns/movement/generate_movements.py` & `osm2gmns-0.7.6/osm2gmns/movement/generate_movements.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,179 +1,179 @@
-from osm2gmns.movement.autoconintd import CAutoConnectorIntD
-from osm2gmns.movement.autoconm import CAutoConnectorM
-from osm2gmns.movement.util_mvmt import getMovementDescription, getMovementGeometry
-from osm2gmns.networkclass.macronet import Movement
-import osm2gmns.settings as og_settings
-
-
-def _generateMovementsForOneNode(node, max_movement_id, GT):
-    number_of_incoming_links = len(node.incoming_link_list)
-    number_of_outgoing_links = len(node.outgoing_link_list)
-
-    if number_of_incoming_links == 0 or number_of_outgoing_links == 0: return
-
-    movement_id = max_movement_id
-
-    if number_of_outgoing_links == 1:
-        # merge
-        ob_link = node.outgoing_link_list[0]
-        ib_link_list = []
-        for ib_link in node.incoming_link_list:
-            if ib_link.from_node.node_id != ob_link.to_node.node_id:
-                ib_link_list.append(ib_link)
-
-        if len(ib_link_list) == 0: return
-
-        CAutoConnectorM.ob_link, CAutoConnectorM.ib_link_list = ob_link, ib_link_list
-        connection_list = CAutoConnectorM.buildConnector()
-
-        for ib_link_no, ib_link in enumerate(ib_link_list):
-            ib_lane_index_start = connection_list[ib_link_no][0][0]
-            ib_lane_index_end = connection_list[ib_link_no][0][1]
-            ob_lane_index_start = connection_list[ib_link_no][1][0]
-            ob_lane_index_end = connection_list[ib_link_no][1][1]
-            number_of_lanes = ib_lane_index_end - ib_lane_index_start + 1
-
-            mvmt = Movement(movement_id)
-            mvmt.node = node
-            mvmt.ib_link = ib_link
-            mvmt.ob_link = ob_link
-            mvmt.start_ib_lane_seq_no, mvmt.end_ib_lane_seq_no = ib_lane_index_start, ib_lane_index_end
-            mvmt.start_ob_lane_seq_no, mvmt.end_ob_lane_seq_no = ob_lane_index_start, ob_lane_index_end
-            mvmt.start_ib_lane, mvmt.end_ib_lane = ib_link.outgoing_lane_indices[ib_lane_index_start], ib_link.outgoing_lane_indices[ib_lane_index_end]
-            mvmt.start_ob_lane, mvmt.end_ob_lane = ob_link.incoming_lane_indices[ob_lane_index_start], ob_link.incoming_lane_indices[ob_lane_index_end]
-            mvmt.lanes = number_of_lanes
-            mvmt_txt_id, mvmt_type = getMovementDescription(ib_link, ob_link)
-            mvmt.mvmt_txt_id = mvmt_txt_id
-            mvmt.type = mvmt_type
-            mvmt.geometry_xy = getMovementGeometry(ib_link, ob_link)
-            mvmt.geometry = GT.geo_to_latlon(mvmt.geometry_xy)
-            mvmt.generated_by_osm2gmns = True
-
-            if node.ctrl_type == 1: mvmt.ctrl_type = 'signal'               # todo: check ctrl_type
-            mvmt.allowed_uses = ib_link.allowed_uses
-            node.movement_list.append(mvmt)
-            movement_id += 1
-    else:
-        # diverge and intersections
-        for ib_link in node.incoming_link_list:
-            ob_link_list = []
-            for ob_link in node.outgoing_link_list:
-                if ib_link.from_node.node_id != ob_link.to_node.node_id:
-                    ob_link_list.append(ob_link)
-
-            if len(ob_link_list) == 0: continue
-
-            CAutoConnectorIntD.ib_link, CAutoConnectorIntD.ob_link_list = ib_link, ob_link_list
-            connection_list = CAutoConnectorIntD.buildConnector()
-
-            for ob_link_no, ob_link in enumerate(ob_link_list):
-                ib_lane_index_start = connection_list[ob_link_no][0][0]
-                ib_lane_index_end = connection_list[ob_link_no][0][1]
-                ob_lane_index_start = connection_list[ob_link_no][1][0]
-                ob_lane_index_end = connection_list[ob_link_no][1][1]
-                number_of_lanes = ib_lane_index_end - ib_lane_index_start + 1
-
-                mvmt = Movement(movement_id)
-                mvmt.node = node
-                mvmt.ib_link = ib_link
-                mvmt.ob_link = ob_link
-                mvmt.start_ib_lane_seq_no, mvmt.end_ib_lane_seq_no = ib_lane_index_start, ib_lane_index_end
-                mvmt.start_ob_lane_seq_no, mvmt.end_ob_lane_seq_no = ob_lane_index_start, ob_lane_index_end
-                mvmt.start_ib_lane, mvmt.end_ib_lane = ib_link.outgoing_lane_indices[ib_lane_index_start], ib_link.outgoing_lane_indices[ib_lane_index_end]
-                mvmt.start_ob_lane, mvmt.end_ob_lane = ob_link.incoming_lane_indices[ob_lane_index_start], ob_link.incoming_lane_indices[ob_lane_index_end]
-                mvmt.lanes = number_of_lanes
-                mvmt_txt_id, mvmt_type = getMovementDescription(ib_link, ob_link)
-                mvmt.mvmt_txt_id = mvmt_txt_id
-                mvmt.type = mvmt_type
-                mvmt.geometry_xy = getMovementGeometry(ib_link, ob_link)
-                mvmt.geometry = GT.geo_to_latlon(mvmt.geometry_xy)
-                mvmt.generated_by_osm2gmns = True
-
-                if node.ctrl_type == 1: mvmt.ctrl_type = 'signal'
-                mvmt.allowed_uses = ib_link.allowed_uses
-                node.movement_list.append(mvmt)
-                movement_id += 1
-
-
-def validateUserInputMovements(network):
-    for movement in network.user_input_movement_list:
-        ib_link, ob_link = movement.ib_link, movement.ob_link
-
-        if movement.start_ib_lane not in ib_link.outgoing_lane_indices:
-            print(f'WARNING: start_ib_lane of movement {movement.movement_id} does not belong to ib_link {ib_link.link_id} outgoing lane indices {ib_link.outgoing_lane_indices}')
-            continue
-        start_ib_lane_seq_no = ib_link.outgoing_lane_indices.index(movement.start_ib_lane)
-
-        if movement.end_ib_lane not in ib_link.outgoing_lane_indices:
-            print(f'WARNING: end_ib_lane of movement {movement.movement_id} does not belong to ib_link {ib_link.link_id} outgoing lane indices {ib_link.outgoing_lane_indices}')
-            continue
-        end_ib_lane_seq_no = ib_link.outgoing_lane_indices.index(movement.end_ib_lane)
-
-        if movement.start_ob_lane not in ob_link.incoming_lane_indices:
-            print(f'WARNING: start_ob_lane of movement {movement.movement_id} does not belong to ob_link {ob_link.link_id} incoming lane indices {ob_link.incoming_lane_indices}')
-            continue
-        start_ob_lane_seq_no = ob_link.incoming_lane_indices.index(movement.start_ob_lane)
-
-        if movement.end_ob_lane not in ob_link.incoming_lane_indices:
-            print(f'WARNING: end_ob_lane of movement {movement.movement_id} does not belong to ob_link {ob_link.link_id} incoming lane indices {ob_link.incoming_lane_indices}')
-            continue
-        end_ob_lane_seq_no = ob_link.incoming_lane_indices.index(movement.end_ob_lane)
-
-        ib_lanes, ob_lanes = end_ib_lane_seq_no - start_ib_lane_seq_no + 1, end_ob_lane_seq_no - start_ob_lane_seq_no + 1
-
-        if ib_lanes < ob_lanes:
-            end_ob_lane_seq_no -= (ob_lanes - ib_lanes)
-            end_ob_lane = ob_link.incoming_lane_indices[end_ob_lane_seq_no]
-            print(f'WARNING: movement {movement.movement_id} - number of ib lanes ({ib_lanes}) is less than that of ob lanes ({ob_lanes}), end_ob_lane is changed to {end_ob_lane}')
-            movement.lanes = ib_lanes
-        elif ib_lanes > ob_lanes:
-            end_ib_lane_seq_no -= (ib_lanes - ob_lanes)
-            end_ib_lane = ib_link.outgoing_lane_indices[end_ib_lane_seq_no]
-            print(f'WARNING: movement {movement.movement_id} - number of ib lanes ({ib_lanes}) is more than that of ob lanes ({ob_lanes}), end_ib_lane is changed to {end_ib_lane}')
-            movement.lanes = ob_lanes
-        else:
-            movement.lanes = ib_lanes
-
-        movement.end_ib_lane, movement.start_ib_lane_seq_no, movement.end_ib_lane_seq_no = movement.end_ib_lane, start_ib_lane_seq_no, end_ib_lane_seq_no
-        movement.end_ob_lane, movement.start_ob_lane_seq_no, movement.end_ob_lane_seq_no = movement.end_ob_lane, start_ob_lane_seq_no, end_ob_lane_seq_no
-        movement.node.movement_list.append(movement)
-
-
-def generateMovements(network):
-    """
-    Use osm2gmns built-in methods to generate movements for each node (intersection) in a network
-
-    Parameters
-    ----------
-    network: Network
-        an osm2gmns Network object
-
-    Returns
-    -------
-    None
-    """
-
-    if og_settings.verbose:
-        print('Generating Movements')
-
-    if not network.complete_link_lane_info:
-        print('WARNING: Movement generation will be skipped because some links do not have lanes information.\n'
-              '         If the network is parsed from a OSM file, set "default_lanes" as "True" when parsing networks to assign default lanes for links without lanes information.\n'
-              '         If the network is loaded from a CSV file, make sure all links have lanes information before loading the network.')
-        return
-
-    for _, link in network.link_dict.items():
-        link.linkLaneListFromSegment()
-
-    validateUserInputMovements(network)
-
-    max_movement_id = network.max_movement_id
-    for node_id, node in network.node_dict.items():
-
-        if node.movement_list:
-            continue
-
-        _generateMovementsForOneNode(node, max_movement_id, network.GT)
-        max_movement_id += len(node.movement_list)
-
-    network.max_movement_id = max_movement_id
+from osm2gmns.movement.autoconintd import CAutoConnectorIntD
+from osm2gmns.movement.autoconm import CAutoConnectorM
+from osm2gmns.movement.util_mvmt import getMovementDescription, getMovementGeometry
+from osm2gmns.networkclass.macronet import Movement
+import osm2gmns.settings as og_settings
+
+
+def _generateMovementsForOneNode(node, max_movement_id, GT):
+    number_of_incoming_links = len(node.incoming_link_list)
+    number_of_outgoing_links = len(node.outgoing_link_list)
+
+    if number_of_incoming_links == 0 or number_of_outgoing_links == 0: return
+
+    movement_id = max_movement_id
+
+    if number_of_outgoing_links == 1:
+        # merge
+        ob_link = node.outgoing_link_list[0]
+        ib_link_list = []
+        for ib_link in node.incoming_link_list:
+            if ib_link.from_node.node_id != ob_link.to_node.node_id:
+                ib_link_list.append(ib_link)
+
+        if len(ib_link_list) == 0: return
+
+        CAutoConnectorM.ob_link, CAutoConnectorM.ib_link_list = ob_link, ib_link_list
+        connection_list = CAutoConnectorM.buildConnector()
+
+        for ib_link_no, ib_link in enumerate(ib_link_list):
+            ib_lane_index_start = connection_list[ib_link_no][0][0]
+            ib_lane_index_end = connection_list[ib_link_no][0][1]
+            ob_lane_index_start = connection_list[ib_link_no][1][0]
+            ob_lane_index_end = connection_list[ib_link_no][1][1]
+            number_of_lanes = ib_lane_index_end - ib_lane_index_start + 1
+
+            mvmt = Movement(movement_id)
+            mvmt.node = node
+            mvmt.ib_link = ib_link
+            mvmt.ob_link = ob_link
+            mvmt.start_ib_lane_seq_no, mvmt.end_ib_lane_seq_no = ib_lane_index_start, ib_lane_index_end
+            mvmt.start_ob_lane_seq_no, mvmt.end_ob_lane_seq_no = ob_lane_index_start, ob_lane_index_end
+            mvmt.start_ib_lane, mvmt.end_ib_lane = ib_link.outgoing_lane_indices[ib_lane_index_start], ib_link.outgoing_lane_indices[ib_lane_index_end]
+            mvmt.start_ob_lane, mvmt.end_ob_lane = ob_link.incoming_lane_indices[ob_lane_index_start], ob_link.incoming_lane_indices[ob_lane_index_end]
+            mvmt.lanes = number_of_lanes
+            mvmt_txt_id, mvmt_type = getMovementDescription(ib_link, ob_link)
+            mvmt.mvmt_txt_id = mvmt_txt_id
+            mvmt.type = mvmt_type
+            mvmt.geometry_xy = getMovementGeometry(ib_link, ob_link)
+            mvmt.geometry = GT.geo_to_latlon(mvmt.geometry_xy)
+            mvmt.generated_by_osm2gmns = True
+
+            if node.ctrl_type == 1: mvmt.ctrl_type = 'signal'               # todo: check ctrl_type
+            mvmt.allowed_uses = ib_link.allowed_uses
+            node.movement_list.append(mvmt)
+            movement_id += 1
+    else:
+        # diverge and intersections
+        for ib_link in node.incoming_link_list:
+            ob_link_list = []
+            for ob_link in node.outgoing_link_list:
+                if ib_link.from_node.node_id != ob_link.to_node.node_id:
+                    ob_link_list.append(ob_link)
+
+            if len(ob_link_list) == 0: continue
+
+            CAutoConnectorIntD.ib_link, CAutoConnectorIntD.ob_link_list = ib_link, ob_link_list
+            connection_list = CAutoConnectorIntD.buildConnector()
+
+            for ob_link_no, ob_link in enumerate(ob_link_list):
+                ib_lane_index_start = connection_list[ob_link_no][0][0]
+                ib_lane_index_end = connection_list[ob_link_no][0][1]
+                ob_lane_index_start = connection_list[ob_link_no][1][0]
+                ob_lane_index_end = connection_list[ob_link_no][1][1]
+                number_of_lanes = ib_lane_index_end - ib_lane_index_start + 1
+
+                mvmt = Movement(movement_id)
+                mvmt.node = node
+                mvmt.ib_link = ib_link
+                mvmt.ob_link = ob_link
+                mvmt.start_ib_lane_seq_no, mvmt.end_ib_lane_seq_no = ib_lane_index_start, ib_lane_index_end
+                mvmt.start_ob_lane_seq_no, mvmt.end_ob_lane_seq_no = ob_lane_index_start, ob_lane_index_end
+                mvmt.start_ib_lane, mvmt.end_ib_lane = ib_link.outgoing_lane_indices[ib_lane_index_start], ib_link.outgoing_lane_indices[ib_lane_index_end]
+                mvmt.start_ob_lane, mvmt.end_ob_lane = ob_link.incoming_lane_indices[ob_lane_index_start], ob_link.incoming_lane_indices[ob_lane_index_end]
+                mvmt.lanes = number_of_lanes
+                mvmt_txt_id, mvmt_type = getMovementDescription(ib_link, ob_link)
+                mvmt.mvmt_txt_id = mvmt_txt_id
+                mvmt.type = mvmt_type
+                mvmt.geometry_xy = getMovementGeometry(ib_link, ob_link)
+                mvmt.geometry = GT.geo_to_latlon(mvmt.geometry_xy)
+                mvmt.generated_by_osm2gmns = True
+
+                if node.ctrl_type == 1: mvmt.ctrl_type = 'signal'
+                mvmt.allowed_uses = ib_link.allowed_uses
+                node.movement_list.append(mvmt)
+                movement_id += 1
+
+
+def validateUserInputMovements(network):
+    for movement in network.user_input_movement_list:
+        ib_link, ob_link = movement.ib_link, movement.ob_link
+
+        if movement.start_ib_lane not in ib_link.outgoing_lane_indices:
+            print(f'WARNING: start_ib_lane of movement {movement.movement_id} does not belong to ib_link {ib_link.link_id} outgoing lane indices {ib_link.outgoing_lane_indices}')
+            continue
+        start_ib_lane_seq_no = ib_link.outgoing_lane_indices.index(movement.start_ib_lane)
+
+        if movement.end_ib_lane not in ib_link.outgoing_lane_indices:
+            print(f'WARNING: end_ib_lane of movement {movement.movement_id} does not belong to ib_link {ib_link.link_id} outgoing lane indices {ib_link.outgoing_lane_indices}')
+            continue
+        end_ib_lane_seq_no = ib_link.outgoing_lane_indices.index(movement.end_ib_lane)
+
+        if movement.start_ob_lane not in ob_link.incoming_lane_indices:
+            print(f'WARNING: start_ob_lane of movement {movement.movement_id} does not belong to ob_link {ob_link.link_id} incoming lane indices {ob_link.incoming_lane_indices}')
+            continue
+        start_ob_lane_seq_no = ob_link.incoming_lane_indices.index(movement.start_ob_lane)
+
+        if movement.end_ob_lane not in ob_link.incoming_lane_indices:
+            print(f'WARNING: end_ob_lane of movement {movement.movement_id} does not belong to ob_link {ob_link.link_id} incoming lane indices {ob_link.incoming_lane_indices}')
+            continue
+        end_ob_lane_seq_no = ob_link.incoming_lane_indices.index(movement.end_ob_lane)
+
+        ib_lanes, ob_lanes = end_ib_lane_seq_no - start_ib_lane_seq_no + 1, end_ob_lane_seq_no - start_ob_lane_seq_no + 1
+
+        if ib_lanes < ob_lanes:
+            end_ob_lane_seq_no -= (ob_lanes - ib_lanes)
+            end_ob_lane = ob_link.incoming_lane_indices[end_ob_lane_seq_no]
+            print(f'WARNING: movement {movement.movement_id} - number of ib lanes ({ib_lanes}) is less than that of ob lanes ({ob_lanes}), end_ob_lane is changed to {end_ob_lane}')
+            movement.lanes = ib_lanes
+        elif ib_lanes > ob_lanes:
+            end_ib_lane_seq_no -= (ib_lanes - ob_lanes)
+            end_ib_lane = ib_link.outgoing_lane_indices[end_ib_lane_seq_no]
+            print(f'WARNING: movement {movement.movement_id} - number of ib lanes ({ib_lanes}) is more than that of ob lanes ({ob_lanes}), end_ib_lane is changed to {end_ib_lane}')
+            movement.lanes = ob_lanes
+        else:
+            movement.lanes = ib_lanes
+
+        movement.end_ib_lane, movement.start_ib_lane_seq_no, movement.end_ib_lane_seq_no = movement.end_ib_lane, start_ib_lane_seq_no, end_ib_lane_seq_no
+        movement.end_ob_lane, movement.start_ob_lane_seq_no, movement.end_ob_lane_seq_no = movement.end_ob_lane, start_ob_lane_seq_no, end_ob_lane_seq_no
+        movement.node.movement_list.append(movement)
+
+
+def generateMovements(network):
+    """
+    Use osm2gmns built-in methods to generate movements for each node (intersection) in a network
+
+    Parameters
+    ----------
+    network: Network
+        an osm2gmns Network object
+
+    Returns
+    -------
+    None
+    """
+
+    if og_settings.verbose:
+        print('Generating Movements')
+
+    if not network.complete_link_lane_info:
+        print('WARNING: Movement generation will be skipped because some links do not have lanes information.\n'
+              '         If the network is parsed from a OSM file, set "default_lanes" as "True" when parsing networks to assign default lanes for links without lanes information.\n'
+              '         If the network is loaded from a CSV file, make sure all links have lanes information before loading the network.')
+        return
+
+    for _, link in network.link_dict.items():
+        link.linkLaneListFromSegment()
+
+    validateUserInputMovements(network)
+
+    max_movement_id = network.max_movement_id
+    for node_id, node in network.node_dict.items():
+
+        if node.movement_list:
+            continue
+
+        _generateMovementsForOneNode(node, max_movement_id, network.GT)
+        max_movement_id += len(node.movement_list)
+
+    network.max_movement_id = max_movement_id
```

### Comparing `osm2gmns-0.7.5/osm2gmns/movement/util_mvmt.py` & `osm2gmns-0.7.6/osm2gmns/movement/util_mvmt.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-import math
-from shapely import geometry
-
-_indent = 8.0
-
-
-def getMovementDescription(ib_link, ob_link):
-    ib_start, ib_end = ib_link.geometry_xy.coords[0], ib_link.geometry_xy.coords[-1]
-    ob_end = ob_link.geometry_xy.coords[-1]
-
-    angle_ib = math.atan2(ib_end[1] - ib_start[1], ib_end[0] - ib_start[0])
-    if -0.75 * math.pi <= angle_ib < -0.25 * math.pi:
-        direction = 'SB'
-    elif -0.25 * math.pi <= angle_ib < 0.25 * math.pi:
-        direction = 'EB'
-    elif 0.25 * math.pi <= angle_ib < 0.75 * math.pi:
-        direction = 'NB'
-    else:
-        direction = 'WB'
-
-    angle_ob = math.atan2(ob_end[1] - ib_end[1], ob_end[0] - ib_end[0])
-    angle = angle_ob - angle_ib
-    if angle < -1 * math.pi:
-        angle += 2 * math.pi
-    if angle > math.pi:
-        angle -= 2 * math.pi
-
-    if -0.25 * math.pi <= angle <= 0.25 * math.pi:
-        mvmt = 'T'
-        mvmt_type = 'thru'
-    elif angle < -0.25 * math.pi:
-        mvmt = 'R'
-        mvmt_type = 'right'
-    elif angle <= 0.75 * math.pi:
-        mvmt = 'L'
-        mvmt_type = 'left'
-    else:
-        mvmt = 'U'
-        mvmt_type = 'uturn'
-
-    mvmt_txt_id = direction + mvmt
-    return mvmt_txt_id, mvmt_type
-
-
-def getMovementGeometry(ib_link, ob_link):
-    ib_geometry_xy = ib_link.geometry_xy
-    ib_indent = _indent if ib_geometry_xy.length > _indent else ib_geometry_xy.length / 2
-    ib_point = ib_geometry_xy.interpolate(-1 * ib_indent)
-
-    ob_geometry_xy = ob_link.geometry_xy
-    ob_indent = _indent if ob_geometry_xy.length > _indent else ob_geometry_xy.length / 2
-    ob_point = ob_geometry_xy.interpolate(ob_indent)
-
-    geometry_xy = geometry.LineString([ib_point, ob_point])
-    return geometry_xy
-
-
+import math
+from shapely import geometry
+
+_indent = 8.0
+
+
+def getMovementDescription(ib_link, ob_link):
+    ib_start, ib_end = ib_link.geometry_xy.coords[0], ib_link.geometry_xy.coords[-1]
+    ob_end = ob_link.geometry_xy.coords[-1]
+
+    angle_ib = math.atan2(ib_end[1] - ib_start[1], ib_end[0] - ib_start[0])
+    if -0.75 * math.pi <= angle_ib < -0.25 * math.pi:
+        direction = 'SB'
+    elif -0.25 * math.pi <= angle_ib < 0.25 * math.pi:
+        direction = 'EB'
+    elif 0.25 * math.pi <= angle_ib < 0.75 * math.pi:
+        direction = 'NB'
+    else:
+        direction = 'WB'
+
+    angle_ob = math.atan2(ob_end[1] - ib_end[1], ob_end[0] - ib_end[0])
+    angle = angle_ob - angle_ib
+    if angle < -1 * math.pi:
+        angle += 2 * math.pi
+    if angle > math.pi:
+        angle -= 2 * math.pi
+
+    if -0.25 * math.pi <= angle <= 0.25 * math.pi:
+        mvmt = 'T'
+        mvmt_type = 'thru'
+    elif angle < -0.25 * math.pi:
+        mvmt = 'R'
+        mvmt_type = 'right'
+    elif angle <= 0.75 * math.pi:
+        mvmt = 'L'
+        mvmt_type = 'left'
+    else:
+        mvmt = 'U'
+        mvmt_type = 'uturn'
+
+    mvmt_txt_id = direction + mvmt
+    return mvmt_txt_id, mvmt_type
+
+
+def getMovementGeometry(ib_link, ob_link):
+    ib_geometry_xy = ib_link.geometry_xy
+    ib_indent = _indent if ib_geometry_xy.length > _indent else ib_geometry_xy.length / 2
+    ib_point = ib_geometry_xy.interpolate(-1 * ib_indent)
+
+    ob_geometry_xy = ob_link.geometry_xy
+    ob_indent = _indent if ob_geometry_xy.length > _indent else ob_geometry_xy.length / 2
+    ob_point = ob_geometry_xy.interpolate(ob_indent)
+
+    geometry_xy = geometry.LineString([ib_point, ob_point])
+    return geometry_xy
+
+
```

### Comparing `osm2gmns-0.7.5/osm2gmns/multiresolutionnet/build_mrnet.py` & `osm2gmns-0.7.6/osm2gmns/multiresolutionnet/build_mrnet.py`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,281 +1,281 @@
-# @author       Jiawei Lu (jiaweil9@asu.edu)
-# @time         2021/11/27 12:05
-# @desc         [script description]
-import copy
-
-from osm2gmns.networkclass.macronet import Network
-from osm2gmns.multiresolutionnet.netgen import NetGenerator
-from osm2gmns.movement.generate_movements import generateMovements, validateUserInputMovements
-from osm2gmns.utils.util_geo import getLineAngle, offsetLine
-import osm2gmns.settings as og_settings
-from shapely import geometry
-from shapely.ops import substring
-import math
-
-
-# todo: connector and centroid
-
-_length_of_short_cut = 0.1
-_length_of_cut = {0: 2.0, 1: 8.0, 2: 12.0, 3: 14.0, 4: 16.0, 5: 18.0, 6: 20, 7:22, 8:24}  # e.g. 2:8.0 cut 8 meters if the original macro link has 2 lanes, etc
-for i_ in range(9,100): _length_of_cut[i_] = 25
-_minimum_cutted_length = 2.0
-
-
-def _checkMovementLinkNecessity(node_dict):
-    for node_id, node in node_dict.items():
-        if node.ctrl_type == 'signal': continue
-
-        if len(node.incoming_link_list) == 1 and len(node.outgoing_link_list) >= 1:
-            # one imcoming link
-            ib_link = node.incoming_link_list[0]
-
-            angle_flag = True
-            for ob_link in node.outgoing_link_list:
-                angle = getLineAngle(ib_link.geometry_xy, ob_link.geometry_xy)
-                if angle > 0.75 * math.pi or angle < -0.75 * math.pi:
-                    angle_flag = False
-                    break
-            if not angle_flag: continue
-
-            ob_link_set = set()
-            multiple_connection = False
-            for movement in node.movement_list:
-                if movement.ob_link in ob_link_set:
-                    multiple_connection = True
-                    break
-                else:
-                    ob_link_set.add(movement.ob_link)
-            if multiple_connection: continue
-
-            node.movement_link_needed = False
-            ib_link.downstream_short_cut = True
-            ib_link.downstream_is_target = True
-            for ob_link in node.outgoing_link_list:
-                ob_link.upstream_short_cut = True
-
-        elif len(node.outgoing_link_list) == 1 and len(node.incoming_link_list) >= 1:
-            # one outgoing link
-            ob_link = node.outgoing_link_list[0]
-
-            angle_flag = True
-            for ib_link in node.incoming_link_list:
-                angle = getLineAngle(ib_link.geometry_xy, ob_link.geometry_xy)
-                if angle > 0.75 * math.pi or angle < -0.75 * math.pi:
-                    angle_flag = False
-                    break
-            if not angle_flag: continue
-
-            ib_link_set = set()
-            multiple_connection = False
-            for movement in node.movement_list:
-                if movement.ib_link in ib_link_set:
-                    multiple_connection = True
-                    break
-                else:
-                    ib_link_set.add(movement.ib_link)
-            if multiple_connection: continue
-
-            node.movement_link_needed = False
-
-            ob_link.upstream_short_cut = True
-            ob_link.upstream_is_target = True
-            for ib_link in node.incoming_link_list:
-                ib_link.downstream_short_cut = True
-
-
-def _offsetLinkGeometry(link_dict, width_of_lane, GT):
-    # check if a link needs offset
-    link_offset_dict = {}
-    link_ids = tuple(link_dict.keys())
-    for link_no_a, link_id_a in enumerate(link_ids):
-        link_a = link_dict[link_id_a]
-        if link_a in link_offset_dict.keys():
-            continue
-        geometry_xy_a_r = geometry.LineString(list(link_a.geometry_xy.coords)[::-1])
-        reversed_link_found = False
-        for link_id_b in link_ids[link_no_a+1:]:
-            link_b = link_dict[link_id_b]
-            if geometry_xy_a_r.equals_exact(link_b.geometry_xy, tolerance=0.1):
-                reversed_link_found = True
-                link_offset_dict[link_a] = True
-                link_offset_dict[link_b] = True
-                break
-        if not reversed_link_found:
-            link_offset_dict[link_a] = False
-
-    # offset links
-    for link, need_offset in link_offset_dict.items():
-        if need_offset:
-            offset_distance = (link.max_lanes / 2 + 0.5) * width_of_lane
-            geometry_xy_offset = link.geometry_xy.offset_curve(distance=-1*offset_distance, join_style=2)
-            if isinstance(geometry_xy_offset, geometry.MultiLineString):
-                link.geometry_xy_offset = offsetLine(link.geometry_xy, offset_distance)
-            else:
-                link.geometry_xy_offset = geometry_xy_offset
-
-
-
-            # offset_distance = (link.max_lanes / 2 + 0.5) * width_of_lane
-            # geometry_xy_offset_ = link.geometry_xy.parallel_offset(distance=offset_distance, side='right', join_style=2)
-            # if isinstance(geometry_xy_offset_, geometry.MultiLineString):
-            #     link.geometry_xy_offset = offsetLine(link.geometry_xy, offset_distance)
-            # else:
-            #     link.geometry_xy_offset = geometry.LineString(list(geometry_xy_offset_.coords)[::-1])
-
-
-            link.geometry_offset = GT.geo_to_latlon(link.geometry_xy_offset)
-        else:
-            link.geometry_offset = link.geometry
-            link.geometry_xy_offset = link.geometry_xy
-
-    # update breakpoints due to the change of geometry
-    for link_id, link in link_dict.items():
-        link.lanes_change_point_list = [item / link.length * link.length_offset for item in link.lanes_change_point_list]
-
-
-def _linkLengthToCut(link):
-    # should not change number of lanes at the two ends of a macro link
-    upstream_max_cut = max(_length_of_short_cut, link.lanes_change_point_list[1] - link.lanes_change_point_list[0] - 3)
-    downstream_max_cut = max(_length_of_short_cut, link.lanes_change_point_list[-1] - link.lanes_change_point_list[-2] - 3)
-
-    if link.upstream_short_cut and link.downstream_short_cut:
-        total_length_needed = 2 * _length_of_short_cut + _minimum_cutted_length
-        if link.length_offset > total_length_needed:
-            link.length_of_cut_upstream = _length_of_short_cut
-            link.length_of_cut_downstream = _length_of_short_cut
-        else:
-            link.length_of_cut_upstream = link.length_offset / total_length_needed * _length_of_short_cut
-            link.length_of_cut_downstream = link.length_offset / total_length_needed * _length_of_short_cut
-
-    elif link.upstream_short_cut:
-        length_found = False
-        ii = 0
-        for i in range(link.lanes_list[-1], -1, -1):
-            if link.length_offset > min(downstream_max_cut, _length_of_cut[i]) + _length_of_short_cut + _minimum_cutted_length:
-                ii = i
-                length_found = True
-                break
-
-        if length_found:
-            link.length_of_cut_upstream = _length_of_short_cut
-            link.length_of_cut_downstream = min(downstream_max_cut, _length_of_cut[ii])
-        else:
-            downstream_needed = min(downstream_max_cut, _length_of_cut[0])
-            total_length_needed = downstream_needed + _length_of_short_cut + _minimum_cutted_length
-            link.length_of_cut_upstream = link.length_offset / total_length_needed * _length_of_short_cut
-            link.length_of_cut_downstream = link.length_offset / total_length_needed * downstream_needed
-
-    elif link.downstream_short_cut:
-        length_found = False
-        ii = 0
-        for i in range(link.lanes_list[-1], -1, -1):
-            if link.length_offset > min(upstream_max_cut, _length_of_cut[i]) + _length_of_short_cut + _minimum_cutted_length:
-                ii = i
-                length_found = True
-                break
-
-        if length_found:
-            link.length_of_cut_upstream = min(upstream_max_cut, _length_of_cut[ii])
-            link.length_of_cut_downstream = _length_of_short_cut
-        else:
-            upstream_needed = min(upstream_max_cut, _length_of_cut[0])
-            total_length_needed = upstream_needed + _length_of_short_cut + _minimum_cutted_length
-            link.length_of_cut_upstream = link.length_offset / total_length_needed * _length_of_cut[0]
-            link.length_of_cut_downstream = link.length_offset / total_length_needed * _length_of_short_cut
-
-    else:
-        length_found = False
-        ii = 0
-        for i in range(link.lanes_list[-1], -1, -1):
-            if link.length_offset > min(upstream_max_cut, _length_of_cut[i]) + min(downstream_max_cut, _length_of_cut[i]) + _minimum_cutted_length:
-                ii = i
-                length_found = True
-                break
-
-        if length_found:
-            link.length_of_cut_upstream = min(upstream_max_cut, _length_of_cut[ii])
-            link.length_of_cut_downstream = min(downstream_max_cut, _length_of_cut[ii])
-        else:
-            upstream_needed = min(upstream_max_cut, _length_of_cut[0])
-            downstream_needed = min(downstream_max_cut, _length_of_cut[0])
-            total_length_needed = downstream_needed + upstream_needed + _minimum_cutted_length
-            link.length_of_cut_upstream = link.length_offset / total_length_needed * upstream_needed
-            link.length_of_cut_downstream = link.length_offset / total_length_needed * downstream_needed
-
-
-def _performLinkCut(link, GT):
-    link.cutted_lanes_change_point_list = link.lanes_change_point_list.copy()
-    link.cutted_lanes_list = link.lanes_list.copy()
-    link.cutted_lanes_change_list = link.lanes_change_list.copy()
-
-    link.cutted_lanes_change_point_list[0], link.cutted_lanes_change_point_list[-1] = link.length_of_cut_upstream, link.length_offset - link.length_of_cut_downstream
-
-    for i in range(len(link.cutted_lanes_list)):
-        start_position = link.cutted_lanes_change_point_list[i]
-        end_position = link.cutted_lanes_change_point_list[i+1]
-
-        segment_geometry_xy = substring(link.geometry_xy_offset, start_dist=start_position, end_dist=end_position)
-        link.cutted_geometry_xy_list.append(segment_geometry_xy)
-        link.cutted_geometry_list.append(GT.geo_to_latlon(segment_geometry_xy))
-
-
-def _cutMacroLinks(link_dict, GT):
-    # cut macro links to stop lines to enable movement links generation
-    for link_id, link in link_dict.items():
-        _linkLengthToCut(link)
-        _performLinkCut(link, GT)
-
-
-def buildMultiResolutionNets(macronet, generate_micro_net=True,
-                             auto_movement_generation=True, exclusive_bike_walk_lanes=True, connector_type=None,
-                             width_of_lane=3.5, length_of_cell=7.0):
-    """
-    Build the corresponding mesoscopic and microscopic networks for a source (macroscopic) network
-
-    Parameters
-    ----------
-    macronet: Network
-        a soucrce osm2gmns Network object
-    generate_micro_net: bool
-        True: generate meso and micro networks; False: only generate meso network
-    auto_movement_generation: bool
-        automatically generate movements for intersections without movement information by calling function generateMovements
-        in osm2gmns. if auto_movement_generation is set as False, movements at intersections without movement information will not be generated
-    exclusive_bike_walk_lanes: bool
-        build exclusive lanes for bike and walk
-    connector_type: int
-        link_type of connectors
-    width_of_lane: float
-        width of lanes in meter
-    length_of_cell: float
-        lenght of cells in meter
-
-    Returns
-    -------
-    None
-
-    """
-    if og_settings.verbose:
-        print('Building Multiresolution Networks')
-
-    if not macronet.complete_link_lane_info:
-        print('WARNING: Multiresolution network generation will be skipped because some links do not have lanes information.\n'
-              '         If the network is parsed from a OSM file, set "default_lanes" as "True" when parsing networks to assign default lanes for links without lanes information.\n'
-              '         If the network is loaded from a CSV file, make sure all links have lanes information before loading the network.')
-        return
-
-
-    if auto_movement_generation:
-        generateMovements(macronet)
-    else:
-        for _, link in macronet.link_dict.items():
-            link.linkLaneListFromSegment()
-        validateUserInputMovements(macronet)
-
-    _offsetLinkGeometry(macronet.link_dict, width_of_lane, macronet.GT)
-    _checkMovementLinkNecessity(macronet.node_dict)
-    _cutMacroLinks(macronet.link_dict, macronet.GT)
-
-    net_generator = NetGenerator(macronet, generate_micro_net, exclusive_bike_walk_lanes, length_of_cell, width_of_lane)
-    net_generator.generateNet()
-    macronet.mesonet, macronet.micronet = net_generator.mesonet, net_generator.micronet
+# @author       Jiawei Lu (jiaweil9@asu.edu)
+# @time         2021/11/27 12:05
+# @desc         [script description]
+import copy
+
+from osm2gmns.networkclass.macronet import Network
+from osm2gmns.multiresolutionnet.netgen import NetGenerator
+from osm2gmns.movement.generate_movements import generateMovements, validateUserInputMovements
+from osm2gmns.utils.util_geo import getLineAngle, offsetLine
+import osm2gmns.settings as og_settings
+from shapely import geometry
+from shapely.ops import substring
+import math
+
+
+# todo: connector and centroid
+
+_length_of_short_cut = 0.1
+_length_of_cut = {0: 2.0, 1: 8.0, 2: 12.0, 3: 14.0, 4: 16.0, 5: 18.0, 6: 20, 7:22, 8:24}  # e.g. 2:8.0 cut 8 meters if the original macro link has 2 lanes, etc
+for i_ in range(9,100): _length_of_cut[i_] = 25
+_minimum_cutted_length = 2.0
+
+
+def _checkMovementLinkNecessity(node_dict):
+    for node_id, node in node_dict.items():
+        if node.ctrl_type == 'signal': continue
+
+        if len(node.incoming_link_list) == 1 and len(node.outgoing_link_list) >= 1:
+            # one imcoming link
+            ib_link = node.incoming_link_list[0]
+
+            angle_flag = True
+            for ob_link in node.outgoing_link_list:
+                angle = getLineAngle(ib_link.geometry_xy, ob_link.geometry_xy)
+                if angle > 0.75 * math.pi or angle < -0.75 * math.pi:
+                    angle_flag = False
+                    break
+            if not angle_flag: continue
+
+            ob_link_set = set()
+            multiple_connection = False
+            for movement in node.movement_list:
+                if movement.ob_link in ob_link_set:
+                    multiple_connection = True
+                    break
+                else:
+                    ob_link_set.add(movement.ob_link)
+            if multiple_connection: continue
+
+            node.movement_link_needed = False
+            ib_link.downstream_short_cut = True
+            ib_link.downstream_is_target = True
+            for ob_link in node.outgoing_link_list:
+                ob_link.upstream_short_cut = True
+
+        elif len(node.outgoing_link_list) == 1 and len(node.incoming_link_list) >= 1:
+            # one outgoing link
+            ob_link = node.outgoing_link_list[0]
+
+            angle_flag = True
+            for ib_link in node.incoming_link_list:
+                angle = getLineAngle(ib_link.geometry_xy, ob_link.geometry_xy)
+                if angle > 0.75 * math.pi or angle < -0.75 * math.pi:
+                    angle_flag = False
+                    break
+            if not angle_flag: continue
+
+            ib_link_set = set()
+            multiple_connection = False
+            for movement in node.movement_list:
+                if movement.ib_link in ib_link_set:
+                    multiple_connection = True
+                    break
+                else:
+                    ib_link_set.add(movement.ib_link)
+            if multiple_connection: continue
+
+            node.movement_link_needed = False
+
+            ob_link.upstream_short_cut = True
+            ob_link.upstream_is_target = True
+            for ib_link in node.incoming_link_list:
+                ib_link.downstream_short_cut = True
+
+
+def _offsetLinkGeometry(link_dict, width_of_lane, GT):
+    # check if a link needs offset
+    link_offset_dict = {}
+    link_ids = tuple(link_dict.keys())
+    for link_no_a, link_id_a in enumerate(link_ids):
+        link_a = link_dict[link_id_a]
+        if link_a in link_offset_dict.keys():
+            continue
+        geometry_xy_a_r = geometry.LineString(list(link_a.geometry_xy.coords)[::-1])
+        reversed_link_found = False
+        for link_id_b in link_ids[link_no_a+1:]:
+            link_b = link_dict[link_id_b]
+            if geometry_xy_a_r.equals_exact(link_b.geometry_xy, tolerance=0.1):
+                reversed_link_found = True
+                link_offset_dict[link_a] = True
+                link_offset_dict[link_b] = True
+                break
+        if not reversed_link_found:
+            link_offset_dict[link_a] = False
+
+    # offset links
+    for link, need_offset in link_offset_dict.items():
+        if need_offset:
+            offset_distance = (link.max_lanes / 2 + 0.5) * width_of_lane
+            geometry_xy_offset = link.geometry_xy.offset_curve(distance=-1*offset_distance, join_style=2)
+            if isinstance(geometry_xy_offset, geometry.MultiLineString):
+                link.geometry_xy_offset = offsetLine(link.geometry_xy, offset_distance)
+            else:
+                link.geometry_xy_offset = geometry_xy_offset
+
+
+
+            # offset_distance = (link.max_lanes / 2 + 0.5) * width_of_lane
+            # geometry_xy_offset_ = link.geometry_xy.parallel_offset(distance=offset_distance, side='right', join_style=2)
+            # if isinstance(geometry_xy_offset_, geometry.MultiLineString):
+            #     link.geometry_xy_offset = offsetLine(link.geometry_xy, offset_distance)
+            # else:
+            #     link.geometry_xy_offset = geometry.LineString(list(geometry_xy_offset_.coords)[::-1])
+
+
+            link.geometry_offset = GT.geo_to_latlon(link.geometry_xy_offset)
+        else:
+            link.geometry_offset = link.geometry
+            link.geometry_xy_offset = link.geometry_xy
+
+    # update breakpoints due to the change of geometry
+    for link_id, link in link_dict.items():
+        link.lanes_change_point_list = [item / link.length * link.length_offset for item in link.lanes_change_point_list]
+
+
+def _linkLengthToCut(link):
+    # should not change number of lanes at the two ends of a macro link
+    upstream_max_cut = max(_length_of_short_cut, link.lanes_change_point_list[1] - link.lanes_change_point_list[0] - 3)
+    downstream_max_cut = max(_length_of_short_cut, link.lanes_change_point_list[-1] - link.lanes_change_point_list[-2] - 3)
+
+    if link.upstream_short_cut and link.downstream_short_cut:
+        total_length_needed = 2 * _length_of_short_cut + _minimum_cutted_length
+        if link.length_offset > total_length_needed:
+            link.length_of_cut_upstream = _length_of_short_cut
+            link.length_of_cut_downstream = _length_of_short_cut
+        else:
+            link.length_of_cut_upstream = link.length_offset / total_length_needed * _length_of_short_cut
+            link.length_of_cut_downstream = link.length_offset / total_length_needed * _length_of_short_cut
+
+    elif link.upstream_short_cut:
+        length_found = False
+        ii = 0
+        for i in range(link.lanes_list[-1], -1, -1):
+            if link.length_offset > min(downstream_max_cut, _length_of_cut[i]) + _length_of_short_cut + _minimum_cutted_length:
+                ii = i
+                length_found = True
+                break
+
+        if length_found:
+            link.length_of_cut_upstream = _length_of_short_cut
+            link.length_of_cut_downstream = min(downstream_max_cut, _length_of_cut[ii])
+        else:
+            downstream_needed = min(downstream_max_cut, _length_of_cut[0])
+            total_length_needed = downstream_needed + _length_of_short_cut + _minimum_cutted_length
+            link.length_of_cut_upstream = link.length_offset / total_length_needed * _length_of_short_cut
+            link.length_of_cut_downstream = link.length_offset / total_length_needed * downstream_needed
+
+    elif link.downstream_short_cut:
+        length_found = False
+        ii = 0
+        for i in range(link.lanes_list[-1], -1, -1):
+            if link.length_offset > min(upstream_max_cut, _length_of_cut[i]) + _length_of_short_cut + _minimum_cutted_length:
+                ii = i
+                length_found = True
+                break
+
+        if length_found:
+            link.length_of_cut_upstream = min(upstream_max_cut, _length_of_cut[ii])
+            link.length_of_cut_downstream = _length_of_short_cut
+        else:
+            upstream_needed = min(upstream_max_cut, _length_of_cut[0])
+            total_length_needed = upstream_needed + _length_of_short_cut + _minimum_cutted_length
+            link.length_of_cut_upstream = link.length_offset / total_length_needed * _length_of_cut[0]
+            link.length_of_cut_downstream = link.length_offset / total_length_needed * _length_of_short_cut
+
+    else:
+        length_found = False
+        ii = 0
+        for i in range(link.lanes_list[-1], -1, -1):
+            if link.length_offset > min(upstream_max_cut, _length_of_cut[i]) + min(downstream_max_cut, _length_of_cut[i]) + _minimum_cutted_length:
+                ii = i
+                length_found = True
+                break
+
+        if length_found:
+            link.length_of_cut_upstream = min(upstream_max_cut, _length_of_cut[ii])
+            link.length_of_cut_downstream = min(downstream_max_cut, _length_of_cut[ii])
+        else:
+            upstream_needed = min(upstream_max_cut, _length_of_cut[0])
+            downstream_needed = min(downstream_max_cut, _length_of_cut[0])
+            total_length_needed = downstream_needed + upstream_needed + _minimum_cutted_length
+            link.length_of_cut_upstream = link.length_offset / total_length_needed * upstream_needed
+            link.length_of_cut_downstream = link.length_offset / total_length_needed * downstream_needed
+
+
+def _performLinkCut(link, GT):
+    link.cutted_lanes_change_point_list = link.lanes_change_point_list.copy()
+    link.cutted_lanes_list = link.lanes_list.copy()
+    link.cutted_lanes_change_list = link.lanes_change_list.copy()
+
+    link.cutted_lanes_change_point_list[0], link.cutted_lanes_change_point_list[-1] = link.length_of_cut_upstream, link.length_offset - link.length_of_cut_downstream
+
+    for i in range(len(link.cutted_lanes_list)):
+        start_position = link.cutted_lanes_change_point_list[i]
+        end_position = link.cutted_lanes_change_point_list[i+1]
+
+        segment_geometry_xy = substring(link.geometry_xy_offset, start_dist=start_position, end_dist=end_position)
+        link.cutted_geometry_xy_list.append(segment_geometry_xy)
+        link.cutted_geometry_list.append(GT.geo_to_latlon(segment_geometry_xy))
+
+
+def _cutMacroLinks(link_dict, GT):
+    # cut macro links to stop lines to enable movement links generation
+    for link_id, link in link_dict.items():
+        _linkLengthToCut(link)
+        _performLinkCut(link, GT)
+
+
+def buildMultiResolutionNets(macronet, generate_micro_net=True,
+                             auto_movement_generation=True, exclusive_bike_walk_lanes=True, connector_type=None,
+                             width_of_lane=3.5, length_of_cell=7.0):
+    """
+    Build the corresponding mesoscopic and microscopic networks for a source (macroscopic) network
+
+    Parameters
+    ----------
+    macronet: Network
+        a soucrce osm2gmns Network object
+    generate_micro_net: bool
+        True: generate meso and micro networks; False: only generate meso network
+    auto_movement_generation: bool
+        automatically generate movements for intersections without movement information by calling function generateMovements
+        in osm2gmns. if auto_movement_generation is set as False, movements at intersections without movement information will not be generated
+    exclusive_bike_walk_lanes: bool
+        build exclusive lanes for bike and walk
+    connector_type: int
+        link_type of connectors
+    width_of_lane: float
+        width of lanes in meter
+    length_of_cell: float
+        lenght of cells in meter
+
+    Returns
+    -------
+    None
+
+    """
+    if og_settings.verbose:
+        print('Building Multiresolution Networks')
+
+    if not macronet.complete_link_lane_info:
+        print('WARNING: Multiresolution network generation will be skipped because some links do not have lanes information.\n'
+              '         If the network is parsed from a OSM file, set "default_lanes" as "True" when parsing networks to assign default lanes for links without lanes information.\n'
+              '         If the network is loaded from a CSV file, make sure all links have lanes information before loading the network.')
+        return
+
+
+    if auto_movement_generation:
+        generateMovements(macronet)
+    else:
+        for _, link in macronet.link_dict.items():
+            link.linkLaneListFromSegment()
+        validateUserInputMovements(macronet)
+
+    _offsetLinkGeometry(macronet.link_dict, width_of_lane, macronet.GT)
+    _checkMovementLinkNecessity(macronet.node_dict)
+    _cutMacroLinks(macronet.link_dict, macronet.GT)
+
+    net_generator = NetGenerator(macronet, generate_micro_net, exclusive_bike_walk_lanes, length_of_cell, width_of_lane)
+    net_generator.generateNet()
+    macronet.mesonet, macronet.micronet = net_generator.mesonet, net_generator.micronet
```

### Comparing `osm2gmns-0.7.5/osm2gmns/multiresolutionnet/netgen.py` & `osm2gmns-0.7.6/osm2gmns/multiresolutionnet/netgen.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,523 +1,523 @@
-import copy
-
-from osm2gmns.networkclass.mesonet import MesoNode, MesoLink, MesoNetwork
-from osm2gmns.networkclass.micronet import MicroNode, MicroLink, MicroNetwork
-from osm2gmns.utils.util_geo import offsetLine
-import osm2gmns.settings as og_settings
-from shapely import geometry
-import sys
-
-
-
-class NetGenerator:
-    def __init__(self, macronet, generate_micro_net, exclusive_bike_walk_lanes, length_of_cell, width_of_lane):
-        self.macronet = macronet
-        self.generate_micro_net = generate_micro_net
-        # self.exclusive_bike_walk_lanes = exclusive_bike_walk_lanes
-        self.exclusive_bike_walk_lanes = False          # todo: update in the next release
-        self.length_of_cell = length_of_cell
-        self.width_of_lane = width_of_lane
-
-        self.bike_lane_width = 0.5
-        self.walk_lane_width = 0.5
-
-        self.mesonet = MesoNetwork()
-        self.micronet = MicroNetwork() if generate_micro_net else None
-
-        self.number_of_expanded_mesonode = {}       # macronode: number_of_expanded_mesonode
-
-
-    def getMultimoalUse(self, allowed_uses):
-        if self.exclusive_bike_walk_lanes:
-            if len(allowed_uses) <= 1:
-                return {'mainlane_allowed_uses': allowed_uses, 'extra_bike': False, 'extra_walk': False}
-            else:
-                allowed_uses_set = set(allowed_uses).union({'auto','bike','walk'})
-                if allowed_uses_set == {'auto','bike'}:
-                    return {'mainlane_allowed_uses':['auto'], 'extra_bike':True, 'extra_walk':False}
-                elif allowed_uses_set == {'auto','walk'}:
-                    return {'mainlane_allowed_uses':['auto'], 'extra_bike':False, 'extra_walk':True}
-                elif allowed_uses_set == {'bike','walk'}:
-                    return {'mainlane_allowed_uses':['bike'], 'extra_bike':False, 'extra_walk':True}
-                elif allowed_uses_set == {'auto','bike','walk'}:
-                    return {'mainlane_allowed_uses':['auto'], 'extra_bike':True, 'extra_walk':True}
-        else:
-            return {'mainlane_allowed_uses':allowed_uses, 'extra_bike':False, 'extra_walk':False}
-
-
-    def getLaneGeometry(self, original_geometry, lane_offset):
-        if lane_offset < -1e-3 or lane_offset > 1e-3:
-
-            lane_geometry_xy = original_geometry.offset_curve(distance=-1*lane_offset, join_style=2)
-            if isinstance(lane_geometry_xy, geometry.MultiLineString):
-                lane_geometry_xy = offsetLine(original_geometry, lane_offset)
-
-            if lane_geometry_xy.is_empty:
-                return self.getLaneGeometry(original_geometry, lane_offset*0.6)
-
-            return lane_geometry_xy
-
-        else:
-            return copy.copy(original_geometry)
-
-
-    def createMicroNetForNormalLink(self, link):
-        max_micronode_id = self.micronet.max_node_id
-        max_microlink_id = self.micronet.max_link_id
-
-        MultimoalUse = self.getMultimoalUse(link.allowed_uses)
-        mainlane_allowed_uses, extra_bike, extra_walk = MultimoalUse['mainlane_allowed_uses'], MultimoalUse['extra_bike'], MultimoalUse['extra_walk']
-
-        # create micronodes on each mesolink
-        for mesolink in link.mesolink_list:
-            original_number_of_lanes = mesolink.macrolink.lanes
-            lane_changes_left = mesolink.lanes_change[0]
-            num_of_lane_offset_between_left_most_and_central = -1 * (original_number_of_lanes / 2 - 0.5 + lane_changes_left)
-
-            lane_geometry_xy_list = []
-            extra_bike_geometry_xy, extra_walk_geometry_xy = None, None
-            lane_offset = 0
-            for i in range(mesolink.lanes):
-                lane_offset = (num_of_lane_offset_between_left_most_and_central + i) * self.width_of_lane
-                lane_geometry_xy_list.append(self.getLaneGeometry(mesolink.geometry_xy, lane_offset))
-            if extra_bike and not extra_walk:
-                bike_lane_offset = lane_offset + self.bike_lane_width
-                extra_bike_geometry_xy = self.getLaneGeometry(mesolink.geometry_xy, bike_lane_offset)
-            if not extra_bike and extra_walk:
-                walk_lane_offset = lane_offset + self.walk_lane_width
-                extra_walk_geometry_xy = self.getLaneGeometry(mesolink.geometry_xy, walk_lane_offset)
-            if extra_bike and extra_walk:
-                bike_lane_offset = lane_offset + self.bike_lane_width
-                walk_lane_offset = bike_lane_offset + self.walk_lane_width
-                extra_bike_geometry_xy = self.getLaneGeometry(mesolink.geometry_xy, bike_lane_offset)
-                extra_walk_geometry_xy = self.getLaneGeometry(mesolink.geometry_xy, walk_lane_offset)
-
-            number_of_cells = max(1, round(mesolink.length / self.length_of_cell))
-            micronode_geometry_xy_list = [[lane_geometry_xy.interpolate(i/number_of_cells, normalized=True) for i in range(number_of_cells+1)] for lane_geometry_xy in lane_geometry_xy_list]
-            micronode_geometry_xy_bike = [extra_bike_geometry_xy.interpolate(i / number_of_cells, normalized=True) for i in range(number_of_cells + 1)] if extra_bike_geometry_xy is not None else None
-            micronode_geometry_xy_walk = [extra_walk_geometry_xy.interpolate(i / number_of_cells, normalized=True) for i in range(number_of_cells + 1)] if extra_walk_geometry_xy is not None else None
-
-            for i in range(mesolink.lanes):
-                micronode_list_lane = []
-                for micronode_geometry_xy in micronode_geometry_xy_list[i]:
-                    micronode = MicroNode(max_micronode_id)
-                    micronode.geometry_xy = micronode_geometry_xy
-                    micronode.geometry = self.macronet.GT.geo_to_latlon(micronode_geometry_xy)
-                    micronode.mesolink = mesolink
-                    micronode.lane_no = i + 1
-                    micronode_list_lane.append(micronode)
-                    self.micronet.node_dict[micronode.node_id] = micronode
-                    max_micronode_id += 1
-                mesolink.micronode_list.append(micronode_list_lane)
-
-            if extra_bike:
-                for micronode_geometry_xy in micronode_geometry_xy_bike:
-                    micronode = MicroNode(max_micronode_id)
-                    micronode.geometry_xy = micronode_geometry_xy
-                    micronode.geometry = self.macronet.GT.geo_to_latlon(micronode_geometry_xy)
-                    micronode.mesolink = mesolink
-                    # micronode.lane_no = i + 1
-                    mesolink.micronode_bike.append(micronode)
-                    self.micronet.node_dict[micronode.node_id] = micronode
-                    max_micronode_id += 1
-
-            if extra_walk:
-                for micronode_geometry_xy in micronode_geometry_xy_walk:
-                    micronode = MicroNode(max_micronode_id)
-                    micronode.geometry_xy = micronode_geometry_xy
-                    micronode.geometry = self.macronet.GT.geo_to_latlon(micronode_geometry_xy)
-                    micronode.mesolink = mesolink
-                    # micronode.lane_no = i + 1
-                    mesolink.micronode_walk.append(micronode)
-                    self.micronet.node_dict[micronode.node_id] = micronode
-                    max_micronode_id += 1
-
-        # micronodes on two ends
-        first_mesolink = link.mesolink_list[0]
-        for micronode_list_lane in first_mesolink.micronode_list:
-            micronode_list_lane[0].is_link_upstream_end_node = True
-        if extra_bike: first_mesolink.micronode_bike[0].is_link_upstream_end_node = True
-        if extra_walk: first_mesolink.micronode_walk[0].is_link_upstream_end_node = True
-        last_mesolink = link.mesolink_list[-1]
-        for micronode_list_lane in last_mesolink.micronode_list:
-            micronode_list_lane[-1].is_link_downstream_end_node = True
-        if extra_bike: last_mesolink.micronode_bike[-1].is_link_downstream_end_node = True
-        if extra_walk: last_mesolink.micronode_walk[-1].is_link_downstream_end_node = True
-
-        # micronodes between two adjacent mesolinks
-        for i in range(len(link.mesolink_list)-1):
-            upstream_mesolink = link.mesolink_list[i]
-            downstream_mesolink = link.mesolink_list[i+1]
-
-            up_index_of_left_most_lane_of_original_link = upstream_mesolink.lanes_change[0]
-            down_index_of_left_most_lane_of_original_link = downstream_mesolink.lanes_change[0]
-            min_left_most_lane_index = min(up_index_of_left_most_lane_of_original_link, down_index_of_left_most_lane_of_original_link)
-            up_lane_index_start = up_index_of_left_most_lane_of_original_link - min_left_most_lane_index
-            down_lane_index_start = down_index_of_left_most_lane_of_original_link - min_left_most_lane_index
-
-            number_of_connecting_lanes = min(upstream_mesolink.lanes-up_lane_index_start,
-                                             downstream_mesolink.lanes-down_lane_index_start)
-
-            for j in range(number_of_connecting_lanes):
-                up_lane_index = up_lane_index_start + j
-                down_lane_index = down_lane_index_start + j
-                up_micronode = upstream_mesolink.micronode_list[up_lane_index][-1]
-                down_micronode = downstream_mesolink.micronode_list[down_lane_index][0]
-                upstream_mesolink.micronode_list[up_lane_index][-1] = down_micronode
-                del self.micronet.node_dict[up_micronode.node_id]
-
-            if extra_bike:
-                up_micronode = upstream_mesolink.micronode_bike[-1]
-                down_micronode = downstream_mesolink.micronode_bike[0]
-                upstream_mesolink.micronode_bike[-1] = down_micronode
-                del self.micronet.node_dict[up_micronode.node_id]
-            if extra_walk:
-                up_micronode = upstream_mesolink.micronode_walk[-1]
-                down_micronode = downstream_mesolink.micronode_walk[0]
-                upstream_mesolink.micronode_walk = down_micronode
-                del self.micronet.node_dict[up_micronode.node_id]
-
-        # create cell
-        for mesolink in link.mesolink_list:
-            # mainline
-            for i in range(mesolink.lanes):
-                # travelling
-                for j in range(len(mesolink.micronode_list[i])-1):
-                    microlink = MicroLink(max_microlink_id)
-                    microlink.from_node = mesolink.micronode_list[i][j]
-                    microlink.to_node = mesolink.micronode_list[i][j+1]
-                    microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
-                    microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
-                    microlink.mesolink = mesolink
-                    microlink.cell_type = 1	            # //1:traveling; 2:changing
-                    microlink.allowed_uses = mainlane_allowed_uses
-                    self.micronet.link_dict[microlink.link_id] = microlink
-                    max_microlink_id += 1
-                    microlink.from_node.outgoing_link_list.append(microlink)
-                    microlink.to_node.incoming_link_list.append(microlink)
-
-                # changing
-                if i <= mesolink.lanes - 2:
-                    # to left
-                    for j in range(len(mesolink.micronode_list[i])-1):
-                        microlink = MicroLink(max_microlink_id)
-                        microlink.from_node = mesolink.micronode_list[i][j]
-                        microlink.to_node = mesolink.micronode_list[i+1][j+1]
-                        microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
-                        microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
-                        microlink.mesolink = mesolink
-                        microlink.cell_type = 2	            # //1:traveling; 2:changing
-                        microlink.allowed_uses = mainlane_allowed_uses
-                        self.micronet.link_dict[microlink.link_id] = microlink
-                        max_microlink_id += 1
-                        microlink.from_node.outgoing_link_list.append(microlink)
-                        microlink.to_node.incoming_link_list.append(microlink)
-
-                if i >= 1:
-                    # to right
-                    for j in range(len(mesolink.micronode_list[i])-1):
-                        microlink = MicroLink(max_microlink_id)
-                        microlink.from_node = mesolink.micronode_list[i][j]
-                        microlink.to_node = mesolink.micronode_list[i-1][j+1]
-                        microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
-                        microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
-                        microlink.mesolink = mesolink
-                        microlink.cell_type = 2	            # //1:traveling; 2:changing
-                        microlink.allowed_uses = mainlane_allowed_uses
-                        self.micronet.link_dict[microlink.link_id] = microlink
-                        max_microlink_id += 1
-                        microlink.from_node.outgoing_link_list.append(microlink)
-                        microlink.to_node.incoming_link_list.append(microlink)
-
-            # bike
-            if extra_bike:
-                for j in range(len(mesolink.micronode_bike) - 1):
-                    microlink = MicroLink(max_microlink_id)
-                    microlink.from_node = mesolink.micronode_bike[j]
-                    microlink.to_node = mesolink.micronode_bike[j + 1]
-                    microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
-                    microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
-                    microlink.mesolink = mesolink
-                    microlink.cell_type = 1  # //1:traveling; 2:changing
-                    microlink.allowed_uses = ['bike']
-                    self.micronet.link_dict[microlink.link_id] = microlink
-                    max_microlink_id += 1
-                    microlink.from_node.outgoing_link_list.append(microlink)
-                    microlink.to_node.incoming_link_list.append(microlink)
-
-            # walk
-            if extra_walk:
-                for j in range(len(mesolink.micronode_walk) - 1):
-                    microlink = MicroLink(max_microlink_id)
-                    microlink.from_node = mesolink.micronode_walk[j]
-                    microlink.to_node = mesolink.micronode_walk[j + 1]
-                    microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
-                    microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
-                    microlink.mesolink = mesolink
-                    microlink.cell_type = 1  # //1:traveling; 2:changing
-                    microlink.allowed_uses = ['walk']
-                    self.micronet.link_dict[microlink.link_id] = microlink
-                    max_microlink_id += 1
-                    microlink.from_node.outgoing_link_list.append(microlink)
-                    microlink.to_node.incoming_link_list.append(microlink)
-
-        self.micronet.max_node_id = max_micronode_id
-        self.micronet.max_link_id = max_microlink_id
-
-
-    def createMicroNetForConnector(self, mesolink, ib_mesolink, ib_lane_index_start, ob_mesolink, ob_lane_index_start):
-        max_micronode_id = self.micronet.max_node_id
-        max_microlink_id = self.micronet.max_link_id
-
-        for i in range(mesolink.lanes):
-            start_micronode = ib_mesolink.micronode_list[ib_lane_index_start+i][-1]
-            end_micronode = ob_mesolink.micronode_list[ob_lane_index_start+i][0]
-            lane_geometry_xy = geometry.LineString([start_micronode.geometry_xy, end_micronode.geometry_xy])
-
-            number_of_cells = max(1, round(lane_geometry_xy.length / self.length_of_cell))
-            micronode_geometry_xy_list = [lane_geometry_xy.interpolate(i/number_of_cells, normalized=True) for i in range(1,number_of_cells)]
-
-            mesolink.micronode_list.append([])
-            mesolink.microlink_list.append([])
-            last_micronode = start_micronode
-
-            first_movement_cell = True
-
-            for micronode_geometry_xy in micronode_geometry_xy_list:
-                micronode = MicroNode(max_micronode_id)
-                micronode.geometry_xy = micronode_geometry_xy
-                micronode.geometry = self.macronet.GT.geo_to_latlon(micronode_geometry_xy)
-                micronode.mesolink = mesolink
-                micronode.lane_no = i + 1
-                mesolink.micronode_list[-1].append(micronode)
-                self.micronet.node_dict[micronode.node_id] = micronode
-                max_micronode_id += 1
-
-                microlink = MicroLink(max_microlink_id)
-                microlink.from_node = last_micronode
-                microlink.to_node = micronode
-                microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
-                microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
-                microlink.mesolink = mesolink
-                microlink.cell_type = 1	            # //1:traveling; 2:changing
-
-                if first_movement_cell:
-                    microlink.is_first_movement_cell = True
-                    first_movement_cell = False
-
-                mesolink.microlink_list[-1].append(microlink)
-                self.micronet.link_dict[microlink.link_id] = microlink
-                max_microlink_id += 1
-                microlink.from_node.outgoing_link_list.append(microlink)
-                microlink.to_node.incoming_link_list.append(microlink)
-
-                last_micronode = micronode
-
-            microlink = MicroLink(max_microlink_id)
-            microlink.from_node = last_micronode
-            microlink.to_node = end_micronode
-            microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
-            microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
-            microlink.mesolink = mesolink
-            microlink.cell_type = 1	            # //1:traveling; 2:changing
-
-            if first_movement_cell:
-                microlink.is_first_movement_cell = True
-
-            mesolink.microlink_list[-1].append(microlink)
-            self.micronet.link_dict[microlink.link_id] = microlink
-            max_microlink_id += 1
-            microlink.from_node.outgoing_link_list.append(microlink)
-            microlink.to_node.incoming_link_list.append(microlink)
-
-        self.micronet.max_node_id = max_micronode_id
-        self.micronet.max_link_id = max_microlink_id
-
-
-    def createMesoNodeForCentriod(self):
-        # create new meso nodes for centroids
-        for node_id, node in self.macronet.node_dict.items():
-            if node.is_centroid:
-
-                if node not in self.number_of_expanded_mesonode.keys():
-                    self.number_of_expanded_mesonode[node] = 0
-                number_of_expanded_mesonode = self.number_of_expanded_mesonode[node]
-                self.number_of_expanded_mesonode[node] += 1
-
-                mesonode = MesoNode(node.node_id * 100 + number_of_expanded_mesonode)
-                mesonode.geometry = node.geometry
-                mesonode.geometry_xy = node.geometry_xy
-                mesonode.macronode = node
-                node.centroid_mesonode = mesonode
-                self.mesonet.node_dict[mesonode.node_id] = mesonode
-
-
-    def createNormalLinks(self):
-        if og_settings.verbose:
-            print('  generating normal meso links...')
-
-        max_mesolink_id = self.mesonet.max_link_id
-
-        for _, link in self.macronet.link_dict.items():
-            macro_from_node = link.from_node
-            if macro_from_node.is_centroid:
-                upstream_node = macro_from_node.centroid_meso_node
-            else:
-                if macro_from_node not in self.number_of_expanded_mesonode.keys():
-                    self.number_of_expanded_mesonode[macro_from_node] = 0
-                number_of_expanded_mesonode = self.number_of_expanded_mesonode[macro_from_node]
-                self.number_of_expanded_mesonode[macro_from_node] += 1
-
-                upstream_node = MesoNode(macro_from_node.node_id * 100 + number_of_expanded_mesonode)
-                upstream_node.geometry = geometry.Point(link.cutted_geometry_list[0].coords[0])
-                upstream_node.geometry_xy = geometry.Point(link.cutted_geometry_xy_list[0].coords[0])
-                upstream_node.macronode = macro_from_node
-
-                self.mesonet.node_dict[upstream_node.node_id] = upstream_node
-
-            cutted_number_of_segments = len(link.cutted_lanes_list)
-            macro_to_node = link.to_node
-            for section_no in range(cutted_number_of_segments):
-                if macro_to_node.is_centroid and section_no == cutted_number_of_segments - 1:
-                    downstream_node = macro_to_node.centroid_meso_node
-                else:
-                    if macro_to_node not in self.number_of_expanded_mesonode.keys():
-                        self.number_of_expanded_mesonode[macro_to_node] = 0
-                    number_of_expanded_mesonode = self.number_of_expanded_mesonode[macro_to_node]
-                    self.number_of_expanded_mesonode[macro_to_node] += 1
-
-                    downstream_node = MesoNode(macro_to_node.node_id * 100 + number_of_expanded_mesonode)
-                    downstream_node.geometry = geometry.Point(link.cutted_geometry_list[section_no].coords[-1])
-                    downstream_node.geometry_xy = geometry.Point(link.cutted_geometry_xy_list[section_no].coords[-1])
-                    if section_no == cutted_number_of_segments - 1:
-                        downstream_node.macronode = macro_to_node
-                    else:
-                        downstream_node.macrolink = link
-
-                    self.mesonet.node_dict[downstream_node.node_id] = downstream_node
-
-                mesolink = MesoLink(max_mesolink_id)
-                mesolink.from_node = upstream_node
-                mesolink.to_node = downstream_node
-                mesolink.lanes = link.cutted_lanes_list[section_no]
-                mesolink.lanes_change = link.cutted_lanes_change_list[section_no]
-                mesolink.geometry = link.cutted_geometry_list[section_no]
-                mesolink.geometry_xy = link.cutted_geometry_xy_list[section_no]
-                mesolink.macrolink = link
-
-                link.mesolink_list.append(mesolink)
-                upstream_node.outgoing_link_list.append(mesolink)
-                downstream_node.incoming_link_list.append(mesolink)
-
-                self.mesonet.link_dict[mesolink.link_id] = mesolink
-                max_mesolink_id += 1
-                upstream_node = downstream_node
-
-            if self.generate_micro_net:
-                self.createMicroNetForNormalLink(link)
-
-        self.mesonet.max_link_id = max_mesolink_id
-
-
-    def connectMesoLinksMVMT(self):
-        if og_settings.verbose:
-            print('  generating movement meso links...')
-
-        max_mesolink_id = self.mesonet.max_link_id
-
-        for _, macronode in self.macronet.node_dict.items():
-            for mvmt in macronode.movement_list:
-                ib_link, ob_link = mvmt.ib_link, mvmt.ob_link
-                # ib_lane_seq_no_list = [lane_no for lane_no in range(int(mvmt.start_ib_lane_seq_no), int(mvmt.end_ib_lane_seq_no + 1))]
-                # ob_lane_seq_no_list = [lane_no for lane_no in range(int(mvmt.start_ob_lane_seq_no), int(mvmt.end_ob_lane_seq_no + 1))]
-
-                ib_mesolink = ib_link.mesolink_list[-1]
-                ob_mesolink = ob_link.mesolink_list[0]
-
-                # if len(ib_lane_seq_no_list) != len(ob_lane_seq_no_list):
-                #     print('  warning: number of inbound lanes and outbound lanes at movement {} is not consistent, movement info will be discarded'.format(mvmt.movement_id))
-                #     continue
-                # if (0 in ib_lane_seq_no_list) or (0 in ob_lane_seq_no_list):
-                #     print('  warning: lane number 0 detected at movement {}, movement info will be discarded'.format(mvmt.movement_id))
-                #     continue
-                # number_of_lanes = len(ib_lane_seq_no_list)
-
-                # lane index starts from 0
-                # ib_lane_index_start = ib_mesolink.lanes_change[0] + ib_lane_seq_no_list[0] if ib_lane_seq_no_list[0] < 0 else ib_mesolink.lanes_change[0] + ib_lane_seq_no_list[0] - 1
-                # ib_lane_index_end = ib_mesolink.lanes_change[0] + ib_lane_seq_no_list[-1] if ib_lane_seq_no_list[-1] < 0 else ib_mesolink.lanes_change[0] + ib_lane_seq_no_list[-1] - 1
-                # ob_lane_index_start = ob_mesolink.lanes_change[0] + ob_lane_seq_no_list[0] if ob_lane_seq_no_list[0] < 0 else ob_mesolink.lanes_change[0] + ob_lane_seq_no_list[0] - 1
-                # ob_lane_index_end = ob_mesolink.lanes_change[0] + ob_lane_seq_no_list[-1] if ob_lane_seq_no_list[-1] < 0 else ob_mesolink.lanes_change[0] + ob_lane_seq_no_list[-1] - 1
-
-                # if (ib_lane_index_start < 0) or (ob_lane_index_start < 0) or (ib_lane_index_end > ib_mesolink.lanes - 1) or (ob_lane_index_end > ob_mesolink.lanes - 1):
-                #     print('  warning: inbound or outbound lane info of movement {} is not consistent with what inbound or outbound link has,'
-                #         ' movement info will be discarded'.format(mvmt.movement_id))
-                #     continue
-
-                if macronode.movement_link_needed:
-                    mesolink = MesoLink(max_mesolink_id)
-                    mesolink.from_node = ib_mesolink.to_node
-                    mesolink.to_node = ob_mesolink.from_node
-                    mesolink.lanes = mvmt.lanes
-                    mesolink.isconnector = True
-                    mesolink.movement = mvmt
-                    mesolink.macronode = macronode
-
-                    mesolink.geometry = geometry.LineString([ib_mesolink.geometry.coords[-1], ob_mesolink.geometry.coords[0]])
-                    mesolink.geometry_xy = geometry.LineString([ib_mesolink.geometry_xy.coords[-1], ob_mesolink.geometry_xy.coords[0]])
-
-                    self.mesonet.link_dict[mesolink.link_id] = mesolink
-                    max_mesolink_id += 1
-
-                    mesolink.from_node.outgoing_link_list.append(mesolink)
-                    mesolink.to_node.incoming_link_list.append(mesolink)
-
-                    if self.generate_micro_net:
-                        self.createMicroNetForConnector(mesolink, ib_mesolink, mvmt.start_ib_lane_seq_no, ob_mesolink, mvmt.start_ob_lane_seq_no)
-                else:
-                    if ib_link.downstream_is_target and not ob_link.upstream_is_target:
-                        # remove incoming micro nodes and links of ob_mesolink, then connect to ib_mesolink
-                        ib_mesolink_to_node = ib_mesolink.to_node
-                        ob_mesolink_from_node = ob_mesolink.from_node
-                        ob_mesolink.from_node = ib_mesolink_to_node
-                        ob_mesolink.geometry = geometry.LineString([ib_mesolink.geometry.coords[-1]] + ob_mesolink.geometry.coords[1:])
-                        ob_mesolink.geometry_xy = geometry.LineString([ib_mesolink.geometry_xy.coords[-1]] + ob_mesolink.geometry_xy.coords[1:])
-                        del self.mesonet.node_dict[ob_mesolink_from_node.node_id]
-
-                        if self.generate_micro_net:
-                            for i in range(mvmt.lanes):
-                                ib_lane_index = mvmt.start_ib_lane_seq_no + i
-                                ob_lane_index = mvmt.start_ob_lane_seq_no + i
-                                ib_mesolink_outgoing_micro_node = ib_mesolink.micronode_list[ib_lane_index][-1]
-                                ob_mesolink_incoming_micro_node = ob_mesolink.micronode_list[ob_lane_index][0]
-                                for microlink in ob_mesolink_incoming_micro_node.outgoing_link_list:
-                                    microlink.from_node = ib_mesolink_outgoing_micro_node
-                                del self.micronet.node_dict[ob_mesolink_incoming_micro_node.node_id]
-                    elif not ib_link.downstream_is_target and ob_link.upstream_is_target:
-                        # remove outgoing micro nodes and links of ib_mesolink, then connect to ob_mesolink
-                        ib_mesolink_to_node = ib_mesolink.to_node
-                        ob_mesolink_from_node = ob_mesolink.from_node
-                        ib_mesolink.to_node = ob_mesolink_from_node
-                        ib_mesolink.geometry = geometry.LineString(ib_mesolink.geometry.coords[:-1] + [ob_mesolink.geometry.coords[0]])
-                        ib_mesolink.geometry_xy = geometry.LineString(ib_mesolink.geometry_xy.coords[:-1] + [ob_mesolink.geometry_xy.coords[0]])
-                        del self.mesonet.node_dict[ib_mesolink_to_node.node_id]
-
-                        if self.generate_micro_net:
-                            for i in range(mvmt.lanes):
-                                ib_lane_index = mvmt.start_ib_lane_seq_no + i
-                                ob_lane_index = mvmt.start_ob_lane_seq_no + i
-                                ib_mesolink_outgoing_micro_node = ib_mesolink.micronode_list[ib_lane_index][-1]
-                                ob_mesolink_incoming_micro_node = ob_mesolink.micronode_list[ob_lane_index][0]
-                                for microlink in ib_mesolink_outgoing_micro_node.incoming_link_list:
-                                    microlink.to_node = ob_mesolink_incoming_micro_node
-                                del self.micronet.node_dict[ib_mesolink_outgoing_micro_node.node_id]
-                    else:
-                        sys.exit('Target link defintion error')
-
-        self.mesonet.max_link_id = max_mesolink_id
-
-
-    def generateNet(self):
-        self.createMesoNodeForCentriod()
-        self.createNormalLinks()
-        self.connectMesoLinksMVMT()
-
+import copy
+
+from osm2gmns.networkclass.mesonet import MesoNode, MesoLink, MesoNetwork
+from osm2gmns.networkclass.micronet import MicroNode, MicroLink, MicroNetwork
+from osm2gmns.utils.util_geo import offsetLine
+import osm2gmns.settings as og_settings
+from shapely import geometry
+import sys
+
+
+
+class NetGenerator:
+    def __init__(self, macronet, generate_micro_net, exclusive_bike_walk_lanes, length_of_cell, width_of_lane):
+        self.macronet = macronet
+        self.generate_micro_net = generate_micro_net
+        # self.exclusive_bike_walk_lanes = exclusive_bike_walk_lanes
+        self.exclusive_bike_walk_lanes = False          # todo: update in the next release
+        self.length_of_cell = length_of_cell
+        self.width_of_lane = width_of_lane
+
+        self.bike_lane_width = 0.5
+        self.walk_lane_width = 0.5
+
+        self.mesonet = MesoNetwork()
+        self.micronet = MicroNetwork() if generate_micro_net else None
+
+        self.number_of_expanded_mesonode = {}       # macronode: number_of_expanded_mesonode
+
+
+    def getMultimoalUse(self, allowed_uses):
+        if self.exclusive_bike_walk_lanes:
+            if len(allowed_uses) <= 1:
+                return {'mainlane_allowed_uses': allowed_uses, 'extra_bike': False, 'extra_walk': False}
+            else:
+                allowed_uses_set = set(allowed_uses).union({'auto','bike','walk'})
+                if allowed_uses_set == {'auto','bike'}:
+                    return {'mainlane_allowed_uses':['auto'], 'extra_bike':True, 'extra_walk':False}
+                elif allowed_uses_set == {'auto','walk'}:
+                    return {'mainlane_allowed_uses':['auto'], 'extra_bike':False, 'extra_walk':True}
+                elif allowed_uses_set == {'bike','walk'}:
+                    return {'mainlane_allowed_uses':['bike'], 'extra_bike':False, 'extra_walk':True}
+                elif allowed_uses_set == {'auto','bike','walk'}:
+                    return {'mainlane_allowed_uses':['auto'], 'extra_bike':True, 'extra_walk':True}
+        else:
+            return {'mainlane_allowed_uses':allowed_uses, 'extra_bike':False, 'extra_walk':False}
+
+
+    def getLaneGeometry(self, original_geometry, lane_offset):
+        if lane_offset < -1e-3 or lane_offset > 1e-3:
+
+            lane_geometry_xy = original_geometry.offset_curve(distance=-1*lane_offset, join_style=2)
+            if isinstance(lane_geometry_xy, geometry.MultiLineString):
+                lane_geometry_xy = offsetLine(original_geometry, lane_offset)
+
+            if lane_geometry_xy.is_empty:
+                return self.getLaneGeometry(original_geometry, lane_offset*0.6)
+
+            return lane_geometry_xy
+
+        else:
+            return copy.copy(original_geometry)
+
+
+    def createMicroNetForNormalLink(self, link):
+        max_micronode_id = self.micronet.max_node_id
+        max_microlink_id = self.micronet.max_link_id
+
+        MultimoalUse = self.getMultimoalUse(link.allowed_uses)
+        mainlane_allowed_uses, extra_bike, extra_walk = MultimoalUse['mainlane_allowed_uses'], MultimoalUse['extra_bike'], MultimoalUse['extra_walk']
+
+        # create micronodes on each mesolink
+        for mesolink in link.mesolink_list:
+            original_number_of_lanes = mesolink.macrolink.lanes
+            lane_changes_left = mesolink.lanes_change[0]
+            num_of_lane_offset_between_left_most_and_central = -1 * (original_number_of_lanes / 2 - 0.5 + lane_changes_left)
+
+            lane_geometry_xy_list = []
+            extra_bike_geometry_xy, extra_walk_geometry_xy = None, None
+            lane_offset = 0
+            for i in range(mesolink.lanes):
+                lane_offset = (num_of_lane_offset_between_left_most_and_central + i) * self.width_of_lane
+                lane_geometry_xy_list.append(self.getLaneGeometry(mesolink.geometry_xy, lane_offset))
+            if extra_bike and not extra_walk:
+                bike_lane_offset = lane_offset + self.bike_lane_width
+                extra_bike_geometry_xy = self.getLaneGeometry(mesolink.geometry_xy, bike_lane_offset)
+            if not extra_bike and extra_walk:
+                walk_lane_offset = lane_offset + self.walk_lane_width
+                extra_walk_geometry_xy = self.getLaneGeometry(mesolink.geometry_xy, walk_lane_offset)
+            if extra_bike and extra_walk:
+                bike_lane_offset = lane_offset + self.bike_lane_width
+                walk_lane_offset = bike_lane_offset + self.walk_lane_width
+                extra_bike_geometry_xy = self.getLaneGeometry(mesolink.geometry_xy, bike_lane_offset)
+                extra_walk_geometry_xy = self.getLaneGeometry(mesolink.geometry_xy, walk_lane_offset)
+
+            number_of_cells = max(1, round(mesolink.length / self.length_of_cell))
+            micronode_geometry_xy_list = [[lane_geometry_xy.interpolate(i/number_of_cells, normalized=True) for i in range(number_of_cells+1)] for lane_geometry_xy in lane_geometry_xy_list]
+            micronode_geometry_xy_bike = [extra_bike_geometry_xy.interpolate(i / number_of_cells, normalized=True) for i in range(number_of_cells + 1)] if extra_bike_geometry_xy is not None else None
+            micronode_geometry_xy_walk = [extra_walk_geometry_xy.interpolate(i / number_of_cells, normalized=True) for i in range(number_of_cells + 1)] if extra_walk_geometry_xy is not None else None
+
+            for i in range(mesolink.lanes):
+                micronode_list_lane = []
+                for micronode_geometry_xy in micronode_geometry_xy_list[i]:
+                    micronode = MicroNode(max_micronode_id)
+                    micronode.geometry_xy = micronode_geometry_xy
+                    micronode.geometry = self.macronet.GT.geo_to_latlon(micronode_geometry_xy)
+                    micronode.mesolink = mesolink
+                    micronode.lane_no = i + 1
+                    micronode_list_lane.append(micronode)
+                    self.micronet.node_dict[micronode.node_id] = micronode
+                    max_micronode_id += 1
+                mesolink.micronode_list.append(micronode_list_lane)
+
+            if extra_bike:
+                for micronode_geometry_xy in micronode_geometry_xy_bike:
+                    micronode = MicroNode(max_micronode_id)
+                    micronode.geometry_xy = micronode_geometry_xy
+                    micronode.geometry = self.macronet.GT.geo_to_latlon(micronode_geometry_xy)
+                    micronode.mesolink = mesolink
+                    # micronode.lane_no = i + 1
+                    mesolink.micronode_bike.append(micronode)
+                    self.micronet.node_dict[micronode.node_id] = micronode
+                    max_micronode_id += 1
+
+            if extra_walk:
+                for micronode_geometry_xy in micronode_geometry_xy_walk:
+                    micronode = MicroNode(max_micronode_id)
+                    micronode.geometry_xy = micronode_geometry_xy
+                    micronode.geometry = self.macronet.GT.geo_to_latlon(micronode_geometry_xy)
+                    micronode.mesolink = mesolink
+                    # micronode.lane_no = i + 1
+                    mesolink.micronode_walk.append(micronode)
+                    self.micronet.node_dict[micronode.node_id] = micronode
+                    max_micronode_id += 1
+
+        # micronodes on two ends
+        first_mesolink = link.mesolink_list[0]
+        for micronode_list_lane in first_mesolink.micronode_list:
+            micronode_list_lane[0].is_link_upstream_end_node = True
+        if extra_bike: first_mesolink.micronode_bike[0].is_link_upstream_end_node = True
+        if extra_walk: first_mesolink.micronode_walk[0].is_link_upstream_end_node = True
+        last_mesolink = link.mesolink_list[-1]
+        for micronode_list_lane in last_mesolink.micronode_list:
+            micronode_list_lane[-1].is_link_downstream_end_node = True
+        if extra_bike: last_mesolink.micronode_bike[-1].is_link_downstream_end_node = True
+        if extra_walk: last_mesolink.micronode_walk[-1].is_link_downstream_end_node = True
+
+        # micronodes between two adjacent mesolinks
+        for i in range(len(link.mesolink_list)-1):
+            upstream_mesolink = link.mesolink_list[i]
+            downstream_mesolink = link.mesolink_list[i+1]
+
+            up_index_of_left_most_lane_of_original_link = upstream_mesolink.lanes_change[0]
+            down_index_of_left_most_lane_of_original_link = downstream_mesolink.lanes_change[0]
+            min_left_most_lane_index = min(up_index_of_left_most_lane_of_original_link, down_index_of_left_most_lane_of_original_link)
+            up_lane_index_start = up_index_of_left_most_lane_of_original_link - min_left_most_lane_index
+            down_lane_index_start = down_index_of_left_most_lane_of_original_link - min_left_most_lane_index
+
+            number_of_connecting_lanes = min(upstream_mesolink.lanes-up_lane_index_start,
+                                             downstream_mesolink.lanes-down_lane_index_start)
+
+            for j in range(number_of_connecting_lanes):
+                up_lane_index = up_lane_index_start + j
+                down_lane_index = down_lane_index_start + j
+                up_micronode = upstream_mesolink.micronode_list[up_lane_index][-1]
+                down_micronode = downstream_mesolink.micronode_list[down_lane_index][0]
+                upstream_mesolink.micronode_list[up_lane_index][-1] = down_micronode
+                del self.micronet.node_dict[up_micronode.node_id]
+
+            if extra_bike:
+                up_micronode = upstream_mesolink.micronode_bike[-1]
+                down_micronode = downstream_mesolink.micronode_bike[0]
+                upstream_mesolink.micronode_bike[-1] = down_micronode
+                del self.micronet.node_dict[up_micronode.node_id]
+            if extra_walk:
+                up_micronode = upstream_mesolink.micronode_walk[-1]
+                down_micronode = downstream_mesolink.micronode_walk[0]
+                upstream_mesolink.micronode_walk = down_micronode
+                del self.micronet.node_dict[up_micronode.node_id]
+
+        # create cell
+        for mesolink in link.mesolink_list:
+            # mainline
+            for i in range(mesolink.lanes):
+                # travelling
+                for j in range(len(mesolink.micronode_list[i])-1):
+                    microlink = MicroLink(max_microlink_id)
+                    microlink.from_node = mesolink.micronode_list[i][j]
+                    microlink.to_node = mesolink.micronode_list[i][j+1]
+                    microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
+                    microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
+                    microlink.mesolink = mesolink
+                    microlink.cell_type = 1	            # //1:traveling; 2:changing
+                    microlink.allowed_uses = mainlane_allowed_uses
+                    self.micronet.link_dict[microlink.link_id] = microlink
+                    max_microlink_id += 1
+                    microlink.from_node.outgoing_link_list.append(microlink)
+                    microlink.to_node.incoming_link_list.append(microlink)
+
+                # changing
+                if i <= mesolink.lanes - 2:
+                    # to left
+                    for j in range(len(mesolink.micronode_list[i])-1):
+                        microlink = MicroLink(max_microlink_id)
+                        microlink.from_node = mesolink.micronode_list[i][j]
+                        microlink.to_node = mesolink.micronode_list[i+1][j+1]
+                        microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
+                        microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
+                        microlink.mesolink = mesolink
+                        microlink.cell_type = 2	            # //1:traveling; 2:changing
+                        microlink.allowed_uses = mainlane_allowed_uses
+                        self.micronet.link_dict[microlink.link_id] = microlink
+                        max_microlink_id += 1
+                        microlink.from_node.outgoing_link_list.append(microlink)
+                        microlink.to_node.incoming_link_list.append(microlink)
+
+                if i >= 1:
+                    # to right
+                    for j in range(len(mesolink.micronode_list[i])-1):
+                        microlink = MicroLink(max_microlink_id)
+                        microlink.from_node = mesolink.micronode_list[i][j]
+                        microlink.to_node = mesolink.micronode_list[i-1][j+1]
+                        microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
+                        microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
+                        microlink.mesolink = mesolink
+                        microlink.cell_type = 2	            # //1:traveling; 2:changing
+                        microlink.allowed_uses = mainlane_allowed_uses
+                        self.micronet.link_dict[microlink.link_id] = microlink
+                        max_microlink_id += 1
+                        microlink.from_node.outgoing_link_list.append(microlink)
+                        microlink.to_node.incoming_link_list.append(microlink)
+
+            # bike
+            if extra_bike:
+                for j in range(len(mesolink.micronode_bike) - 1):
+                    microlink = MicroLink(max_microlink_id)
+                    microlink.from_node = mesolink.micronode_bike[j]
+                    microlink.to_node = mesolink.micronode_bike[j + 1]
+                    microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
+                    microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
+                    microlink.mesolink = mesolink
+                    microlink.cell_type = 1  # //1:traveling; 2:changing
+                    microlink.allowed_uses = ['bike']
+                    self.micronet.link_dict[microlink.link_id] = microlink
+                    max_microlink_id += 1
+                    microlink.from_node.outgoing_link_list.append(microlink)
+                    microlink.to_node.incoming_link_list.append(microlink)
+
+            # walk
+            if extra_walk:
+                for j in range(len(mesolink.micronode_walk) - 1):
+                    microlink = MicroLink(max_microlink_id)
+                    microlink.from_node = mesolink.micronode_walk[j]
+                    microlink.to_node = mesolink.micronode_walk[j + 1]
+                    microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
+                    microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
+                    microlink.mesolink = mesolink
+                    microlink.cell_type = 1  # //1:traveling; 2:changing
+                    microlink.allowed_uses = ['walk']
+                    self.micronet.link_dict[microlink.link_id] = microlink
+                    max_microlink_id += 1
+                    microlink.from_node.outgoing_link_list.append(microlink)
+                    microlink.to_node.incoming_link_list.append(microlink)
+
+        self.micronet.max_node_id = max_micronode_id
+        self.micronet.max_link_id = max_microlink_id
+
+
+    def createMicroNetForConnector(self, mesolink, ib_mesolink, ib_lane_index_start, ob_mesolink, ob_lane_index_start):
+        max_micronode_id = self.micronet.max_node_id
+        max_microlink_id = self.micronet.max_link_id
+
+        for i in range(mesolink.lanes):
+            start_micronode = ib_mesolink.micronode_list[ib_lane_index_start+i][-1]
+            end_micronode = ob_mesolink.micronode_list[ob_lane_index_start+i][0]
+            lane_geometry_xy = geometry.LineString([start_micronode.geometry_xy, end_micronode.geometry_xy])
+
+            number_of_cells = max(1, round(lane_geometry_xy.length / self.length_of_cell))
+            micronode_geometry_xy_list = [lane_geometry_xy.interpolate(i/number_of_cells, normalized=True) for i in range(1,number_of_cells)]
+
+            mesolink.micronode_list.append([])
+            mesolink.microlink_list.append([])
+            last_micronode = start_micronode
+
+            first_movement_cell = True
+
+            for micronode_geometry_xy in micronode_geometry_xy_list:
+                micronode = MicroNode(max_micronode_id)
+                micronode.geometry_xy = micronode_geometry_xy
+                micronode.geometry = self.macronet.GT.geo_to_latlon(micronode_geometry_xy)
+                micronode.mesolink = mesolink
+                micronode.lane_no = i + 1
+                mesolink.micronode_list[-1].append(micronode)
+                self.micronet.node_dict[micronode.node_id] = micronode
+                max_micronode_id += 1
+
+                microlink = MicroLink(max_microlink_id)
+                microlink.from_node = last_micronode
+                microlink.to_node = micronode
+                microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
+                microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
+                microlink.mesolink = mesolink
+                microlink.cell_type = 1	            # //1:traveling; 2:changing
+
+                if first_movement_cell:
+                    microlink.is_first_movement_cell = True
+                    first_movement_cell = False
+
+                mesolink.microlink_list[-1].append(microlink)
+                self.micronet.link_dict[microlink.link_id] = microlink
+                max_microlink_id += 1
+                microlink.from_node.outgoing_link_list.append(microlink)
+                microlink.to_node.incoming_link_list.append(microlink)
+
+                last_micronode = micronode
+
+            microlink = MicroLink(max_microlink_id)
+            microlink.from_node = last_micronode
+            microlink.to_node = end_micronode
+            microlink.geometry = geometry.LineString([microlink.from_node.geometry, microlink.to_node.geometry])
+            microlink.geometry_xy = geometry.LineString([microlink.from_node.geometry_xy, microlink.to_node.geometry_xy])
+            microlink.mesolink = mesolink
+            microlink.cell_type = 1	            # //1:traveling; 2:changing
+
+            if first_movement_cell:
+                microlink.is_first_movement_cell = True
+
+            mesolink.microlink_list[-1].append(microlink)
+            self.micronet.link_dict[microlink.link_id] = microlink
+            max_microlink_id += 1
+            microlink.from_node.outgoing_link_list.append(microlink)
+            microlink.to_node.incoming_link_list.append(microlink)
+
+        self.micronet.max_node_id = max_micronode_id
+        self.micronet.max_link_id = max_microlink_id
+
+
+    def createMesoNodeForCentriod(self):
+        # create new meso nodes for centroids
+        for node_id, node in self.macronet.node_dict.items():
+            if node.is_centroid:
+
+                if node not in self.number_of_expanded_mesonode.keys():
+                    self.number_of_expanded_mesonode[node] = 0
+                number_of_expanded_mesonode = self.number_of_expanded_mesonode[node]
+                self.number_of_expanded_mesonode[node] += 1
+
+                mesonode = MesoNode(node.node_id * 100 + number_of_expanded_mesonode)
+                mesonode.geometry = node.geometry
+                mesonode.geometry_xy = node.geometry_xy
+                mesonode.macronode = node
+                node.centroid_mesonode = mesonode
+                self.mesonet.node_dict[mesonode.node_id] = mesonode
+
+
+    def createNormalLinks(self):
+        if og_settings.verbose:
+            print('  generating normal meso links...')
+
+        max_mesolink_id = self.mesonet.max_link_id
+
+        for _, link in self.macronet.link_dict.items():
+            macro_from_node = link.from_node
+            if macro_from_node.is_centroid:
+                upstream_node = macro_from_node.centroid_meso_node
+            else:
+                if macro_from_node not in self.number_of_expanded_mesonode.keys():
+                    self.number_of_expanded_mesonode[macro_from_node] = 0
+                number_of_expanded_mesonode = self.number_of_expanded_mesonode[macro_from_node]
+                self.number_of_expanded_mesonode[macro_from_node] += 1
+
+                upstream_node = MesoNode(macro_from_node.node_id * 100 + number_of_expanded_mesonode)
+                upstream_node.geometry = geometry.Point(link.cutted_geometry_list[0].coords[0])
+                upstream_node.geometry_xy = geometry.Point(link.cutted_geometry_xy_list[0].coords[0])
+                upstream_node.macronode = macro_from_node
+
+                self.mesonet.node_dict[upstream_node.node_id] = upstream_node
+
+            cutted_number_of_segments = len(link.cutted_lanes_list)
+            macro_to_node = link.to_node
+            for section_no in range(cutted_number_of_segments):
+                if macro_to_node.is_centroid and section_no == cutted_number_of_segments - 1:
+                    downstream_node = macro_to_node.centroid_meso_node
+                else:
+                    if macro_to_node not in self.number_of_expanded_mesonode.keys():
+                        self.number_of_expanded_mesonode[macro_to_node] = 0
+                    number_of_expanded_mesonode = self.number_of_expanded_mesonode[macro_to_node]
+                    self.number_of_expanded_mesonode[macro_to_node] += 1
+
+                    downstream_node = MesoNode(macro_to_node.node_id * 100 + number_of_expanded_mesonode)
+                    downstream_node.geometry = geometry.Point(link.cutted_geometry_list[section_no].coords[-1])
+                    downstream_node.geometry_xy = geometry.Point(link.cutted_geometry_xy_list[section_no].coords[-1])
+                    if section_no == cutted_number_of_segments - 1:
+                        downstream_node.macronode = macro_to_node
+                    else:
+                        downstream_node.macrolink = link
+
+                    self.mesonet.node_dict[downstream_node.node_id] = downstream_node
+
+                mesolink = MesoLink(max_mesolink_id)
+                mesolink.from_node = upstream_node
+                mesolink.to_node = downstream_node
+                mesolink.lanes = link.cutted_lanes_list[section_no]
+                mesolink.lanes_change = link.cutted_lanes_change_list[section_no]
+                mesolink.geometry = link.cutted_geometry_list[section_no]
+                mesolink.geometry_xy = link.cutted_geometry_xy_list[section_no]
+                mesolink.macrolink = link
+
+                link.mesolink_list.append(mesolink)
+                upstream_node.outgoing_link_list.append(mesolink)
+                downstream_node.incoming_link_list.append(mesolink)
+
+                self.mesonet.link_dict[mesolink.link_id] = mesolink
+                max_mesolink_id += 1
+                upstream_node = downstream_node
+
+            if self.generate_micro_net:
+                self.createMicroNetForNormalLink(link)
+
+        self.mesonet.max_link_id = max_mesolink_id
+
+
+    def connectMesoLinksMVMT(self):
+        if og_settings.verbose:
+            print('  generating movement meso links...')
+
+        max_mesolink_id = self.mesonet.max_link_id
+
+        for _, macronode in self.macronet.node_dict.items():
+            for mvmt in macronode.movement_list:
+                ib_link, ob_link = mvmt.ib_link, mvmt.ob_link
+                # ib_lane_seq_no_list = [lane_no for lane_no in range(int(mvmt.start_ib_lane_seq_no), int(mvmt.end_ib_lane_seq_no + 1))]
+                # ob_lane_seq_no_list = [lane_no for lane_no in range(int(mvmt.start_ob_lane_seq_no), int(mvmt.end_ob_lane_seq_no + 1))]
+
+                ib_mesolink = ib_link.mesolink_list[-1]
+                ob_mesolink = ob_link.mesolink_list[0]
+
+                # if len(ib_lane_seq_no_list) != len(ob_lane_seq_no_list):
+                #     print('  warning: number of inbound lanes and outbound lanes at movement {} is not consistent, movement info will be discarded'.format(mvmt.movement_id))
+                #     continue
+                # if (0 in ib_lane_seq_no_list) or (0 in ob_lane_seq_no_list):
+                #     print('  warning: lane number 0 detected at movement {}, movement info will be discarded'.format(mvmt.movement_id))
+                #     continue
+                # number_of_lanes = len(ib_lane_seq_no_list)
+
+                # lane index starts from 0
+                # ib_lane_index_start = ib_mesolink.lanes_change[0] + ib_lane_seq_no_list[0] if ib_lane_seq_no_list[0] < 0 else ib_mesolink.lanes_change[0] + ib_lane_seq_no_list[0] - 1
+                # ib_lane_index_end = ib_mesolink.lanes_change[0] + ib_lane_seq_no_list[-1] if ib_lane_seq_no_list[-1] < 0 else ib_mesolink.lanes_change[0] + ib_lane_seq_no_list[-1] - 1
+                # ob_lane_index_start = ob_mesolink.lanes_change[0] + ob_lane_seq_no_list[0] if ob_lane_seq_no_list[0] < 0 else ob_mesolink.lanes_change[0] + ob_lane_seq_no_list[0] - 1
+                # ob_lane_index_end = ob_mesolink.lanes_change[0] + ob_lane_seq_no_list[-1] if ob_lane_seq_no_list[-1] < 0 else ob_mesolink.lanes_change[0] + ob_lane_seq_no_list[-1] - 1
+
+                # if (ib_lane_index_start < 0) or (ob_lane_index_start < 0) or (ib_lane_index_end > ib_mesolink.lanes - 1) or (ob_lane_index_end > ob_mesolink.lanes - 1):
+                #     print('  warning: inbound or outbound lane info of movement {} is not consistent with what inbound or outbound link has,'
+                #         ' movement info will be discarded'.format(mvmt.movement_id))
+                #     continue
+
+                if macronode.movement_link_needed:
+                    mesolink = MesoLink(max_mesolink_id)
+                    mesolink.from_node = ib_mesolink.to_node
+                    mesolink.to_node = ob_mesolink.from_node
+                    mesolink.lanes = mvmt.lanes
+                    mesolink.isconnector = True
+                    mesolink.movement = mvmt
+                    mesolink.macronode = macronode
+
+                    mesolink.geometry = geometry.LineString([ib_mesolink.geometry.coords[-1], ob_mesolink.geometry.coords[0]])
+                    mesolink.geometry_xy = geometry.LineString([ib_mesolink.geometry_xy.coords[-1], ob_mesolink.geometry_xy.coords[0]])
+
+                    self.mesonet.link_dict[mesolink.link_id] = mesolink
+                    max_mesolink_id += 1
+
+                    mesolink.from_node.outgoing_link_list.append(mesolink)
+                    mesolink.to_node.incoming_link_list.append(mesolink)
+
+                    if self.generate_micro_net:
+                        self.createMicroNetForConnector(mesolink, ib_mesolink, mvmt.start_ib_lane_seq_no, ob_mesolink, mvmt.start_ob_lane_seq_no)
+                else:
+                    if ib_link.downstream_is_target and not ob_link.upstream_is_target:
+                        # remove incoming micro nodes and links of ob_mesolink, then connect to ib_mesolink
+                        ib_mesolink_to_node = ib_mesolink.to_node
+                        ob_mesolink_from_node = ob_mesolink.from_node
+                        ob_mesolink.from_node = ib_mesolink_to_node
+                        ob_mesolink.geometry = geometry.LineString([ib_mesolink.geometry.coords[-1]] + ob_mesolink.geometry.coords[1:])
+                        ob_mesolink.geometry_xy = geometry.LineString([ib_mesolink.geometry_xy.coords[-1]] + ob_mesolink.geometry_xy.coords[1:])
+                        del self.mesonet.node_dict[ob_mesolink_from_node.node_id]
+
+                        if self.generate_micro_net:
+                            for i in range(mvmt.lanes):
+                                ib_lane_index = mvmt.start_ib_lane_seq_no + i
+                                ob_lane_index = mvmt.start_ob_lane_seq_no + i
+                                ib_mesolink_outgoing_micro_node = ib_mesolink.micronode_list[ib_lane_index][-1]
+                                ob_mesolink_incoming_micro_node = ob_mesolink.micronode_list[ob_lane_index][0]
+                                for microlink in ob_mesolink_incoming_micro_node.outgoing_link_list:
+                                    microlink.from_node = ib_mesolink_outgoing_micro_node
+                                del self.micronet.node_dict[ob_mesolink_incoming_micro_node.node_id]
+                    elif not ib_link.downstream_is_target and ob_link.upstream_is_target:
+                        # remove outgoing micro nodes and links of ib_mesolink, then connect to ob_mesolink
+                        ib_mesolink_to_node = ib_mesolink.to_node
+                        ob_mesolink_from_node = ob_mesolink.from_node
+                        ib_mesolink.to_node = ob_mesolink_from_node
+                        ib_mesolink.geometry = geometry.LineString(ib_mesolink.geometry.coords[:-1] + [ob_mesolink.geometry.coords[0]])
+                        ib_mesolink.geometry_xy = geometry.LineString(ib_mesolink.geometry_xy.coords[:-1] + [ob_mesolink.geometry_xy.coords[0]])
+                        del self.mesonet.node_dict[ib_mesolink_to_node.node_id]
+
+                        if self.generate_micro_net:
+                            for i in range(mvmt.lanes):
+                                ib_lane_index = mvmt.start_ib_lane_seq_no + i
+                                ob_lane_index = mvmt.start_ob_lane_seq_no + i
+                                ib_mesolink_outgoing_micro_node = ib_mesolink.micronode_list[ib_lane_index][-1]
+                                ob_mesolink_incoming_micro_node = ob_mesolink.micronode_list[ob_lane_index][0]
+                                for microlink in ib_mesolink_outgoing_micro_node.incoming_link_list:
+                                    microlink.to_node = ob_mesolink_incoming_micro_node
+                                del self.micronet.node_dict[ib_mesolink_outgoing_micro_node.node_id]
+                    else:
+                        sys.exit('Target link defintion error')
+
+        self.mesonet.max_link_id = max_mesolink_id
+
+
+    def generateNet(self):
+        self.createMesoNodeForCentriod()
+        self.createNormalLinks()
+        self.connectMesoLinksMVMT()
+
```

### Comparing `osm2gmns-0.7.5/osm2gmns/networkclass/macronet.py` & `osm2gmns-0.7.6/osm2gmns/networkclass/macronet.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,324 +1,324 @@
-# @author       Jiawei Lu (jiaweil9@asu.edu)
-# @time         2021/11/27 15:34
-# @desc         [script description]
-
-from osm2gmns.networkclass.basenet import BaseNode, BaseLink, BaseNetwork
-from osm2gmns.osmnet.osmclasses import OSMNode
-from osm2gmns.utils.util_geo import getLineFromNodes
-import osm2gmns.settings as og_settings
-import math
-
-
-class Node(BaseNode):
-    def __init__(self, node_id):
-        super().__init__(node_id)
-        self.zone_id = None
-        self.osm_node_id = None     # str
-        self.intersection_id = None
-        self.osm_highway = None
-        self.node_type = ''
-        self.ctrl_type = ''
-        self.activity_type = ''
-        self.controller_id = None
-        self.is_boundary = None        # -1:in, 1:out, 2:in&out, 0:no
-        self.poi_id = None
-        self.notes = ''
-
-        self.movement_list = []
-
-        # ======== FOR MULTIRESOLUTION ========
-        self.is_centroid = False
-        self.centroid_mesonode = None
-        self.movement_link_needed = True
-
-
-    def buildFromOSMNode(self, osmnode):
-        """
-        initialize the node from an osmnode
-
-        Parameters
-        ----------
-        osmnode: OSMNode
-            osmnode instance
-
-        Returns
-        -------
-
-        """
-        self.name = osmnode.name
-        self.osm_node_id = osmnode.osm_node_id
-        self.osm_highway = osmnode.osm_highway
-        self.ctrl_type = osmnode.ctrl_type
-        self.geometry = osmnode.geometry
-        self.geometry_xy = osmnode.geometry_xy
-        self.notes = osmnode.notes
-
-
-
-class Link(BaseLink):
-    def __init__(self, link_id):
-        super().__init__(link_id)
-        self.osm_way_id = None      # str
-        self.free_speed = None
-        self.capacity = None
-        self.link_class = ''        # highway, railway, aeroway
-        self.link_type_name = ''
-        self.link_type = 0
-        self.allowed_uses = None
-        self.is_link = False
-        self.is_connector = False
-
-
-        self.from_bidirectional_way = False
-        self.VDF_fftt1 = None
-        self.VDF_cap1 = None
-        self.ctrl_type = None       # signal node in the middle
-
-        self.segment_list = []
-
-        # ======== FOR MULTIRESOLUTION ========
-        self.lanes_list = []
-        self.lanes_change_point_list = []
-        self.lanes_change_list = []
-        self.geometry_offset = None
-        self.geometry_xy_offset = None
-
-        self.upstream_short_cut = False         # no movement needed at upstream
-        self.upstream_is_target = False         # connect with other links while keeping its upstream unchanged
-        self.downstream_short_cut = False       # no movement needed at downstream
-        self.downstream_is_target = False       # connect with other links while keeping its upstream unchanged
-
-        self.length_of_cut_upstream = 0.0
-        self.length_of_cut_downstream = 0.0
-
-        # self.cutted_number_of_sections = 0
-        # self.cutted_length = 0.0
-        # self.cutted_length_in_km = 0.0
-        self.cutted_geometry_list = []      # for each segment
-        self.cutted_geometry_xy_list = []  # for each segment
-        self.cutted_lanes_list = []
-        self.cutted_lanes_change_point_list = []
-        self.cutted_lanes_change_list = []
-
-        self.mesolink_list = []
-
-    @property
-    def incoming_lanes(self):
-        return self.lanes_list[0]
-    @property
-    def outgoing_lanes(self):
-        return self.lanes_list[-1]
-    @property
-    def max_lanes(self):
-        return max(self.lanes_list)
-    def _lane_indices(self, lanes_change_left, lanes_change_right):
-        lane_indices = list(range(1, self.lanes+1))
-        if lanes_change_left < 0:
-            lane_indices = lane_indices[-1*lanes_change_left:]
-        elif lanes_change_left > 0:
-            lane_indices = list(range(-1*lanes_change_left,0)) + lane_indices
-        if lanes_change_right < 0:
-            lane_indices = lane_indices[:lanes_change_right]
-        elif lanes_change_right > 0:
-            lane_indices = lane_indices + list(range(self.lanes+1, self.lanes+1+lanes_change_right))
-        return lane_indices
-    @property
-    def incoming_lane_indices(self):
-        return self._lane_indices(*self.lanes_change_list[0])
-    @property
-    def outgoing_lane_indices(self):
-        return self._lane_indices(*self.lanes_change_list[-1])
-    @property
-    def length_offset(self):
-        return round(self.geometry_xy_offset.length, og_settings.local_coord_precision)
-
-    def buildFromOSMWay(self, way, direction, ref_node_list, default_lanes, default_speed, default_capacity):
-        self.osm_way_id = way.osm_way_id
-        self.name = way.name
-        self.link_class = way.link_class
-        self.link_type_name = way.link_type_name
-        self.link_type = way.link_type
-        self.is_link = way.is_link
-
-        if way.maxspeed:
-            self.free_speed = way.maxspeed
-        elif default_speed:
-            self.free_speed = default_speed[self.link_type_name]
-
-        if default_capacity:
-            self.capacity = default_capacity[self.link_type_name]
-
-        self.allowed_uses = way.allowed_uses
-        if not way.oneway: self.from_bidirectional_way = True
-
-        if way.oneway:
-            self.lanes = way.lanes
-        else:
-            if direction == 1:
-                if way.forward_lanes is not None:
-                    self.lanes = way.forward_lanes
-                elif way.lanes is not None:
-                    self.lanes = math.ceil(way.lanes / 2)
-                else:
-                    self.lanes = way.lanes
-            else:
-                if way.backward_lanes is not None:
-                    self.lanes = way.backward_lanes
-                elif way.lanes is not None:
-                    self.lanes = math.ceil(way.lanes / 2)
-                else:
-                    self.lanes = way.lanes
-
-        if (self.lanes is None) and default_lanes:
-            self.lanes = default_lanes[self.link_type_name]
-
-        for ref_node in ref_node_list[1:-1]:
-            if ref_node.ctrl_type == 'signal':
-                self.ctrl_type = 'signal'
-
-        self.from_node = ref_node_list[0].node
-        self.to_node = ref_node_list[-1].node
-        self.geometry, self.geometry_xy = getLineFromNodes(ref_node_list)
-        self.from_node.outgoing_link_list.append(self)
-        self.to_node.incoming_link_list.append(self)
-
-    def linkLaneListFromSegment(self):
-        self.lanes_list = []
-        self.lanes_change_point_list = []
-        self.lanes_change_list = []
-
-        lanes_change_point_list_temp = [0.0, self.length]
-
-        if self.length <= og_settings.segment_resolution:
-            self.lanes_change_point_list = lanes_change_point_list_temp.copy()
-        else:
-            for segment in self.segment_list:
-                lanes_change_point_list_temp.append(max(0.0, segment.start_lr))
-                lanes_change_point_list_temp.append(min(self.length, segment.end_lr))
-
-            while lanes_change_point_list_temp:
-                target_point = lanes_change_point_list_temp[0]
-                remove_list = []
-                for item in lanes_change_point_list_temp:
-                    if target_point - og_settings.segment_resolution <= item <= target_point + og_settings.segment_resolution:
-                        remove_list.append(item)
-                self.lanes_change_point_list.append(target_point)
-                for item in remove_list: lanes_change_point_list_temp.remove(item)
-            self.lanes_change_point_list.sort()
-
-        for i in range(len(self.lanes_change_point_list) - 1):
-            self.lanes_list.append(self.lanes)
-            self.lanes_change_list.append([0, 0])
-            from_point = self.lanes_change_point_list[i]
-            to_point = self.lanes_change_point_list[i+1]
-            for segment in self.segment_list:
-                length_of_overlapping = min(to_point, segment.end_lr) - max(from_point, segment.start_lr)
-                if length_of_overlapping >= og_settings.segment_resolution:
-                    self.lanes_list[-1] += (segment.l_lanes_added + segment.r_lanes_added)
-                    self.lanes_change_list[-1][0] += segment.l_lanes_added
-                    self.lanes_change_list[-1][1] += segment.r_lanes_added
-
-
-class Segment:
-    def __init__(self, segment_id):
-        self.segment_id = segment_id
-        self.link = None
-        self.ref_node = None
-        self.start_lr = 0.0
-        self.end_lr = 0.0
-        self.l_lanes_added = 0
-        self.r_lanes_added = 0
-
-        self.other_attrs = {}
-
-
-class Movement:
-    def __init__(self, movement_id):
-        self.movement_id = movement_id
-        self.node = None
-        self.ib_link = None
-        self.ob_link = None
-
-        self.start_ib_lane = None
-        self.end_ib_lane = None
-        self.start_ob_lane = None
-        self.end_ob_lane = None
-
-        self.start_ib_lane_seq_no = None
-        self.end_ib_lane_seq_no = None
-        self.start_ob_lane_seq_no = None
-        self.end_ob_lane_seq_no = None
-
-        self.name = ''
-        self.lanes = 0
-        self.type = ''
-        self.penalty = 0.0
-        self.capacity = 0.0
-        self.ctrl_type = ''
-        self.volume = None
-        self.free_speed = None
-        # self.intersection_id = None
-        self.mvmt_txt_id = ''
-        self.allowed_uses = []
-
-        self.geometry = None
-        self.geometry_xy = None
-
-        self.generated_by_osm2gmns = False
-
-        self.other_attrs = {}
-
-
-class POI:
-    def __init__(self):
-        self.poi_id = 0
-        self.osm_way_id = None      # str
-        self.osm_relation_id = None
-        self.name = None
-        self.geometry = None
-        self.geometry_xy = None
-        self.centroid = None
-        self.centroid_xy = None
-        self.nearest_node = None
-        self.building = None
-        self.amenity = None
-        self.leisure = None
-        self.way = None         # highway,railway,aeroway poi
-
-
-class Network(BaseNetwork):
-    def __init__(self):
-        super().__init__()
-
-        self.default_lanes = False
-        self.default_speed = False
-        self.default_capacity = False
-
-        self.max_intersection_id = 0
-        self.max_segment_id = 0
-        self.max_poi_id = 0
-        self.max_movement_id = 0
-
-        self.user_input_movement_list = []
-
-        self.POI_list = []
-
-        self.movement_other_attrs = []
-        self.segment_other_attrs = []
-
-        self.mesonet = None
-        self.micronet = None
-
-
-    @property
-    def number_of_pois(self):
-        return len(self.POI_list)
-    @property
-    def complete_link_lane_info(self):
-        complete_link_lane_info = True
-        for _, link in self.link_dict.items():
-            if link.lanes is None:
-                complete_link_lane_info = False
-                break
-        return complete_link_lane_info
-
+# @author       Jiawei Lu (jiaweil9@asu.edu)
+# @time         2021/11/27 15:34
+# @desc         [script description]
+
+from osm2gmns.networkclass.basenet import BaseNode, BaseLink, BaseNetwork
+from osm2gmns.osmnet.osmclasses import OSMNode
+from osm2gmns.utils.util_geo import getLineFromNodes
+import osm2gmns.settings as og_settings
+import math
+
+
+class Node(BaseNode):
+    def __init__(self, node_id):
+        super().__init__(node_id)
+        self.zone_id = None
+        self.osm_node_id = None     # str
+        self.intersection_id = None
+        self.osm_highway = None
+        self.node_type = ''
+        self.ctrl_type = ''
+        self.activity_type = ''
+        self.controller_id = None
+        self.is_boundary = None        # -1:in, 1:out, 2:in&out, 0:no
+        self.poi_id = None
+        self.notes = ''
+
+        self.movement_list = []
+
+        # ======== FOR MULTIRESOLUTION ========
+        self.is_centroid = False
+        self.centroid_mesonode = None
+        self.movement_link_needed = True
+
+
+    def buildFromOSMNode(self, osmnode):
+        """
+        initialize the node from an osmnode
+
+        Parameters
+        ----------
+        osmnode: OSMNode
+            osmnode instance
+
+        Returns
+        -------
+
+        """
+        self.name = osmnode.name
+        self.osm_node_id = osmnode.osm_node_id
+        self.osm_highway = osmnode.osm_highway
+        self.ctrl_type = osmnode.ctrl_type
+        self.geometry = osmnode.geometry
+        self.geometry_xy = osmnode.geometry_xy
+        self.notes = osmnode.notes
+
+
+
+class Link(BaseLink):
+    def __init__(self, link_id):
+        super().__init__(link_id)
+        self.osm_way_id = None      # str
+        self.free_speed = None
+        self.capacity = None
+        self.link_class = ''        # highway, railway, aeroway
+        self.link_type_name = ''
+        self.link_type = 0
+        self.allowed_uses = None
+        self.is_link = False
+        self.is_connector = False
+
+
+        self.from_bidirectional_way = False
+        self.VDF_fftt1 = None
+        self.VDF_cap1 = None
+        self.ctrl_type = None       # signal node in the middle
+
+        self.segment_list = []
+
+        # ======== FOR MULTIRESOLUTION ========
+        self.lanes_list = []
+        self.lanes_change_point_list = []
+        self.lanes_change_list = []
+        self.geometry_offset = None
+        self.geometry_xy_offset = None
+
+        self.upstream_short_cut = False         # no movement needed at upstream
+        self.upstream_is_target = False         # connect with other links while keeping its upstream unchanged
+        self.downstream_short_cut = False       # no movement needed at downstream
+        self.downstream_is_target = False       # connect with other links while keeping its upstream unchanged
+
+        self.length_of_cut_upstream = 0.0
+        self.length_of_cut_downstream = 0.0
+
+        # self.cutted_number_of_sections = 0
+        # self.cutted_length = 0.0
+        # self.cutted_length_in_km = 0.0
+        self.cutted_geometry_list = []      # for each segment
+        self.cutted_geometry_xy_list = []  # for each segment
+        self.cutted_lanes_list = []
+        self.cutted_lanes_change_point_list = []
+        self.cutted_lanes_change_list = []
+
+        self.mesolink_list = []
+
+    @property
+    def incoming_lanes(self):
+        return self.lanes_list[0]
+    @property
+    def outgoing_lanes(self):
+        return self.lanes_list[-1]
+    @property
+    def max_lanes(self):
+        return max(self.lanes_list)
+    def _lane_indices(self, lanes_change_left, lanes_change_right):
+        lane_indices = list(range(1, self.lanes+1))
+        if lanes_change_left < 0:
+            lane_indices = lane_indices[-1*lanes_change_left:]
+        elif lanes_change_left > 0:
+            lane_indices = list(range(-1*lanes_change_left,0)) + lane_indices
+        if lanes_change_right < 0:
+            lane_indices = lane_indices[:lanes_change_right]
+        elif lanes_change_right > 0:
+            lane_indices = lane_indices + list(range(self.lanes+1, self.lanes+1+lanes_change_right))
+        return lane_indices
+    @property
+    def incoming_lane_indices(self):
+        return self._lane_indices(*self.lanes_change_list[0])
+    @property
+    def outgoing_lane_indices(self):
+        return self._lane_indices(*self.lanes_change_list[-1])
+    @property
+    def length_offset(self):
+        return round(self.geometry_xy_offset.length, og_settings.local_coord_precision)
+
+    def buildFromOSMWay(self, way, direction, ref_node_list, default_lanes, default_speed, default_capacity):
+        self.osm_way_id = way.osm_way_id
+        self.name = way.name
+        self.link_class = way.link_class
+        self.link_type_name = way.link_type_name
+        self.link_type = way.link_type
+        self.is_link = way.is_link
+
+        if way.maxspeed:
+            self.free_speed = way.maxspeed
+        elif default_speed:
+            self.free_speed = default_speed[self.link_type_name]
+
+        if default_capacity:
+            self.capacity = default_capacity[self.link_type_name]
+
+        self.allowed_uses = way.allowed_uses
+        if not way.oneway: self.from_bidirectional_way = True
+
+        if way.oneway:
+            self.lanes = way.lanes
+        else:
+            if direction == 1:
+                if way.forward_lanes is not None:
+                    self.lanes = way.forward_lanes
+                elif way.lanes is not None:
+                    self.lanes = math.ceil(way.lanes / 2)
+                else:
+                    self.lanes = way.lanes
+            else:
+                if way.backward_lanes is not None:
+                    self.lanes = way.backward_lanes
+                elif way.lanes is not None:
+                    self.lanes = math.ceil(way.lanes / 2)
+                else:
+                    self.lanes = way.lanes
+
+        if (self.lanes is None) and default_lanes:
+            self.lanes = default_lanes[self.link_type_name]
+
+        for ref_node in ref_node_list[1:-1]:
+            if ref_node.ctrl_type == 'signal':
+                self.ctrl_type = 'signal'
+
+        self.from_node = ref_node_list[0].node
+        self.to_node = ref_node_list[-1].node
+        self.geometry, self.geometry_xy = getLineFromNodes(ref_node_list)
+        self.from_node.outgoing_link_list.append(self)
+        self.to_node.incoming_link_list.append(self)
+
+    def linkLaneListFromSegment(self):
+        self.lanes_list = []
+        self.lanes_change_point_list = []
+        self.lanes_change_list = []
+
+        lanes_change_point_list_temp = [0.0, self.length]
+
+        if self.length <= og_settings.segment_resolution:
+            self.lanes_change_point_list = lanes_change_point_list_temp.copy()
+        else:
+            for segment in self.segment_list:
+                lanes_change_point_list_temp.append(max(0.0, segment.start_lr))
+                lanes_change_point_list_temp.append(min(self.length, segment.end_lr))
+
+            while lanes_change_point_list_temp:
+                target_point = lanes_change_point_list_temp[0]
+                remove_list = []
+                for item in lanes_change_point_list_temp:
+                    if target_point - og_settings.segment_resolution <= item <= target_point + og_settings.segment_resolution:
+                        remove_list.append(item)
+                self.lanes_change_point_list.append(target_point)
+                for item in remove_list: lanes_change_point_list_temp.remove(item)
+            self.lanes_change_point_list.sort()
+
+        for i in range(len(self.lanes_change_point_list) - 1):
+            self.lanes_list.append(self.lanes)
+            self.lanes_change_list.append([0, 0])
+            from_point = self.lanes_change_point_list[i]
+            to_point = self.lanes_change_point_list[i+1]
+            for segment in self.segment_list:
+                length_of_overlapping = min(to_point, segment.end_lr) - max(from_point, segment.start_lr)
+                if length_of_overlapping >= og_settings.segment_resolution:
+                    self.lanes_list[-1] += (segment.l_lanes_added + segment.r_lanes_added)
+                    self.lanes_change_list[-1][0] += segment.l_lanes_added
+                    self.lanes_change_list[-1][1] += segment.r_lanes_added
+
+
+class Segment:
+    def __init__(self, segment_id):
+        self.segment_id = segment_id
+        self.link = None
+        self.ref_node = None
+        self.start_lr = 0.0
+        self.end_lr = 0.0
+        self.l_lanes_added = 0
+        self.r_lanes_added = 0
+
+        self.other_attrs = {}
+
+
+class Movement:
+    def __init__(self, movement_id):
+        self.movement_id = movement_id
+        self.node = None
+        self.ib_link = None
+        self.ob_link = None
+
+        self.start_ib_lane = None
+        self.end_ib_lane = None
+        self.start_ob_lane = None
+        self.end_ob_lane = None
+
+        self.start_ib_lane_seq_no = None
+        self.end_ib_lane_seq_no = None
+        self.start_ob_lane_seq_no = None
+        self.end_ob_lane_seq_no = None
+
+        self.name = ''
+        self.lanes = 0
+        self.type = ''
+        self.penalty = 0.0
+        self.capacity = 0.0
+        self.ctrl_type = ''
+        self.volume = None
+        self.free_speed = None
+        # self.intersection_id = None
+        self.mvmt_txt_id = ''
+        self.allowed_uses = []
+
+        self.geometry = None
+        self.geometry_xy = None
+
+        self.generated_by_osm2gmns = False
+
+        self.other_attrs = {}
+
+
+class POI:
+    def __init__(self):
+        self.poi_id = 0
+        self.osm_way_id = None      # str
+        self.osm_relation_id = None
+        self.name = None
+        self.geometry = None
+        self.geometry_xy = None
+        self.centroid = None
+        self.centroid_xy = None
+        self.nearest_node = None
+        self.building = None
+        self.amenity = None
+        self.leisure = None
+        self.way = None         # highway,railway,aeroway poi
+
+
+class Network(BaseNetwork):
+    def __init__(self):
+        super().__init__()
+
+        self.default_lanes = False
+        self.default_speed = False
+        self.default_capacity = False
+
+        self.max_intersection_id = 0
+        self.max_segment_id = 0
+        self.max_poi_id = 0
+        self.max_movement_id = 0
+
+        self.user_input_movement_list = []
+
+        self.POI_list = []
+
+        self.movement_other_attrs = []
+        self.segment_other_attrs = []
+
+        self.mesonet = None
+        self.micronet = None
+
+
+    @property
+    def number_of_pois(self):
+        return len(self.POI_list)
+    @property
+    def complete_link_lane_info(self):
+        complete_link_lane_info = True
+        for _, link in self.link_dict.items():
+            if link.lanes is None:
+                complete_link_lane_info = False
+                break
+        return complete_link_lane_info
+
```

### Comparing `osm2gmns-0.7.5/osm2gmns/networkclass/mesonet.py` & `osm2gmns-0.7.6/osm2gmns/networkclass/mesonet.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-# @author       Jiawei Lu (jiaweil9@asu.edu)
-# @time         2021/11/27 15:34
-# @desc         [script description]
-
-from osm2gmns.networkclass.basenet import BaseNode, BaseLink, BaseNetwork
-
-
-class MesoNode(BaseNode):
-    def __init__(self, node_id):
-        super().__init__(node_id)
-        self.macronode = None
-        self.macrolink = None
-    @property
-    def zone_id(self):
-        return self.macronode.zone_id if self.macronode is not None else None
-    @property
-    def macro_node_id(self):
-        return self.macronode.node_id if self.macronode is not None else None
-    @property
-    def macro_link_id(self):
-        return self.macrolink.link_id if self.macrolink is not None else None
-    @property
-    def activity_type(self):
-        return self.macronode.activity_type if self.macronode is not None else None
-    @property
-    def is_boundary(self):
-        if self.macronode is None:
-            if self.macrolink.from_node.is_boundary is None:
-                return None
-            else:
-                return 0
-        else:
-            if self.macronode.is_boundary is None:
-                return None
-            elif self.macronode.is_boundary != 2:
-                return self.macronode.is_boundary
-            else:
-                return -1 if self.incoming_link_list else 1
-
-
-class MesoLink(BaseLink):
-    def __init__(self, link_id):
-        super().__init__(link_id)
-        self.macronode = None
-        self.macrolink = None
-        self.movement = None
-
-        self.lanes_change = []
-
-        self.micronode_list = []  # micronode, lane by lane;
-        self.microlink_list = []  # microlink
-
-        self.micronode_bike = []
-        self.microlink_bike = []
-        self.micronode_walk = []
-        self.microlink_walk = []
-
-    @property
-    def upstream_normal_link_of_movement_link(self):
-        return self.from_node.incoming_link_list[0]
-    @property
-    def macro_node_id(self):
-        return self.macronode.node_id if self.macronode is not None else None
-    @property
-    def macro_link_id(self):
-        return self.macrolink.link_id if self.macrolink is not None else None
-    @property
-    def movement_id(self):
-        return self.movement.movement_id if self.movement is not None else None
-    @property
-    def mvmt_txt_id(self):
-        return self.movement.mvmt_txt_id if self.movement is not None else None
-    @property
-    def ctrl_type(self):
-        return self.macronode.ctrl_type if self.macronode is not None else None
-    @property
-    def link_type_name(self):
-        if self.macrolink is not None:
-            return self.macrolink.link_type_name
-        else:
-            return self.upstream_normal_link_of_movement_link.link_type_name
-    @property
-    def link_type(self):
-        if self.macrolink is not None:
-            return self.macrolink.link_type
-        else:
-            return self.upstream_normal_link_of_movement_link.link_type
-    @property
-    def free_speed(self):
-        if self.macrolink is not None:
-            return self.macrolink.free_speed
-        else:
-            return self.upstream_normal_link_of_movement_link.free_speed
-    @property
-    def capacity(self):
-        if self.macrolink is not None:
-            return self.macrolink.capacity
-        else:
-            return self.upstream_normal_link_of_movement_link.capacity
-    @property
-    def allowed_uses(self):
-        if self.macrolink is not None:
-            return self.macrolink.allowed_uses
-        else:
-            return self.upstream_normal_link_of_movement_link.allowed_uses
-
-
-
-class MesoNetwork(BaseNetwork):
-    def __init__(self):
+# @author       Jiawei Lu (jiaweil9@asu.edu)
+# @time         2021/11/27 15:34
+# @desc         [script description]
+
+from osm2gmns.networkclass.basenet import BaseNode, BaseLink, BaseNetwork
+
+
+class MesoNode(BaseNode):
+    def __init__(self, node_id):
+        super().__init__(node_id)
+        self.macronode = None
+        self.macrolink = None
+    @property
+    def zone_id(self):
+        return self.macronode.zone_id if self.macronode is not None else None
+    @property
+    def macro_node_id(self):
+        return self.macronode.node_id if self.macronode is not None else None
+    @property
+    def macro_link_id(self):
+        return self.macrolink.link_id if self.macrolink is not None else None
+    @property
+    def activity_type(self):
+        return self.macronode.activity_type if self.macronode is not None else None
+    @property
+    def is_boundary(self):
+        if self.macronode is None:
+            if self.macrolink.from_node.is_boundary is None:
+                return None
+            else:
+                return 0
+        else:
+            if self.macronode.is_boundary is None:
+                return None
+            elif self.macronode.is_boundary != 2:
+                return self.macronode.is_boundary
+            else:
+                return -1 if self.incoming_link_list else 1
+
+
+class MesoLink(BaseLink):
+    def __init__(self, link_id):
+        super().__init__(link_id)
+        self.macronode = None
+        self.macrolink = None
+        self.movement = None
+
+        self.lanes_change = []
+
+        self.micronode_list = []  # micronode, lane by lane;
+        self.microlink_list = []  # microlink
+
+        self.micronode_bike = []
+        self.microlink_bike = []
+        self.micronode_walk = []
+        self.microlink_walk = []
+
+    @property
+    def upstream_normal_link_of_movement_link(self):
+        return self.from_node.incoming_link_list[0]
+    @property
+    def macro_node_id(self):
+        return self.macronode.node_id if self.macronode is not None else None
+    @property
+    def macro_link_id(self):
+        return self.macrolink.link_id if self.macrolink is not None else None
+    @property
+    def movement_id(self):
+        return self.movement.movement_id if self.movement is not None else None
+    @property
+    def mvmt_txt_id(self):
+        return self.movement.mvmt_txt_id if self.movement is not None else None
+    @property
+    def ctrl_type(self):
+        return self.macronode.ctrl_type if self.macronode is not None else None
+    @property
+    def link_type_name(self):
+        if self.macrolink is not None:
+            return self.macrolink.link_type_name
+        else:
+            return self.upstream_normal_link_of_movement_link.link_type_name
+    @property
+    def link_type(self):
+        if self.macrolink is not None:
+            return self.macrolink.link_type
+        else:
+            return self.upstream_normal_link_of_movement_link.link_type
+    @property
+    def free_speed(self):
+        if self.macrolink is not None:
+            return self.macrolink.free_speed
+        else:
+            return self.upstream_normal_link_of_movement_link.free_speed
+    @property
+    def capacity(self):
+        if self.macrolink is not None:
+            return self.macrolink.capacity
+        else:
+            return self.upstream_normal_link_of_movement_link.capacity
+    @property
+    def allowed_uses(self):
+        if self.macrolink is not None:
+            return self.macrolink.allowed_uses
+        else:
+            return self.upstream_normal_link_of_movement_link.allowed_uses
+
+
+
+class MesoNetwork(BaseNetwork):
+    def __init__(self):
         super().__init__()
```

### Comparing `osm2gmns-0.7.5/osm2gmns/osmnet/build_net.py` & `osm2gmns-0.7.6/osm2gmns/osmnet/build_net.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,491 +1,491 @@
-from osm2gmns.networkclass.macronet import Node, Link, Network
-from osm2gmns.io.read_from_osm import readOSMFile
-from osm2gmns.osmnet.osmclasses import OSMNode
-from osm2gmns.osmnet.combine_links import combineShortLinks
-from osm2gmns.osmnet.pois import generatePOIs
-from osm2gmns.osmnet.wayfilters import *
-from osm2gmns.osmnet.check_args import checkArgs_getNetFromFile
-from osm2gmns.utils.util import getLogger
-from osm2gmns.utils.util_geo import offsetLine
-import osm2gmns.settings as og_settings
-from shapely import geometry
-
-# todo: remove useless nodes link_type
-
-def _createNodeOnBoundary(node_in, node_outside, network):
-    line = network.bounds.intersection(geometry.LineString([node_in.geometry,node_outside.geometry]))
-    lon, lat = line.coords[1]
-    geometry_lonlat = geometry.Point((round(lon,og_settings.lonlat_coord_precision),round(lat,og_settings.lonlat_coord_precision)))
-    boundary_osm_node = OSMNode('', '', geometry_lonlat, True, '', '')
-    boundary_osm_node.geometry_xy = network.GT.geo_from_latlon(geometry_lonlat)
-    boundary_osm_node.is_crossing = True
-    boundary_osm_node.notes = 'boundary node created by osm2gmns'
-    return boundary_osm_node
-
-
-def _getSegmentNodeList(way, segment_no, network):
-    m_segment_node_list = way.segment_node_list[segment_no]
-    if way.is_reversed: m_segment_node_list = list(reversed(m_segment_node_list))
-    number_of_nodes = len(m_segment_node_list)
-
-    m_segment_node_list_group = []
-
-    if m_segment_node_list[0].in_region:
-        idx_first_outside = -1
-        for idx, node in enumerate(m_segment_node_list):
-            if not node.in_region:
-                idx_first_outside = idx
-                break
-
-        if idx_first_outside == -1:
-            m_segment_node_list_group.append(m_segment_node_list)
-            return m_segment_node_list_group
-        else:
-            new_node = _createNodeOnBoundary(m_segment_node_list[idx_first_outside-1],m_segment_node_list[idx_first_outside], network)
-            m_segment_node_list_group.append(m_segment_node_list[:idx_first_outside] + [new_node])
-
-    if m_segment_node_list[-1].in_region:
-        idx_last_outside = -1
-        for idx in range(number_of_nodes-2,-1,-1):
-            if not m_segment_node_list[idx].in_region:
-                idx_last_outside = idx
-                break
-        new_node = _createNodeOnBoundary(m_segment_node_list[idx_last_outside+1],m_segment_node_list[idx_last_outside], network)
-        m_segment_node_list_group.append([new_node] + m_segment_node_list[idx_last_outside+1:])
-
-    return m_segment_node_list_group
-
-
-def _createNodeFromOSMNode(network, osmnode):
-    if osmnode.node is None:
-        node = Node(network.max_node_id)
-        node.buildFromOSMNode(osmnode)
-        osmnode.node = node
-        network.node_dict[node.node_id] = node
-        network.max_node_id += 1
-
-
-def _createNodesAndLinks(network, link_way_list):
-    if og_settings.verbose:
-        print('    generating nodes and links')
-
-    link_dict = {}
-    max_link_id = network.max_link_id
-    for way in link_way_list:
-        if way.is_pure_cycle: continue
-        way.getNodeListForSegments()
-        for segment_no in range(way.number_of_segments):
-            m_segment_node_list_group = _getSegmentNodeList(way, segment_no, network)
-            for m_segment_node_list in m_segment_node_list_group:
-                if len(m_segment_node_list) < 2: continue
-                _createNodeFromOSMNode(network, m_segment_node_list[0])
-                _createNodeFromOSMNode(network, m_segment_node_list[-1])
-
-                link = Link(max_link_id)
-                link.buildFromOSMWay(way, 1, m_segment_node_list, network.default_lanes, network.default_speed, network.default_capacity)
-                link_dict[link.link_id] = link
-                max_link_id += 1
-                if not way.oneway:
-                    linkb = Link(max_link_id)
-                    linkb.buildFromOSMWay(way, -1, list(reversed(m_segment_node_list)), network.default_lanes, network.default_speed, network.default_capacity)
-                    link_dict[linkb.link_id] = linkb
-                    max_link_id += 1
-    network.link_dict = link_dict
-    network.max_link_id = max_link_id
-
-
-def _identifyPureCycleWays(link_way_list):
-    for way in link_way_list:
-        if way.is_cycle:
-            way.is_pure_cycle = True
-            for node in way.ref_node_list[1:-1]:
-                if node.is_crossing:
-                    way.is_pure_cycle = False
-                    break
-
-
-def _addSignalFromLink(network):
-    for link_id, link in network.link_dict.items():
-        if link.ctrl_type == 'signal':
-            to_node = link.to_node
-            if to_node.ctrl_type != 'signal':
-                if len(to_node.incoming_link_list) > 1 or len(to_node.outgoing_link_list) > 1:
-                    to_node.ctrl_type = 'signal'
-
-
-def _removeIsolated(network, min_nodes):
-    if og_settings.verbose:
-        print(f'    removing sub networks with less than {min_nodes} nodes')
-
-    node_list = []
-    node_to_idx_dict = {}
-    for idx, (node_id,node) in enumerate(network.node_dict.items()):
-        node_list.append(node)
-        node_to_idx_dict[node] = idx
-
-    number_of_nodes = len(node_list)
-    node_group_id_list = [-1] * number_of_nodes
-
-    group_id = 0
-    start_idx = 0
-
-    while True:
-        unprocessed_node_list = [node_list[start_idx]]
-        node_group_id_list[start_idx] = group_id
-        while unprocessed_node_list:
-            node = unprocessed_node_list.pop()
-            for ob_link in node.outgoing_link_list:
-                ob_node = ob_link.to_node
-                if node_group_id_list[node_to_idx_dict[ob_node]] == -1:
-                    node_group_id_list[node_to_idx_dict[ob_node]] = group_id
-                    unprocessed_node_list.append(ob_node)
-
-            for ib_link in node.incoming_link_list:
-                ib_node = ib_link.from_node
-                if node_group_id_list[node_to_idx_dict[ib_node]] == -1:
-                    node_group_id_list[node_to_idx_dict[ib_node]] = group_id
-                    unprocessed_node_list.append(ib_node)
-
-        unreachable_node_exits = False
-        idx = 0
-        for idx in range(start_idx+1,number_of_nodes):
-            if node_group_id_list[idx] == -1:
-                unreachable_node_exits = True
-                break
-
-        if unreachable_node_exits:
-            start_idx = idx
-            group_id += 1
-        else:
-            break
-
-    group_id_set = set(node_group_id_list)
-    group_isolated_dict = {}
-    for group_id in group_id_set:
-        group_size = node_group_id_list.count(group_id)
-        if group_size < min_nodes:
-            group_isolated_dict[group_id] = True
-        else:
-            group_isolated_dict[group_id] = False
-
-    removal_link_set = set()
-    for idx, node in enumerate(node_list):
-        if group_isolated_dict[node_group_id_list[idx]]:
-            del network.node_dict[node.node_id]
-            for ob_link in node.outgoing_link_list: removal_link_set.add(ob_link)
-            for ib_link in node.incoming_link_list: removal_link_set.add(ib_link)
-    for link in removal_link_set:
-        del network.link_dict[link.link_id]
-
-
-def _updateDefaultLSC(default_lanes, default_speed, default_capacity, network):
-    if default_lanes:
-        if isinstance(default_lanes,bool):
-            network.default_lanes = og_settings.default_lanes_dict
-        elif isinstance(default_lanes,dict):
-            network.default_lanes = default_lanes
-            for link_type_name, lanes in og_settings.default_lanes_dict.items():
-                if link_type_name not in default_lanes.keys():
-                    network.default_lanes[link_type_name] = lanes
-
-    if default_speed:
-        if isinstance(default_speed,bool):
-            network.default_speed = og_settings.default_speed_dict
-        elif isinstance(default_speed,dict):
-            network.default_speed = default_speed
-            for link_type_name, speed in og_settings.default_speed_dict.items():
-                if link_type_name not in default_speed.keys():
-                    network.default_speed[link_type_name] = speed
-
-    if default_capacity:
-        if isinstance(default_capacity,bool):
-            network.default_capacity = og_settings.default_capacity_dict
-        elif isinstance(default_capacity,dict):
-            network.default_capacity = default_capacity
-            for link_type_name, capacity in og_settings.default_capacity_dict.items():
-                if link_type_name not in default_speed.keys():
-                    network.default_capacity[link_type_name] = capacity
-
-
-def _offsetLinks(network, offset):
-    if og_settings.verbose:
-        print('    offseting link geometries')
-
-    distance_sp = -2 if offset == 'right' else 2
-    distance_ma = 2 if offset == 'right' else -2
-
-    GT = network.GT
-
-    for _, link in network.link_dict.items():
-        if link.from_bidirectional_way:
-            geometry_xy = link.geometry_xy.offset_curve(distance=distance_sp, join_style=2)
-            if isinstance(geometry_xy, geometry.MultiLineString):
-                geometry_xy = offsetLine(link.geometry_xy, distance_ma)
-
-            link.geometry_xy = geometry_xy
-            link.geometry = GT.geo_to_latlon(link.geometry_xy)
-
-            # distance = max(link.lanes_list) / 2 * 3.5
-            # geometry_xy = link.geometry_xy.parallel_offset(distance=2, side=offset, join_style=2)
-            # if offset == 'right':
-            #     if isinstance(geometry_xy, geometry.MultiLineString):
-            #         coords = []
-            #         for ls in geometry_xy.geoms: coords += list(ls.coords)[::-1]
-            #         link.geometry_xy = geometry.LineString(coords)
-            #     else:
-            #         link.geometry_xy = geometry.LineString(list(geometry_xy.coords)[::-1])
-            # elif offset == 'left':
-            #     link.geometry_xy = geometry_xy
-            #
-            # link.geometry = GT.geo_to_latlon(link.geometry_xy)
-
-
-def _preprocessWays(osmnetwork, link_types, network_types):
-    link_way_list = []
-    POI_way_list = []
-    network_types_set = set(network_types)
-    include_railway = True if 'railway' in network_types_set else False
-    include_aeroway = True if 'aeroway' in network_types_set else False
-
-    for _, way in osmnetwork.osm_way_dict.items():
-        if way.building or way.amenity or way.leisure:
-            POI_way_list.append(way)
-
-        elif way.highway:
-            if way.highway in highway_poi_set:
-                way.way_poi = way.highway
-                POI_way_list.append(way)
-                continue
-            if way.area and way.area != 'no':
-                continue
-            if way.highway in negligible_highway_type_set:
-                continue
-            if len(way.ref_node_list) < 2:
-                continue
-
-            try:
-                way.link_type_name, way.is_link = og_settings.osm_highway_type_dict[way.highway]
-                way.link_type = og_settings.link_type_no_dict[way.link_type_name]
-            except KeyError:
-                logger = getLogger()
-                if logger: logger.warning(f'new highway type at way {way.osm_way_id}, {way.highway}')
-                continue
-
-            valid_link_type = link_types == 'all' or way.link_type_name in link_types
-            if not valid_link_type:
-                continue
-
-            allowable_agent_type_list = getAllowableAgentType(way)
-            way.allowable_agent_type_list = list(set(allowable_agent_type_list).intersection(network_types_set))
-            if len(way.allowable_agent_type_list) == 0:
-                continue
-            way.allowed_uses = way.allowable_agent_type_list
-
-            way.ref_node_list[0].is_crossing = True
-            way.ref_node_list[-1].is_crossing = True
-            for node in way.ref_node_list:
-                node.usage_count += 1
-
-            if way.ref_node_list[0] is way.ref_node_list[-1]:
-                way.is_cycle = True
-            if way.oneway is None:
-                if way.junction in ['circular', 'roundabout']:
-                    way.oneway = True
-                else:
-                    way.oneway = og_settings.default_oneway_flag_dict[way.link_type_name]
-            way.link_class = 'highway'
-            link_way_list.append(way)
-
-        elif way.railway:
-            if not include_railway: continue
-
-            if way.railway in railway_poi_set:
-                way.way_poi = way.railway
-                POI_way_list.append(way)
-                continue
-            if way.area and way.area != 'no':
-                continue
-            if way.railway in negligible_railway_type_set:
-                continue
-            if len(way.ref_node_list) < 2:
-                continue
-
-            way.ref_node_list[0].is_crossing = True
-            way.ref_node_list[-1].is_crossing = True
-            for node in way.ref_node_list[1:-1]: node.usage_count += 1
-
-            way.link_type_name = way.railway
-            way.link_type = og_settings.link_type_no_dict['railway']
-            if way.oneway is None:
-                way.oneway = og_settings.default_oneway_flag_dict['railway']
-            way.link_class = 'railway'
-            link_way_list.append(way)
-
-        elif way.aeroway:
-            if not include_aeroway: continue
-
-            if way.aeroway in aeroway_poi_set:
-                way.way_poi = way.aeroway
-                POI_way_list.append(way)
-                continue
-            if way.area and way.area != 'no':
-                continue
-            if way.aeroway in negligible_aeroway_type_set:
-                continue
-            if len(way.ref_node_list) < 2:
-                continue
-
-            way.ref_node_list[0].is_crossing = True
-            way.ref_node_list[-1].is_crossing = True
-            for node in way.ref_node_list[1:-1]: node.usage_count += 1
-
-            way.link_type_name = way.aeroway
-            way.link_type = og_settings.link_type_no_dict['aeroway']
-            if way.oneway is None:
-                way.oneway = og_settings.default_oneway_flag_dict['aeroway']
-            way.link_class = 'aeroway'
-            link_way_list.append(way)
-
-        else:
-            pass
-
-    osmnetwork.link_way_list = link_way_list
-    osmnetwork.POI_way_list = POI_way_list
-
-
-def _identifyCrossingOSMNodes(osm_node_dict):
-    for _, osmnode in osm_node_dict.items():
-        if osmnode.usage_count >= 2 or osmnode.ctrl_type == 'signal':
-            osmnode.is_crossing = True
-
-
-def _createNLPs(osmnetwork, network, link_types, network_types, POI, POI_percentage):
-    _preprocessWays(osmnetwork, link_types, network_types)
-    _identifyCrossingOSMNodes(osmnetwork.osm_node_dict)
-    _identifyPureCycleWays(osmnetwork.link_way_list)
-    _createNodesAndLinks(network, osmnetwork.link_way_list)
-    _addSignalFromLink(network)
-
-    if POI: generatePOIs(osmnetwork.POI_way_list, osmnetwork.osm_relation_list, network, POI_percentage)
-
-
-
-def _buildNet(osmnetwork, network_types, link_types, POI, POI_percentage, offset, min_nodes, combine, default_lanes,
-              default_speed, default_capacity, start_node_id, start_link_id):
-    if og_settings.verbose:
-        print('  parsing osm network')
-
-    network = Network()
-    network.max_node_id = start_node_id
-    network.max_link_id = start_link_id
-
-    network.GT, network.bounds = osmnetwork.GT, osmnetwork.bounds
-
-    # update default lanes, speed, and capacity
-    _updateDefaultLSC(default_lanes, default_speed, default_capacity, network)
-
-    # create node, link, poi
-    _createNLPs(osmnetwork, network, link_types, network_types, POI, POI_percentage)
-
-    # remove isolated nodes and links
-    if min_nodes > 1: _removeIsolated(network, min_nodes)
-
-    # combine adjacent links at two-degree nodes
-    if combine: combineShortLinks(network)
-
-    # offset two-way overlapping links
-    if offset != 'no': _offsetLinks(network, offset)
-
-    return network
-
-
-def getNetFromFile(filename='map.osm', network_types=('auto',), link_types='all', POI=False, POI_sampling_ratio=1.0,
-                   strict_mode=True, offset='no', min_nodes=1, combine=False, bbox=None,
-                   default_lanes=False, default_speed=False, default_capacity=False, start_node_id=0, start_link_id=0):
-    """
-    Get an osm2gmns Network object from an osm file
-
-    Parameters
-    ----------
-    filename: str
-        path of an osm file; can be absolute or relative path; supported osm file formats: .osm, .xml, and .pbf
-    network_types: str, tuple of strings, list of strings, or set of strings
-        osm2gmns supports five different network types, including auto, bike, walk, railway, and aeroway.
-        network_types can be any one or any combinations of the five supported network types
-    link_types: str, tuple of strings, list of strings, or set of strings
-        supported link types: motorway, trunk, primary, secondary, tertiary, residential, service, cycleway,
-        footway, track, unclassified, connector, railway, and aeroway.
-    POI: bool
-        if extract point of interest information
-    POI_sampling_ratio: float
-        prcentage of POIs to be extracted if POI is set as True. this value should be a float number between 0.0 and 1.0.
-    strict_mode: bool
-        if True, network elements (node, link, poi) outside the boundary will be discarded
-    offset: str
-        offset overlapping links. the value of this argument can be 'left', 'right', or 'no'
-    min_nodes: int
-        a network return by the function may contain several sub-networks that are disconnected from each other.
-        sub-networks with the number of nodes less than min_nodes will be discarded
-    combine: bool
-        if True, adjacent short links with the same attributes will be combined into a long link. the operation will only
-        be performed on short links connected with a two-degree nodes (one incoming link and one outgoing link)
-    bbox: tuple of four float/int values, list of four float/int values, None
-        specify the boundary of the network to be extracted, consisting of minimum latitude, minimum longtitude, maximum latitude, and maximum longitud.
-        if None, osm2gmns will try to find network boundary from the input osm file
-    default_lanes: bool, dict
-        if True, assign a default value for links without lanes information based on built-in settings. if a dict,
-        assign a default value for links without lanes information based on the dict passed by users.
-    default_speed: bool, dict
-        if True, assign a default value for links without speed information based on built-in settings. if a dict,
-        assign a default value for links without speed information based on the dict passed by users.
-    default_capacity: bool, dict
-        if True, assign a default value for links without capacity information based on built-in settings. if a dict,
-        assign a default value for links without capacity information based on the dict passed by users.
-    start_node_id: int
-        osm2gmns assigns node_ids to generated nodes starting from start_node_id.
-    start_link_id: int
-        osm2gmns assigns link_ids to generated links starting from start_link_id
-
-    Returns
-    -------
-    network: Network
-        osm2gmns Network object
-    """
-
-    if og_settings.verbose:
-        print('arguments used for network parsing:')
-        print(f'  filename: {filename}')
-        print(f'  network_types: {network_types}')
-        print(f'  link_types: {link_types}')
-        print(f'  POI: {POI}')
-        print(f'  POI_sampling_ratio: {POI_sampling_ratio}')
-        print(f'  strict_mode: {strict_mode}')
-        print(f'  offset: {offset}')
-        print(f'  min_nodes: {min_nodes}')
-        print(f'  combine: {combine}')
-        print(f'  bbox: {bbox}')
-        print(f'  default_lanes: {default_lanes}')
-        print(f'  default_speed: {default_speed}')
-        print(f'  default_capacity: {default_capacity}')
-        print(f'  start_node_id: {start_node_id}')
-        print(f'  start_link_id: {start_link_id}\n')
-
-        print('Building Network from OSM file')
-
-    network_types_, link_types_, POI_, POI_sampling_ratio_, strict_mode_, offset_, min_nodes_, combine_, \
-        bbox_, default_lanes_, default_speed_, default_capacity_, start_node_id_, start_link_id_ = \
-        checkArgs_getNetFromFile(filename, network_types, link_types, POI, POI_sampling_ratio, strict_mode, offset,
-                                min_nodes, combine, bbox, default_lanes, default_speed, default_capacity, start_node_id,
-                                 start_link_id)
-
-    osmnetwork = readOSMFile(filename, POI_, strict_mode_, bbox_)
-
-    network = _buildNet(osmnetwork, network_types_, link_types_, POI_, POI_sampling_ratio_, offset_, min_nodes_, combine_,
-                        default_lanes_, default_speed_, default_capacity_, start_node_id_, start_link_id_)
-
-    if og_settings.verbose:
-        print(f'  number of nodes: {len(network.node_dict)}, number of links: {len(network.link_dict)}, number of pois: {len(network.POI_list)}')
-
-    return network
-
-
+from osm2gmns.networkclass.macronet import Node, Link, Network
+from osm2gmns.io.read_from_osm import readOSMFile
+from osm2gmns.osmnet.osmclasses import OSMNode
+from osm2gmns.osmnet.combine_links import combineShortLinks
+from osm2gmns.osmnet.pois import generatePOIs
+from osm2gmns.osmnet.wayfilters import *
+from osm2gmns.osmnet.check_args import checkArgs_getNetFromFile
+from osm2gmns.utils.util import getLogger
+from osm2gmns.utils.util_geo import offsetLine
+import osm2gmns.settings as og_settings
+from shapely import geometry
+
+# todo: remove useless nodes link_type
+
+def _createNodeOnBoundary(node_in, node_outside, network):
+    line = network.bounds.intersection(geometry.LineString([node_in.geometry,node_outside.geometry]))
+    lon, lat = line.coords[1]
+    geometry_lonlat = geometry.Point((round(lon,og_settings.lonlat_coord_precision),round(lat,og_settings.lonlat_coord_precision)))
+    boundary_osm_node = OSMNode('', '', geometry_lonlat, True, '', '')
+    boundary_osm_node.geometry_xy = network.GT.geo_from_latlon(geometry_lonlat)
+    boundary_osm_node.is_crossing = True
+    boundary_osm_node.notes = 'boundary node created by osm2gmns'
+    return boundary_osm_node
+
+
+def _getSegmentNodeList(way, segment_no, network):
+    m_segment_node_list = way.segment_node_list[segment_no]
+    if way.is_reversed: m_segment_node_list = list(reversed(m_segment_node_list))
+    number_of_nodes = len(m_segment_node_list)
+
+    m_segment_node_list_group = []
+
+    if m_segment_node_list[0].in_region:
+        idx_first_outside = -1
+        for idx, node in enumerate(m_segment_node_list):
+            if not node.in_region:
+                idx_first_outside = idx
+                break
+
+        if idx_first_outside == -1:
+            m_segment_node_list_group.append(m_segment_node_list)
+            return m_segment_node_list_group
+        else:
+            new_node = _createNodeOnBoundary(m_segment_node_list[idx_first_outside-1],m_segment_node_list[idx_first_outside], network)
+            m_segment_node_list_group.append(m_segment_node_list[:idx_first_outside] + [new_node])
+
+    if m_segment_node_list[-1].in_region:
+        idx_last_outside = -1
+        for idx in range(number_of_nodes-2,-1,-1):
+            if not m_segment_node_list[idx].in_region:
+                idx_last_outside = idx
+                break
+        new_node = _createNodeOnBoundary(m_segment_node_list[idx_last_outside+1],m_segment_node_list[idx_last_outside], network)
+        m_segment_node_list_group.append([new_node] + m_segment_node_list[idx_last_outside+1:])
+
+    return m_segment_node_list_group
+
+
+def _createNodeFromOSMNode(network, osmnode):
+    if osmnode.node is None:
+        node = Node(network.max_node_id)
+        node.buildFromOSMNode(osmnode)
+        osmnode.node = node
+        network.node_dict[node.node_id] = node
+        network.max_node_id += 1
+
+
+def _createNodesAndLinks(network, link_way_list):
+    if og_settings.verbose:
+        print('    generating nodes and links')
+
+    link_dict = {}
+    max_link_id = network.max_link_id
+    for way in link_way_list:
+        if way.is_pure_cycle: continue
+        way.getNodeListForSegments()
+        for segment_no in range(way.number_of_segments):
+            m_segment_node_list_group = _getSegmentNodeList(way, segment_no, network)
+            for m_segment_node_list in m_segment_node_list_group:
+                if len(m_segment_node_list) < 2: continue
+                _createNodeFromOSMNode(network, m_segment_node_list[0])
+                _createNodeFromOSMNode(network, m_segment_node_list[-1])
+
+                link = Link(max_link_id)
+                link.buildFromOSMWay(way, 1, m_segment_node_list, network.default_lanes, network.default_speed, network.default_capacity)
+                link_dict[link.link_id] = link
+                max_link_id += 1
+                if not way.oneway:
+                    linkb = Link(max_link_id)
+                    linkb.buildFromOSMWay(way, -1, list(reversed(m_segment_node_list)), network.default_lanes, network.default_speed, network.default_capacity)
+                    link_dict[linkb.link_id] = linkb
+                    max_link_id += 1
+    network.link_dict = link_dict
+    network.max_link_id = max_link_id
+
+
+def _identifyPureCycleWays(link_way_list):
+    for way in link_way_list:
+        if way.is_cycle:
+            way.is_pure_cycle = True
+            for node in way.ref_node_list[1:-1]:
+                if node.is_crossing:
+                    way.is_pure_cycle = False
+                    break
+
+
+def _addSignalFromLink(network):
+    for link_id, link in network.link_dict.items():
+        if link.ctrl_type == 'signal':
+            to_node = link.to_node
+            if to_node.ctrl_type != 'signal':
+                if len(to_node.incoming_link_list) > 1 or len(to_node.outgoing_link_list) > 1:
+                    to_node.ctrl_type = 'signal'
+
+
+def _removeIsolated(network, min_nodes):
+    if og_settings.verbose:
+        print(f'    removing sub networks with less than {min_nodes} nodes')
+
+    node_list = []
+    node_to_idx_dict = {}
+    for idx, (node_id,node) in enumerate(network.node_dict.items()):
+        node_list.append(node)
+        node_to_idx_dict[node] = idx
+
+    number_of_nodes = len(node_list)
+    node_group_id_list = [-1] * number_of_nodes
+
+    group_id = 0
+    start_idx = 0
+
+    while True:
+        unprocessed_node_list = [node_list[start_idx]]
+        node_group_id_list[start_idx] = group_id
+        while unprocessed_node_list:
+            node = unprocessed_node_list.pop()
+            for ob_link in node.outgoing_link_list:
+                ob_node = ob_link.to_node
+                if node_group_id_list[node_to_idx_dict[ob_node]] == -1:
+                    node_group_id_list[node_to_idx_dict[ob_node]] = group_id
+                    unprocessed_node_list.append(ob_node)
+
+            for ib_link in node.incoming_link_list:
+                ib_node = ib_link.from_node
+                if node_group_id_list[node_to_idx_dict[ib_node]] == -1:
+                    node_group_id_list[node_to_idx_dict[ib_node]] = group_id
+                    unprocessed_node_list.append(ib_node)
+
+        unreachable_node_exits = False
+        idx = 0
+        for idx in range(start_idx+1,number_of_nodes):
+            if node_group_id_list[idx] == -1:
+                unreachable_node_exits = True
+                break
+
+        if unreachable_node_exits:
+            start_idx = idx
+            group_id += 1
+        else:
+            break
+
+    group_id_set = set(node_group_id_list)
+    group_isolated_dict = {}
+    for group_id in group_id_set:
+        group_size = node_group_id_list.count(group_id)
+        if group_size < min_nodes:
+            group_isolated_dict[group_id] = True
+        else:
+            group_isolated_dict[group_id] = False
+
+    removal_link_set = set()
+    for idx, node in enumerate(node_list):
+        if group_isolated_dict[node_group_id_list[idx]]:
+            del network.node_dict[node.node_id]
+            for ob_link in node.outgoing_link_list: removal_link_set.add(ob_link)
+            for ib_link in node.incoming_link_list: removal_link_set.add(ib_link)
+    for link in removal_link_set:
+        del network.link_dict[link.link_id]
+
+
+def _updateDefaultLSC(default_lanes, default_speed, default_capacity, network):
+    if default_lanes:
+        if isinstance(default_lanes,bool):
+            network.default_lanes = og_settings.default_lanes_dict
+        elif isinstance(default_lanes,dict):
+            network.default_lanes = default_lanes
+            for link_type_name, lanes in og_settings.default_lanes_dict.items():
+                if link_type_name not in default_lanes.keys():
+                    network.default_lanes[link_type_name] = lanes
+
+    if default_speed:
+        if isinstance(default_speed,bool):
+            network.default_speed = og_settings.default_speed_dict
+        elif isinstance(default_speed,dict):
+            network.default_speed = default_speed
+            for link_type_name, speed in og_settings.default_speed_dict.items():
+                if link_type_name not in default_speed.keys():
+                    network.default_speed[link_type_name] = speed
+
+    if default_capacity:
+        if isinstance(default_capacity,bool):
+            network.default_capacity = og_settings.default_capacity_dict
+        elif isinstance(default_capacity,dict):
+            network.default_capacity = default_capacity
+            for link_type_name, capacity in og_settings.default_capacity_dict.items():
+                if link_type_name not in default_speed.keys():
+                    network.default_capacity[link_type_name] = capacity
+
+
+def _offsetLinks(network, offset):
+    if og_settings.verbose:
+        print('    offseting link geometries')
+
+    distance_sp = -2 if offset == 'right' else 2
+    distance_ma = 2 if offset == 'right' else -2
+
+    GT = network.GT
+
+    for _, link in network.link_dict.items():
+        if link.from_bidirectional_way:
+            geometry_xy = link.geometry_xy.offset_curve(distance=distance_sp, join_style=2)
+            if isinstance(geometry_xy, geometry.MultiLineString):
+                geometry_xy = offsetLine(link.geometry_xy, distance_ma)
+
+            link.geometry_xy = geometry_xy
+            link.geometry = GT.geo_to_latlon(link.geometry_xy)
+
+            # distance = max(link.lanes_list) / 2 * 3.5
+            # geometry_xy = link.geometry_xy.parallel_offset(distance=2, side=offset, join_style=2)
+            # if offset == 'right':
+            #     if isinstance(geometry_xy, geometry.MultiLineString):
+            #         coords = []
+            #         for ls in geometry_xy.geoms: coords += list(ls.coords)[::-1]
+            #         link.geometry_xy = geometry.LineString(coords)
+            #     else:
+            #         link.geometry_xy = geometry.LineString(list(geometry_xy.coords)[::-1])
+            # elif offset == 'left':
+            #     link.geometry_xy = geometry_xy
+            #
+            # link.geometry = GT.geo_to_latlon(link.geometry_xy)
+
+
+def _preprocessWays(osmnetwork, link_types, network_types):
+    link_way_list = []
+    POI_way_list = []
+    network_types_set = set(network_types)
+    include_railway = True if 'railway' in network_types_set else False
+    include_aeroway = True if 'aeroway' in network_types_set else False
+
+    for _, way in osmnetwork.osm_way_dict.items():
+        if way.building or way.amenity or way.leisure:
+            POI_way_list.append(way)
+
+        elif way.highway:
+            if way.highway in highway_poi_set:
+                way.way_poi = way.highway
+                POI_way_list.append(way)
+                continue
+            if way.area and way.area != 'no':
+                continue
+            if way.highway in negligible_highway_type_set:
+                continue
+            if len(way.ref_node_list) < 2:
+                continue
+
+            try:
+                way.link_type_name, way.is_link = og_settings.osm_highway_type_dict[way.highway]
+                way.link_type = og_settings.link_type_no_dict[way.link_type_name]
+            except KeyError:
+                logger = getLogger()
+                if logger: logger.warning(f'new highway type at way {way.osm_way_id}, {way.highway}')
+                continue
+
+            valid_link_type = link_types == 'all' or way.link_type_name in link_types
+            if not valid_link_type:
+                continue
+
+            allowable_agent_type_list = getAllowableAgentType(way)
+            way.allowable_agent_type_list = list(set(allowable_agent_type_list).intersection(network_types_set))
+            if len(way.allowable_agent_type_list) == 0:
+                continue
+            way.allowed_uses = way.allowable_agent_type_list
+
+            way.ref_node_list[0].is_crossing = True
+            way.ref_node_list[-1].is_crossing = True
+            for node in way.ref_node_list:
+                node.usage_count += 1
+
+            if way.ref_node_list[0] is way.ref_node_list[-1]:
+                way.is_cycle = True
+            if way.oneway is None:
+                if way.junction in ['circular', 'roundabout']:
+                    way.oneway = True
+                else:
+                    way.oneway = og_settings.default_oneway_flag_dict[way.link_type_name]
+            way.link_class = 'highway'
+            link_way_list.append(way)
+
+        elif way.railway:
+            if not include_railway: continue
+
+            if way.railway in railway_poi_set:
+                way.way_poi = way.railway
+                POI_way_list.append(way)
+                continue
+            if way.area and way.area != 'no':
+                continue
+            if way.railway in negligible_railway_type_set:
+                continue
+            if len(way.ref_node_list) < 2:
+                continue
+
+            way.ref_node_list[0].is_crossing = True
+            way.ref_node_list[-1].is_crossing = True
+            for node in way.ref_node_list[1:-1]: node.usage_count += 1
+
+            way.link_type_name = way.railway
+            way.link_type = og_settings.link_type_no_dict['railway']
+            if way.oneway is None:
+                way.oneway = og_settings.default_oneway_flag_dict['railway']
+            way.link_class = 'railway'
+            link_way_list.append(way)
+
+        elif way.aeroway:
+            if not include_aeroway: continue
+
+            if way.aeroway in aeroway_poi_set:
+                way.way_poi = way.aeroway
+                POI_way_list.append(way)
+                continue
+            if way.area and way.area != 'no':
+                continue
+            if way.aeroway in negligible_aeroway_type_set:
+                continue
+            if len(way.ref_node_list) < 2:
+                continue
+
+            way.ref_node_list[0].is_crossing = True
+            way.ref_node_list[-1].is_crossing = True
+            for node in way.ref_node_list[1:-1]: node.usage_count += 1
+
+            way.link_type_name = way.aeroway
+            way.link_type = og_settings.link_type_no_dict['aeroway']
+            if way.oneway is None:
+                way.oneway = og_settings.default_oneway_flag_dict['aeroway']
+            way.link_class = 'aeroway'
+            link_way_list.append(way)
+
+        else:
+            pass
+
+    osmnetwork.link_way_list = link_way_list
+    osmnetwork.POI_way_list = POI_way_list
+
+
+def _identifyCrossingOSMNodes(osm_node_dict):
+    for _, osmnode in osm_node_dict.items():
+        if osmnode.usage_count >= 2 or osmnode.ctrl_type == 'signal':
+            osmnode.is_crossing = True
+
+
+def _createNLPs(osmnetwork, network, link_types, network_types, POI, POI_percentage):
+    _preprocessWays(osmnetwork, link_types, network_types)
+    _identifyCrossingOSMNodes(osmnetwork.osm_node_dict)
+    _identifyPureCycleWays(osmnetwork.link_way_list)
+    _createNodesAndLinks(network, osmnetwork.link_way_list)
+    _addSignalFromLink(network)
+
+    if POI: generatePOIs(osmnetwork.POI_way_list, osmnetwork.osm_relation_list, network, POI_percentage)
+
+
+
+def _buildNet(osmnetwork, network_types, link_types, POI, POI_percentage, offset, min_nodes, combine, default_lanes,
+              default_speed, default_capacity, start_node_id, start_link_id):
+    if og_settings.verbose:
+        print('  parsing osm network')
+
+    network = Network()
+    network.max_node_id = start_node_id
+    network.max_link_id = start_link_id
+
+    network.GT, network.bounds = osmnetwork.GT, osmnetwork.bounds
+
+    # update default lanes, speed, and capacity
+    _updateDefaultLSC(default_lanes, default_speed, default_capacity, network)
+
+    # create node, link, poi
+    _createNLPs(osmnetwork, network, link_types, network_types, POI, POI_percentage)
+
+    # remove isolated nodes and links
+    if min_nodes > 1: _removeIsolated(network, min_nodes)
+
+    # combine adjacent links at two-degree nodes
+    if combine: combineShortLinks(network)
+
+    # offset two-way overlapping links
+    if offset != 'no': _offsetLinks(network, offset)
+
+    return network
+
+
+def getNetFromFile(filename='map.osm', network_types=('auto',), link_types='all', POI=False, POI_sampling_ratio=1.0,
+                   strict_mode=True, offset='no', min_nodes=1, combine=False, bbox=None,
+                   default_lanes=False, default_speed=False, default_capacity=False, start_node_id=0, start_link_id=0):
+    """
+    Get an osm2gmns Network object from an osm file
+
+    Parameters
+    ----------
+    filename: str
+        path of an osm file; can be absolute or relative path; supported osm file formats: .osm, .xml, and .pbf
+    network_types: str, tuple of strings, list of strings, or set of strings
+        osm2gmns supports five different network types, including auto, bike, walk, railway, and aeroway.
+        network_types can be any one or any combinations of the five supported network types
+    link_types: str, tuple of strings, list of strings, or set of strings
+        supported link types: motorway, trunk, primary, secondary, tertiary, residential, service, cycleway,
+        footway, track, unclassified, connector, railway, and aeroway.
+    POI: bool
+        if extract point of interest information
+    POI_sampling_ratio: float
+        prcentage of POIs to be extracted if POI is set as True. this value should be a float number between 0.0 and 1.0.
+    strict_mode: bool
+        if True, network elements (node, link, poi) outside the boundary will be discarded
+    offset: str
+        offset overlapping links. the value of this argument can be 'left', 'right', or 'no'
+    min_nodes: int
+        a network return by the function may contain several sub-networks that are disconnected from each other.
+        sub-networks with the number of nodes less than min_nodes will be discarded
+    combine: bool
+        if True, adjacent short links with the same attributes will be combined into a long link. the operation will only
+        be performed on short links connected with a two-degree nodes (one incoming link and one outgoing link)
+    bbox: tuple of four float/int values, list of four float/int values, None
+        specify the boundary of the network to be extracted, consisting of minimum latitude, minimum longtitude, maximum latitude, and maximum longitud.
+        if None, osm2gmns will try to find network boundary from the input osm file
+    default_lanes: bool, dict
+        if True, assign a default value for links without lanes information based on built-in settings. if a dict,
+        assign a default value for links without lanes information based on the dict passed by users.
+    default_speed: bool, dict
+        if True, assign a default value for links without speed information based on built-in settings. if a dict,
+        assign a default value for links without speed information based on the dict passed by users.
+    default_capacity: bool, dict
+        if True, assign a default value for links without capacity information based on built-in settings. if a dict,
+        assign a default value for links without capacity information based on the dict passed by users.
+    start_node_id: int
+        osm2gmns assigns node_ids to generated nodes starting from start_node_id.
+    start_link_id: int
+        osm2gmns assigns link_ids to generated links starting from start_link_id
+
+    Returns
+    -------
+    network: Network
+        osm2gmns Network object
+    """
+
+    if og_settings.verbose:
+        print('arguments used for network parsing:')
+        print(f'  filename: {filename}')
+        print(f'  network_types: {network_types}')
+        print(f'  link_types: {link_types}')
+        print(f'  POI: {POI}')
+        print(f'  POI_sampling_ratio: {POI_sampling_ratio}')
+        print(f'  strict_mode: {strict_mode}')
+        print(f'  offset: {offset}')
+        print(f'  min_nodes: {min_nodes}')
+        print(f'  combine: {combine}')
+        print(f'  bbox: {bbox}')
+        print(f'  default_lanes: {default_lanes}')
+        print(f'  default_speed: {default_speed}')
+        print(f'  default_capacity: {default_capacity}')
+        print(f'  start_node_id: {start_node_id}')
+        print(f'  start_link_id: {start_link_id}\n')
+
+        print('Building Network from OSM file')
+
+    network_types_, link_types_, POI_, POI_sampling_ratio_, strict_mode_, offset_, min_nodes_, combine_, \
+        bbox_, default_lanes_, default_speed_, default_capacity_, start_node_id_, start_link_id_ = \
+        checkArgs_getNetFromFile(filename, network_types, link_types, POI, POI_sampling_ratio, strict_mode, offset,
+                                min_nodes, combine, bbox, default_lanes, default_speed, default_capacity, start_node_id,
+                                 start_link_id)
+
+    osmnetwork = readOSMFile(filename, POI_, strict_mode_, bbox_)
+
+    network = _buildNet(osmnetwork, network_types_, link_types_, POI_, POI_sampling_ratio_, offset_, min_nodes_, combine_,
+                        default_lanes_, default_speed_, default_capacity_, start_node_id_, start_link_id_)
+
+    if og_settings.verbose:
+        print(f'  number of nodes: {len(network.node_dict)}, number of links: {len(network.link_dict)}, number of pois: {len(network.POI_list)}')
+
+    return network
+
+
```

### Comparing `osm2gmns-0.7.5/osm2gmns/osmnet/check_args.py` & `osm2gmns-0.7.6/osm2gmns/osmnet/check_args.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,141 +1,141 @@
-from osm2gmns.osmnet.wayfilters import network_types_all
-import os
-import sys
-
-
-def checkArgs_getNetFromFile(filename, network_types, link_types, POI, POI_sampling_ratio,
-               strict_mode, offset, min_nodes, combine, bbox,
-               default_lanes, default_speed, default_capacity, start_node_id, start_link_id):
-    # filename
-    file_extension = os.path.splitext(filename)[-1]
-    if not file_extension:
-        sys.exit(f'ERROR: cannot detect the format of file {filename}. If it is a xml-based text file, please add extension .xml or .osm after the filename')
-    if not os.path.exists(filename):
-        sys.exit(f'ERROR: file {filename} does not exist')
-
-    # network_types
-    if isinstance(network_types, str):
-        network_types_temp = [network_types,]
-    elif isinstance(network_types, list) or isinstance(network_types, set) or isinstance(network_types, tuple):
-        network_types_temp = network_types
-    else:
-        sys.exit(f'ERROR: network_types must be a string, list, set, or tuple')
-
-    network_types_ = []
-    for net_type in network_types_temp:
-        if net_type not in network_types_all:
-            print(f'WARNING: network_type \'{net_type}\' does not belong to {network_types_all}, it will be skipped')
-        else:
-            network_types_.append(net_type)
-
-    # link_types
-    if link_types != 'all':
-        if isinstance(link_types, str):
-            link_types_ = (link_types,)
-        elif isinstance(link_types, list) or isinstance(link_types, set) or isinstance(link_types, tuple):
-            link_types_ = link_types
-        else:
-            sys.exit(f'ERROR: argument link_types must be a string, list, set, or tuple')
-    else:
-        link_types_ = link_types
-
-    # POIs
-    if isinstance(POI, bool):
-        POI_ = POI
-    else:
-        print('WARNING: argument POI should be a bool. The default value False has been applied')
-        POI_ = False
-
-    # POI_sampling_ratio
-    if isinstance(POI_sampling_ratio, int) or isinstance(POI_sampling_ratio, float):
-        if POI_sampling_ratio < 0.0 or POI_sampling_ratio > 1.0:
-            print('WARNING: argument POI_sampling_ratio should be a float between 0.0 and 1.0. The default value 1.0 has been applied')
-            POI_sampling_ratio_ = 1.0
-        else:
-            POI_sampling_ratio_ = POI_sampling_ratio
-    else:
-        print('WARNING: argument POI_sampling_ratio should be a float between 0.0 and 1.0. The default value 1.0 has been applied')
-        POI_sampling_ratio_ = 1.0
-
-    # strict_mode
-    if isinstance(strict_mode, bool):
-        strict_mode_ = strict_mode
-    else:
-        print('WARNING: argument strict_mode should be a bool. The default value True has been applied')
-        strict_mode_ = True
-
-    # offset
-    if offset in ('left', 'right', 'no'):
-        offset_ = offset
-    else:
-        print("WARNING: argument offset should be chosen from 'left', 'right', 'no'. The default value 'no' has been applied")
-        offset_ = 'no'
-
-    # min_nodes
-    if isinstance(min_nodes, int):
-        if min_nodes < 1:
-            print('WARNING: argument min_nodes should be a integer greater than or equal to 1. The default value 1 has been applied')
-            min_nodes_ = 1
-        else:
-            min_nodes_ = min_nodes
-    else:
-        print('WARNING: argument min_nodes should be an integer greater than or equal to 1. The default value 1 has been applied')
-        min_nodes_ = 1
-
-    # combine
-    if isinstance(combine, bool):
-        combine_ = combine
-    else:
-        print('WARNING: argument combine should be a bool. The default value False has been applied')
-        combine_ = False
-
-    # bbox
-    if bbox is None:
-        bbox_ = bbox
-    elif isinstance(bbox, tuple) or isinstance(bbox, list):
-        if len(bbox) == 4:
-            for ll in bbox:
-                if not(isinstance(ll, int) or isinstance(ll, float)):
-                    sys.exit('ERROR: argument bbox should be a tuple with four floats: (minlat, minlon, maxlat, maxlon)')
-            bbox_ = bbox
-        else:
-            sys.exit('ERROR: argument bbox should be a tuple with four floats: (minlat, minlon, maxlat, maxlon)')
-    else:
-        sys.exit('ERROR: argument bbox should be a tuple with four floats: (minlat, minlon, maxlat, maxlon)')
-
-    # default_lanes
-    if isinstance(default_lanes, bool) or isinstance(default_lanes, dict):
-        default_lanes_ = default_lanes
-    else:
-        print('WARNING: argument default_lanes should be a bool or a dict. The default value False has been applied')
-        default_lanes_ = False
-
-    # default_speed
-    if isinstance(default_speed, bool) or isinstance(default_speed, dict):
-        default_speed_ = default_speed
-    else:
-        print('WARNING: argument default_speed should be a bool or a dict. The default value False has been applied')
-        default_speed_ = False
-
-    # default_capacity
-    if isinstance(default_capacity, bool) or isinstance(default_capacity, dict):
-        default_capacity_ = default_capacity
-    else:
-        print('WARNING: argument default_capacity should be a bool or a dict. The default value False has been applied')
-        default_capacity_ = False
-
-    # start node/link id
-    if isinstance(start_node_id, int):
-        start_node_id_ = start_node_id
-    else:
-        print('WARNING: argument start_node_id should be a int. The default value 0 has been applied')
-        start_node_id_ = 0
-
-    if isinstance(start_link_id, int):
-        start_link_id_ = start_link_id
-    else:
-        print('WARNING: argument start_link_id should be a int. The default value 0 has been applied')
-        start_link_id_ = 0
-
-    return network_types_, link_types_, POI_, POI_sampling_ratio_, strict_mode_, offset_, min_nodes_, combine_,\
+from osm2gmns.osmnet.wayfilters import network_types_all
+import os
+import sys
+
+
+def checkArgs_getNetFromFile(filename, network_types, link_types, POI, POI_sampling_ratio,
+               strict_mode, offset, min_nodes, combine, bbox,
+               default_lanes, default_speed, default_capacity, start_node_id, start_link_id):
+    # filename
+    file_extension = os.path.splitext(filename)[-1]
+    if not file_extension:
+        sys.exit(f'ERROR: cannot detect the format of file {filename}. If it is a xml-based text file, please add extension .xml or .osm after the filename')
+    if not os.path.exists(filename):
+        sys.exit(f'ERROR: file {filename} does not exist')
+
+    # network_types
+    if isinstance(network_types, str):
+        network_types_temp = [network_types,]
+    elif isinstance(network_types, list) or isinstance(network_types, set) or isinstance(network_types, tuple):
+        network_types_temp = network_types
+    else:
+        sys.exit(f'ERROR: network_types must be a string, list, set, or tuple')
+
+    network_types_ = []
+    for net_type in network_types_temp:
+        if net_type not in network_types_all:
+            print(f'WARNING: network_type \'{net_type}\' does not belong to {network_types_all}, it will be skipped')
+        else:
+            network_types_.append(net_type)
+
+    # link_types
+    if link_types != 'all':
+        if isinstance(link_types, str):
+            link_types_ = (link_types,)
+        elif isinstance(link_types, list) or isinstance(link_types, set) or isinstance(link_types, tuple):
+            link_types_ = link_types
+        else:
+            sys.exit(f'ERROR: argument link_types must be a string, list, set, or tuple')
+    else:
+        link_types_ = link_types
+
+    # POIs
+    if isinstance(POI, bool):
+        POI_ = POI
+    else:
+        print('WARNING: argument POI should be a bool. The default value False has been applied')
+        POI_ = False
+
+    # POI_sampling_ratio
+    if isinstance(POI_sampling_ratio, int) or isinstance(POI_sampling_ratio, float):
+        if POI_sampling_ratio < 0.0 or POI_sampling_ratio > 1.0:
+            print('WARNING: argument POI_sampling_ratio should be a float between 0.0 and 1.0. The default value 1.0 has been applied')
+            POI_sampling_ratio_ = 1.0
+        else:
+            POI_sampling_ratio_ = POI_sampling_ratio
+    else:
+        print('WARNING: argument POI_sampling_ratio should be a float between 0.0 and 1.0. The default value 1.0 has been applied')
+        POI_sampling_ratio_ = 1.0
+
+    # strict_mode
+    if isinstance(strict_mode, bool):
+        strict_mode_ = strict_mode
+    else:
+        print('WARNING: argument strict_mode should be a bool. The default value True has been applied')
+        strict_mode_ = True
+
+    # offset
+    if offset in ('left', 'right', 'no'):
+        offset_ = offset
+    else:
+        print("WARNING: argument offset should be chosen from 'left', 'right', 'no'. The default value 'no' has been applied")
+        offset_ = 'no'
+
+    # min_nodes
+    if isinstance(min_nodes, int):
+        if min_nodes < 1:
+            print('WARNING: argument min_nodes should be a integer greater than or equal to 1. The default value 1 has been applied')
+            min_nodes_ = 1
+        else:
+            min_nodes_ = min_nodes
+    else:
+        print('WARNING: argument min_nodes should be an integer greater than or equal to 1. The default value 1 has been applied')
+        min_nodes_ = 1
+
+    # combine
+    if isinstance(combine, bool):
+        combine_ = combine
+    else:
+        print('WARNING: argument combine should be a bool. The default value False has been applied')
+        combine_ = False
+
+    # bbox
+    if bbox is None:
+        bbox_ = bbox
+    elif isinstance(bbox, tuple) or isinstance(bbox, list):
+        if len(bbox) == 4:
+            for ll in bbox:
+                if not(isinstance(ll, int) or isinstance(ll, float)):
+                    sys.exit('ERROR: argument bbox should be a tuple with four floats: (minlat, minlon, maxlat, maxlon)')
+            bbox_ = bbox
+        else:
+            sys.exit('ERROR: argument bbox should be a tuple with four floats: (minlat, minlon, maxlat, maxlon)')
+    else:
+        sys.exit('ERROR: argument bbox should be a tuple with four floats: (minlat, minlon, maxlat, maxlon)')
+
+    # default_lanes
+    if isinstance(default_lanes, bool) or isinstance(default_lanes, dict):
+        default_lanes_ = default_lanes
+    else:
+        print('WARNING: argument default_lanes should be a bool or a dict. The default value False has been applied')
+        default_lanes_ = False
+
+    # default_speed
+    if isinstance(default_speed, bool) or isinstance(default_speed, dict):
+        default_speed_ = default_speed
+    else:
+        print('WARNING: argument default_speed should be a bool or a dict. The default value False has been applied')
+        default_speed_ = False
+
+    # default_capacity
+    if isinstance(default_capacity, bool) or isinstance(default_capacity, dict):
+        default_capacity_ = default_capacity
+    else:
+        print('WARNING: argument default_capacity should be a bool or a dict. The default value False has been applied')
+        default_capacity_ = False
+
+    # start node/link id
+    if isinstance(start_node_id, int):
+        start_node_id_ = start_node_id
+    else:
+        print('WARNING: argument start_node_id should be a int. The default value 0 has been applied')
+        start_node_id_ = 0
+
+    if isinstance(start_link_id, int):
+        start_link_id_ = start_link_id
+    else:
+        print('WARNING: argument start_link_id should be a int. The default value 0 has been applied')
+        start_link_id_ = 0
+
+    return network_types_, link_types_, POI_, POI_sampling_ratio_, strict_mode_, offset_, min_nodes_, combine_,\
         bbox_, default_lanes_, default_speed_, default_capacity_, start_node_id_, start_link_id_
```

### Comparing `osm2gmns-0.7.5/osm2gmns/osmnet/combine_links.py` & `osm2gmns-0.7.6/osm2gmns/osmnet/combine_links.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,119 +1,119 @@
-from osm2gmns.networkclass.macronet import Link
-from osm2gmns.utils.util_geo import getLineAngle
-import osm2gmns.settings as og_settings
-from shapely import ops
-import math
-
-
-def _checkLinkAttr(ib_link, ob_link):
-    if ib_link.name != ob_link.name: return False
-    if ib_link.link_type != ob_link.link_type: return False
-    if ib_link.is_link != ob_link.is_link: return False
-    if ib_link.free_speed != ob_link.free_speed: return False
-    if set(ib_link.allowed_uses) != set(ob_link.allowed_uses): return False
-
-    if ib_link.lanes != ob_link.lanes: return False
-
-    if ib_link.from_bidirectional_way != ob_link.from_bidirectional_way: return False
-    if ib_link.ctrl_type != ob_link.ctrl_type: return False
-    return True
-
-
-def _checkAngle(ib_link, ob_link):
-    angle = getLineAngle(ib_link.geometry_xy, ob_link.geometry_xy, False)
-
-    if angle > 0.5 * math.pi or angle < -0.5 * math.pi:
-        return False
-    else:
-        return True
-
-
-def _newLinkFromLinks(link_id, up_link, down_link):
-    link = Link(link_id)
-    link.osm_way_id = f'{up_link.osm_way_id};{down_link.osm_way_id}'
-    link.name = up_link.name
-    link.link_class = up_link.link_class
-    link.link_type_name = up_link.link_type_name
-    link.link_type = up_link.link_type
-    link.is_link = up_link.is_link
-    link.free_speed = up_link.free_speed
-    link.capacity = up_link.capacity
-    link.allowed_uses = up_link.allowed_uses
-    link.from_bidirectional_way = up_link.from_bidirectional_way
-    link.lanes = up_link.lanes
-    link.ctrl_type = up_link.ctrl_type
-
-    link.from_node = up_link.from_node
-    link.to_node = down_link.to_node
-    link.from_node.outgoing_link_list.remove(up_link)
-    link.to_node.incoming_link_list.remove(down_link)
-    link.from_node.outgoing_link_list.append(link)
-    link.to_node.incoming_link_list.append(link)
-
-    link.geometry = ops.linemerge([up_link.geometry, down_link.geometry])
-    link.geometry_xy = ops.linemerge([up_link.geometry_xy, down_link.geometry_xy])
-    return link
-
-
-def _combLinks(network):
-
-    removal_node_set = set()
-    removal_link_set = set()
-
-    for node_id, node in network.node_dict.items():
-        if node.ctrl_type and 'signal' in node.ctrl_type:
-            continue
-
-        if len(node.incoming_link_list) != 1 or len(node.outgoing_link_list) != 1:
-            continue
-
-        ib_link, ob_link = node.incoming_link_list[0], node.outgoing_link_list[0]
-        if ib_link.from_node is ob_link.to_node:
-            continue
-
-        if (ib_link.ctrl_type is not None) or (ob_link.ctrl_type is not None):
-            continue
-
-        if not _checkLinkAttr(ib_link, ob_link):
-            continue
-        
-        if not _checkAngle(ib_link, ob_link):
-            continue
-
-        new_link = _newLinkFromLinks(network.max_link_id, ib_link, ob_link)
-        network.link_dict[new_link.link_id] = new_link
-        network.max_link_id += 1
-
-        removal_node_set.add(node.node_id)
-        removal_link_set.add(ib_link.link_id)
-        removal_link_set.add(ob_link.link_id)
-
-    for node_id in removal_node_set: del network.node_dict[node_id]
-    for link_id in removal_link_set: del network.link_dict[link_id]
-
-
-
-def combineShortLinks(network):
-    """
-    Combine links connected by two-degree nodes into a longer link
-
-    Parameters
-    ----------
-    network: Network
-        osm2gmns Network object
-
-    Returns
-    -------
-    None
-    """
-
-    if og_settings.verbose:
-        print('    combining links')
-        print(f'    before: {network.number_of_nodes} nodes, {network.number_of_links} links')
-
-    _combLinks(network)
-
-    if og_settings.verbose:
-        print(f'    after: {network.number_of_nodes} nodes, {network.number_of_links} links')
-
-
+from osm2gmns.networkclass.macronet import Link
+from osm2gmns.utils.util_geo import getLineAngle
+import osm2gmns.settings as og_settings
+from shapely import ops
+import math
+
+
+def _checkLinkAttr(ib_link, ob_link):
+    if ib_link.name != ob_link.name: return False
+    if ib_link.link_type != ob_link.link_type: return False
+    if ib_link.is_link != ob_link.is_link: return False
+    if ib_link.free_speed != ob_link.free_speed: return False
+    if set(ib_link.allowed_uses) != set(ob_link.allowed_uses): return False
+
+    if ib_link.lanes != ob_link.lanes: return False
+
+    if ib_link.from_bidirectional_way != ob_link.from_bidirectional_way: return False
+    if ib_link.ctrl_type != ob_link.ctrl_type: return False
+    return True
+
+
+def _checkAngle(ib_link, ob_link):
+    angle = getLineAngle(ib_link.geometry_xy, ob_link.geometry_xy, False)
+
+    if angle > 0.5 * math.pi or angle < -0.5 * math.pi:
+        return False
+    else:
+        return True
+
+
+def _newLinkFromLinks(link_id, up_link, down_link):
+    link = Link(link_id)
+    link.osm_way_id = f'{up_link.osm_way_id};{down_link.osm_way_id}'
+    link.name = up_link.name
+    link.link_class = up_link.link_class
+    link.link_type_name = up_link.link_type_name
+    link.link_type = up_link.link_type
+    link.is_link = up_link.is_link
+    link.free_speed = up_link.free_speed
+    link.capacity = up_link.capacity
+    link.allowed_uses = up_link.allowed_uses
+    link.from_bidirectional_way = up_link.from_bidirectional_way
+    link.lanes = up_link.lanes
+    link.ctrl_type = up_link.ctrl_type
+
+    link.from_node = up_link.from_node
+    link.to_node = down_link.to_node
+    link.from_node.outgoing_link_list.remove(up_link)
+    link.to_node.incoming_link_list.remove(down_link)
+    link.from_node.outgoing_link_list.append(link)
+    link.to_node.incoming_link_list.append(link)
+
+    link.geometry = ops.linemerge([up_link.geometry, down_link.geometry])
+    link.geometry_xy = ops.linemerge([up_link.geometry_xy, down_link.geometry_xy])
+    return link
+
+
+def _combLinks(network):
+
+    removal_node_set = set()
+    removal_link_set = set()
+
+    for node_id, node in network.node_dict.items():
+        if node.ctrl_type and 'signal' in node.ctrl_type:
+            continue
+
+        if len(node.incoming_link_list) != 1 or len(node.outgoing_link_list) != 1:
+            continue
+
+        ib_link, ob_link = node.incoming_link_list[0], node.outgoing_link_list[0]
+        if ib_link.from_node is ob_link.to_node:
+            continue
+
+        if (ib_link.ctrl_type is not None) or (ob_link.ctrl_type is not None):
+            continue
+
+        if not _checkLinkAttr(ib_link, ob_link):
+            continue
+        
+        if not _checkAngle(ib_link, ob_link):
+            continue
+
+        new_link = _newLinkFromLinks(network.max_link_id, ib_link, ob_link)
+        network.link_dict[new_link.link_id] = new_link
+        network.max_link_id += 1
+
+        removal_node_set.add(node.node_id)
+        removal_link_set.add(ib_link.link_id)
+        removal_link_set.add(ob_link.link_id)
+
+    for node_id in removal_node_set: del network.node_dict[node_id]
+    for link_id in removal_link_set: del network.link_dict[link_id]
+
+
+
+def combineShortLinks(network):
+    """
+    Combine links connected by two-degree nodes into a longer link
+
+    Parameters
+    ----------
+    network: Network
+        osm2gmns Network object
+
+    Returns
+    -------
+    None
+    """
+
+    if og_settings.verbose:
+        print('    combining links')
+        print(f'    before: {network.number_of_nodes} nodes, {network.number_of_links} links')
+
+    _combLinks(network)
+
+    if og_settings.verbose:
+        print(f'    after: {network.number_of_nodes} nodes, {network.number_of_links} links')
+
+
```

### Comparing `osm2gmns-0.7.5/osm2gmns/osmnet/complex_intersection.py` & `osm2gmns-0.7.6/osm2gmns/osmnet/complex_intersection.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,223 +1,223 @@
-from osm2gmns.networkclass.macronet import Node, Network
-import osm2gmns.settings as og_settings
-from shapely import geometry
-import csv
-import os
-import sys
-
-
-def _designateComplexIntersectionsFromIntFile(network, int_file, int_buffer):
-    if not os.path.exists(int_file):
-        sys.exit(f'ERROR: int_file {int_file} does not exist')
-
-    fin = open(int_file, 'r')
-    reader = csv.DictReader(fin)
-
-    for field in ['x_coord', 'y_coord']:
-        if field not in reader.fieldnames:
-            sys.exit(f'ERROR: required field ({field}) does not exist in the int_file')
-
-    max_intersection_id = network.max_intersection_id
-    for int_info in reader:
-        int_center = geometry.Point(float(int_info['x_coord']), float(int_info['y_coord']))
-        int_center_xy = network.GT.geo_from_latlon(int_center)
-        if 'int_buffer' in reader.fieldnames:
-            buffer_ = int_info['int_buffer']
-            buffer_ = float(buffer_) if buffer_ else int_buffer
-        else:
-            buffer_ = int_buffer
-
-        intersection_nodes = [node for _, node in network.node_dict.items() if node.intersection_id is None and int_center_xy.distance(node.geometry_xy) <= buffer_]
-
-        if len(intersection_nodes) < 2:
-            continue
-
-        for node in intersection_nodes:
-            node.intersection_id = max_intersection_id
-        max_intersection_id += 1
-
-    network.max_intersection_id = max_intersection_id
-
-
-
-def _autoidentifyComplexIntersections(network, int_buffer):
-    """
-    Identify nodes that belongs to one intersection in real life. Nodes that
-    belong to one intersection will be assigned with the same intersection_id.
-    Only signalized nodes will be checked.
-
-    The reason why only signalized nodes will be checked is that we use a
-    distance-based rule here, and there are many short links in osm. If all
-    nodes are checked, some short links will be indentified as intersections
-    by mistake.
-
-    Parameters
-    ----------
-    network : Network
-        Network instance
-    int_buffer : float
-        A threshold to check if two connected nodes belong to one intersection.
-        If the length of a link that connects two nodes is shorter than int_buffer,
-        these two nodes come from one intersection.
-
-    Returns
-    -------
-    None
-    """
-
-    group_list = []
-    group_status = []
-    for _,link in network.link_dict.items():
-        if link.length > int_buffer: continue
-        if not (link.from_node.intersection_id is None and link.to_node.intersection_id is None): continue
-        if not (link.from_node.ctrl_type == 'signal' and link.to_node.ctrl_type == 'signal'): continue
-        group_list.append({link.from_node, link.to_node})
-        group_status.append(1)
-
-    number_of_valid_groups = sum(group_status)
-    while True:
-        for group_no1,group1 in enumerate(group_list):
-            if group_status[group_no1] == 0: continue
-            for group_no2,group2 in enumerate(group_list):
-                if group_status[group_no2] == 0: continue
-                if group_no1 == group_no2: continue
-                if len(group1.intersection(group2)) > 0:
-                    group1.update(group2)
-                    group_status[group_no2] = 0
-
-        new_number_of_valid_groups = sum(group_status)
-        if number_of_valid_groups == new_number_of_valid_groups:
-            break
-        else:
-            number_of_valid_groups = new_number_of_valid_groups
-
-    max_intersection_id = network.max_intersection_id
-    for group_no, group in enumerate(group_list):
-        if group_status[group_no] == 0: continue
-        for node in group: node.intersection_id = max_intersection_id
-        max_intersection_id += 1
-    network.max_intersection_id = max_intersection_id
-
-
-def consolidateComplexIntersections(network, auto_identify=False, intersection_file=None, int_buffer=og_settings.default_int_buffer):
-    """
-    Consolidate each complex intersection that are originally represented by multiple nodes in osm into one node. Nodes
-    with the same intersection_id will be consolidated into one node. intersection_id of nodes can be obtained in three ways.
-
-    (1) set the argument auto_identify as True, then osm2gmns will automatically identify complex intersections and assign
-    intersection_id for corresponding nodes.
-
-    (2) provide an intersection file that specifies the central position (required) and buffer (optional) of each complex intersection.
-
-    (3) user can assign intersection_id to nodes manually in network csv files (node.csv), and load the network using function loadNetFromCSV provided by osm2gmns.
-
-    The priority of the three approaches is (3) > (2) > (1).
-    Rules used in the approach (1) to identify if two nodes belong to a complex intersection: (a) ctrl_type of the two nodes must be signal;
-    (b) there is a link connecting these two nodes, and the length of the link is shorter than or equal to the argument int_buffer.
-
-    Parameters
-    ----------
-    network: Network
-        osm2gmns Network object
-    auto_identify: bool
-        if automatically identify complex intersections using built-in methods in osm2gmns. nodes that belong to a complex
-        intersection will be assigned with the same intersection_id
-    intersection_file: str
-        path of an intersction csv file that specifies complex intersections. required fields: central position of intersections
-        (in the form of x_coord and y_coord); optional field: int_buffer (if not specified, the global int_buffer will be used,
-        i.e., the forth arugment). For each record in the intersection_file, osm2gmns consolidates all nodes with a distance to the
-        central position shorter than buffer.
-    int_buffer: float
-        the threshold used to check if two nodes belong to one complex intersection. the unit is meter
-
-    Returns
-    -------
-    None
-
-    """
-
-    if intersection_file is not None:
-        _designateComplexIntersectionsFromIntFile(network, intersection_file, int_buffer)
-
-    if auto_identify:
-        _autoidentifyComplexIntersections(network, int_buffer)
-
-    if og_settings.verbose:
-        print('Consolidating Complex Intersections')
-
-    node_group_dict = {}
-    node_group_ctrl_type_dict = {}
-    for _, node in network.node_dict.items():
-        if node.intersection_id is not None:
-            if node.intersection_id in node_group_dict.keys():
-                node_group_dict[node.intersection_id].append(node)
-            else:
-                node_group_dict[node.intersection_id] = [node]
-                node_group_ctrl_type_dict[node.intersection_id] = False
-            if node.ctrl_type == 'signal':
-                node_group_ctrl_type_dict[node.intersection_id] = True
-
-    removal_node_set = set()
-    removal_link_set = set()
-    number_of_intersections_consolidated = 0
-
-    for intersection_id, node_group in node_group_dict.items():
-        if len(node_group) < 2:
-            continue
-
-        new_node = Node(network.max_node_id)
-        new_node.intersection_id = intersection_id
-        if node_group_ctrl_type_dict[intersection_id]:
-            new_node.ctrl_type = 'signal'
-        osm_node_id_list = []
-        x_coord_sum, y_coord_sum = 0.0, 0.0
-        x_coord_xy_sum, y_coord_xy_sum = 0.0, 0.0
-
-        for node in node_group:
-            removal_node_set.add(node)
-            osm_node_id_list.append(node.osm_node_id if node.osm_node_id is not None else 'None')
-            x_coord_sum += node.geometry.x
-            y_coord_sum += node.geometry.y
-            x_coord_xy_sum += node.geometry_xy.x
-            y_coord_xy_sum += node.geometry_xy.y
-
-            for link in node.incoming_link_list:
-                if link.from_node in node_group:
-                    removal_link_set.add(link)
-                else:
-                    link.to_node = new_node
-                    new_node.incoming_link_list.append(link)
-            for link in node.outgoing_link_list:
-                if link.to_node in node_group:
-                    removal_link_set.add(link)
-                else:
-                    link.from_node = new_node
-                    new_node.outgoing_link_list.append(link)
-
-            new_node.osm_highway = node.osm_highway
-
-        new_node.osm_node_id = '_'.join(osm_node_id_list)
-        x_coord_ave = round(x_coord_sum / len(node_group), og_settings.lonlat_coord_precision)
-        y_coord_ave = round(y_coord_sum / len(node_group), og_settings.lonlat_coord_precision)
-        new_node.geometry = geometry.Point(x_coord_ave, y_coord_ave)
-        x_coord_xy_ave = round(x_coord_xy_sum / len(node_group), og_settings.local_coord_precision)
-        y_coord_xy_ave = round(y_coord_xy_sum / len(node_group), og_settings.local_coord_precision)
-        new_node.geometry_xy = geometry.Point(x_coord_xy_ave, y_coord_xy_ave)
-
-        # Keep the geometry of the links up to date by adding a small edge to join to the newly created node
-        for link in new_node.incoming_link_list:
-            new_coordinates = list(link.geometry.coords) + list(link.to_node.geometry.coords)
-            link.geometry = geometry.LineString(new_coordinates)
-        for link in new_node.outgoing_link_list:
-            new_coordinates = list(link.from_node.geometry.coords) + list(link.geometry.coords)
-            link.geometry = geometry.LineString(new_coordinates)
-
-        network.node_dict[new_node.node_id] = new_node
-        network.max_node_id += 1
-        number_of_intersections_consolidated += 1
-
-    for node in removal_node_set: del network.node_dict[node.node_id]
-    for link in removal_link_set: del network.link_dict[link.link_id]
-
-    if og_settings.verbose:
+from osm2gmns.networkclass.macronet import Node, Network
+import osm2gmns.settings as og_settings
+from shapely import geometry
+import csv
+import os
+import sys
+
+
+def _designateComplexIntersectionsFromIntFile(network, int_file, int_buffer):
+    if not os.path.exists(int_file):
+        sys.exit(f'ERROR: int_file {int_file} does not exist')
+
+    fin = open(int_file, 'r')
+    reader = csv.DictReader(fin)
+
+    for field in ['x_coord', 'y_coord']:
+        if field not in reader.fieldnames:
+            sys.exit(f'ERROR: required field ({field}) does not exist in the int_file')
+
+    max_intersection_id = network.max_intersection_id
+    for int_info in reader:
+        int_center = geometry.Point(float(int_info['x_coord']), float(int_info['y_coord']))
+        int_center_xy = network.GT.geo_from_latlon(int_center)
+        if 'int_buffer' in reader.fieldnames:
+            buffer_ = int_info['int_buffer']
+            buffer_ = float(buffer_) if buffer_ else int_buffer
+        else:
+            buffer_ = int_buffer
+
+        intersection_nodes = [node for _, node in network.node_dict.items() if node.intersection_id is None and int_center_xy.distance(node.geometry_xy) <= buffer_]
+
+        if len(intersection_nodes) < 2:
+            continue
+
+        for node in intersection_nodes:
+            node.intersection_id = max_intersection_id
+        max_intersection_id += 1
+
+    network.max_intersection_id = max_intersection_id
+
+
+
+def _autoidentifyComplexIntersections(network, int_buffer):
+    """
+    Identify nodes that belongs to one intersection in real life. Nodes that
+    belong to one intersection will be assigned with the same intersection_id.
+    Only signalized nodes will be checked.
+
+    The reason why only signalized nodes will be checked is that we use a
+    distance-based rule here, and there are many short links in osm. If all
+    nodes are checked, some short links will be indentified as intersections
+    by mistake.
+
+    Parameters
+    ----------
+    network : Network
+        Network instance
+    int_buffer : float
+        A threshold to check if two connected nodes belong to one intersection.
+        If the length of a link that connects two nodes is shorter than int_buffer,
+        these two nodes come from one intersection.
+
+    Returns
+    -------
+    None
+    """
+
+    group_list = []
+    group_status = []
+    for _,link in network.link_dict.items():
+        if link.length > int_buffer: continue
+        if not (link.from_node.intersection_id is None and link.to_node.intersection_id is None): continue
+        if not (link.from_node.ctrl_type == 'signal' and link.to_node.ctrl_type == 'signal'): continue
+        group_list.append({link.from_node, link.to_node})
+        group_status.append(1)
+
+    number_of_valid_groups = sum(group_status)
+    while True:
+        for group_no1,group1 in enumerate(group_list):
+            if group_status[group_no1] == 0: continue
+            for group_no2,group2 in enumerate(group_list):
+                if group_status[group_no2] == 0: continue
+                if group_no1 == group_no2: continue
+                if len(group1.intersection(group2)) > 0:
+                    group1.update(group2)
+                    group_status[group_no2] = 0
+
+        new_number_of_valid_groups = sum(group_status)
+        if number_of_valid_groups == new_number_of_valid_groups:
+            break
+        else:
+            number_of_valid_groups = new_number_of_valid_groups
+
+    max_intersection_id = network.max_intersection_id
+    for group_no, group in enumerate(group_list):
+        if group_status[group_no] == 0: continue
+        for node in group: node.intersection_id = max_intersection_id
+        max_intersection_id += 1
+    network.max_intersection_id = max_intersection_id
+
+
+def consolidateComplexIntersections(network, auto_identify=False, intersection_file=None, int_buffer=og_settings.default_int_buffer):
+    """
+    Consolidate each complex intersection that are originally represented by multiple nodes in osm into one node. Nodes
+    with the same intersection_id will be consolidated into one node. intersection_id of nodes can be obtained in three ways.
+
+    (1) set the argument auto_identify as True, then osm2gmns will automatically identify complex intersections and assign
+    intersection_id for corresponding nodes.
+
+    (2) provide an intersection file that specifies the central position (required) and buffer (optional) of each complex intersection.
+
+    (3) user can assign intersection_id to nodes manually in network csv files (node.csv), and load the network using function loadNetFromCSV provided by osm2gmns.
+
+    The priority of the three approaches is (3) > (2) > (1).
+    Rules used in the approach (1) to identify if two nodes belong to a complex intersection: (a) ctrl_type of the two nodes must be signal;
+    (b) there is a link connecting these two nodes, and the length of the link is shorter than or equal to the argument int_buffer.
+
+    Parameters
+    ----------
+    network: Network
+        osm2gmns Network object
+    auto_identify: bool
+        if automatically identify complex intersections using built-in methods in osm2gmns. nodes that belong to a complex
+        intersection will be assigned with the same intersection_id
+    intersection_file: str
+        path of an intersction csv file that specifies complex intersections. required fields: central position of intersections
+        (in the form of x_coord and y_coord); optional field: int_buffer (if not specified, the global int_buffer will be used,
+        i.e., the forth arugment). For each record in the intersection_file, osm2gmns consolidates all nodes with a distance to the
+        central position shorter than buffer.
+    int_buffer: float
+        the threshold used to check if two nodes belong to one complex intersection. the unit is meter
+
+    Returns
+    -------
+    None
+
+    """
+
+    if intersection_file is not None:
+        _designateComplexIntersectionsFromIntFile(network, intersection_file, int_buffer)
+
+    if auto_identify:
+        _autoidentifyComplexIntersections(network, int_buffer)
+
+    if og_settings.verbose:
+        print('Consolidating Complex Intersections')
+
+    node_group_dict = {}
+    node_group_ctrl_type_dict = {}
+    for _, node in network.node_dict.items():
+        if node.intersection_id is not None:
+            if node.intersection_id in node_group_dict.keys():
+                node_group_dict[node.intersection_id].append(node)
+            else:
+                node_group_dict[node.intersection_id] = [node]
+                node_group_ctrl_type_dict[node.intersection_id] = False
+            if node.ctrl_type == 'signal':
+                node_group_ctrl_type_dict[node.intersection_id] = True
+
+    removal_node_set = set()
+    removal_link_set = set()
+    number_of_intersections_consolidated = 0
+
+    for intersection_id, node_group in node_group_dict.items():
+        if len(node_group) < 2:
+            continue
+
+        new_node = Node(network.max_node_id)
+        new_node.intersection_id = intersection_id
+        if node_group_ctrl_type_dict[intersection_id]:
+            new_node.ctrl_type = 'signal'
+        osm_node_id_list = []
+        x_coord_sum, y_coord_sum = 0.0, 0.0
+        x_coord_xy_sum, y_coord_xy_sum = 0.0, 0.0
+
+        for node in node_group:
+            removal_node_set.add(node)
+            osm_node_id_list.append(node.osm_node_id if node.osm_node_id is not None else 'None')
+            x_coord_sum += node.geometry.x
+            y_coord_sum += node.geometry.y
+            x_coord_xy_sum += node.geometry_xy.x
+            y_coord_xy_sum += node.geometry_xy.y
+
+            for link in node.incoming_link_list:
+                if link.from_node in node_group:
+                    removal_link_set.add(link)
+                else:
+                    link.to_node = new_node
+                    new_node.incoming_link_list.append(link)
+            for link in node.outgoing_link_list:
+                if link.to_node in node_group:
+                    removal_link_set.add(link)
+                else:
+                    link.from_node = new_node
+                    new_node.outgoing_link_list.append(link)
+
+            new_node.osm_highway = node.osm_highway
+
+        new_node.osm_node_id = '_'.join(osm_node_id_list)
+        x_coord_ave = round(x_coord_sum / len(node_group), og_settings.lonlat_coord_precision)
+        y_coord_ave = round(y_coord_sum / len(node_group), og_settings.lonlat_coord_precision)
+        new_node.geometry = geometry.Point(x_coord_ave, y_coord_ave)
+        x_coord_xy_ave = round(x_coord_xy_sum / len(node_group), og_settings.local_coord_precision)
+        y_coord_xy_ave = round(y_coord_xy_sum / len(node_group), og_settings.local_coord_precision)
+        new_node.geometry_xy = geometry.Point(x_coord_xy_ave, y_coord_xy_ave)
+
+        # Keep the geometry of the links up to date by adding a small edge to join to the newly created node
+        for link in new_node.incoming_link_list:
+            new_coordinates = list(link.geometry.coords) + list(link.to_node.geometry.coords)
+            link.geometry = geometry.LineString(new_coordinates)
+        for link in new_node.outgoing_link_list:
+            new_coordinates = list(link.from_node.geometry.coords) + list(link.geometry.coords)
+            link.geometry = geometry.LineString(new_coordinates)
+
+        network.node_dict[new_node.node_id] = new_node
+        network.max_node_id += 1
+        number_of_intersections_consolidated += 1
+
+    for node in removal_node_set: del network.node_dict[node.node_id]
+    for link in removal_link_set: del network.link_dict[link.link_id]
+
+    if og_settings.verbose:
         print(f'    {number_of_intersections_consolidated} intersections have been consolidated')
```

### Comparing `osm2gmns-0.7.5/osm2gmns/osmnet/pois.py` & `osm2gmns-0.7.6/osm2gmns/osmnet/pois.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,273 +1,273 @@
-from osm2gmns.networkclass.macronet import Node, Link, POI
-from osm2gmns.osmnet.osmclasses import Way, Relation
-from osm2gmns.utils.util import getLogger
-from osm2gmns.utils.util_geo import getLineFromNodes, getPolygonFromNodes
-import osm2gmns.settings as og_settings
-from shapely import geometry
-import numpy as np
-import random
-
-
-
-def _parseRelations(relations, network):
-    POI_relation_list = []
-    for osm_relation in relations:
-        relation = Relation()
-        relation.osm_relation_id = str(osm_relation.id)
-
-        for member_id, member_type, member_role in osm_relation.members:
-            member_id_str = str(member_id)
-            member_type_lc = member_type.lower()
-            if member_type_lc == 'node':
-                try:
-                    relation.member_list.append(network.osm_node_dict[member_id_str])
-                except KeyError:
-                    logger = getLogger()
-                    if logger: logger.info(f'ref node {member_id} in relation {relation.osm_relation_id} is not defined')
-            elif member_type_lc == 'way':
-                try:
-                    relation.member_list.append(network.osm_way_dict[member_id_str])
-                except KeyError:
-                    logger = getLogger()
-                    if logger: logger.info(f'ref way {member_id} in relation {relation.osm_relation_id} is not defined')
-            elif member_type_lc == 'relation':
-                pass
-            else:
-                logger = getLogger()
-                if logger: logger.warning(f'new member type at relation {relation.osm_relation_id}, {member_type}')
-
-            relation.member_role_list.append(member_role)
-
-        tags = osm_relation.tags
-        if 'building' in tags.keys():
-            relation.building = tags['building']
-        if 'amenity' in tags.keys():
-            relation.amenity = tags['amenity']
-        if 'name' in tags.keys():
-            relation.name = tags['name']
-
-        if relation.building or relation.amenity:
-            POI_relation_list.append(relation)
-    return POI_relation_list
-
-
-def _POIFromWay(POI_way_list, net_bound):
-    POI_list1 = []
-    for way in POI_way_list:
-        poly, poly_xy = getPolygonFromNodes(way.ref_node_list)
-        if poly is None: continue
-        if poly.disjoint(net_bound): continue
-
-        poi = POI()
-        poi.osm_way_id = way.osm_way_id
-        poi.name = way.name
-        poi.building = way.building
-        poi.amenity = way.amenity
-        poi.leisure = way.leisure
-        poi.way = way.way_poi
-
-        poi.geometry, poi.geometry_xy = poly, poly_xy
-        lon, lat = poi.geometry.centroid.x, poi.geometry.centroid.y
-        poi.centroid = geometry.Point((round(lon,og_settings.lonlat_coord_precision),round(lat,og_settings.lonlat_coord_precision)))
-        x, y = poi.geometry_xy.centroid.x, poi.geometry_xy.centroid.y
-        poi.centroid_xy = geometry.Point((round(x,og_settings.local_coord_precision),round(y,og_settings.local_coord_precision)))
-        POI_list1.append(poi)
-    return POI_list1
-
-
-def _POIFromRelation(POI_relation_list, net_bound):
-    POI_list2 = []
-    for relation in POI_relation_list:
-        poi = POI()
-        poi.osm_relation_id = relation.osm_relation_id
-        poi.name = relation.name
-        poi.building = relation.building
-        poi.amenity = relation.amenity
-        poi.leisure = relation.leisure
-        polygon_list = []
-        polygon_list_xy = []
-        number_of_members = len(relation.member_list)
-        m_ref_node_list = []
-        for m in range(number_of_members):
-            member = relation.member_list[m]
-            role = relation.member_role_list[m]
-            if isinstance(member, Way):
-                if role != 'outer': continue
-                if m_ref_node_list:
-                    combined_ref_node_list = []
-                    if m_ref_node_list[-1] is member.ref_node_list[0]:
-                        combined_ref_node_list = m_ref_node_list + member.ref_node_list[1:]
-                    elif m_ref_node_list[-1] is member.ref_node_list[-1]:
-                        combined_ref_node_list = m_ref_node_list + list(reversed(member.ref_node_list[:-1]))
-                    elif m_ref_node_list[0] is member.ref_node_list[0]:
-                        combined_ref_node_list = list(reversed(m_ref_node_list)) + member.ref_node_list[1:]
-                    elif m_ref_node_list[0] is member.ref_node_list[-1]:
-                        combined_ref_node_list = list(reversed(m_ref_node_list)) + list(reversed(member.ref_node_list[:-1]))
-
-                    if combined_ref_node_list:
-                        if combined_ref_node_list[0] is combined_ref_node_list[-1]:
-                            poly, poly_xy = getPolygonFromNodes(combined_ref_node_list)
-                            if poly is not None:
-                                polygon_list.append(poly)
-                                polygon_list_xy.append(poly_xy)
-                            m_ref_node_list = []
-                        else:
-                            m_ref_node_list = combined_ref_node_list
-                    else:
-                        poly, poly_xy = getPolygonFromNodes(m_ref_node_list)
-                        if poly is not None:
-                            polygon_list.append(poly)
-                            polygon_list_xy.append(poly_xy)
-                        if member.ref_node_list[0] is member.ref_node_list[-1]:
-                            poly, poly_xy = getPolygonFromNodes(m_ref_node_list)
-                            if poly is not None:
-                                polygon_list.append(poly)
-                                polygon_list_xy.append(poly_xy)
-                            m_ref_node_list = []
-                        else:
-                            m_ref_node_list = member.ref_node_list
-                else:
-                    if member.ref_node_list[0] is member.ref_node_list[-1]:
-                        poly, poly_xy = getPolygonFromNodes(member.ref_node_list)
-                        if poly is not None:
-                            polygon_list.append(poly)
-                            polygon_list_xy.append(poly_xy)
-                    else:
-                        m_ref_node_list = member.ref_node_list
-            else:
-                logger = getLogger()
-                if logger: logger.warning(f'node member detected at building {relation.osm_relation_id}')
-
-        if m_ref_node_list:
-            poly, poly_xy = getPolygonFromNodes(m_ref_node_list)
-            if poly is not None:
-                polygon_list.append(poly)
-                polygon_list_xy.append(poly_xy)
-
-        if len(polygon_list) == 0:
-            continue
-        else:
-            if len(polygon_list) == 1:
-                poi.geometry = polygon_list[0]
-                if poi.geometry.disjoint(net_bound): continue
-                poi.geometry_xy = polygon_list_xy[0]
-            else:
-                disjoint = True
-                for poly in polygon_list:
-                    if not poly.disjoint(net_bound):
-                        disjoint = False
-                        break
-                if disjoint: continue
-                poi.geometry = geometry.MultiPolygon(polygon_list)
-                poi.geometry_xy = geometry.MultiPolygon(polygon_list_xy)
-
-            lon, lat = poi.geometry.centroid.x, poi.geometry.centroid.y
-            poi.centroid = geometry.Point((round(lon, og_settings.lonlat_coord_precision), round(lat, og_settings.lonlat_coord_precision)))
-            x, y = poi.geometry_xy.centroid.x, poi.geometry_xy.centroid.y
-            poi.centroid_xy = geometry.Point((round(x, og_settings.local_coord_precision), round(y, og_settings.local_coord_precision)))
-
-            POI_list2.append(poi)
-
-    return POI_list2
-
-
-def generatePOIs(POI_way_list, osm_relation_list, network, POI_percentage):
-    if og_settings.verbose:
-        print('    generating POIs')
-
-    POI_list1 = _POIFromWay(POI_way_list, network.bounds)
-    POI_list2 = _POIFromRelation(osm_relation_list, network.bounds)
-
-    POI_list_ = POI_list1 + POI_list2
-    if POI_percentage == 1:
-        POI_list = POI_list_
-    else:
-        POI_list = random.sample(POI_list_,int(len(POI_list_)*POI_percentage))
-
-    max_poi_id = network.max_poi_id
-    for poi in POI_list:
-        poi.poi_id = max_poi_id
-        max_poi_id += 1
-    network.max_poi_id = max_poi_id
-    network.POI_list = POI_list
-
-
-def _findNearestNode(network):
-    coord_list = []
-    idx_to_node_dict = {}
-    for idx, (node_id, node) in enumerate(network.node_dict.items()):
-        coord_list.append((node.geometry_xy.x, node.geometry_xy.y))
-        idx_to_node_dict[idx] = node
-    coord_array = np.array(coord_list)
-
-    for poi in network.POI_list:
-        coord = np.array((poi.centroid_xy.x,poi.centroid_xy.y))
-        coord_diff = coord_array - coord
-        coord_diff_square = np.power(coord_diff,2)
-        coord_diff_sum_square = coord_diff_square.sum(axis=1)
-        distance = np.sqrt(coord_diff_sum_square)
-        idx = int(np.argmin(distance))
-        poi.nearest_node = idx_to_node_dict[idx]
-
-
-def _createConnector(from_node, to_node, link_id):
-    link = Link(link_id)
-    link.link_type_name = 'connector'
-    link.link_type = og_settings.link_type_no_dict[link.link_type_name]
-    link.free_speed = og_settings.default_speed_dict[link.link_type_name]
-    link.allowed_uses = ['auto','bike','walk']
-    link.from_bidirectional_way = True
-    link.lanes = og_settings.default_lanes_dict[link.link_type_name]
-    link.from_node = from_node
-    link.to_node = to_node
-    link.from_node.outgoing_link_list.append(link)
-    link.to_node.incoming_link_list.append(link)
-    link.geometry, link.geometry_xy = getLineFromNodes([link.from_node, link.to_node])
-    return link
-
-
-def _addPOIs(network):
-    for poi in network.POI_list:
-        node = Node(network.max_node_id)
-        node.geometry = poi.geometry.centroid
-        node.geometry_xy = poi.geometry_xy.centroid
-        node.is_crossing = True
-        node.poi_id = poi.poi_id
-        network.node_dict[node.node_id] = node
-        network.max_node_id += 1
-
-        link1 = _createConnector(node,poi.nearest_node,network.max_link_id)
-        network.link_dict[link1.link_id] = link1
-        network.max_link_id += 1
-        link2 = _createConnector(poi.nearest_node, node, network.max_link_id)
-        network.link_dict[link2.link_id] = link2
-        network.max_link_id += 1
-
-
-def connectPOIWithNet(network):
-    """
-    Connect POIs with the traffic network. Specifically, for each POI, osm2gmns will build a bi-directional connector to connect the POI
-    with its nearest node in the traffic network
-
-    Parameters
-    ----------
-    network: Network
-        an osm2gmns Network object
-
-    Returns
-    -------
-    None
-    """
-    if len(network.POI_list) == 0:
-        print('No POIs found in the network. Please set POIs=True when creating network from osm file')
-        return
-
-    _findNearestNode(network)
-    _addPOIs(network)
-
-
-
-
-
-
-
+from osm2gmns.networkclass.macronet import Node, Link, POI
+from osm2gmns.osmnet.osmclasses import Way, Relation
+from osm2gmns.utils.util import getLogger
+from osm2gmns.utils.util_geo import getLineFromNodes, getPolygonFromNodes
+import osm2gmns.settings as og_settings
+from shapely import geometry
+import numpy as np
+import random
+
+
+
+def _parseRelations(relations, network):
+    POI_relation_list = []
+    for osm_relation in relations:
+        relation = Relation()
+        relation.osm_relation_id = str(osm_relation.id)
+
+        for member_id, member_type, member_role in osm_relation.members:
+            member_id_str = str(member_id)
+            member_type_lc = member_type.lower()
+            if member_type_lc == 'node':
+                try:
+                    relation.member_list.append(network.osm_node_dict[member_id_str])
+                except KeyError:
+                    logger = getLogger()
+                    if logger: logger.info(f'ref node {member_id} in relation {relation.osm_relation_id} is not defined')
+            elif member_type_lc == 'way':
+                try:
+                    relation.member_list.append(network.osm_way_dict[member_id_str])
+                except KeyError:
+                    logger = getLogger()
+                    if logger: logger.info(f'ref way {member_id} in relation {relation.osm_relation_id} is not defined')
+            elif member_type_lc == 'relation':
+                pass
+            else:
+                logger = getLogger()
+                if logger: logger.warning(f'new member type at relation {relation.osm_relation_id}, {member_type}')
+
+            relation.member_role_list.append(member_role)
+
+        tags = osm_relation.tags
+        if 'building' in tags.keys():
+            relation.building = tags['building']
+        if 'amenity' in tags.keys():
+            relation.amenity = tags['amenity']
+        if 'name' in tags.keys():
+            relation.name = tags['name']
+
+        if relation.building or relation.amenity:
+            POI_relation_list.append(relation)
+    return POI_relation_list
+
+
+def _POIFromWay(POI_way_list, net_bound):
+    POI_list1 = []
+    for way in POI_way_list:
+        poly, poly_xy = getPolygonFromNodes(way.ref_node_list)
+        if poly is None: continue
+        if poly.disjoint(net_bound): continue
+
+        poi = POI()
+        poi.osm_way_id = way.osm_way_id
+        poi.name = way.name
+        poi.building = way.building
+        poi.amenity = way.amenity
+        poi.leisure = way.leisure
+        poi.way = way.way_poi
+
+        poi.geometry, poi.geometry_xy = poly, poly_xy
+        lon, lat = poi.geometry.centroid.x, poi.geometry.centroid.y
+        poi.centroid = geometry.Point((round(lon,og_settings.lonlat_coord_precision),round(lat,og_settings.lonlat_coord_precision)))
+        x, y = poi.geometry_xy.centroid.x, poi.geometry_xy.centroid.y
+        poi.centroid_xy = geometry.Point((round(x,og_settings.local_coord_precision),round(y,og_settings.local_coord_precision)))
+        POI_list1.append(poi)
+    return POI_list1
+
+
+def _POIFromRelation(POI_relation_list, net_bound):
+    POI_list2 = []
+    for relation in POI_relation_list:
+        poi = POI()
+        poi.osm_relation_id = relation.osm_relation_id
+        poi.name = relation.name
+        poi.building = relation.building
+        poi.amenity = relation.amenity
+        poi.leisure = relation.leisure
+        polygon_list = []
+        polygon_list_xy = []
+        number_of_members = len(relation.member_list)
+        m_ref_node_list = []
+        for m in range(number_of_members):
+            member = relation.member_list[m]
+            role = relation.member_role_list[m]
+            if isinstance(member, Way):
+                if role != 'outer': continue
+                if m_ref_node_list:
+                    combined_ref_node_list = []
+                    if m_ref_node_list[-1] is member.ref_node_list[0]:
+                        combined_ref_node_list = m_ref_node_list + member.ref_node_list[1:]
+                    elif m_ref_node_list[-1] is member.ref_node_list[-1]:
+                        combined_ref_node_list = m_ref_node_list + list(reversed(member.ref_node_list[:-1]))
+                    elif m_ref_node_list[0] is member.ref_node_list[0]:
+                        combined_ref_node_list = list(reversed(m_ref_node_list)) + member.ref_node_list[1:]
+                    elif m_ref_node_list[0] is member.ref_node_list[-1]:
+                        combined_ref_node_list = list(reversed(m_ref_node_list)) + list(reversed(member.ref_node_list[:-1]))
+
+                    if combined_ref_node_list:
+                        if combined_ref_node_list[0] is combined_ref_node_list[-1]:
+                            poly, poly_xy = getPolygonFromNodes(combined_ref_node_list)
+                            if poly is not None:
+                                polygon_list.append(poly)
+                                polygon_list_xy.append(poly_xy)
+                            m_ref_node_list = []
+                        else:
+                            m_ref_node_list = combined_ref_node_list
+                    else:
+                        poly, poly_xy = getPolygonFromNodes(m_ref_node_list)
+                        if poly is not None:
+                            polygon_list.append(poly)
+                            polygon_list_xy.append(poly_xy)
+                        if member.ref_node_list[0] is member.ref_node_list[-1]:
+                            poly, poly_xy = getPolygonFromNodes(m_ref_node_list)
+                            if poly is not None:
+                                polygon_list.append(poly)
+                                polygon_list_xy.append(poly_xy)
+                            m_ref_node_list = []
+                        else:
+                            m_ref_node_list = member.ref_node_list
+                else:
+                    if member.ref_node_list[0] is member.ref_node_list[-1]:
+                        poly, poly_xy = getPolygonFromNodes(member.ref_node_list)
+                        if poly is not None:
+                            polygon_list.append(poly)
+                            polygon_list_xy.append(poly_xy)
+                    else:
+                        m_ref_node_list = member.ref_node_list
+            else:
+                logger = getLogger()
+                if logger: logger.warning(f'node member detected at building {relation.osm_relation_id}')
+
+        if m_ref_node_list:
+            poly, poly_xy = getPolygonFromNodes(m_ref_node_list)
+            if poly is not None:
+                polygon_list.append(poly)
+                polygon_list_xy.append(poly_xy)
+
+        if len(polygon_list) == 0:
+            continue
+        else:
+            if len(polygon_list) == 1:
+                poi.geometry = polygon_list[0]
+                if poi.geometry.disjoint(net_bound): continue
+                poi.geometry_xy = polygon_list_xy[0]
+            else:
+                disjoint = True
+                for poly in polygon_list:
+                    if not poly.disjoint(net_bound):
+                        disjoint = False
+                        break
+                if disjoint: continue
+                poi.geometry = geometry.MultiPolygon(polygon_list)
+                poi.geometry_xy = geometry.MultiPolygon(polygon_list_xy)
+
+            lon, lat = poi.geometry.centroid.x, poi.geometry.centroid.y
+            poi.centroid = geometry.Point((round(lon, og_settings.lonlat_coord_precision), round(lat, og_settings.lonlat_coord_precision)))
+            x, y = poi.geometry_xy.centroid.x, poi.geometry_xy.centroid.y
+            poi.centroid_xy = geometry.Point((round(x, og_settings.local_coord_precision), round(y, og_settings.local_coord_precision)))
+
+            POI_list2.append(poi)
+
+    return POI_list2
+
+
+def generatePOIs(POI_way_list, osm_relation_list, network, POI_percentage):
+    if og_settings.verbose:
+        print('    generating POIs')
+
+    POI_list1 = _POIFromWay(POI_way_list, network.bounds)
+    POI_list2 = _POIFromRelation(osm_relation_list, network.bounds)
+
+    POI_list_ = POI_list1 + POI_list2
+    if POI_percentage == 1:
+        POI_list = POI_list_
+    else:
+        POI_list = random.sample(POI_list_,int(len(POI_list_)*POI_percentage))
+
+    max_poi_id = network.max_poi_id
+    for poi in POI_list:
+        poi.poi_id = max_poi_id
+        max_poi_id += 1
+    network.max_poi_id = max_poi_id
+    network.POI_list = POI_list
+
+
+def _findNearestNode(network):
+    coord_list = []
+    idx_to_node_dict = {}
+    for idx, (node_id, node) in enumerate(network.node_dict.items()):
+        coord_list.append((node.geometry_xy.x, node.geometry_xy.y))
+        idx_to_node_dict[idx] = node
+    coord_array = np.array(coord_list)
+
+    for poi in network.POI_list:
+        coord = np.array((poi.centroid_xy.x,poi.centroid_xy.y))
+        coord_diff = coord_array - coord
+        coord_diff_square = np.power(coord_diff,2)
+        coord_diff_sum_square = coord_diff_square.sum(axis=1)
+        distance = np.sqrt(coord_diff_sum_square)
+        idx = int(np.argmin(distance))
+        poi.nearest_node = idx_to_node_dict[idx]
+
+
+def _createConnector(from_node, to_node, link_id):
+    link = Link(link_id)
+    link.link_type_name = 'connector'
+    link.link_type = og_settings.link_type_no_dict[link.link_type_name]
+    link.free_speed = og_settings.default_speed_dict[link.link_type_name]
+    link.allowed_uses = ['auto','bike','walk']
+    link.from_bidirectional_way = True
+    link.lanes = og_settings.default_lanes_dict[link.link_type_name]
+    link.from_node = from_node
+    link.to_node = to_node
+    link.from_node.outgoing_link_list.append(link)
+    link.to_node.incoming_link_list.append(link)
+    link.geometry, link.geometry_xy = getLineFromNodes([link.from_node, link.to_node])
+    return link
+
+
+def _addPOIs(network):
+    for poi in network.POI_list:
+        node = Node(network.max_node_id)
+        node.geometry = poi.geometry.centroid
+        node.geometry_xy = poi.geometry_xy.centroid
+        node.is_crossing = True
+        node.poi_id = poi.poi_id
+        network.node_dict[node.node_id] = node
+        network.max_node_id += 1
+
+        link1 = _createConnector(node,poi.nearest_node,network.max_link_id)
+        network.link_dict[link1.link_id] = link1
+        network.max_link_id += 1
+        link2 = _createConnector(poi.nearest_node, node, network.max_link_id)
+        network.link_dict[link2.link_id] = link2
+        network.max_link_id += 1
+
+
+def connectPOIWithNet(network):
+    """
+    Connect POIs with the traffic network. Specifically, for each POI, osm2gmns will build a bi-directional connector to connect the POI
+    with its nearest node in the traffic network
+
+    Parameters
+    ----------
+    network: Network
+        an osm2gmns Network object
+
+    Returns
+    -------
+    None
+    """
+    if len(network.POI_list) == 0:
+        print('No POIs found in the network. Please set POIs=True when creating network from osm file')
+        return
+
+    _findNearestNode(network)
+    _addPOIs(network)
+
+
+
+
+
+
+
```

### Comparing `osm2gmns-0.7.5/osm2gmns/osmnet/visualization.py` & `osm2gmns-0.7.6/osm2gmns/osmnet/visualization.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,97 +1,97 @@
-def _draw(network, figsize):
-    import matplotlib.pyplot as plt
-    import numpy as np
-
-    xy_list = []
-    for node_id, node in network.node_dict.items():
-        xy = list(node.geometry_xy.coords)[0]
-        xy_list.append(xy)
-    xy_array = np.array(xy_list)
-
-    if figsize is None:
-        net_length = xy_array[:,0].max() - xy_array[:,0].min()
-        net_width = xy_array[:,1].max() - xy_array[:,1].min()
-        fig_length = 16
-        fig_width = fig_length / net_length * net_width
-        plt.figure(figsize=(fig_length, fig_width))
-    else:
-        plt.figure(figsize=figsize)
-
-    ax = plt.gca()
-    ax.axes.xaxis.set_visible(False)
-    ax.axes.yaxis.set_visible(False)
-
-    plt.scatter(xy_array[:, 0], xy_array[:, 1], s=16.0, color='darkorange', zorder=1)
-
-    for link_id, link in network.link_dict.items():
-        xys = list(link.geometry_xy.coords)
-        xys_array = np.array(xys)
-        plt.plot(xys_array[:,0], xys_array[:,1], linewidth=1, color='deepskyblue', zorder=0)
-
-
-def show(network, save=False, figsize=None):
-    """
-    Show the network in a pop-up window
-
-    Parameters
-    ----------
-    network: Network
-        an osm2gmns Network object
-    save: bool
-        if True, the plot will also be saved to a local file named network.jpg
-    figsize: tuple of int/float, list of int/float
-        size of the figure
-
-    Returns
-    -------
-    None
-    """
-    if network.number_of_nodes == 0:
-        print('WARNING: Cannot show an empty network')
-        return
-
-    try:
-        import matplotlib.pyplot as plt
-    except ImportError as e:
-        raise ImportError("Matplotlib is required to show the network") from e
-
-    _draw(network, figsize)
-    if save:
-        plt.savefig('network.jpg')
-        print(f'Figure is saved to network.jpg')
-
-    plt.show()
-    plt.close()
-
-
-def saveFig(network, picpath='network.jpg',figsize=None):
-    """
-    Save the network plot to a local file
-
-    Parameters
-    ----------
-    network: Network
-        an osm2gmns Network object
-    picpath: str
-        path to store to network plot. can be an absolute or a relative path
-    figsize: tuple of int/float, list of int/float
-        size of the figure
-
-    Returns
-    -------
-    None
-    """
-
-    if network.number_of_nodes == 0:
-        print('WARNING: Cannot show an empty network')
-        return
-
-    try:
-        import matplotlib.pyplot as plt
-    except ImportError as e:
-        raise ImportError("Matplotlib is required to show the network") from e
-
-    _draw(network, figsize)
-    plt.savefig(picpath)
-    plt.close()
-    print(f'Figure is saved to {picpath}')
+def _draw(network, figsize):
+    import matplotlib.pyplot as plt
+    import numpy as np
+
+    xy_list = []
+    for node_id, node in network.node_dict.items():
+        xy = list(node.geometry_xy.coords)[0]
+        xy_list.append(xy)
+    xy_array = np.array(xy_list)
+
+    if figsize is None:
+        net_length = xy_array[:,0].max() - xy_array[:,0].min()
+        net_width = xy_array[:,1].max() - xy_array[:,1].min()
+        fig_length = 16
+        fig_width = fig_length / net_length * net_width
+        plt.figure(figsize=(fig_length, fig_width))
+    else:
+        plt.figure(figsize=figsize)
+
+    ax = plt.gca()
+    ax.axes.xaxis.set_visible(False)
+    ax.axes.yaxis.set_visible(False)
+
+    plt.scatter(xy_array[:, 0], xy_array[:, 1], s=16.0, color='darkorange', zorder=1)
+
+    for link_id, link in network.link_dict.items():
+        xys = list(link.geometry_xy.coords)
+        xys_array = np.array(xys)
+        plt.plot(xys_array[:,0], xys_array[:,1], linewidth=1, color='deepskyblue', zorder=0)
+
+
+def show(network, save=False, figsize=None):
+    """
+    Show the network in a pop-up window
+
+    Parameters
+    ----------
+    network: Network
+        an osm2gmns Network object
+    save: bool
+        if True, the plot will also be saved to a local file named network.jpg
+    figsize: tuple of int/float, list of int/float
+        size of the figure
+
+    Returns
+    -------
+    None
+    """
+    if network.number_of_nodes == 0:
+        print('WARNING: Cannot show an empty network')
+        return
+
+    try:
+        import matplotlib.pyplot as plt
+    except ImportError as e:
+        raise ImportError("Matplotlib is required to show the network") from e
+
+    _draw(network, figsize)
+    if save:
+        plt.savefig('network.jpg')
+        print(f'Figure is saved to network.jpg')
+
+    plt.show()
+    plt.close()
+
+
+def saveFig(network, picpath='network.jpg',figsize=None):
+    """
+    Save the network plot to a local file
+
+    Parameters
+    ----------
+    network: Network
+        an osm2gmns Network object
+    picpath: str
+        path to store to network plot. can be an absolute or a relative path
+    figsize: tuple of int/float, list of int/float
+        size of the figure
+
+    Returns
+    -------
+    None
+    """
+
+    if network.number_of_nodes == 0:
+        print('WARNING: Cannot show an empty network')
+        return
+
+    try:
+        import matplotlib.pyplot as plt
+    except ImportError as e:
+        raise ImportError("Matplotlib is required to show the network") from e
+
+    _draw(network, figsize)
+    plt.savefig(picpath)
+    plt.close()
+    print(f'Figure is saved to {picpath}')
```

### Comparing `osm2gmns-0.7.5/osm2gmns/osmnet/wayfilters.py` & `osm2gmns-0.7.6/osm2gmns/osmnet/wayfilters.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-# todo: walk, bike
-
-negligible_highway_type_set = {'path','construction','proposed','raceway','bridleway','rest_area','su',
-                               'road','abandoned','planned','trailhead','stairs','dismantled','disused','razed','access',
-                               'corridor','stop'}
-negligible_railway_type_set = {'construction','abandoned','disused','proposed','planned','dismantled','razed','ventilation_shaft'}
-negligible_aeroway_type_set = set()
-
-highway_poi_set = {'bus_stop','platform'}
-railway_poi_set = {'depot','station','workshop','halt','interlocking','junction','spur_junction','terminal','platform'}
-aeroway_poi_set = set()
-
-network_types_all = {'auto','bike','walk','railway','aeroway'}
-
-_filter_in = {'auto': {'motor_vehicle':{'yes'},
-                      'motorcar':{'yes'}},
-              'bike': {'bicycle':{'yes'}},
-              'walk': {'foot':{'yes'}}}
-
-_filters_ex = {'auto': {'highway':{'cycleway','footway','pedestrian','steps','track','corridor','elevator','escalator','service','living_street'},
-                       'motor_vehicle':{'no'},
-                       'motorcar':{'no'},
-                       'access':{'private'},
-                       'service':{'parking','parking_aisle','driveway','private','emergency_access'}},
-               'bike': {'highway':{'footway','steps','corridor','elevator','escalator','motor','motorway','motorway_link'},
-                       'bicycle':{'no'},
-                       'service':{'private'},
-                       'access':{'private'}},
-               'walk': {'highway':{'cycleway','motor','motorway','motorway_link'},
-                       'foot':{'no'},
-                       'service':{'private'},
-                       'access':{'private'}}}
-
-_agent_types_all = ['auto', 'bike', 'walk']
-
-
-
-def _checkIn(way, agent_type):
-    m_filter_in = _filter_in[agent_type]
-    for tag, include_list in m_filter_in.items():
-        if getattr(way, tag) in include_list:
-            return True
-    return None
-
-
-def _checkEx(way, agent_type):
-    m_filter_ex = _filters_ex[agent_type]
-    for tag, exclude_list in m_filter_ex.items():
-        if getattr(way, tag) in exclude_list:
-            return False
-    return True
-
-
-def getAllowableAgentType(way):
-    allowable_agent_type_list = []
-
-    for agent_type in _agent_types_all:
-        allowed = _checkIn(way, agent_type)
-        if allowed:
-            allowable_agent_type_list.append(agent_type)
-            continue
-
-        allowed = _checkEx(way, agent_type)
-        if allowed:
-            allowable_agent_type_list.append(agent_type)
-
-    return allowable_agent_type_list
+# todo: walk, bike
+
+negligible_highway_type_set = {'path','construction','proposed','raceway','bridleway','rest_area','su',
+                               'road','abandoned','planned','trailhead','stairs','dismantled','disused','razed','access',
+                               'corridor','stop'}
+negligible_railway_type_set = {'construction','abandoned','disused','proposed','planned','dismantled','razed','ventilation_shaft'}
+negligible_aeroway_type_set = set()
+
+highway_poi_set = {'bus_stop','platform'}
+railway_poi_set = {'depot','station','workshop','halt','interlocking','junction','spur_junction','terminal','platform'}
+aeroway_poi_set = set()
+
+network_types_all = {'auto','bike','walk','railway','aeroway'}
+
+_filter_in = {'auto': {'motor_vehicle':{'yes'},
+                      'motorcar':{'yes'}},
+              'bike': {'bicycle':{'yes'}},
+              'walk': {'foot':{'yes'}}}
+
+_filters_ex = {'auto': {'highway':{'cycleway','footway','pedestrian','steps','track','corridor','elevator','escalator','service','living_street'},
+                       'motor_vehicle':{'no'},
+                       'motorcar':{'no'},
+                       'access':{'private'},
+                       'service':{'parking','parking_aisle','driveway','private','emergency_access'}},
+               'bike': {'highway':{'footway','steps','corridor','elevator','escalator','motor','motorway','motorway_link'},
+                       'bicycle':{'no'},
+                       'service':{'private'},
+                       'access':{'private'}},
+               'walk': {'highway':{'cycleway','motor','motorway','motorway_link'},
+                       'foot':{'no'},
+                       'service':{'private'},
+                       'access':{'private'}}}
+
+_agent_types_all = ['auto', 'bike', 'walk']
+
+
+
+def _checkIn(way, agent_type):
+    m_filter_in = _filter_in[agent_type]
+    for tag, include_list in m_filter_in.items():
+        if getattr(way, tag) in include_list:
+            return True
+    return None
+
+
+def _checkEx(way, agent_type):
+    m_filter_ex = _filters_ex[agent_type]
+    for tag, exclude_list in m_filter_ex.items():
+        if getattr(way, tag) in exclude_list:
+            return False
+    return True
+
+
+def getAllowableAgentType(way):
+    allowable_agent_type_list = []
+
+    for agent_type in _agent_types_all:
+        allowed = _checkIn(way, agent_type)
+        if allowed:
+            allowable_agent_type_list.append(agent_type)
+            continue
+
+        allowed = _checkEx(way, agent_type)
+        if allowed:
+            allowable_agent_type_list.append(agent_type)
+
+    return allowable_agent_type_list
```

### Comparing `osm2gmns-0.7.5/osm2gmns/settings.py` & `osm2gmns-0.7.6/osm2gmns/settings.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-import logging
-
-log = False
-log_level = logging.WARNING
-log_name = 'osm2gmns'
-
-verbose = True
-
-lonlat_coord_precision = 7
-local_coord_precision = 2
-
-
-default_int_buffer = 20.0           # meter
-segment_resolution = 5.0            # meter
-
-osm_highway_type_dict = {'motorway': ('motorway', False),
-                         'motorway_link': ('motorway', True),
-                         'trunk': ('trunk', False),
-                         'trunk_link': ('trunk', True),
-                         'primary': ('primary', False),
-                         'primary_link': ('primary', True),
-                         'secondary': ('secondary', False),
-                         'secondary_link': ('secondary', True),
-                         'tertiary': ('tertiary', False),
-                         'tertiary_link': ('tertiary', True),
-                         'residential': ('residential', False),
-                         'residential_link': ('residential', True),
-                         'living_street': ('living_street', False),
-                         'service': ('service', False),
-                         'services': ('service', False),
-                         'cycleway': ('cycleway', False),
-                         'footway': ('footway', False),
-                         'pedestrian': ('footway', False),
-                         'steps': ('footway', False),
-                         'track': ('track', False),
-                         'unclassified': ('unclassified', False)}
-
-link_type_no_dict = {'motorway': 1, 'trunk': 2, 'primary': 3, 'secondary': 4,
-                     'tertiary': 5, 'residential': 6, 'living_street': 7,
-                     'service': 8, 'cycleway': 9, 'footway': 10, 'track': 11,
-                     'unclassified': 15, 'connector': 20, 'railway': 30, 'aeroway': 31}
-
-default_lanes_dict = {'motorway': 4, 'trunk': 3, 'primary': 3, 'secondary': 2,
-                      'tertiary': 2, 'residential': 1, 'living_street': 1, 'service': 1,
-                      'cycleway': 1, 'footway': 1, 'track': 1, 'unclassified': 1, 'connector': 2}
-
-default_speed_dict = {'motorway': 120, 'trunk': 100, 'primary': 80, 'secondary': 60,
-                      'tertiary': 40, 'residential': 30, 'living_street': 30, 'service': 30,
-                      'cycleway': 5, 'footway': 5, 'track': 30, 'unclassified': 30, 'connector': 120}
-
-default_capacity_dict = {'motorway': 2300, 'trunk': 2200, 'primary': 1800,
-                         'secondary': 1600, 'tertiary': 1200, 'residential': 1000,
-                         'living_street': 1000, 'service': 800,
-                         'cycleway': 800, 'footway': 800, 'track': 800,
-                         'unclassified': 800, 'connector': 9999}
-
-default_oneway_flag_dict = {'motorway': False, 'trunk': False, 'primary': False,
-                            'secondary': False, 'tertiary': False,
-                            'residential': False, 'living_street': False,
-                            'service': False, 'cycleway': True, 'footway': True,
-                            'track': True, 'unclassified': False, 'connector': False,
-                            'railway': True, 'aeroway': True}
-
-default_bounds = {'minlat': -90.0,
-                  'minlon': -180.0,
-                  'maxlat': 90.0,
-                  'maxlon': 180.0}
+import logging
+
+log = False
+log_level = logging.WARNING
+log_name = 'osm2gmns'
+
+verbose = True
+
+lonlat_coord_precision = 7
+local_coord_precision = 2
+
+
+default_int_buffer = 20.0           # meter
+segment_resolution = 5.0            # meter
+
+osm_highway_type_dict = {'motorway': ('motorway', False),
+                         'motorway_link': ('motorway', True),
+                         'trunk': ('trunk', False),
+                         'trunk_link': ('trunk', True),
+                         'primary': ('primary', False),
+                         'primary_link': ('primary', True),
+                         'secondary': ('secondary', False),
+                         'secondary_link': ('secondary', True),
+                         'tertiary': ('tertiary', False),
+                         'tertiary_link': ('tertiary', True),
+                         'residential': ('residential', False),
+                         'residential_link': ('residential', True),
+                         'living_street': ('living_street', False),
+                         'service': ('service', False),
+                         'services': ('service', False),
+                         'cycleway': ('cycleway', False),
+                         'footway': ('footway', False),
+                         'pedestrian': ('footway', False),
+                         'steps': ('footway', False),
+                         'track': ('track', False),
+                         'unclassified': ('unclassified', False)}
+
+link_type_no_dict = {'motorway': 1, 'trunk': 2, 'primary': 3, 'secondary': 4,
+                     'tertiary': 5, 'residential': 6, 'living_street': 7,
+                     'service': 8, 'cycleway': 9, 'footway': 10, 'track': 11,
+                     'unclassified': 15, 'connector': 20, 'railway': 30, 'aeroway': 31}
+
+default_lanes_dict = {'motorway': 4, 'trunk': 3, 'primary': 3, 'secondary': 2,
+                      'tertiary': 2, 'residential': 1, 'living_street': 1, 'service': 1,
+                      'cycleway': 1, 'footway': 1, 'track': 1, 'unclassified': 1, 'connector': 2}
+
+default_speed_dict = {'motorway': 120, 'trunk': 100, 'primary': 80, 'secondary': 60,
+                      'tertiary': 40, 'residential': 30, 'living_street': 30, 'service': 30,
+                      'cycleway': 5, 'footway': 5, 'track': 30, 'unclassified': 30, 'connector': 120}
+
+default_capacity_dict = {'motorway': 2300, 'trunk': 2200, 'primary': 1800,
+                         'secondary': 1600, 'tertiary': 1200, 'residential': 1000,
+                         'living_street': 1000, 'service': 800,
+                         'cycleway': 800, 'footway': 800, 'track': 800,
+                         'unclassified': 800, 'connector': 9999}
+
+default_oneway_flag_dict = {'motorway': False, 'trunk': False, 'primary': False,
+                            'secondary': False, 'tertiary': False,
+                            'residential': False, 'living_street': False,
+                            'service': False, 'cycleway': True, 'footway': True,
+                            'track': True, 'unclassified': False, 'connector': False,
+                            'railway': True, 'aeroway': True}
+
+default_bounds = {'minlat': -90.0,
+                  'minlon': -180.0,
+                  'maxlat': 90.0,
+                  'maxlon': 180.0}
```

### Comparing `osm2gmns-0.7.5/osm2gmns/utils/util.py` & `osm2gmns-0.7.6/osm2gmns/utils/util.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-import osm2gmns.settings as og_settings
-import logging
-
-
-_log_created = False
-
-
-def getLogger():
-    global _log_created
-
-    if not og_settings.log:
-        return None
-
-    logger = logging.getLogger(og_settings.log_name)
-
-    if not _log_created:
-        logger.setLevel(og_settings.log_level)
-        handler = logging.FileHandler('osm2gmns.log', 'w')
-        formatter = logging.Formatter('%(asctime)s %(filename)s[line:%(lineno)d] %(levelname)s %(message)s', '%H:%M:%S')
-        handler.setFormatter(formatter)
-        logger.addHandler(handler)
-
-        _log_created = True
-
-    return logger
-
-
-
-def config(verbose=og_settings.verbose,
-           lonlat_coord_precision=og_settings.lonlat_coord_precision,
-           local_coord_precision=og_settings.local_coord_precision,
-           log_level=None):
-    og_settings.verbose = verbose
-    og_settings.lonlat_coord_precision = lonlat_coord_precision
-    og_settings.local_coord_precision = local_coord_precision
-
-    if log_level is not None:
-        if not isinstance(log_level, str):
-            print('WARNING: log_level must be a string and chosen from DEBUG, INFO, WARNING, ERROR, CRITICAL')
-        else:
-            log_level_upper = log_level.upper()
-            if log_level_upper == 'DEBUG':
-                og_settings.log = True
-                og_settings.log_level = logging.DEBUG
-            elif log_level_upper == 'INFO':
-                og_settings.log = True
-                og_settings.log_level = logging.INFO
-            elif log_level_upper == 'WARNING':
-                og_settings.log = True
-                og_settings.log_level = logging.WARNING
-            elif log_level_upper == 'ERROR':
-                og_settings.log = True
-                og_settings.log_level = logging.ERROR
-            elif log_level_upper == 'CRITICAL':
-                og_settings.log = True
-                og_settings.log_level = logging.CRITICAL
-            else:
-                print('WARNING: log_level must be a string and chosen from DEBUG, INFO, WARNING, ERROR, CRITICAL')
-
+import osm2gmns.settings as og_settings
+import logging
+
+
+_log_created = False
+
+
+def getLogger():
+    global _log_created
+
+    if not og_settings.log:
+        return None
+
+    logger = logging.getLogger(og_settings.log_name)
+
+    if not _log_created:
+        logger.setLevel(og_settings.log_level)
+        handler = logging.FileHandler('osm2gmns.log', 'w')
+        formatter = logging.Formatter('%(asctime)s %(filename)s[line:%(lineno)d] %(levelname)s %(message)s', '%H:%M:%S')
+        handler.setFormatter(formatter)
+        logger.addHandler(handler)
+
+        _log_created = True
+
+    return logger
+
+
+
+def config(verbose=og_settings.verbose,
+           lonlat_coord_precision=og_settings.lonlat_coord_precision,
+           local_coord_precision=og_settings.local_coord_precision,
+           log_level=None):
+    og_settings.verbose = verbose
+    og_settings.lonlat_coord_precision = lonlat_coord_precision
+    og_settings.local_coord_precision = local_coord_precision
+
+    if log_level is not None:
+        if not isinstance(log_level, str):
+            print('WARNING: log_level must be a string and chosen from DEBUG, INFO, WARNING, ERROR, CRITICAL')
+        else:
+            log_level_upper = log_level.upper()
+            if log_level_upper == 'DEBUG':
+                og_settings.log = True
+                og_settings.log_level = logging.DEBUG
+            elif log_level_upper == 'INFO':
+                og_settings.log = True
+                og_settings.log_level = logging.INFO
+            elif log_level_upper == 'WARNING':
+                og_settings.log = True
+                og_settings.log_level = logging.WARNING
+            elif log_level_upper == 'ERROR':
+                og_settings.log = True
+                og_settings.log_level = logging.ERROR
+            elif log_level_upper == 'CRITICAL':
+                og_settings.log = True
+                og_settings.log_level = logging.CRITICAL
+            else:
+                print('WARNING: log_level must be a string and chosen from DEBUG, INFO, WARNING, ERROR, CRITICAL')
+
```

### Comparing `osm2gmns-0.7.5/osm2gmns/utils/util_coord.py` & `osm2gmns-0.7.6/osm2gmns/utils/util_coord.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,187 +1,187 @@
-# Copyright (C) 2012 Tobias Bieniek <Tobias.Bieniek@gmx.de>
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
-# documentation files (the "Software"), to deal in the Software without restriction, including without limitation
-# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
-# and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-#
-# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-#
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
-# WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
-# OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
-# OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
-try:
-    import numpy as mathlib
-    use_numpy = True
-except ImportError:
-    import math as mathlib
-    use_numpy = False
-
-
-K0 = 0.9996
-
-E = 0.00669438
-E2 = E * E
-E3 = E2 * E
-E_P2 = E / (1.0 - E)
-
-SQRT_E = (1 - E)**0.5
-_E = (1 - SQRT_E) / (1 + SQRT_E)
-_E2 = _E * _E
-_E3 = _E2 * _E
-_E4 = _E3 * _E
-_E5 = _E4 * _E
-
-M1 = (1 - E / 4 - 3 * E2 / 64 - 5 * E3 / 256)
-M2 = (3 * E / 8 + 3 * E2 / 32 + 45 * E3 / 1024)
-M3 = (15 * E2 / 256 + 45 * E3 / 1024)
-M4 = (35 * E3 / 3072)
-
-P2 = (3. / 2 * _E - 27. / 32 * _E3 + 269. / 512 * _E5)
-P3 = (21. / 16 * _E2 - 55. / 32 * _E4)
-P4 = (151. / 96 * _E3 - 417. / 128 * _E5)
-P5 = (1097. / 512 * _E4)
-
-R = 6378137
-
-ZONE_LETTERS = "CDEFGHJKLMNPQRSTUVWXX"
-
-
-def in_bounds(x, lower, upper, upper_strict=False):
-    if upper_strict and use_numpy:
-        return lower <= mathlib.min(x) and mathlib.max(x) < upper
-    elif upper_strict and not use_numpy:
-        return lower <= x < upper
-    elif use_numpy:
-        return lower <= mathlib.min(x) and mathlib.max(x) <= upper
-    return lower <= x <= upper
-
-
-def mixed_signs(x):
-    return use_numpy and mathlib.min(x) < 0 <= mathlib.max(x)
-
-
-def negative(x):
-    return mathlib.max(x) < 0 if use_numpy else x < 0
-
-
-def latitude_to_zone_letter(latitude):
-    # If the input is a numpy array, just use the first element
-    # User responsibility to make sure that all points are in one zone
-    if use_numpy and isinstance(latitude, mathlib.ndarray):
-        latitude = latitude.flat[0]
-
-    return ZONE_LETTERS[int(latitude + 80) >> 3] if -80 <= latitude <= 84 else None
-
-
-class OutOfRangeError(ValueError):
-    pass
-
-
-def from_latlon(longitude, latitude, central_longitude):
-    central_lon_rad = mathlib.radians(central_longitude)
-
-    lat_rad = mathlib.radians(latitude)
-    lat_sin = mathlib.sin(lat_rad)
-    lat_cos = mathlib.cos(lat_rad)
-
-    lat_tan = lat_sin / lat_cos
-    lat_tan2 = lat_tan * lat_tan
-    lat_tan4 = lat_tan2 * lat_tan2
-
-    lon_rad = mathlib.radians(longitude)
-
-    n = R / mathlib.sqrt(1 - E * lat_sin ** 2)
-    c = E_P2 * lat_cos ** 2
-
-    a = lat_cos * (lon_rad - central_lon_rad)
-    a2 = a * a
-    a3 = a2 * a
-    a4 = a3 * a
-    a5 = a4 * a
-    a6 = a5 * a
-
-    m = R * (M1 * lat_rad - M2 * mathlib.sin(2 * lat_rad) + M3 * mathlib.sin(4 * lat_rad) - M4 * mathlib.sin(6 * lat_rad))
-    easting = K0 * n * (a + a3 / 6 * (1 - lat_tan2 + c) + a5 / 120 * (5 - 18 * lat_tan2 + lat_tan4 + 72 * c - 58 * E_P2)) + 500000
-    northing = K0 * (m + n * lat_tan * (a2 / 2 + a4 / 24 * (5 - lat_tan2 + 9 * c + 4 * c ** 2) + a6 / 720 * (61 - 58 * lat_tan2 + lat_tan4 + 600 * c - 330 * E_P2)))
-
-    if mixed_signs(latitude):
-        raise ValueError("latitudes must all have the same sign")
-    elif negative(latitude):
-        northing += 10000000
-
-    return easting, northing
-
-
-def to_latlon(easting, northing, central_longitude, northern):  # , zone_number, zone_letter=None, northern=None, strict=True
-    # if not zone_letter and northern is None:
-    #     raise ValueError('either zone_letter or northern needs to be set')
-    #
-    # elif zone_letter and northern is not None:
-    #     raise ValueError('set either zone_letter or northern, but not both')
-    #
-    #
-    if not in_bounds(easting, 100000, 1000000, upper_strict=True):
-        raise OutOfRangeError('easting out of range (must be between 100.000 m and 999.999 m)')
-    if not in_bounds(northing, 0, 10000000):
-        raise OutOfRangeError('northing out of range (must be between 0 m and 10.000.000 m)')
-    #
-    # check_valid_zone(zone_number, zone_letter)
-    #
-    # if zone_letter:
-    #     zone_letter = zone_letter.upper()
-    #     northern = (zone_letter >= 'N')
-
-    x = easting - 500000
-    y = northing
-
-    if not northern:
-        y -= 10000000
-
-    m = y / K0
-    mu = m / (R * M1)
-
-    p_rad = (mu +
-             P2 * mathlib.sin(2 * mu) +
-             P3 * mathlib.sin(4 * mu) +
-             P4 * mathlib.sin(6 * mu) +
-             P5 * mathlib.sin(8 * mu))
-
-    p_sin = mathlib.sin(p_rad)
-    p_sin2 = p_sin * p_sin
-
-    p_cos = mathlib.cos(p_rad)
-
-    p_tan = p_sin / p_cos
-    p_tan2 = p_tan * p_tan
-    p_tan4 = p_tan2 * p_tan2
-
-    ep_sin = 1 - E * p_sin2
-    ep_sin_sqrt = mathlib.sqrt(1 - E * p_sin2)
-
-    n = R / ep_sin_sqrt
-    r = (1 - E) / ep_sin
-
-    c = _E * p_cos ** 2
-    c2 = c * c
-
-    d = x / (n * K0)
-    d2 = d * d
-    d3 = d2 * d
-    d4 = d3 * d
-    d5 = d4 * d
-    d6 = d5 * d
-
-    latitude = (p_rad - (p_tan / r) *
-                (d2 / 2 -
-                 d4 / 24 * (5 + 3 * p_tan2 + 10 * c - 4 * c2 - 9 * E_P2)) +
-                d6 / 720 * (61 + 90 * p_tan2 + 298 * c + 45 * p_tan4 - 252 * E_P2 - 3 * c2))
-
-    longitude = (d -
-                 d3 / 6 * (1 + 2 * p_tan2 + c) +
-                 d5 / 120 * (5 - 2 * c + 28 * p_tan2 - 3 * c2 + 8 * E_P2 + 24 * p_tan4)) / p_cos
-
-    return mathlib.degrees(longitude) + central_longitude, mathlib.degrees(latitude)
+# Copyright (C) 2012 Tobias Bieniek <Tobias.Bieniek@gmx.de>
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+# documentation files (the "Software"), to deal in the Software without restriction, including without limitation
+# the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
+# and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+#
+# The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+#
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
+# WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS
+# OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR
+# OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
+try:
+    import numpy as mathlib
+    use_numpy = True
+except ImportError:
+    import math as mathlib
+    use_numpy = False
+
+
+K0 = 0.9996
+
+E = 0.00669438
+E2 = E * E
+E3 = E2 * E
+E_P2 = E / (1.0 - E)
+
+SQRT_E = (1 - E)**0.5
+_E = (1 - SQRT_E) / (1 + SQRT_E)
+_E2 = _E * _E
+_E3 = _E2 * _E
+_E4 = _E3 * _E
+_E5 = _E4 * _E
+
+M1 = (1 - E / 4 - 3 * E2 / 64 - 5 * E3 / 256)
+M2 = (3 * E / 8 + 3 * E2 / 32 + 45 * E3 / 1024)
+M3 = (15 * E2 / 256 + 45 * E3 / 1024)
+M4 = (35 * E3 / 3072)
+
+P2 = (3. / 2 * _E - 27. / 32 * _E3 + 269. / 512 * _E5)
+P3 = (21. / 16 * _E2 - 55. / 32 * _E4)
+P4 = (151. / 96 * _E3 - 417. / 128 * _E5)
+P5 = (1097. / 512 * _E4)
+
+R = 6378137
+
+ZONE_LETTERS = "CDEFGHJKLMNPQRSTUVWXX"
+
+
+def in_bounds(x, lower, upper, upper_strict=False):
+    if upper_strict and use_numpy:
+        return lower <= mathlib.min(x) and mathlib.max(x) < upper
+    elif upper_strict and not use_numpy:
+        return lower <= x < upper
+    elif use_numpy:
+        return lower <= mathlib.min(x) and mathlib.max(x) <= upper
+    return lower <= x <= upper
+
+
+def mixed_signs(x):
+    return use_numpy and mathlib.min(x) < 0 <= mathlib.max(x)
+
+
+def negative(x):
+    return mathlib.max(x) < 0 if use_numpy else x < 0
+
+
+def latitude_to_zone_letter(latitude):
+    # If the input is a numpy array, just use the first element
+    # User responsibility to make sure that all points are in one zone
+    if use_numpy and isinstance(latitude, mathlib.ndarray):
+        latitude = latitude.flat[0]
+
+    return ZONE_LETTERS[int(latitude + 80) >> 3] if -80 <= latitude <= 84 else None
+
+
+class OutOfRangeError(ValueError):
+    pass
+
+
+def from_latlon(longitude, latitude, central_longitude):
+    central_lon_rad = mathlib.radians(central_longitude)
+
+    lat_rad = mathlib.radians(latitude)
+    lat_sin = mathlib.sin(lat_rad)
+    lat_cos = mathlib.cos(lat_rad)
+
+    lat_tan = lat_sin / lat_cos
+    lat_tan2 = lat_tan * lat_tan
+    lat_tan4 = lat_tan2 * lat_tan2
+
+    lon_rad = mathlib.radians(longitude)
+
+    n = R / mathlib.sqrt(1 - E * lat_sin ** 2)
+    c = E_P2 * lat_cos ** 2
+
+    a = lat_cos * (lon_rad - central_lon_rad)
+    a2 = a * a
+    a3 = a2 * a
+    a4 = a3 * a
+    a5 = a4 * a
+    a6 = a5 * a
+
+    m = R * (M1 * lat_rad - M2 * mathlib.sin(2 * lat_rad) + M3 * mathlib.sin(4 * lat_rad) - M4 * mathlib.sin(6 * lat_rad))
+    easting = K0 * n * (a + a3 / 6 * (1 - lat_tan2 + c) + a5 / 120 * (5 - 18 * lat_tan2 + lat_tan4 + 72 * c - 58 * E_P2)) + 500000
+    northing = K0 * (m + n * lat_tan * (a2 / 2 + a4 / 24 * (5 - lat_tan2 + 9 * c + 4 * c ** 2) + a6 / 720 * (61 - 58 * lat_tan2 + lat_tan4 + 600 * c - 330 * E_P2)))
+
+    if mixed_signs(latitude):
+        raise ValueError("latitudes must all have the same sign")
+    elif negative(latitude):
+        northing += 10000000
+
+    return easting, northing
+
+
+def to_latlon(easting, northing, central_longitude, northern):  # , zone_number, zone_letter=None, northern=None, strict=True
+    # if not zone_letter and northern is None:
+    #     raise ValueError('either zone_letter or northern needs to be set')
+    #
+    # elif zone_letter and northern is not None:
+    #     raise ValueError('set either zone_letter or northern, but not both')
+    #
+    #
+    if not in_bounds(easting, 100000, 1000000, upper_strict=True):
+        raise OutOfRangeError('easting out of range (must be between 100.000 m and 999.999 m)')
+    if not in_bounds(northing, 0, 10000000):
+        raise OutOfRangeError('northing out of range (must be between 0 m and 10.000.000 m)')
+    #
+    # check_valid_zone(zone_number, zone_letter)
+    #
+    # if zone_letter:
+    #     zone_letter = zone_letter.upper()
+    #     northern = (zone_letter >= 'N')
+
+    x = easting - 500000
+    y = northing
+
+    if not northern:
+        y -= 10000000
+
+    m = y / K0
+    mu = m / (R * M1)
+
+    p_rad = (mu +
+             P2 * mathlib.sin(2 * mu) +
+             P3 * mathlib.sin(4 * mu) +
+             P4 * mathlib.sin(6 * mu) +
+             P5 * mathlib.sin(8 * mu))
+
+    p_sin = mathlib.sin(p_rad)
+    p_sin2 = p_sin * p_sin
+
+    p_cos = mathlib.cos(p_rad)
+
+    p_tan = p_sin / p_cos
+    p_tan2 = p_tan * p_tan
+    p_tan4 = p_tan2 * p_tan2
+
+    ep_sin = 1 - E * p_sin2
+    ep_sin_sqrt = mathlib.sqrt(1 - E * p_sin2)
+
+    n = R / ep_sin_sqrt
+    r = (1 - E) / ep_sin
+
+    c = _E * p_cos ** 2
+    c2 = c * c
+
+    d = x / (n * K0)
+    d2 = d * d
+    d3 = d2 * d
+    d4 = d3 * d
+    d5 = d4 * d
+    d6 = d5 * d
+
+    latitude = (p_rad - (p_tan / r) *
+                (d2 / 2 -
+                 d4 / 24 * (5 + 3 * p_tan2 + 10 * c - 4 * c2 - 9 * E_P2)) +
+                d6 / 720 * (61 + 90 * p_tan2 + 298 * c + 45 * p_tan4 - 252 * E_P2 - 3 * c2))
+
+    longitude = (d -
+                 d3 / 6 * (1 + 2 * p_tan2 + c) +
+                 d5 / 120 * (5 - 2 * c + 28 * p_tan2 - 3 * c2 + 8 * E_P2 + 24 * p_tan4)) / p_cos
+
+    return mathlib.degrees(longitude) + central_longitude, mathlib.degrees(latitude)
```

### Comparing `osm2gmns-0.7.5/osm2gmns/utils/util_geo.py` & `osm2gmns-0.7.6/osm2gmns/utils/util_geo.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,133 +1,133 @@
-from osm2gmns.utils.util_coord import to_latlon, from_latlon
-import osm2gmns.settings as og_settings
-from shapely import geometry
-import functools
-import numpy as np
-import math
-
-
-
-def getLineFromNodes(node_list):
-    if len(node_list) < 2: return None, None
-    point_list = [node.geometry for node in node_list]
-    line = geometry.LineString(point_list)
-    point_list_xy = [node.geometry_xy for node in node_list]
-    line_xy = geometry.LineString(point_list_xy)
-    return line, line_xy
-
-
-def getPolygonFromNodes(node_list):
-    if len(node_list) < 3: return None, None
-    point_list = [(node.geometry.x, node.geometry.y) for node in node_list]
-    poly = geometry.Polygon(point_list)
-    point_list_xy = [(node.geometry_xy.x, node.geometry_xy.y) for node in node_list]
-    poly_xy = geometry.Polygon(point_list_xy)
-    return poly, poly_xy
-
-
-def getLineAngle(ib_line, ob_line, complete_line=True):
-    # complete_line - True (False): use the last and first (second last) coords to calculate line direction
-    # ob_line counter clockwise: 0 to 180; ob_line clockwise: 0 to -180
-
-    if complete_line:
-        angle_ib = math.atan2(ib_line.coords[-1][1] - ib_line.coords[0][1],
-                              ib_line.coords[-1][0] - ib_line.coords[0][0])
-        angle_ob = math.atan2(ob_line.coords[-1][1] - ob_line.coords[0][1],
-                              ob_line.coords[-1][0] - ob_line.coords[0][0])
-    else:
-        angle_ib = math.atan2(ib_line.coords[-1][1] - ib_line.coords[-2][1],
-                              ib_line.coords[-1][0] - ib_line.coords[-2][0])
-        angle_ob = math.atan2(ob_line.coords[-1][1] - ob_line.coords[-2][1],
-                              ob_line.coords[-1][0] - ob_line.coords[-2][0])
-
-    angle = angle_ob - angle_ib
-    if angle < -1 * math.pi:
-        angle += 2 * math.pi
-    if angle > math.pi:
-        angle -= 2 * math.pi
-    return angle
-
-
-def offsetLine(line, distance):
-    coords = list(line.coords)
-    offset_coord_list_temp = []
-    for i in range(len(coords) - 1):
-        start_x, start_y = coords[i]
-        end_x, end_y = coords[i+1]
-
-        delta_x = end_x - start_x
-        delta_y = end_y - start_y
-        length = (delta_x ** 2 + delta_y ** 2) ** 0.5
-        offset_x = delta_y / length * distance
-        offset_y = -1 * delta_x / length * distance
-
-        offset_coord_list_temp.append(((start_x + offset_x, start_y + offset_y), (end_x + offset_x, end_y + offset_y)))
-
-    coords_offset = [offset_coord_list_temp[0][0]]
-    for i in range(len(offset_coord_list_temp) - 1):
-        uf = offset_coord_list_temp[i][0]
-        ut = offset_coord_list_temp[i][1]
-        df = offset_coord_list_temp[i + 1][0]
-        dt = offset_coord_list_temp[i + 1][1]
-
-        d_utdf = ((ut[0] - df[0]) ** 2 + ((ut[1] - df[1]) ** 2)) ** 0.5
-        if d_utdf < 0.1:
-            x, y = (ut[0] + df[0]) * 0.5, (ut[1] + df[1]) * 0.5
-            coords_offset.append((x, y))
-        else:
-            A = [[ut[1] - uf[1], uf[0] - ut[0]], [dt[1] - df[1], df[0] - dt[0]]]
-            b = [(ut[1] - uf[1]) * uf[0] - (ut[0] - uf[0]) * uf[1],
-                 (dt[1] - df[1]) * df[0] - (dt[0] - df[0]) * df[1]]
-            A_mat = np.mat(A)
-            b_mat = np.mat(b).T
-            solution = np.linalg.inv(A_mat) * b_mat
-            x, y = solution[0, 0], solution[1, 0]
-
-            d_mut = ((ut[0] - x) ** 2 + ((ut[1] - y) ** 2)) ** 0.5
-            if d_mut > 200:
-                x, y = (ut[0] + df[0]) * 0.5, (ut[1] + df[1]) * 0.5
-            coords_offset.append((x, y))
-
-    coords_offset.append(offset_coord_list_temp[-1][1])
-    return geometry.LineString(coords_offset)
-
-
-class GeoTransformer:
-    def __init__(self, central_lon, central_lat, northern):
-        self.central_lon = central_lon
-        self.central_lat = central_lat
-        self.northern = northern
-
-        self.from_latlon = functools.partial(from_latlon, central_longitude=self.central_lon)
-        self.to_latlon = functools.partial(to_latlon, central_longitude=self.central_lon, northern=self.northern)
-
-    def _from_latlon_(self, p):
-        return np.round(self.from_latlon(*p), og_settings.local_coord_precision)
-
-    def _to_latlon_(self, p):
-        return np.round(self.to_latlon(*p), og_settings.lonlat_coord_precision)
-
-    def _transform(self, shape, func):
-        construct = shape.__class__
-
-        if shape.geom_type.startswith('Multi'):
-            parts = [self._transform(geom, func) for geom in shape.geoms]
-            return construct(parts)
-
-        if shape.geom_type == 'Point':
-            return construct(list(map(func, shape.coords))[0])
-
-        if shape.geom_type in ('Point', 'LineString'):
-            return construct(map(func, shape.coords))
-
-        if shape.geom_type == 'Polygon':
-            exterior = map(func, shape.exterior.coords)
-            rings = [map(func, ring.coords) for ring in shape.interiors]
-            return construct(exterior, rings)
-
-
-    def geo_from_latlon(self, shape):
-        return self._transform(shape, self._from_latlon_)
-
-    def geo_to_latlon(self, shape):
-        return self._transform(shape, self._to_latlon_)
+from osm2gmns.utils.util_coord import to_latlon, from_latlon
+import osm2gmns.settings as og_settings
+from shapely import geometry
+import functools
+import numpy as np
+import math
+
+
+
+def getLineFromNodes(node_list):
+    if len(node_list) < 2: return None, None
+    point_list = [node.geometry for node in node_list]
+    line = geometry.LineString(point_list)
+    point_list_xy = [node.geometry_xy for node in node_list]
+    line_xy = geometry.LineString(point_list_xy)
+    return line, line_xy
+
+
+def getPolygonFromNodes(node_list):
+    if len(node_list) < 3: return None, None
+    point_list = [(node.geometry.x, node.geometry.y) for node in node_list]
+    poly = geometry.Polygon(point_list)
+    point_list_xy = [(node.geometry_xy.x, node.geometry_xy.y) for node in node_list]
+    poly_xy = geometry.Polygon(point_list_xy)
+    return poly, poly_xy
+
+
+def getLineAngle(ib_line, ob_line, complete_line=True):
+    # complete_line - True (False): use the last and first (second last) coords to calculate line direction
+    # ob_line counter clockwise: 0 to 180; ob_line clockwise: 0 to -180
+
+    if complete_line:
+        angle_ib = math.atan2(ib_line.coords[-1][1] - ib_line.coords[0][1],
+                              ib_line.coords[-1][0] - ib_line.coords[0][0])
+        angle_ob = math.atan2(ob_line.coords[-1][1] - ob_line.coords[0][1],
+                              ob_line.coords[-1][0] - ob_line.coords[0][0])
+    else:
+        angle_ib = math.atan2(ib_line.coords[-1][1] - ib_line.coords[-2][1],
+                              ib_line.coords[-1][0] - ib_line.coords[-2][0])
+        angle_ob = math.atan2(ob_line.coords[-1][1] - ob_line.coords[-2][1],
+                              ob_line.coords[-1][0] - ob_line.coords[-2][0])
+
+    angle = angle_ob - angle_ib
+    if angle < -1 * math.pi:
+        angle += 2 * math.pi
+    if angle > math.pi:
+        angle -= 2 * math.pi
+    return angle
+
+
+def offsetLine(line, distance):
+    coords = list(line.coords)
+    offset_coord_list_temp = []
+    for i in range(len(coords) - 1):
+        start_x, start_y = coords[i]
+        end_x, end_y = coords[i+1]
+
+        delta_x = end_x - start_x
+        delta_y = end_y - start_y
+        length = (delta_x ** 2 + delta_y ** 2) ** 0.5
+        offset_x = delta_y / length * distance
+        offset_y = -1 * delta_x / length * distance
+
+        offset_coord_list_temp.append(((start_x + offset_x, start_y + offset_y), (end_x + offset_x, end_y + offset_y)))
+
+    coords_offset = [offset_coord_list_temp[0][0]]
+    for i in range(len(offset_coord_list_temp) - 1):
+        uf = offset_coord_list_temp[i][0]
+        ut = offset_coord_list_temp[i][1]
+        df = offset_coord_list_temp[i + 1][0]
+        dt = offset_coord_list_temp[i + 1][1]
+
+        d_utdf = ((ut[0] - df[0]) ** 2 + ((ut[1] - df[1]) ** 2)) ** 0.5
+        if d_utdf < 0.1:
+            x, y = (ut[0] + df[0]) * 0.5, (ut[1] + df[1]) * 0.5
+            coords_offset.append((x, y))
+        else:
+            A = [[ut[1] - uf[1], uf[0] - ut[0]], [dt[1] - df[1], df[0] - dt[0]]]
+            b = [(ut[1] - uf[1]) * uf[0] - (ut[0] - uf[0]) * uf[1],
+                 (dt[1] - df[1]) * df[0] - (dt[0] - df[0]) * df[1]]
+            A_mat = np.mat(A)
+            b_mat = np.mat(b).T
+            solution = np.linalg.inv(A_mat) * b_mat
+            x, y = solution[0, 0], solution[1, 0]
+
+            d_mut = ((ut[0] - x) ** 2 + ((ut[1] - y) ** 2)) ** 0.5
+            if d_mut > 200:
+                x, y = (ut[0] + df[0]) * 0.5, (ut[1] + df[1]) * 0.5
+            coords_offset.append((x, y))
+
+    coords_offset.append(offset_coord_list_temp[-1][1])
+    return geometry.LineString(coords_offset)
+
+
+class GeoTransformer:
+    def __init__(self, central_lon, central_lat, northern):
+        self.central_lon = central_lon
+        self.central_lat = central_lat
+        self.northern = northern
+
+        self.from_latlon = functools.partial(from_latlon, central_longitude=self.central_lon)
+        self.to_latlon = functools.partial(to_latlon, central_longitude=self.central_lon, northern=self.northern)
+
+    def _from_latlon_(self, p):
+        return np.round(self.from_latlon(*p), og_settings.local_coord_precision)
+
+    def _to_latlon_(self, p):
+        return np.round(self.to_latlon(*p), og_settings.lonlat_coord_precision)
+
+    def _transform(self, shape, func):
+        construct = shape.__class__
+
+        if shape.geom_type.startswith('Multi'):
+            parts = [self._transform(geom, func) for geom in shape.geoms]
+            return construct(parts)
+
+        if shape.geom_type == 'Point':
+            return construct(list(map(func, shape.coords))[0])
+
+        if shape.geom_type in ('Point', 'LineString'):
+            return construct(map(func, shape.coords))
+
+        if shape.geom_type == 'Polygon':
+            exterior = map(func, shape.exterior.coords)
+            rings = [map(func, ring.coords) for ring in shape.interiors]
+            return construct(exterior, rings)
+
+
+    def geo_from_latlon(self, shape):
+        return self._transform(shape, self._from_latlon_)
+
+    def geo_to_latlon(self, shape):
+        return self._transform(shape, self._to_latlon_)
```

### Comparing `osm2gmns-0.7.5/osm2gmns.egg-info/PKG-INFO` & `osm2gmns-0.7.6/osm2gmns.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,165 +1,154 @@
-Metadata-Version: 2.1
-Name: osm2gmns
-Version: 0.7.5
-Summary: convert map data from OpenStreetMap to network files in GMNS format
-Home-page: https://github.com/jiawlu/OSM2GMNS
-Author: Jiawei Lu, Xuesong Zhou
-Author-email: jiaweil9@asu.edu, xzhou74@asu.edu
-License: GPLv3+
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9.0
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: numpy>=1.26.4
-Requires-Dist: osmium>=3.7.0
-Requires-Dist: Requests>=2.31.0
-Requires-Dist: setuptools>=68.2.2
-Requires-Dist: Shapely>=2.0.3
-Requires-Dist: matplotlib>=3.8.2
-
-osm2gmns
-====================================
-| **Authors**: Jiawei Lu, Xuesong (Simon) Zhou
-| **Email**: jiaweil9@asu.edu, xzhou74@asu.edu
-
-
-osm2gmns is an open-source Python package that enables users to conveniently obtain and
-manipulate any networks from `OpenStreetMap`_ (OSM). With a single line of Python code,
-users can obtian and model drivable, bikeable, walkable, railway, and aeroway networks
-for any region in the world, and output networks to csv files in `GMNS`_ format for seamless
-data sharing and research collaboration. osm2gmns mainly focus on providing researchers and
-practitioners with flexible, standard and ready-to-use multi-module transportation networks,
-as well as a bunch of customized and practical functions to facilitate various reseaches
-and applications on traffic modeling.
-
-
-Publication
-====================================
-
-Lu, J., & Zhou, X.S. (2023). Virtual track networks: A hierarchical modeling framework and
-open-source tools for simplified and efficient connected and automated mobility (CAM) system
-design based on general modeling network specification (GMNS). Transportation Research
-Part C: Emerging Technologies, 153, 104223. `paper link`_
-
-
-Main Features
-====================================
-
-- Obtain any networks from OSM. osm2gmns parses map data from OSM and output networks to
-  csv files in GMNS format.
-- Standard network format. osm2gmns adopts GMNS as the network format for seamless data
-  sharing and research collaboration.
-- Ready-to-use network. osm2gmns cleans erroneous information from osm map data and is able
-  to fill up critical missing values, i.e., lanes, speed and capacity, to quickly provide
-  ready-to-use networks.
-- Directed network. two directed road links are generated for each bi-directional osm ways identified by osm2gmns
-- Multi-module support. five different network types are supported, including auto, bike, walk, railway, and aeroway
-- Customized and practical functions to facilitate traffic modeling. functions include
-  complex intersection consolidation, moevement generation, traffic zone creation, short link combination,
-  network visualization.
-- Multi-Resolution modeling. osm2gmns automatically construct the corresponding mesoscopic and microscopic
-  networks for any macroscopic network in GMNS format.
-
-
-Installation
-====================================
-
-.. code-block:: bash
-
-    pip install osm2gmns
-
-If you meet installation issues, please refer to the `user's guide`_ for solutions.
-
-
-Simple examples
-====================================
-
-You can find the osm map file used in the examples below at 'sample networks/Arizona State University, Tempe Campus'
-
-Quickly get the network with point of interest (POI) information from an osm file
-
-.. code:: python
-
-    >>> import osm2gmns as og
-    >>> net = og.getNetFromFile('asu.osm', POI=True)
-    >>> og.outputNetToCSV(net)
-
-Generate multi-resolution networks from an osm file
-
-.. code:: python
-
-    >>> import osm2gmns as og
-    >>> net = og.getNetFromFile('asu.osm')
-    >>> og.consolidateComplexIntersections(net, auto_identify=True)
-    >>> og.buildMultiResolutionNets(net)
-    >>> og.outputNetToCSV(net)
-
-
-Get relation id of a place of interest and download the corresponding osm file
-=====================================================================================================================
-You can use the following code to get the relation id of a place of interest and download the corresponding osm file.
-
-.. code:: python
-
-    >>> import osm2gmns as og
-    # get relation id of a place of interest
-    # For the place of interest, e.g. Arizona State University
-    # e.g. "Tempe, Arizona, United States"
-    # e.g. "Arizona, US"
-    # e.g. "Beijing Jiaotong University, Beijing, China"
-    >>> rel_id = og.getOSMRelationID('Arizona State University')
-    >>> rel_id
-        Info: Found relation id 3444656 from web
-        Info: location of the place of interest:
-        {
-            "place_id": 318528634,
-            "licence": "Data \u00a9 OpenStreetMap contributors, ODbL 1.0. http://osm.org/copyright",
-            "osm_type": "relation",
-            "osm_id": 3444656,
-            "lat": "33.4213174",
-            "lon": "-111.93316305413154",
-            "class": "amenity",
-            "type": "university",
-            "place_rank": 30,
-            "importance": 0.5547365758311374,
-            "addresstype": "amenity",
-            "name": "Arizona State University",
-            "display_name": "Arizona State University, 1151, South Forest Avenue, Tempe Junction, Tempe, Maricopa County, Arizona, 85281, United States",
-            "boundingbox": [
-                "33.4102062",
-                "33.4329786",
-                "-111.9411651",
-                "-111.9092447"
-            ]
-        }
-    3444656
-
-    # download the corresponding osm file
-    >>> og.downloadOSMData(rel_id, 'asu.osm')
-
-
-Visualization
-====================================
-
-You can visualize generated networks using `NeXTA`_ or `QGIS`_.
-
-.. figure:: https://github.com/jiawlu/OSM2GMNS/blob/master/sample%20networks/Arizona%20State%20University%2C%20Tempe%20Campus/net_asu.png
-    :name: case_asu
-    :align: center
-    :width: 80%
-
-    Arizona State Unversity, Tempe Campus
-
-
-User's guide
-====================================
-You can check the `user's guide`_ for a detailed introduction of osm2gmns.
-
-
-.. _`OpenStreetMap`: https://www.openstreetmap.org
-.. _`GMNS`: https://github.com/zephyr-data-specs/GMNS
-.. _`paper link`: https://doi.org/10.1016/j.trc.2023.104223
-.. _`NeXTA`: https://github.com/asu-trans-ai-lab/NeXTA4GMNS
-.. _`QGIS`: https://qgis.org
-.. _`user's guide`: https://osm2gmns.readthedocs.io
+Metadata-Version: 2.1
+Name: osm2gmns
+Version: 0.7.6
+Summary: convert map data from OpenStreetMap to network files in GMNS format
+Home-page: https://github.com/jiawlu/OSM2GMNS
+Author: Jiawei Lu, Xuesong Zhou
+Author-email: jiaweil9@asu.edu, xzhou74@asu.edu
+License: GPLv3+
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.10
+Description-Content-Type: text/x-rst
+License-File: LICENSE
+Requires-Dist: numpy>=1.26.4
+Requires-Dist: osmium>=3.7.0
+Requires-Dist: pyufunc>=0.2.1
+Requires-Dist: Requests>=2.31.0
+Requires-Dist: setuptools>=68.2.2
+Requires-Dist: Shapely>=2.0.3
+Requires-Dist: matplotlib>=3.8.2
+
+osm2gmns
+====================================
+| **Authors**: Jiawei Lu, Xuesong (Simon) Zhou
+| **Email**: jiaweil9@asu.edu, xzhou74@asu.edu
+
+
+osm2gmns is an open-source Python package that enables users to conveniently obtain and
+manipulate any networks from OpenStreetMap (OSM). With a single line of Python code,
+users can obtain and model drivable, bikeable, walkable, railway, and aeroway networks
+for any region in the world and output networks to CSV files in GMNS format for seamless
+data sharing and research collaboration. osm2gmns mainly focuses on providing researchers and
+practitioners with flexible, standard and ready-to-use multi-modal transportation networks,
+as well as a bunch of customized and practical functions to facilitate various research
+and applications on traffic modeling.
+
+
+Publication
+====================================
+
+Lu, J., & Zhou, X.S. (2023). Virtual track networks: A hierarchical modeling framework and
+open-source tools for simplified and efficient connected and automated mobility (CAM) system
+design based on general modeling network specification (GMNS). Transportation Research
+Part C: Emerging Technologies, 153, 104223. `paper link`_
+
+
+Main Features
+====================================
+
+- Obtain any networks from OSM. osm2gmns parses map data from OSM and output networks to
+  csv files in GMNS format.
+- Standard network format. osm2gmns adopts GMNS as the network format for seamless data
+  sharing and research collaboration.
+- Ready-to-use network. osm2gmns cleans erroneous information from osm map data and is able
+  to fill up critical missing values, i.e., lanes, speed and capacity, to quickly provide
+  ready-to-use networks.
+- Directed network. two directed road links are generated for each bi-directional osm ways identified by osm2gmns
+- Multi-module support. five different network types are supported, including auto, bike, walk, railway, and aeroway
+- Customized and practical functions to facilitate traffic modeling. functions include
+  complex intersection consolidation, moevement generation, traffic zone creation, short link combination,
+  network visualization.
+- Multi-Resolution modeling. osm2gmns automatically construct the corresponding mesoscopic and microscopic
+  networks for any macroscopic network in GMNS format.
+
+
+Installation
+====================================
+
+.. code-block:: bash
+
+    pip install osm2gmns
+
+If you meet installation issues, please refer to the `user's guide`_ for solutions.
+
+
+Simple examples
+====================================
+
+You can find the osm map file used in the examples below at 'sample networks/Arizona State University, Tempe Campus'
+
+Quickly get the network with point of interest (POI) information from an osm file
+
+.. code:: python
+
+    >>> import osm2gmns as og
+    >>> net = og.getNetFromFile('asu.osm', POI=True)
+    >>> og.outputNetToCSV(net)
+
+Generate multi-resolution networks from an osm file
+
+.. code:: python
+
+    >>> import osm2gmns as og
+    >>> net = og.getNetFromFile('asu.osm')
+    >>> og.consolidateComplexIntersections(net, auto_identify=True)
+    >>> og.buildMultiResolutionNets(net)
+    >>> og.outputNetToCSV(net)
+
+
+Get relation id of a place of interest and download the corresponding osm file
+=====================================================================================================================
+You can use the following code to get the relation id of a place of interest and download the corresponding osm file.
+
+.. code:: python
+
+    >>> import osm2gmns as og
+    # get relation id of a place of interest
+    # For the place of interest, e.g. Arizona State University
+    # e.g. "Tempe, Arizona, United States"
+    # e.g. "Arizona, US"
+    # e.g. "Beijing Jiaotong University, Beijing, China"
+    >>> rel_id = og.getOSMRelationID('Arizona State University')
+    >>> rel_id
+        Info: Found relation id 3444656 from web
+        Info: location of the place of interest:
+        {
+            "place_id": 318528634,
+            "licence": "Data \u00a9 OpenStreetMap contributors, ODbL 1.0. http://osm.org/copyright",
+            "osm_type": "relation",
+            "osm_id": 3444656,
+            "lat": "33.4213174",
+            "lon": "-111.93316305413154",
+            "class": "amenity",
+            "type": "university",
+            "place_rank": 30,
+            "importance": 0.5547365758311374,
+            "addresstype": "amenity",
+            "name": "Arizona State University",
+            "display_name": "Arizona State University, 1151, South Forest Avenue, Tempe Junction, Tempe, Maricopa County, Arizona, 85281, United States",
+            "boundingbox": [
+                "33.4102062",
+                "33.4329786",
+                "-111.9411651",
+                "-111.9092447"
+            ]
+        }
+    3444656
+
+    # download the corresponding osm file
+    >>> og.downloadOSMData(rel_id, 'asu.osm')
+
+
+User's guide
+====================================
+You can check the `user's guide`_ for a detailed introduction of osm2gmns.
+
+
+.. _`OpenStreetMap`: https://www.openstreetmap.org
+.. _`GMNS`: https://github.com/zephyr-data-specs/GMNS
+.. _`paper link`: https://doi.org/10.1016/j.trc.2023.104223
+.. _`user's guide`: https://osm2gmns.readthedocs.io
```

### Comparing `osm2gmns-0.7.5/osm2gmns.egg-info/SOURCES.txt` & `osm2gmns-0.7.6/osm2gmns.egg-info/SOURCES.txt`

 * *Files identical despite different names*

