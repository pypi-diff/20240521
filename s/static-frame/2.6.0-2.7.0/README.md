# Comparing `tmp/static-frame-2.6.0.tar.gz` & `tmp/static-frame-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-2.6.0.tar", last modified: Sun Apr 14 21:01:15 2024, max compression
+gzip compressed data, was "static-frame-2.7.0.tar", last modified: Tue May 21 15:21:45 2024, max compression
```

## Comparing `static-frame-2.6.0.tar` & `static-frame-2.7.0.tar`

### file list

```diff
@@ -1,139 +1,139 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:01:15.174146 static-frame-2.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-14 21:00:37.000000 static-frame-2.6.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-14 21:00:37.000000 static-frame-2.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    21350 2024-04-14 21:01:15.174146 static-frame-2.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24088 2024-04-14 21:00:37.000000 static-frame-2.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-14 21:00:37.000000 static-frame-2.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-14 21:00:37.000000 static-frame-2.6.0/requirements-extras.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-14 21:00:37.000000 static-frame-2.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-14 21:01:15.174146 static-frame-2.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-14 21:00:37.000000 static-frame-2.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:01:15.150146 static-frame-2.6.0/static_frame/
--rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:01:15.162146 static-frame-2.6.0/static_frame/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45334 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/archive_npy.py
--rw-r--r--   0 runner    (1001) docker     (127)    22196 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/archive_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/axis_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    60237 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    53545 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/bus.py
--rw-r--r--   0 runner    (1001) docker     (127)    25063 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    74176 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/container_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    35749 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/display.py
--rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/display_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    17573 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/display_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/display_html_datatables.py
--rw-r--r--   0 runner    (1001) docker     (127)    15899 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/display_visidata.py
--rw-r--r--   0 runner    (1001) docker     (127)    30186 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/doc_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/fill_value_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)   389646 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/frame.py
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/generic_aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/hloc.py
--rw-r--r--   0 runner    (1001) docker     (127)    59388 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)    20628 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index_correspondence.py
--rw-r--r--   0 runner    (1001) docker     (127)    21797 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)   109246 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17248 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/index_hierarchy_set_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    50743 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/interface_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/join.py
--rw-r--r--   0 runner    (1001) docker     (127)    24238 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/loc_map.py
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/memory_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    36391 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_dt.py
--rw-r--r--   0 runner    (1001) docker     (127)    24378 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_fill_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    32552 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    14455 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_re.py
--rw-r--r--   0 runner    (1001) docker     (127)    21953 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)    34564 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_str.py
--rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_transpose.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/node_values.py
--rw-r--r--   0 runner    (1001) docker     (127)    32403 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/protocol_dfi.py
--rw-r--r--   0 runner    (1001) docker     (127)    17373 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/protocol_dfi_abc.py
--rw-r--r--   0 runner    (1001) docker     (127)    56284 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/quilt.py
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/rank.py
--rw-r--r--   0 runner    (1001) docker     (127)   130410 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/series.py
--rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_client_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     7273 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    26245 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (127)    21843 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/store_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/style_config.py
--rw-r--r--   0 runner    (1001) docker     (127)   182216 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/type_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    60093 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/type_clinic.py
--rw-r--r--   0 runner    (1001) docker     (127)   136804 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/www.py
--rw-r--r--   0 runner    (1001) docker     (127)    39939 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/core/yarn.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:01:15.162146 static-frame-2.6.0/static_frame/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13287 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:01:15.174146 static-frame-2.6.0/static_frame/test/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26053 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_archive_npy.py
--rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_archive_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_axis_map.py
--rw-r--r--   0 runner    (1001) docker     (127)   139072 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)    85364 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    37362 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_container_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_display.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_display_color.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_display_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_fill_value_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)   651135 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_frame_he.py
--rw-r--r--   0 runner    (1001) docker     (127)    60937 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_frame_iter.py
--rw-r--r--   0 runner    (1001) docker     (127)    31762 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_frame_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_frame_via_fill_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_frame_via_re.py
--rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_hloc.py
--rw-r--r--   0 runner    (1001) docker     (127)    66981 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index_correspondence.py
--rw-r--r--   0 runner    (1001) docker     (127)    41680 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index_datetime.py
--rw-r--r--   0 runner    (1001) docker     (127)   166603 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_index_hierarchy_set_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_loc_map.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_memory_measure.py
--rw-r--r--   0 runner    (1001) docker     (127)    22703 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_memory_measure_getsizeof.py
--rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_pivot.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_platform.py
--rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_protocol_dfi.py
--rw-r--r--   0 runner    (1001) docker     (127)    75455 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_quilt.py
--rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_rank.py
--rw-r--r--   0 runner    (1001) docker     (127)   251061 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_series.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_series_he.py
--rw-r--r--   0 runner    (1001) docker     (127)    13504 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_store_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_store_hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_store_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_store_xlsx.py
--rw-r--r--   0 runner    (1001) docker     (127)    17427 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_store_zip.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_style_config.py
--rw-r--r--   0 runner    (1001) docker     (127)   161671 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_type_blocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    69155 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_type_clinic.py
--rw-r--r--   0 runner    (1001) docker     (127)   119583 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11883 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_www.py
--rw-r--r--   0 runner    (1001) docker     (127)    66889 2024-04-14 21:00:37.000000 static-frame-2.6.0/static_frame/test/unit/test_yarn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 21:01:15.150146 static-frame-2.6.0/static_frame.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21350 2024-04-14 21:01:15.000000 static-frame-2.6.0/static_frame.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-04-14 21:01:15.000000 static-frame-2.6.0/static_frame.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 21:01:15.000000 static-frame-2.6.0/static_frame.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-14 21:01:15.000000 static-frame-2.6.0/static_frame.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-14 21:01:15.000000 static-frame-2.6.0/static_frame.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:21:45.943434 static-frame-2.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-05-21 15:21:10.000000 static-frame-2.7.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 15:21:10.000000 static-frame-2.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    21350 2024-05-21 15:21:45.947435 static-frame-2.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24088 2024-05-21 15:21:10.000000 static-frame-2.7.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-21 15:21:10.000000 static-frame-2.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-21 15:21:10.000000 static-frame-2.7.0/requirements-extras.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 15:21:10.000000 static-frame-2.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-21 15:21:45.947435 static-frame-2.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-21 15:21:10.000000 static-frame-2.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:21:45.919434 static-frame-2.7.0/static_frame/
+-rw-r--r--   0 runner    (1001) docker     (127)     9748 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:21:45.935434 static-frame-2.7.0/static_frame/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45334 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/archive_npy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22196 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/archive_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/axis_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60237 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53545 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25063 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74176 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/container_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35758 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9277 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/display_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17573 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/display_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/display_html_datatables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15899 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/display_visidata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30186 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/doc_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/fill_value_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)   389738 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/generic_aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/hloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59424 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6612 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/index_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20628 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/index_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5733 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/index_correspondence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21797 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/index_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)   109246 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/index_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17248 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/index_hierarchy_set_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50743 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/interface_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11015 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/join.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24238 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/loc_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/memory_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6098 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36391 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/node_dt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24378 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/node_fill_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5277 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/node_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32552 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/node_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14455 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/node_re.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21953 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/node_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34564 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/node_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15526 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/node_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/node_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32403 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12060 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/protocol_dfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17373 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/protocol_dfi_abc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56284 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/quilt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130410 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/series.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10614 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6343 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/store_client_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15234 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/store_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/store_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6162 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/store_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7273 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/store_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26350 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/store_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21843 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/store_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5195 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/style_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182216 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/type_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64290 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/type_clinic.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136804 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10515 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/www.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39939 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/core/yarn.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:21:45.935434 static-frame-2.7.0/static_frame/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13151 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:21:45.943434 static-frame-2.7.0/static_frame/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26053 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_archive_npy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7252 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_archive_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7427 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_axis_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139072 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85364 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37362 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_container_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36791 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_display.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_display_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_display_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5295 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_fill_value_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)   651135 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_frame_he.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60937 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_frame_iter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31762 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_frame_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_frame_via_fill_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5058 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_frame_via_re.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2353 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_hloc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66981 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3997 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_index_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_index_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_index_correspondence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41680 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_index_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (127)   166603 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_index_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_index_hierarchy_set_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6655 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19814 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_loc_map.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_memory_measure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22703 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_memory_measure_getsizeof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4639 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4491 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_pivot.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_platform.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15289 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_protocol_dfi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75455 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_quilt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11299 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_rank.py
+-rw-r--r--   0 runner    (1001) docker     (127)   251061 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_series_he.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13504 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14542 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_store_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7493 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_store_hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8261 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_store_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16051 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_store_xlsx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17427 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_store_zip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_style_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)   161671 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_type_blocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80504 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_type_clinic.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119583 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11883 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_www.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66889 2024-05-21 15:21:10.000000 static-frame-2.7.0/static_frame/test/unit/test_yarn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 15:21:45.919434 static-frame-2.7.0/static_frame.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21350 2024-05-21 15:21:45.000000 static-frame-2.7.0/static_frame.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-05-21 15:21:45.000000 static-frame-2.7.0/static_frame.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 15:21:45.000000 static-frame-2.7.0/static_frame.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-21 15:21:45.000000 static-frame-2.7.0/static_frame.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 15:21:45.000000 static-frame-2.7.0/static_frame.egg-info/top_level.txt
```

### Comparing `static-frame-2.6.0/LICENSE.txt` & `static-frame-2.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/PKG-INFO` & `static-frame-2.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 2.6.0
+Version: 2.7.0
 Summary: Immutable and statically-typeable DataFrames with runtime type and data validation.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Keywords: staticframe pandas numpy immutable array
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `static-frame-2.6.0/README.rst` & `static-frame-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/pyproject.toml` & `static-frame-2.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/setup.py` & `static-frame-2.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/__init__.py` & `static-frame-2.7.0/static_frame/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,8 +131,8 @@
 from static_frame.core.util import TLocSelectorCompound as TLocSelectorCompound
 from static_frame.core.util import TPathSpecifierOrBinaryIO as TPathSpecifierOrBinaryIO
 from static_frame.core.util import TPathSpecifierOrTextIO as TPathSpecifierOrTextIO
 from static_frame.core.util import TSeriesInitializer as TSeriesInitializer
 from static_frame.core.www import WWW as WWW
 from static_frame.core.yarn import Yarn as Yarn
 
-__version__ = '2.6.0'
+__version__ = '2.7.0'
```

### Comparing `static-frame-2.6.0/static_frame/__main__.py` & `static-frame-2.7.0/static_frame/__main__.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/archive_npy.py` & `static-frame-2.7.0/static_frame/core/archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/archive_zip.py` & `static-frame-2.7.0/static_frame/core/archive_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/axis_map.py` & `static-frame-2.7.0/static_frame/core/axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/batch.py` & `static-frame-2.7.0/static_frame/core/batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/bus.py` & `static-frame-2.7.0/static_frame/core/bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/container.py` & `static-frame-2.7.0/static_frame/core/container.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/container_util.py` & `static-frame-2.7.0/static_frame/core/container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/display.py` & `static-frame-2.7.0/static_frame/core/display.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,15 +314,15 @@
     CELL_EMPTY = DisplayCell(FORMAT_EMPTY, '')
     ELLIPSIS = '...' # this string is appended to truncated entries
     CELL_ELLIPSIS = DisplayCell(FORMAT_EMPTY, ELLIPSIS)
     ELLIPSIS_CENTER_SENTINEL = object()
     ANSI_ESCAPE = re.compile(
             r'\x1B'
             r'\['
-            r'(\d{1,2}(;\d{1,2})*)?' # Optional numeric codes separated by ;
+            r'(\d{1,3}(;\d{1,3})*)?' # Optional numeric codes separated by ;
             r'[A-Za-z]' # Letter indicating the type of code; most often "m" for colors
             )
 
 
     #---------------------------------------------------------------------------
     # utility methods
 
@@ -330,15 +330,15 @@
     def type_attributes(
             type_input: THeaderSpecifier,
             config: DisplayConfig
             ) -> tp.Tuple[str, tp.Type[DisplayTypeCategory]]:
         '''
         Return the `type_input` as a string, applying delimters to either numpy dtypes or Python classes.
         '''
-        type_ref: THeaderSpecifier
+        type_ref: tp.Union[type, TDtypeAny]
         if isinstance(type_input, np.dtype):
             type_str = str(type_input)
             type_ref = type_input
         elif isinstance(type_input, DisplayHeader):
             type_str = repr(type_input)
             type_ref = type_input.cls
         elif inspect.isclass(type_input):
```

### Comparing `static-frame-2.6.0/static_frame/core/display_color.py` & `static-frame-2.7.0/static_frame/core/display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/display_config.py` & `static-frame-2.7.0/static_frame/core/display_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/display_html_datatables.py` & `static-frame-2.7.0/static_frame/core/display_html_datatables.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/display_visidata.py` & `static-frame-2.7.0/static_frame/core/display_visidata.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/doc_str.py` & `static-frame-2.7.0/static_frame/core/doc_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/exception.py` & `static-frame-2.7.0/static_frame/core/exception.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/fill_value_auto.py` & `static-frame-2.7.0/static_frame/core/fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/frame.py` & `static-frame-2.7.0/static_frame/core/frame.py`

 * *Files 0% similar despite different names*

```diff
@@ -5200,30 +5200,33 @@
         '''
         if isinstance(key, tuple):
             r, c = key
             return self._extract(r, c)
         return self._extract(key)
 
     def _compound_loc_to_iloc(self,
-            key: TLocSelectorCompound) -> TILocSelectorCompound:
+            key: TLocSelectorCompound,
+            # ) -> TILocSelectorCompound:
+            ) -> tp.Tuple[TILocSelector, TILocSelector]:
         '''
         Given a compound iloc key, return a tuple of row, column keys. Assumes the first argument is always a row extractor.
         '''
         if isinstance(key, tuple):
             loc_row_key, loc_column_key = key # pyright: ignore
             iloc_column_key = self._columns._loc_to_iloc(loc_column_key)
         else:
             loc_row_key = key
             iloc_column_key = None
 
         iloc_row_key = self._index._loc_to_iloc(loc_row_key)
         return iloc_row_key, iloc_column_key
 
     def _extract_loc(self, key: TLocSelectorCompound) -> tp.Any:
-        return self._extract(*self._compound_loc_to_iloc(key))
+        r, c = self._compound_loc_to_iloc(key)
+        return self._extract(r, c)
 
     def _extract_loc_columns(self, key: TLocSelector) -> TFrameOrSeries:
         '''Alternate extract of a columns only selection.
         '''
         return self._extract(None,
                 self._columns._loc_to_iloc(key),
                 )
```

### Comparing `static-frame-2.6.0/static_frame/core/generic_aliases.py` & `static-frame-2.7.0/static_frame/core/generic_aliases.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/hloc.py` & `static-frame-2.7.0/static_frame/core/hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/index.py` & `static-frame-2.7.0/static_frame/core/index.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,25 +341,26 @@
             # coerce to target type
             elif labels.dtype != dtype_extract: #type: ignore
                 labels = labels.astype(dtype_extract) #type: ignore
                 labels.flags.writeable = False
 
         self._name = None if name is NAME_DEFAULT else name_filter(name) # pyright: ignore
 
+        size: int
         if self._map is None: # if _map not shared from another Index
             if not loc_is_iloc:
                 if isinstance(labels, str):
                     # NOTE: this is necessary as otherwise a malformed Index will be created, whereby the _map will treat the string as an iterable of chars, while the labels will not and have a single string value. This is consisten as other elements (ints, Booleans) are rejected on instantiation of the AutoMap
                     raise ErrorInitIndex('Cannot create an Index from a single string; provide an iterable of strings.')
                 try:
                     self._map = FrozenAutoMap(labels) if self.STATIC else AutoMap(labels)
                 except NonUniqueError: # Automap will raise ValueError of non-unique values are encountered
                     raise self._error_init_index_non_unique(labels) from None
                 # must take length after map as might be iterator
-                size = len(self._map)
+                size = len(self._map) # pyright: ignore
             else:
                 # if loc_is_iloc, labels must be positions and we assume that internal clients that provided loc_is_iloc will not give a generator
                 size = len(labels) #type: ignore
                 if positions is None:
                     positions = labels # type: ignore
         else: # map shared from another Index
             size = len(self._map)
```

### Comparing `static-frame-2.6.0/static_frame/core/index_auto.py` & `static-frame-2.7.0/static_frame/core/index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/index_base.py` & `static-frame-2.7.0/static_frame/core/index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/index_correspondence.py` & `static-frame-2.7.0/static_frame/core/index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/index_datetime.py` & `static-frame-2.7.0/static_frame/core/index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/index_hierarchy.py` & `static-frame-2.7.0/static_frame/core/index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/index_hierarchy_set_utils.py` & `static-frame-2.7.0/static_frame/core/index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/interface.py` & `static-frame-2.7.0/static_frame/core/interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/interface_meta.py` & `static-frame-2.7.0/static_frame/core/interface_meta.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/join.py` & `static-frame-2.7.0/static_frame/core/join.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/loc_map.py` & `static-frame-2.7.0/static_frame/core/loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/memory_measure.py` & `static-frame-2.7.0/static_frame/core/memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/metadata.py` & `static-frame-2.7.0/static_frame/core/metadata.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/node_dt.py` & `static-frame-2.7.0/static_frame/core/node_dt.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/node_fill_value.py` & `static-frame-2.7.0/static_frame/core/node_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/node_hashlib.py` & `static-frame-2.7.0/static_frame/core/node_hashlib.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/node_iter.py` & `static-frame-2.7.0/static_frame/core/node_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/node_re.py` & `static-frame-2.7.0/static_frame/core/node_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/node_selector.py` & `static-frame-2.7.0/static_frame/core/node_selector.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/node_str.py` & `static-frame-2.7.0/static_frame/core/node_str.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/node_transpose.py` & `static-frame-2.7.0/static_frame/core/node_transpose.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/node_values.py` & `static-frame-2.7.0/static_frame/core/node_values.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/pivot.py` & `static-frame-2.7.0/static_frame/core/pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/platform.py` & `static-frame-2.7.0/static_frame/core/platform.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/protocol_dfi.py` & `static-frame-2.7.0/static_frame/core/protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/protocol_dfi_abc.py` & `static-frame-2.7.0/static_frame/core/protocol_dfi_abc.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/quilt.py` & `static-frame-2.7.0/static_frame/core/quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/rank.py` & `static-frame-2.7.0/static_frame/core/rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/series.py` & `static-frame-2.7.0/static_frame/core/series.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/store.py` & `static-frame-2.7.0/static_frame/core/store.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/store_client_mixin.py` & `static-frame-2.7.0/static_frame/core/store_client_mixin.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/store_config.py` & `static-frame-2.7.0/static_frame/core/store_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/store_filter.py` & `static-frame-2.7.0/static_frame/core/store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/store_hdf5.py` & `static-frame-2.7.0/static_frame/core/store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/store_sqlite.py` & `static-frame-2.7.0/static_frame/core/store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/store_xlsx.py` & `static-frame-2.7.0/static_frame/core/store_xlsx.py`

 * *Files 2% similar despite different names*

```diff
@@ -409,35 +409,35 @@
                 ws = wb[wb.sheetnames[0]] # pyright: ignore
                 name = None # do not set to default sheet name
             else:
                 label_encoded = config_map.default.label_encode(label)
                 ws = wb[label_encoded] # pyright: ignore
                 name = label # set name to the un-encoded hashable
 
-            if ws.max_column <= 1 or ws.max_row <= 1:
+            if ws.max_column <= 1 or ws.max_row <= 1: # pyright: ignore
                 # https://openpyxl.readthedocs.io/en/stable/optimized.html
                 # says that some clients might not report correct dimensions
-                ws.calculate_dimension()
+                ws.calculate_dimension() # pyright: ignore
 
-            max_column = ws.max_column
-            max_row = ws.max_row
+            max_column: int = ws.max_column # pyright: ignore
+            max_row: int = ws.max_row # pyright: ignore
 
             # adjust for downward shift for skipping header, then reduce for footer; at this value and beyond we stop
-            last_row_count = max_row - skip_header - skip_footer
+            last_row_count: int = max_row - skip_header - skip_footer
 
             index_values: tp.List[tp.Any] = []
             columns_values: tp.List[tp.Any] = []
             data = []
             apex_rows = []
 
             if trim_nadir:
                 mask = np.full((last_row_count, max_column), False)
 
             for row_count, row in enumerate(
-                    ws.iter_rows(max_row=max_row), start=-skip_header):
+                    ws.iter_rows(max_row=max_row), start=-skip_header): # pyright: ignore
                 if row_count < 0:
                     continue # due to skip header; preserves comparison to columns_depth
                 if row_count >= last_row_count:
                     break
 
                 if trim_nadir:
                     row_data: tp.Sequence[tp.Any] = []
```

### Comparing `static-frame-2.6.0/static_frame/core/store_zip.py` & `static-frame-2.7.0/static_frame/core/store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/style_config.py` & `static-frame-2.7.0/static_frame/core/style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/type_blocks.py` & `static-frame-2.7.0/static_frame/core/type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/type_clinic.py` & `static-frame-2.7.0/static_frame/core/type_clinic.py`

 * *Files 4% similar despite different names*

```diff
@@ -124,18 +124,28 @@
             if hasattr(origin, '__name__'):
                 name = origin.__name__
             elif is_unpack(origin, v): # needed for backwards compat
                 name = 'Unpack'
             else:
                 name = str(origin)
         s = f'{name}[{", ".join(to_name(q) for q in tp.get_args(v))}]'
+    elif isinstance(v, tp.TypeVar):
+        # str() gets tilde, __name__ does not have tilde
+        if v.__bound__:
+            s = f'{v}: {to_name(v.__bound__)}'
+        elif v.__constraints__:
+            s = f'{v}: {to_name(v.__constraints__)}'
+        else:
+            s = str(v)
     elif hasattr(v, '__name__'):
         s = v.__name__
     elif v is ...:
         s = '...'
+    elif isinstance(v, tuple):
+        s = f"({', '.join(to_name(w) for w in v)})"
     else:
         s = func_to_str(v)
     return s
 
 def to_signature(
         sig: BoundArguments,
         hints: tp.Mapping[str, tp.Any]) -> str:
@@ -701,14 +711,88 @@
             if not bool(post):
                 yield (ERROR_MESSAGE_TYPE,
                         f'{to_name(type(value))} failed validation with {self._prepare_callable(self._func)}', parent_hints,
                         parent_values,
                         )
 
 #-------------------------------------------------------------------------------
+
+def _value_to_hint(value: tp.Any) -> tp.Any: # tp._GenericAlias
+    if isinstance(value, type):
+        return tp.Type[value]
+
+    if isinstance(value, tuple):
+        return value.__class__.__class_getitem__(tuple(_value_to_hint(v) for v in value))
+
+    if isinstance(value, Sequence) and not isinstance(value, str):
+        if not len(value):
+            return value.__class__.__class_getitem__(tp.Any) # type: ignore[attr-defined]
+
+        # as classes may not be hashable, we key to string name to from a set; this is imperfect
+        ut = {v.__class__.__name__: v.__class__ for v in value}
+        if len(ut) == 1:
+            return value.__class__.__class_getitem__(ut[next(iter(ut.keys()))]) # type: ignore[attr-defined]
+
+        hu = tp.Union.__getitem__(tuple(ut.values())) # pyright: ignore
+        return value.__class__.__class_getitem__(hu) # type: ignore[attr-defined]
+
+    if isinstance(value, MutableMapping):
+        if not len(value):
+            return value.__class__.__class_getitem__((tp.Any, tp.Any)) # type: ignore[attr-defined]
+
+        keys_ut = {k.__class__.__name__: k.__class__ for k in value.keys()}
+        values_ut = {v.__class__.__name__: v.__class__ for v in value.values()}
+
+        if len(keys_ut) == 1:
+            kt = keys_ut[next(iter(keys_ut.keys()))]
+        else:
+            kt = tp.Union.__getitem__(tuple(keys_ut.values())) # pyright: ignore
+
+        if len(values_ut) == 1:
+            vt = values_ut[next(iter(values_ut.keys()))]
+        else:
+            vt = tp.Union.__getitem__(tuple(values_ut.values())) # pyright: ignore
+
+        return value.__class__.__class_getitem__((kt, vt)) # type: ignore[attr-defined]
+
+    # --------------------------------------------------------------------------
+    # SF containers
+
+    if isinstance(value, Frame):
+        hints = [_value_to_hint(value.index), _value_to_hint(value.columns)]
+        hints.extend(dt.type().__class__ for dt in value._blocks._iter_dtypes())
+        return value.__class__.__class_getitem__(tuple(hints)) # type: ignore
+
+    if isinstance(value, Series):
+        return value.__class__[_value_to_hint(value.index), value.dtype.type().__class__] # type: ignore
+
+    # must come before index
+    if isinstance(value, IndexDatetime):
+        return value.__class__
+
+    if isinstance(value, Index):
+        return value.__class__[value.dtype.type().__class__] # type: ignore
+
+    if isinstance(value, IndexHierarchy):
+        hints = list(_value_to_hint(value.index_at_depth(i)) for i in range(value.depth))
+        return value.__class__.__class_getitem__(tuple(hints)) # type: ignore
+
+    if isinstance(value, (Bus, Yarn)):
+        return value.__class__[_value_to_hint(value.index)] # type: ignore
+
+
+    if isinstance(value, np.dtype):
+        return np.dtype.__class_getitem__(value.type().__class__)
+
+    if isinstance(value, np.ndarray):
+        return value.__class__.__class_getitem__(_value_to_hint(value.dtype))
+
+    return value.__class__
+
+#-------------------------------------------------------------------------------
 # handlers for getting components out of generics
 
 def iter_sequence_checks(
         value: tp.Any,
         hint: tp.Any,
         parent_hints: TParent,
         parent_values: TParent,
@@ -758,15 +842,15 @@
     for v, h in chain(
             zip(value.keys(), repeat(h_keys)),
             zip(value.values(), repeat(h_values)),
             ):
         yield v, h, parent_hints, pv_next
 
 
-def iter_typeddict(
+def iter_typeddict_checks(
         value: tp.Any,
         hint: tp.Any,
         parent_hints: TParent,
         parent_values: TParent,
         ) -> tp.Iterable[TValidation]:
 
     # hint is a typedict class; returns dict of key name and value
@@ -1120,18 +1204,103 @@
         if value.dtype.kind == DTYPE_COMPLEX_KIND:
             # complex is represented with two hints, each half of the whole itemsize; adjust value bits and let each side check independently
             yield v_bits // 2, BIT_TO_LITERAL[h_bits], parent_hints, pv_next
         else:
             yield v_bits, BIT_TO_LITERAL[h_bits], parent_hints, pv_next
 
 #-------------------------------------------------------------------------------
+class TypeVarState:
+    __slots__ = (
+            '_var',
+            '_value',
+            '_bound',
+            '_bound_unset',
+            '_is_bound_union',
+            )
+
+    def __init__(self, var: tp.Any, value: tp.Any):
+        '''Provide `TypeVar` and and the first-encountered value for that `TypeVar`
+        '''
+        self._var = var
+        self._value = value
+        # as bounds might have unions that need specialization, we store the current bound type here and update it if needed
+        self._bound = var.__bound__ # might be None
+        if self._bound is not None and is_union(self._bound):
+            self._is_bound_union = True
+            self._bound_unset = set(range(len(tp.get_args(self._bound))))
+        else:
+            self._is_bound_union = False
+
+    @property
+    def is_bound_union(self) -> bool:
+        return self._is_bound_union
+
+    def _specialize_bound_union(self,
+            value: tp.Any,
+            ) -> None:
+        '''If `hint` is a Union, given value that is assigned to the type var, find value in the Union and replace that hint with the hint of the value.
+        '''
+        components = list(tp.get_args(self._bound))
+        # NOTE: this refence to a set is mutated inplace
+        for i, hint in enumerate(components):
+            if i in self._bound_unset and _check(value, hint).validated:
+                components[i] = _value_to_hint(value)
+                self._bound_unset.discard(i)
+        self._bound = tp.Union.__getitem__(tuple(components)) # pyright: ignore
+
+
+    @property
+    def constraints(self) -> tp.Any:
+        return self._var.__constraints__
+
+    def get_hint(self, value: tp.Any) -> tp.Any:
+        '''Return a hint from derived from the stored value. If this is a bound union, the value is used to specialize the union.
+        '''
+        if self.is_bound_union:
+            self._specialize_bound_union(value)
+            return self._bound
+
+        return _value_to_hint(self._value) # this could be stored on init
+
+
+class TypeVarRegistry:
+    __slots__ = (
+            '_id_to_var',
+            )
+    _id_to_var: tp.Dict[tp.TypeVar, TypeVarState]
+
+    def __init__(self) -> None:
+        self._id_to_var = dict()
+
+    def iter_checks(self,
+            value: tp.Any,
+            var: tp.TypeVar,
+            parent_hints: TParent,
+            parent_values: TParent,
+            ) -> tp.Iterator[TValidation]:
+
+        pv_next = parent_values + (value,)
+
+        if var not in self._id_to_var:
+            tvs = TypeVarState(var, value)
+            self._id_to_var[var] = tvs
+            if hints := tvs.constraints:
+                # with constratings we select one option and use it for the life of the Typevar; on the first value, check that the value meets the constraints (recast as a uion); subsequent checks will be based on the stored value
+                yield value, tp.Union.__getitem__(hints), parent_hints, pv_next # pyright: ignore
+        else:
+            tvs = self._id_to_var[var]
+
+        yield value, tvs.get_hint(value), parent_hints, pv_next
+
+#-------------------------------------------------------------------------------
 
 def _check(
         value: tp.Any,
         hint: tp.Any,
+        tvr: tp.Optional[TypeVarRegistry] = None,
         parent_hints: TParent = (),
         parent_values: TParent = (),
         fail_fast: bool = False,
         ) -> ClinicResult:
 
     # Check queue: queue all checks
     q = deque(((value, hint, parent_hints, parent_values),))
@@ -1149,34 +1318,41 @@
     while q:
         if fail_fast and e_log:
             return ClinicResult(e_log)
 
         v, h, ph, pv = q.popleft()
         # an ERROR_MESSAGE_TYPE should only be used as a place holder in error logs, not queued checks
         assert v is not ERROR_MESSAGE_TYPE
+        # print(v, h, ph, pv)
 
         if h is tp.Any:
             continue
 
         ph_next = ph + (h,)
         if is_union(h):
             # NOTE: must check union types first as tp.Union matches as generic type
             u_log: tp.List[TValidation] = []
             for c_hint in tp.get_args(h): # get components
                 # handing one pair at a time with a secondary call will allow nested types in the union to be evaluated on their own
-                c_log = _check(v, c_hint, ph_next, pv, fail_fast)
+                c_log = _check(v, c_hint, tvr, ph_next, pv, fail_fast)
                 if not c_log: # no error found, can exit
                     break
                 u_log.extend(c_log)
             else: # no breaks, so no matches within union
                 e_log.extend(u_log)
 
         elif isinstance(h, Validator):
             e_log.extend(h._iter_errors(v, h, ph_next, pv))
 
+        elif isinstance(h, tp.TypeVar):
+            if tvr is not None:
+                tee_error_or_check(tvr.iter_checks(v, h, ph_next, pv))
+            else: # ignore typevar
+                continue
+
         elif is_generic(h):
             origin = tp.get_origin(h)
 
             if origin is type: # a tp.Type[x] generic
                 [t] = tp.get_args(h)
                 try: # the v should be a subclass of t
                     t_check = issubclass(t, v)
@@ -1190,18 +1366,18 @@
                 h_type, *h_annotations = tp.get_args(h)
                 # perform the un-annotated check
                 q.append((v, h_type, ph_next, pv))
                 for h_annotation in h_annotations:
                     if isinstance(h_annotation, Validator):
                         q.append((v, h_annotation, ph_next, pv))
 
-            elif origin == tp.Literal: # NOTE: cannot use is due backwards compat
+            elif origin == tp.Literal: # NOTE: cannot use `is` due backwards compat
                 l_log: tp.List[TValidation] = []
                 for l_hint in tp.get_args(h): # get components
-                    c_log = _check(v, l_hint, ph_next, pv, fail_fast)
+                    c_log = _check(v, l_hint, tvr, ph_next, pv, fail_fast)
                     if not c_log: # no error found, can exit
                         break
                     l_log.extend(c_log)
                 else: # no breaks, so no matches within literal
                     e_log.extend(l_log)
 
             elif origin == tp.Required or origin == tp.NotRequired:
@@ -1240,15 +1416,15 @@
                 elif isinstance(v, np.dtype):
                     tee_error_or_check(iter_dtype_checks(v, h, ph_next, pv))
                 elif isinstance(v, np.generic):
                     tee_error_or_check(iter_np_generic_checks(v, h, ph_next, pv))
                 else:
                     raise NotImplementedError(f'no handling for generic {origin}') #pragma: no cover
         elif tp.is_typeddict(h):
-            tee_error_or_check(iter_typeddict(v, h, ph_next, pv))
+            tee_error_or_check(iter_typeddict_checks(v, h, ph_next, pv))
 
         elif not isinstance(h, type): # h is a value from a literal
             # must check type: https://peps.python.org/pep-0586/#equivalence-of-two-literals
             if type(v) != type(h) or v != h: # pylint: disable=C0123
                 e_log.append((v, h, ph, pv))
 
         # h is a class
@@ -1268,87 +1444,14 @@
             e_log.append((v, h, ph, pv))
 
     return ClinicResult(e_log)
 
 #-------------------------------------------------------------------------------
 # public interfaces
 
-def _value_to_hint(value: tp.Any) -> tp.Any: # tp._GenericAlias
-    if isinstance(value, type):
-        return tp.Type[value]
-
-    if isinstance(value, tuple):
-        return value.__class__.__class_getitem__(tuple(_value_to_hint(v) for v in value))
-
-    if isinstance(value, Sequence) and not isinstance(value, str):
-        if not len(value):
-            return value.__class__.__class_getitem__(tp.Any) # type: ignore[attr-defined]
-
-        # as classes may not be hashable, we key to string name to from a set; this is imperfect
-        ut = {v.__class__.__name__: v.__class__ for v in value}
-        if len(ut) == 1:
-            return value.__class__.__class_getitem__(ut[next(iter(ut.keys()))]) # type: ignore[attr-defined]
-
-        hu = tp.Union.__getitem__(tuple(ut.values())) # pyright: ignore
-        return value.__class__.__class_getitem__(hu) # type: ignore[attr-defined]
-
-    if isinstance(value, MutableMapping):
-        if not len(value):
-            return value.__class__.__class_getitem__((tp.Any, tp.Any)) # type: ignore[attr-defined]
-
-        keys_ut = {k.__class__.__name__: k.__class__ for k in value.keys()}
-        values_ut = {v.__class__.__name__: v.__class__ for v in value.values()}
-
-        if len(keys_ut) == 1:
-            kt = keys_ut[next(iter(keys_ut.keys()))]
-        else:
-            kt = tp.Union.__getitem__(tuple(keys_ut.values())) # pyright: ignore
-
-        if len(values_ut) == 1:
-            vt = values_ut[next(iter(values_ut.keys()))]
-        else:
-            vt = tp.Union.__getitem__(tuple(values_ut.values())) # pyright: ignore
-
-        return value.__class__.__class_getitem__((kt, vt)) # type: ignore[attr-defined]
-
-    # --------------------------------------------------------------------------
-    # SF containers
-
-    if isinstance(value, Frame):
-        hints = [_value_to_hint(value.index), _value_to_hint(value.columns)]
-        hints.extend(dt.type().__class__ for dt in value._blocks._iter_dtypes())
-        return value.__class__.__class_getitem__(tuple(hints)) # type: ignore
-
-    if isinstance(value, Series):
-        return value.__class__[_value_to_hint(value.index), value.dtype.type().__class__] # type: ignore
-
-    # must come before index
-    if isinstance(value, IndexDatetime):
-        return value.__class__
-
-    if isinstance(value, Index):
-        return value.__class__[value.dtype.type().__class__] # type: ignore
-
-    if isinstance(value, IndexHierarchy):
-        hints = list(_value_to_hint(value.index_at_depth(i)) for i in range(value.depth))
-        return value.__class__.__class_getitem__(tuple(hints)) # type: ignore
-
-    if isinstance(value, (Bus, Yarn)):
-        return value.__class__[_value_to_hint(value.index)] # type: ignore
-
-
-    if isinstance(value, np.dtype):
-        return np.dtype.__class_getitem__(value.type().__class__)
-
-    if isinstance(value, np.ndarray):
-        return value.__class__.__class_getitem__(_value_to_hint(value.dtype))
-
-    return value.__class__
-
-
 class TypeClinic:
     '''A ``TypeClinic`` instance, created from (almost) any object, can be used to derive a type hint (or type hint string), or test the object against a provided hint.
     '''
 
     __slots__ = ('_value',)
 
     _INTERFACE = (
@@ -1408,16 +1511,17 @@
             fail_fast: bool = False,
             ) -> ClinicResult:
         '''Given a hint (a type and/or generic alias), return a ``ClinicResult`` object describing the result of the check.
 
         Args:
             fail_fast: If True, return on first failure. If False, all failures are discovered and reported.
         '''
-        return _check(self._value, hint, fail_fast=fail_fast)
-
+        tvr = TypeVarRegistry()
+        post = _check(self._value, hint, tvr, fail_fast=fail_fast)
+        return post
 
 
 class ErrorAction(Enum):
     RAISE = 0
     WARN = 1
     RETURN = 2
 
@@ -1435,29 +1539,34 @@
     sig = Signature.from_callable(func)
     sig_bound = sig.bind(*args, **kwargs)
     sig_bound.apply_defaults()
     sig_str = to_signature(sig_bound, hints)
     parent_hints = (f'args of {sig_str}',)
     parent_values = (func,)
 
+    # NOTE: we create one TV registry per check, so state associated with typevars will be bound by the context of one function
+    tvr = TypeVarRegistry()
+
     for k, v in sig_bound.arguments.items():
         if h_p := hints.get(k, None):
-            if cr := _check(v, h_p, parent_hints, parent_values, fail_fast=fail_fast):
+            arg_hints = parent_hints + (f'In arg {k}',)
+            if cr := _check(v, h_p, tvr, arg_hints, parent_values, fail_fast=fail_fast):
                 if error_action is ErrorAction.RAISE:
                     raise ClinicError(cr)
                 elif error_action is ErrorAction.WARN:
                     warnings.warn(cr.to_str(), category)
                 elif error_action is ErrorAction.RETURN:
                     return cr
 
     post = func(*args, **kwargs)
 
     if h_return := hints.get('return', None):
         if cr := _check(post,
                 h_return,
+                tvr,
                 (f'return of {sig_str}',),
                 parent_values,
                 fail_fast=fail_fast,
                 ):
             if error_action is ErrorAction.RAISE:
                 raise ClinicError(cr)
             elif error_action is ErrorAction.WARN:
@@ -1472,15 +1581,15 @@
 
 class CallGuard:
     '''A family of decorators for run-time type checking and data validation of functions.
     '''
 
     @tp.overload
     @staticmethod
-    def check(func: TVFunc) -> TVFunc: ...
+    def check(func: TVFunc, /) -> TVFunc: ...
 
     @tp.overload
     @staticmethod
     def check(*, fail_fast: bool) -> tp.Callable[[TVFunc], TVFunc]: ...
 
     @tp.overload
     @staticmethod
@@ -1508,15 +1617,15 @@
         if func is not None:
             return decorator(func)
         return decorator
 
 
     @tp.overload
     @staticmethod
-    def warn(func: TVFunc) -> TVFunc: ...
+    def warn(func: TVFunc, /) -> TVFunc: ...
 
     @tp.overload
     @staticmethod
     def warn(*, fail_fast: bool, category: tp.Type[Warning]) -> tp.Callable[[TVFunc], TVFunc]: ...
 
     @tp.overload
     @staticmethod
```

### Comparing `static-frame-2.6.0/static_frame/core/util.py` & `static-frame-2.7.0/static_frame/core/util.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/www.py` & `static-frame-2.7.0/static_frame/core/www.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/core/yarn.py` & `static-frame-2.7.0/static_frame/core/yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/test_case.py` & `static-frame-2.7.0/static_frame/test/test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,20 +65,14 @@
         )
 
 skip_pyle310 = pytest.mark.skipif(
         sys.version_info[:2] <= (3, 10),
         reason='Python less than or equal to 3.10'
         )
 
-skip_pyle38 = pytest.mark.skipif(
-        sys.version_info[:2] <= (3, 8),
-        reason='Python less than or equal to 3.8'
-        )
-
-
 #-------------------------------------------------------------------------------
 class Timer():
 
     def __init__(self, label: str = ''):
         self._start = time.time()
         self._label = label
```

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_archive_npy.py` & `static-frame-2.7.0/static_frame/test/unit/test_archive_npy.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_archive_zip.py` & `static-frame-2.7.0/static_frame/test/unit/test_archive_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_axis_map.py` & `static-frame-2.7.0/static_frame/test/unit/test_axis_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_batch.py` & `static-frame-2.7.0/static_frame/test/unit/test_batch.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_bus.py` & `static-frame-2.7.0/static_frame/test/unit/test_bus.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_container.py` & `static-frame-2.7.0/static_frame/test/unit/test_container.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_container_util.py` & `static-frame-2.7.0/static_frame/test/unit/test_container_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_display.py` & `static-frame-2.7.0/static_frame/test/unit/test_display.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_display_color.py` & `static-frame-2.7.0/static_frame/test/unit/test_display_color.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_doc.py` & `static-frame-2.7.0/static_frame/test/unit/test_doc.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_fill_value_auto.py` & `static-frame-2.7.0/static_frame/test/unit/test_fill_value_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_frame.py` & `static-frame-2.7.0/static_frame/test/unit/test_frame.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_frame_he.py` & `static-frame-2.7.0/static_frame/test/unit/test_frame_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_frame_iter.py` & `static-frame-2.7.0/static_frame/test/unit/test_frame_iter.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_frame_join.py` & `static-frame-2.7.0/static_frame/test/unit/test_frame_join.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_frame_via_fill_value.py` & `static-frame-2.7.0/static_frame/test/unit/test_frame_via_fill_value.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_frame_via_re.py` & `static-frame-2.7.0/static_frame/test/unit/test_frame_via_re.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_hloc.py` & `static-frame-2.7.0/static_frame/test/unit/test_hloc.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_index.py` & `static-frame-2.7.0/static_frame/test/unit/test_index.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_index_auto.py` & `static-frame-2.7.0/static_frame/test/unit/test_index_auto.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_index_base.py` & `static-frame-2.7.0/static_frame/test/unit/test_index_base.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_index_correspondence.py` & `static-frame-2.7.0/static_frame/test/unit/test_index_correspondence.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_index_datetime.py` & `static-frame-2.7.0/static_frame/test/unit/test_index_datetime.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_index_hierarchy.py` & `static-frame-2.7.0/static_frame/test/unit/test_index_hierarchy.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_index_hierarchy_set_utils.py` & `static-frame-2.7.0/static_frame/test/unit/test_index_hierarchy_set_utils.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_interface.py` & `static-frame-2.7.0/static_frame/test/unit/test_interface.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_loc_map.py` & `static-frame-2.7.0/static_frame/test/unit/test_loc_map.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_memory_measure.py` & `static-frame-2.7.0/static_frame/test/unit/test_memory_measure.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_memory_measure_getsizeof.py` & `static-frame-2.7.0/static_frame/test/unit/test_memory_measure_getsizeof.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_metadata.py` & `static-frame-2.7.0/static_frame/test/unit/test_metadata.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_pivot.py` & `static-frame-2.7.0/static_frame/test/unit/test_pivot.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_protocol_dfi.py` & `static-frame-2.7.0/static_frame/test/unit/test_protocol_dfi.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_quilt.py` & `static-frame-2.7.0/static_frame/test/unit/test_quilt.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_rank.py` & `static-frame-2.7.0/static_frame/test/unit/test_rank.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_series.py` & `static-frame-2.7.0/static_frame/test/unit/test_series.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_series_he.py` & `static-frame-2.7.0/static_frame/test/unit/test_series_he.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_store.py` & `static-frame-2.7.0/static_frame/test/unit/test_store.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_store_filter.py` & `static-frame-2.7.0/static_frame/test/unit/test_store_filter.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_store_hdf5.py` & `static-frame-2.7.0/static_frame/test/unit/test_store_hdf5.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_store_sqlite.py` & `static-frame-2.7.0/static_frame/test/unit/test_store_sqlite.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_store_xlsx.py` & `static-frame-2.7.0/static_frame/test/unit/test_store_xlsx.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_store_zip.py` & `static-frame-2.7.0/static_frame/test/unit/test_store_zip.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_style_config.py` & `static-frame-2.7.0/static_frame/test/unit/test_style_config.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_type_blocks.py` & `static-frame-2.7.0/static_frame/test/unit/test_type_blocks.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_type_clinic.py` & `static-frame-2.7.0/static_frame/test/unit/test_type_clinic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from __future__ import annotations
+# pylint: disable=C0321
+# from __future__ import annotations # cannot use with TypeVars!
 
 import re
 import warnings
 from functools import partial
 
 import frame_fixtures as ff
 import numpy as np
@@ -13,18 +14,19 @@
 import static_frame as sf
 from static_frame.core.type_clinic import CallGuard
 from static_frame.core.type_clinic import ClinicResult
 from static_frame.core.type_clinic import ErrorAction
 from static_frame.core.type_clinic import Require
 from static_frame.core.type_clinic import TValidation
 from static_frame.core.type_clinic import TypeClinic
+from static_frame.core.type_clinic import TypeVarRegistry
+from static_frame.core.type_clinic import _check
 from static_frame.core.type_clinic import _check_interface
 from static_frame.core.type_clinic import is_union
 from static_frame.core.type_clinic import is_unpack
-from static_frame.test.test_case import skip_pyle38
 from static_frame.test.test_case import skip_pyle310
 from static_frame.test.test_case import skip_win
 
 #-------------------------------------------------------------------------------
 # recreate private nbit types for testing
 
 class _256Bit(NBitBase):  # type: ignore[misc] # pylint: disable=W0240
@@ -47,14 +49,29 @@
 # complex partitions are always balanced
 
 # complex160 = np.complexfloating[_80Bit, _80Bit]
 # complex192 = np.complexfloating[_96Bit, _96Bit]
 # complex256 = np.complexfloating[_128Bit, _128Bit]
 # complex512 = np.complexfloating[_256Bit, _256Bit]
 
+#-------------------------------------------------------------------------------
+def test_check_a():
+    cr = _check([3, 'a'], tp.List[tp.Union[str, int]])
+    assert cr.validated
+
+def test_check_b():
+    T = tp.TypeVar('T')
+    tvr = TypeVarRegistry()
+    cr1 = _check((3, 'a'), tp.Tuple[T, T], tvr=tvr)
+    assert not cr1.validated
+    assert scrub_str(cr1.to_str()) == 'In Tuple[~T, ~T] ~T Expected int, provided str invalid'
+
+    # we can ignore TypeVars
+    cr2 = _check((3, 'a'), tp.Tuple[T, T], tvr=None)
+    assert cr2.validated
 
 #-------------------------------------------------------------------------------
 
 def test_check_type_a():
 
     TypeClinic(sf.IndexDate(('2022-01-01',))).check(sf.IndexDate)
     TypeClinic(sf.IndexDate(('2022-01-01',))).check(tp.Any)
@@ -579,15 +596,15 @@
         assert proc1(2, 3) == 6
     except TypeError as e:
         assert scrub_str(str(e)) == 'In return of (a: int, b: int) -> bool Expected bool, provided int invalid'
 
     try:
         assert proc1(2, 'foo') == 6
     except TypeError as e:
-        assert scrub_str(str(e)) == 'In args of (a: int, b: int) -> bool Expected int, provided str invalid'
+        assert scrub_str(str(e)) == 'In args of (a: int, b: int) -> bool In arg b Expected int, provided str invalid'
 
 def test_check_interface_c1():
 
     @CallGuard.check(fail_fast=False)
     def proc1(a: int, b) -> int:
         return a * b
 
@@ -686,15 +703,15 @@
 def test_check_interface_g1():
     def proc1(x: int) -> int:
         return x
 
     assert _check_interface(proc1, (1,), {}, False, ErrorAction.RAISE) == 1
 
     cr1 = _check_interface(proc1, (False,), {}, False, ErrorAction.RETURN)
-    assert scrub_str(cr1.to_str()) == 'In args of (x: int) -> int Expected int, provided bool invalid'
+    assert scrub_str(cr1.to_str()) == 'In args of (x: int) -> int In arg x Expected int, provided bool invalid'
 
     def proc2(x: int) -> int:
         return 'foo'
 
     cr2 = _check_interface(proc2, (3,), {}, False, ErrorAction.RETURN)
     assert scrub_str(cr2.to_str()) == 'In return of (x: int) -> int Expected int, provided str invalid'
 
@@ -1253,15 +1270,15 @@
 
     cr2 = y1.via_type_clinic(sf.Yarn[sf.Index[np.int64]])
     assert cr2.validated is False
 
 
 #-------------------------------------------------------------------------------
 
-def get_hints(records: tp.Iterable[TValidation] | ClinicResult) -> tp.Tuple[str]:
+def get_hints(records: tp.Union[tp.Iterable[TValidation], ClinicResult]) -> tp.Tuple[str]:
     return tuple(r[1] for r in records)
 
 def test_validate_labels_order_a1():
     idx1 = sf.Index(('a', 'b', 'c'))
     v = Require.LabelsOrder('a', 'b', 'c')
     assert not get_hints(v._iter_errors(idx1, None, (), ()))
 
@@ -1974,43 +1991,38 @@
     assert TypeClinic(sf.Frame).to_hint() == tp.Type[sf.Frame]
 
 @skip_pyle310
 def test_type_clinic_to_hint_f():
     assert TypeClinic(np.dtype(np.float64)).to_hint() == np.dtype[np.float64]
     assert TypeClinic(np.array([False, True])).to_hint() == np.ndarray[np.dtype[np.bool_]]
 
-@skip_pyle38
 def test_type_clinic_to_hint_g1():
     assert TypeClinic((3, 'foo', False)).to_hint() == tuple[int, str, bool]
 
-@skip_pyle38
 def test_type_clinic_to_hint_h1():
     assert TypeClinic([3, 1, 2]).to_hint() == list[int]
     assert TypeClinic([]).to_hint() == list[tp.Any]
     assert TypeClinic([False, True, False]).to_hint() == list[bool]
     assert TypeClinic([False, True, 1, 2]).to_hint() == list[tp.Union[bool, int]]
 
-@skip_pyle38
 def test_type_clinic_to_hint_j1():
     assert TypeClinic({}).to_hint() == dict[tp.Any, tp.Any]
 
     assert TypeClinic({3: 'a'}).to_hint() == dict[int, str]
     assert TypeClinic({3: 'a', 42: 'x'}).to_hint() == dict[int, str]
 
     assert TypeClinic({'a': 3}).to_hint() == dict[str, int]
     assert TypeClinic({'a': 3, 'x': 30}).to_hint() == dict[str, int]
 
-@skip_pyle38
 def test_type_clinic_to_hint_j2():
 
     assert TypeClinic({3: 'a', 42: 'x', 1.2: 'y'}).to_hint() == dict[tp.Union[int, float], str]
 
     assert TypeClinic({'a': 3, 'x': 30, 'z': 10.5}).to_hint() == dict[str, tp.Union[int, float]]
 
-@skip_pyle38
 def test_type_clinic_to_hint_j3():
 
     assert TypeClinic({3: 'a', 42: 'x', 1.2: 'y', 30: b'q'}).to_hint() == dict[tp.Union[int, float], tp.Union[str, bytes]]
 
     assert TypeClinic({'a': 3, 'x': 30, b'z': 10.5}).to_hint() == dict[tp.Union[str, bytes], tp.Union[int, float]]
 
 #-------------------------------------------------------------------------------
@@ -2032,7 +2044,280 @@
 def test_via_type_clinic_b():
     s = sf.Series(('a', 'b'), index=(('x', 'y')))
 
     with pytest.raises(TypeError):
         s.via_type_clinic.check(sf.Series[sf.IndexDate, np.str_])
 
 
+#-------------------------------------------------------------------------------
+def test_type_clinic_typevar_a():
+
+    T = tp.TypeVar('T', bound=np.generic)
+    h1 = sf.Frame[sf.Index[T],
+            sf.Index[T],
+            tp.Unpack[tp.Tuple[tp.Any, ...]],
+            ]
+
+    records = ((1, 3, True), (3, 8, True),)
+    f1 = sf.Frame.from_records(records,
+            columns=('a', 'b', 'c'),
+            index=np.array((1, 2), np.int64),
+            )
+    # NOTE: this is valid if we interpret the bound as simply meaning that the any of the values must independently by subclasses of the bound; the observed values does not set the type
+    assert scrub_str(f1.via_type_clinic(h1).to_str()) == 'In Frame[Index[~T: generic], Index[~T: generic], Unpack[Tuple[Any, ...]]] Index[~T: generic] ~T: generic Expected int64, provided str_ invalid'
+
+def test_type_clinic_typevar_b1():
+
+    T = tp.TypeVar('T', np.int64, np.float64)
+    h1 = sf.Frame[sf.Index[T],
+            sf.Index[T],
+            tp.Unpack[tp.Tuple[tp.Any, ...]],
+            ]
+
+    records = ((1, 3, True), (3, 8, True),)
+    f1 = sf.Frame.from_records(records,
+            columns=sf.Index((10, 20, 30), dtype=np.int64),
+            index=sf.Index((1, 2), dtype=np.int64),
+            )
+    assert TypeClinic(f1)(h1).validated
+
+def test_type_clinic_typevar_b2():
+
+    T = tp.TypeVar('T', np.int64, np.float64)
+    h1 = sf.Frame[sf.Index[T],
+            sf.Index[T],
+            tp.Unpack[tp.Tuple[tp.Any, ...]],
+            ]
+
+    records = ((1, 3, True), (3, 8, True),)
+    f1 = sf.Frame.from_records(records,
+            columns=sf.Index((10, 20, 30), dtype=np.int64),
+            index=sf.Index((1, 2), dtype=np.float64),
+            )
+    cr = TypeClinic(f1)(h1)
+    assert scrub_str(cr.to_str()) == 'In Frame[Index[~T: (int64, float64)], Index[~T: (int64, float64)], Unpack[Tuple[Any, ...]]] Index[~T: (int64, float64)] ~T: (int64, float64) Expected float64, provided int64 invalid'
+
+def test_type_clinic_typevar_c():
+
+    T = tp.TypeVar('T')
+
+    h1 = sf.Frame[sf.Index[T],
+            sf.Index[T],
+            tp.Unpack[tp.Tuple[tp.Any, ...]],
+            ]
+
+    records = ((1, 3, True), (3, 8, True),)
+    f1 = sf.Frame.from_records(records,
+            columns=sf.Index((10, 20, 30), dtype=np.int64),
+            index=('a', 'b'),
+            )
+
+    cr = TypeClinic(f1)(h1)
+    assert scrub_str(cr.to_str()) == 'In Frame[Index[~T], Index[~T], Unpack[Tuple[Any, ...]]] Index[~T] ~T Expected str_, provided int64 invalid'
+
+@skip_pyle310
+def test_type_clinic_typevar_d1():
+
+    class A: ...
+    class A1(A): ...
+    class A2(A): ...
+    class B: ...
+    class B1(B): ...
+    class B2(B): ...
+    class C: ...
+    class C1(C): ...
+    class C2(C): ...
+
+    T = tp.TypeVar('T', bound=tp.Union[A, B, C])
+    h = tp.Tuple[T, T, T]
+
+    v1 = (A2(), C1(), B2())
+    cr = TypeClinic(v1)(h)
+    assert cr.validated
+
+    v2 = (A2(), C1(), A1()) # we specialized the Union to A1, not A2
+    cr = TypeClinic(v2)(h)
+    assert scrub_str(cr.to_str()) == 'In Tuple[~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C]] ~T: Union[A, B, C] Union[A2, B, C1] Expected A2, provided A1 invalid In Tuple[~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C]] ~T: Union[A, B, C] Union[A2, B, C1] Expected B, provided A1 invalid In Tuple[~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C]] ~T: Union[A, B, C] Union[A2, B, C1] Expected C1, provided A1 invalid'
+
+    v3 = (A2(), A2(), A1()) # we specialized the Union to A1, not A2
+    cr = TypeClinic(v3)(h)
+    assert len(cr) == 3
+
+    v4 = (C2(), A2(), C1()) # we specialized the Union to A1, not A2
+    cr = TypeClinic(v4)(h)
+    assert len(cr) == 3
+
+def test_type_clinic_typevar_d2():
+
+    class A: ...
+    class A1(A): ...
+    class A2(A): ...
+    class B: ...
+    class B1(B): ...
+    class B2(B): ...
+    class C: ...
+    class C1(C): ...
+    class C2(C): ...
+
+    T = tp.TypeVar('T', bound=tp.Union[A, B, C])
+    h = tp.Tuple[T, T, T, T, T, T]
+
+    v1 = (A2(), C1(), B2(), A2(), C1(), B2())
+    cr = TypeClinic(v1)(h)
+    assert cr.validated
+
+    v2 = (A2(), C2(), C2(), B1(), C2(), B1())
+    cr = TypeClinic(v2)(h)
+    assert cr.validated
+
+@skip_pyle310
+def test_type_clinic_typevar_d3():
+
+    class A: ...
+    class A1(A): ...
+    class A2(A): ...
+    class B: ...
+    class B1(B): ...
+    class B2(B): ...
+    class C: ...
+    class C1(C): ...
+    class C2(C): ...
+
+    T = tp.TypeVar('T', bound=tp.Union[A, B, C])
+    h = tp.Tuple[T, T, T, T, T, T]
+
+    v = (A2(), C2(), C2(), B1(), C1(), B1())
+    cr = TypeClinic(v)(h)
+    assert not cr.validated
+    assert scrub_str(cr.to_str()) == 'In Tuple[~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C]] ~T: Union[A, B, C] Union[A2, B1, C2] Expected A2, provided C1 invalid In Tuple[~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C]] ~T: Union[A, B, C] Union[A2, B1, C2] Expected B1, provided C1 invalid In Tuple[~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C], ~T: Union[A, B, C]] ~T: Union[A, B, C] Union[A2, B1, C2] Expected C2, provided C1 invalid'
+
+
+#-------------------------------------------------------------------------------
+
+def test_call_guard_typevar_a():
+
+    T1 = tp.TypeVar('T1')
+    T2 = tp.TypeVar('T2')
+
+    @CallGuard.check
+    def process1(a: sf.Series[sf.Index[T1], T2]) -> sf.Series[sf.Index[T1], T2]:
+        return a * 2
+
+    _ = process1(sf.Series((1.2, 5.4), index=sf.Index(('a', 'b'))))
+    _ = process1(sf.Series(('a', 'b'), index=sf.Index((1.2, 5.3))))
+
+    T3 = tp.TypeVar('T3')
+    T4 = tp.TypeVar('T4')
+
+    @CallGuard.warn
+    def process2(a: sf.Series[sf.Index[T3], T4]) -> sf.Series[sf.Index[T3], T4]:
+        return sf.Series(('a', 'b'), index=sf.Index(('a', 'b')))
+
+    with warnings.catch_warnings(record=True) as w:
+        # expected to return float values (based on input) but returned string values
+        _ = process2(sf.Series((1.2, 5.4), index=sf.Index(('a', 'b'))))
+        assert scrub_str(str(w[0].message)) == 'In return of (a: Series[Index[~T3], ~T4]) -> Series[Index[~T3], ~T4] Series[Index[~T3], ~T4] ~T4 Expected float64, provided str_ invalid'
+
+    with warnings.catch_warnings(record=True) as w:
+        # expected to return float values (based on input) but returned string values
+        _ = process2(sf.Series((False, True), index=sf.Index(('a', 'b'))))
+        assert scrub_str(str(w[0].message)) == 'In return of (a: Series[Index[~T3], ~T4]) -> Series[Index[~T3], ~T4] Series[Index[~T3], ~T4] ~T4 Expected bool_, provided str_ invalid'
+
+
+def test_call_guard_typevar_b():
+
+    T = tp.TypeVar('T')
+
+    @sf.CallGuard.warn
+    def process1(
+            a: sf.Series[sf.Index[T], np.number[tp.Any]],
+            b: sf.Series[sf.Index[T], np.number[tp.Any]],
+            ) -> sf.Series[sf.Index[T], np.number[tp.Any]]:
+        return a + b
+
+    with warnings.catch_warnings(record=True) as w:
+        _ = process1(sf.Series((1.2, 5.4), index=('a', 'b')), sf.Series((4, 5), index=np.array((30, 10), dtype=np.int64), dtype=np.int64))
+        assert scrub_str(str(w[0].message)) == 'In args of (a: Series[Index[~T], number[Any]], b: Series[Index[~T], number[Any]]) -> Series[Index[~T], number[Any]] In arg b Series[Index[~T], number[Any]] Index[~T] ~T Expected str_, provided int64 invalid'
+
+
+def test_call_guard_typevar_c1():
+    # based on examples here: https://stackoverflow.com/a/59937840
+
+    T1 = tp.TypeVar('T1', bound=tp.Union[int, str])
+
+    @sf.CallGuard.warn
+    def concat1(x: tp.Iterable[T1], y: tp.Iterable[T1]) -> tp.List[T1]:
+        out = list(x)
+        out.extend(y)
+        return out
+
+    mix1: tp.List[tp.Union[int, str]] = [1, "a", 3]
+    mix2: tp.List[tp.Union[int, str]] = [4, "x", "y"]
+    all_ints = [1, 2, 3]
+    all_strs = ["a", "b", "c"]
+
+    _ = concat1(mix1, mix2) # does not error
+    _ = concat1(all_ints, all_strs) # does not error
+    _ = concat1(all_strs, all_strs) # does not error
+
+@skip_pyle310
+def test_call_guard_typevar_c2():
+    # based on examples here: https://stackoverflow.com/a/59937840
+
+    T1 = tp.TypeVar('T1', int, str)
+
+    @sf.CallGuard.warn(fail_fast=True)
+    def concat1(x: tp.Iterable[T1], y: tp.Iterable[T1]) -> tp.List[T1]:
+        out = list(x)
+        out.extend(y)
+        return out
+
+    mix1: tp.List[tp.Union[int, str]] = [1, "a", 3]
+    mix2: tp.List[tp.Union[int, str]] = [4, "x", "y"]
+    all_ints = [1, 2, 3]
+    all_strs = ["a", "b", "c"]
+
+    with warnings.catch_warnings(record=True) as w:
+        _ = concat1(mix1, mix2) # fails
+        assert scrub_str(str(w[0].message)) == "In args of (x: Iterable[~T1: (int, str)], y: Iterable[~T1: (int, str)]) -> List[~T1: (int, str)] In arg x Iterable[~T1: (int, str)] ~T1: (int, str) Expected int, provided str invalid"
+
+    _ = concat1(all_ints, all_ints) # does not error
+    _ = concat1(all_strs, all_strs) # does not error
+
+    with warnings.catch_warnings(record=True) as w:
+        _ = concat1(all_ints, all_strs) # fails
+        assert scrub_str(str(w[0].message)) == "In args of (x: Iterable[~T1: (int, str)], y: Iterable[~T1: (int, str)]) -> List[~T1: (int, str)] In arg y Iterable[~T1: (int, str)] ~T1: (int, str) Expected int, provided str invalid"
+
+
+def test_call_guard_typevar_d():
+    T = tp.TypeVar('T', np.uint16, np.int8)
+
+    @sf.CallGuard.warn
+    def process1(
+            a: sf.Series[sf.Index[str], T],
+            b: sf.Series[sf.Index[str], T],
+            ) -> sf.Series[sf.Index[str], T]:
+        return a + b
+
+    _ = process1(sf.Series((1.2, 5.4), index=('a', 'b'), dtype=np.int8), sf.Series((4, 5), index=('a', 'b'), dtype=np.int8))
+
+    _ = process1(sf.Series((1.2, 5.4), index=('a', 'b'), dtype=np.uint16), sf.Series((4, 5), index=('a', 'b'), dtype=np.uint16))
+
+    with warnings.catch_warnings(record=True) as w:
+        _ = process1(sf.Series((1.2, 5.4), index=('a', 'b'), dtype=np.uint16), sf.Series((4, 5), index=('a', 'b'), dtype=np.int8))
+        assert scrub_str(str(w[0].message)) == 'In args of (a: Series[Index[str], ~T: (uint16, int8)], b: Series[Index[str], ~T: (uint16, int8)]) -> Series[Index[str], ~T: (uint16, int8)] In arg b Series[Index[str], ~T: (uint16, int8)] ~T: (uint16, int8) Expected uint16, provided int8 invalid'
+
+def test_call_guard_typevar_e():
+
+    T1 = tp.TypeVar('T1', bound=np.number[tp.Any])
+    T2 = tp.TypeVar('T2', bound=np.number[tp.Any])
+
+    @sf.CallGuard.warn
+    def process2(
+            a: sf.Series[sf.Index[T1], T2],
+            b: sf.Series[sf.Index[T1], T2],
+            ) -> sf.Series[sf.Index[T1], T2]:
+        return a + b
+
+    _ = process2(sf.Series((1.2, 5.4), index=('a', 'b')), sf.Series((4.3, 5.1), index=('a', 'c')))
+
+
```

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_util.py` & `static-frame-2.7.0/static_frame/test/unit/test_util.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_www.py` & `static-frame-2.7.0/static_frame/test/unit/test_www.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame/test/unit/test_yarn.py` & `static-frame-2.7.0/static_frame/test/unit/test_yarn.py`

 * *Files identical despite different names*

### Comparing `static-frame-2.6.0/static_frame.egg-info/PKG-INFO` & `static-frame-2.7.0/static_frame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame
-Version: 2.6.0
+Version: 2.7.0
 Summary: Immutable and statically-typeable DataFrames with runtime type and data validation.
 Home-page: https://github.com/static-frame/static-frame
 Author: Christopher Ariza
 License: MIT
 Keywords: staticframe pandas numpy immutable array
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `static-frame-2.6.0/static_frame.egg-info/SOURCES.txt` & `static-frame-2.7.0/static_frame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

