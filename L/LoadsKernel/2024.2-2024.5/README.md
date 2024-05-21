# Comparing `tmp/LoadsKernel-2024.2.tar.gz` & `tmp/loadskernel-2024.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LoadsKernel-2024.2.tar", last modified: Tue Feb 13 18:08:15 2024, max compression
+gzip compressed data, was "loadskernel-2024.5.tar", last modified: Tue May 21 09:38:15 2024, max compression
```

## Comparing `LoadsKernel-2024.2.tar` & `loadskernel-2024.5.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.486015 LoadsKernel-2024.2/
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.486015 LoadsKernel-2024.2/LoadsKernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-02-13 18:08:15.000000 LoadsKernel-2024.2/LoadsKernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2691 2024-02-13 18:08:15.000000 LoadsKernel-2024.2/LoadsKernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-13 18:08:15.000000 LoadsKernel-2024.2/LoadsKernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-13 18:08:15.000000 LoadsKernel-2024.2/LoadsKernel.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-02-13 18:08:15.000000 LoadsKernel-2024.2/LoadsKernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-02-13 18:08:15.000000 LoadsKernel-2024.2/LoadsKernel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     7477 2024-02-13 18:08:15.486015 LoadsKernel-2024.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6368 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.470015 LoadsKernel-2024.2/loadscompare/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadscompare/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13619 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadscompare/compare.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.470015 LoadsKernel-2024.2/loadscompare/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)    62264 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadscompare/graphics/LK_logo2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadscompare/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.474015 LoadsKernel-2024.2/loadskernel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/auxiliary_output.py
--rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/build_aero_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/build_splinegrid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.478015 LoadsKernel-2024.2/loadskernel/cfd_interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/cfd_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/cfd_interfaces/meshdefo.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/cfd_interfaces/mpi_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    30235 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/cfd_interfaces/su2_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    18285 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/cfd_interfaces/tau_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.478015 LoadsKernel-2024.2/loadskernel/engine_interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/engine_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/engine_interfaces/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/engine_interfaces/propeller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.478015 LoadsKernel-2024.2/loadskernel/equations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/equations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/equations/cfd.py
--rw-r--r--   0 runner    (1001) docker     (127)    46158 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/equations/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    33564 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/equations/frequency_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     6837 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/equations/landing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/equations/nonlin_steady.py
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/equations/state_space.py
--rw-r--r--   0 runner    (1001) docker     (127)     9565 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/equations/steady.py
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/equations/unsteady.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.478015 LoadsKernel-2024.2/loadskernel/fem_interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/fem_interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/fem_interfaces/b2000_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/fem_interfaces/cofe_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/fem_interfaces/fem_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/fem_interfaces/nastran_f06_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    17544 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/fem_interfaces/nastran_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/gather_loads.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.482015 LoadsKernel-2024.2/loadskernel/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)    62264 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/graphics/LK_logo2.png
--rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/grid_trafo.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/integrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/interpolate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.482015 LoadsKernel-2024.2/loadskernel/io_functions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/io_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8705 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/io_functions/bdf_cards.py
--rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/io_functions/data_handling.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/io_functions/read_b2000.py
--rw-r--r--   0 runner    (1001) docker     (127)     9244 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/io_functions/read_bdf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12128 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/io_functions/read_cfdgrids.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/io_functions/read_h5.py
--rw-r--r--   0 runner    (1001) docker     (127)    21850 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/io_functions/read_mona.py
--rw-r--r--   0 runner    (1001) docker     (127)    21300 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/io_functions/read_op2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/io_functions/read_op4.py
--rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/io_functions/write_mona.py
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/jcl_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)    35612 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21617 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/plotting_extra.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    34471 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/plotting_standard.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10168 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/post_processing.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27457 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/program_flow.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    27657 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/solution_sequences.py
--rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/solution_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/spline_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/spline_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    28486 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/trim_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.482015 LoadsKernel-2024.2/loadskernel/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/utils/PID.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/utils/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/loadskernel/utils/sparse_matrices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.482015 LoadsKernel-2024.2/modelviewer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/modelviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/modelviewer/cfdgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/modelviewer/iges.py
--rw-r--r--   0 runner    (1001) docker     (127)    20129 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/modelviewer/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/modelviewer/pytran.py
--rw-r--r--   0 runner    (1001) docker     (127)    30398 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/modelviewer/view.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-13 18:08:15.486015 LoadsKernel-2024.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:15.486015 LoadsKernel-2024.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/tests/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/tests/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)    10967 2024-02-13 18:08:06.000000 LoadsKernel-2024.2/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.203273 loadskernel-2024.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-21 09:38:10.000000 loadskernel-2024.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1561 2024-05-21 09:38:10.000000 loadskernel-2024.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.203273 loadskernel-2024.5/LoadsKernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-21 09:38:15.000000 loadskernel-2024.5/LoadsKernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-21 09:38:15.000000 loadskernel-2024.5/LoadsKernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:38:15.000000 loadskernel-2024.5/LoadsKernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-21 09:38:15.000000 loadskernel-2024.5/LoadsKernel.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-21 09:38:15.000000 loadskernel-2024.5/LoadsKernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-21 09:38:15.000000 loadskernel-2024.5/LoadsKernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-21 09:38:15.203273 loadskernel-2024.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-05-21 09:38:10.000000 loadskernel-2024.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.187273 loadskernel-2024.5/loadscompare/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadscompare/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13844 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadscompare/compare.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.187273 loadskernel-2024.5/loadscompare/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)    62264 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadscompare/graphics/LK_logo2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadscompare/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.191273 loadskernel-2024.5/loadskernel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11197 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/auxiliary_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10940 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/build_aero_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/build_splinegrid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.191273 loadskernel-2024.5/loadskernel/cfd_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/cfd_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/cfd_interfaces/meshdefo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/cfd_interfaces/mpi_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30235 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/cfd_interfaces/su2_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18285 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/cfd_interfaces/tau_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.195273 loadskernel-2024.5/loadskernel/engine_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/engine_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/engine_interfaces/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17534 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/engine_interfaces/propeller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.195273 loadskernel-2024.5/loadskernel/equations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/equations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8451 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/equations/cfd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46191 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/equations/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33564 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/equations/frequency_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6762 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/equations/landing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/equations/nonlin_steady.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/equations/state_space.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9557 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/equations/steady.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5174 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/equations/unsteady.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.195273 loadskernel-2024.5/loadskernel/fem_interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/fem_interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/fem_interfaces/b2000_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/fem_interfaces/cofe_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/fem_interfaces/fem_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/fem_interfaces/nastran_f06_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17544 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/fem_interfaces/nastran_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6632 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/gather_loads.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.195273 loadskernel-2024.5/loadskernel/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)    62264 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/graphics/LK_logo2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5541 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/grid_trafo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/integrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/interpolate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.199273 loadskernel-2024.5/loadskernel/io_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/io_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9739 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/io_functions/bdf_cards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5995 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/io_functions/data_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/io_functions/read_b2000.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9784 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/io_functions/read_bdf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12128 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/io_functions/read_cfdgrids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/io_functions/read_h5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21850 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/io_functions/read_mona.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21300 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/io_functions/read_op2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7020 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/io_functions/read_op4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3180 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/io_functions/write_mona.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/jcl_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35612 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    26593 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/plotting_extra.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    30404 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/plotting_standard.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10168 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/post_processing.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27689 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/program_flow.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    27657 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/solution_sequences.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5490 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/solution_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12452 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/spline_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2569 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/spline_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28486 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/trim_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.199273 loadskernel-2024.5/loadskernel/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3787 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/utils/PID.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/utils/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-21 09:38:11.000000 loadskernel-2024.5/loadskernel/utils/sparse_matrices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.199273 loadskernel-2024.5/modelviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:11.000000 loadskernel-2024.5/modelviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-05-21 09:38:11.000000 loadskernel-2024.5/modelviewer/cfdgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-21 09:38:11.000000 loadskernel-2024.5/modelviewer/iges.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20128 2024-05-21 09:38:11.000000 loadskernel-2024.5/modelviewer/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-05-21 09:38:11.000000 loadskernel-2024.5/modelviewer/pytran.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30398 2024-05-21 09:38:11.000000 loadskernel-2024.5/modelviewer/view.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:38:15.203273 loadskernel-2024.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2915 2024-05-21 09:38:11.000000 loadskernel-2024.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:15.199273 loadskernel-2024.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:38:11.000000 loadskernel-2024.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2024-05-21 09:38:11.000000 loadskernel-2024.5/tests/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 09:38:11.000000 loadskernel-2024.5/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10967 2024-05-21 09:38:11.000000 loadskernel-2024.5/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-21 09:38:11.000000 loadskernel-2024.5/tests/test_unittests.py
```

### Comparing `LoadsKernel-2024.2/AUTHORS.md` & `loadskernel-2024.5/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/LICENSE` & `loadskernel-2024.5/LICENSE`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/LoadsKernel.egg-info/PKG-INFO` & `loadskernel-2024.5/LoadsKernel.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,77 @@
 Metadata-Version: 2.1
 Name: LoadsKernel
-Version: 2024.2
+Version: 2024.5
 Summary: The Loads Kernel Software allows for the calculation of quasi-steady and dynamic maneuver loads,
 Home-page: https://github.com/DLR-AE/LoadsKernel
 Author: Arne Voß
 Author-email: arne.voss@dlr.de
 License: BSD 3-Clause License
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: PanelAero
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: psutil
 Requires-Dist: h5py
 Requires-Dist: tables
 Requires-Dist: pyyaml
 Requires-Dist: pandas
 Provides-Extra: extras
 Requires-Dist: mpi4py; extra == "extras"
-Requires-Dist: pyfmi; extra == "extras"
 Requires-Dist: mayavi; extra == "extras"
 Requires-Dist: traits; extra == "extras"
 Requires-Dist: traitsui; extra == "extras"
 Requires-Dist: pyface; extra == "extras"
+Requires-Dist: jupyter; extra == "extras"
 Requires-Dist: pyiges; extra == "extras"
+Provides-Extra: difficult
+Requires-Dist: pyfmi; extra == "difficult"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
-Requires-Dist: jupyter; extra == "test"
 Requires-Dist: jupyter-book==0.15.1; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: pylint; extra == "test"
 
 # Loads Kernel
 
 <p align="left">
 <img width="200" src="./graphics/LK_logo2.png">
 </p>
 
 The Loads Kernel Software allows for the calculation of quasi-steady and dynamic maneuver loads, unsteady gust loads in the time and frequency domain as well as dynamic landing loads based on a generic landing gear module.
 
-[![DOI](https://zenodo.org/badge/537500844.svg)](https://zenodo.org/badge/latestdoi/537500844)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8341566.svg)](https://doi.org/10.5281/zenodo.8341566)
 
 # Theorectical Background & References
 
-[1] Voß, A., “Loads Kernel User Guide, Version 1.01,” Institut für Aeroelastik, Deutsches Zentrum für Luft- und Raumfahrt, Göttingen, Germany, Technical Report DLR-IB-AE-GO-2020-136, Nov. 2021, https://elib.dlr.de/140268/.
+[1] Voß, A., “Loads Kernel User Guide,” Institut für Aeroelastik, Deutsches Zentrum für Luft- und Raumfahrt, Göttingen, Germany, Technical Report DLR-IB-AE-GO-2020-136, Nov. 2021, https://elib.dlr.de/140268/.
 
 [2] Voß, A., “An Implementation of the Vortex Lattice and the Doublet Lattice Method,” Institut für Aeroelastik, Deutsches Zentrum für Luft- und Raumfahrt, Göttingen, Germany, Technical Report DLR-IB-AE-GO-2020-137, Oktober 2020, https://elib.dlr.de/136536/.
 
 If you use this software for your scientific work, we kindly ask you to include a reference [1,2] in your publications. Thank you!
 
 # Installation & Use
 ## Basic Installation 
-Install Loads Kernel as a python package with core dependencies via:
+Install Loads Kernel as a python package with its core dependencies using a package manager (PyPI or Conda):
 
 ```
 pip install LoadsKernel
 ```
 
+or
+
+```
+conda install -c conda-forge LoadsKernel
+```
+
 ## How can I use it?
 
 Copy and adjust the launch script (launch.py, example located in the [scripts folder](https://github.com/DLR-AE/LoadsKernel/tree/master/scripts)) to your needs / for your aircraft configuration. Then, launch the python script with:
 
 ```
 python launch.py
 ```
@@ -70,31 +79,36 @@
 Alternatively, if ~/.local/bin is in your system PATH, you can use the following commands from the command line:
 
 ```
 loads-kernel --job_name jcl_xy --pre True --main True --post True --path_input /path/to/JCLs --path_output /path/to/output
 ```
 
 ## Advanced Installation 
-
-As above, but with access to the code (keep the code where it is so that you can explore and modify):
+As above, but with access to the code (download and keep the code where it is so that you can explore and modify):
 
 ```
 git clone https://github.com/DLR-AE/LoadsKernel.git
 cd <local_repo_path>
 pip install -e . 
 ```
 
 To use the graphical tools and other features, optional libraries definded as extras are necessary:
 
 ```
 pip install -e .[extras]
 ```
 
-Note: Especially with mpi or the graphical libraries, pip frequently fails. In that case, try to install the failing packages using a
-package manager such as conda.
+or
+
+```
+conda install -c conda-forge loadskernel-extras
+```
+
+Note: Especially with mpi or the graphical libraries, pip frequently fails. In that case, try to install the missing/failing packages using a
+package manager such as conda, which is the more robust solution.
 
 There are two GUIs to visualize a simulation model (the Model Viewer) and to compare different sets of loads (Loads Compare), which can be started from the command line as well.
 
 ```
 model-viewer
 loads-compare
 ```
```

### Comparing `LoadsKernel-2024.2/LoadsKernel.egg-info/SOURCES.txt` & `loadskernel-2024.5/LoadsKernel.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -76,10 +76,10 @@
 modelviewer/cfdgrid.py
 modelviewer/iges.py
 modelviewer/plotting.py
 modelviewer/pytran.py
 modelviewer/view.py
 tests/__init__.py
 tests/helper_functions.py
-tests/test_dummy.py
 tests/test_gui.py
-tests/test_integration.py
+tests/test_integration.py
+tests/test_unittests.py
```

### Comparing `LoadsKernel-2024.2/PKG-INFO` & `loadskernel-2024.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,68 +1,77 @@
 Metadata-Version: 2.1
 Name: LoadsKernel
-Version: 2024.2
+Version: 2024.5
 Summary: The Loads Kernel Software allows for the calculation of quasi-steady and dynamic maneuver loads,
 Home-page: https://github.com/DLR-AE/LoadsKernel
 Author: Arne Voß
 Author-email: arne.voss@dlr.de
 License: BSD 3-Clause License
-Requires-Python: >=3.8
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.md
 Requires-Dist: PanelAero
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: psutil
 Requires-Dist: h5py
 Requires-Dist: tables
 Requires-Dist: pyyaml
 Requires-Dist: pandas
 Provides-Extra: extras
 Requires-Dist: mpi4py; extra == "extras"
-Requires-Dist: pyfmi; extra == "extras"
 Requires-Dist: mayavi; extra == "extras"
 Requires-Dist: traits; extra == "extras"
 Requires-Dist: traitsui; extra == "extras"
 Requires-Dist: pyface; extra == "extras"
+Requires-Dist: jupyter; extra == "extras"
 Requires-Dist: pyiges; extra == "extras"
+Provides-Extra: difficult
+Requires-Dist: pyfmi; extra == "difficult"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
-Requires-Dist: jupyter; extra == "test"
 Requires-Dist: jupyter-book==0.15.1; extra == "test"
+Requires-Dist: flake8; extra == "test"
+Requires-Dist: pylint; extra == "test"
 
 # Loads Kernel
 
 <p align="left">
 <img width="200" src="./graphics/LK_logo2.png">
 </p>
 
 The Loads Kernel Software allows for the calculation of quasi-steady and dynamic maneuver loads, unsteady gust loads in the time and frequency domain as well as dynamic landing loads based on a generic landing gear module.
 
-[![DOI](https://zenodo.org/badge/537500844.svg)](https://zenodo.org/badge/latestdoi/537500844)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8341566.svg)](https://doi.org/10.5281/zenodo.8341566)
 
 # Theorectical Background & References
 
-[1] Voß, A., “Loads Kernel User Guide, Version 1.01,” Institut für Aeroelastik, Deutsches Zentrum für Luft- und Raumfahrt, Göttingen, Germany, Technical Report DLR-IB-AE-GO-2020-136, Nov. 2021, https://elib.dlr.de/140268/.
+[1] Voß, A., “Loads Kernel User Guide,” Institut für Aeroelastik, Deutsches Zentrum für Luft- und Raumfahrt, Göttingen, Germany, Technical Report DLR-IB-AE-GO-2020-136, Nov. 2021, https://elib.dlr.de/140268/.
 
 [2] Voß, A., “An Implementation of the Vortex Lattice and the Doublet Lattice Method,” Institut für Aeroelastik, Deutsches Zentrum für Luft- und Raumfahrt, Göttingen, Germany, Technical Report DLR-IB-AE-GO-2020-137, Oktober 2020, https://elib.dlr.de/136536/.
 
 If you use this software for your scientific work, we kindly ask you to include a reference [1,2] in your publications. Thank you!
 
 # Installation & Use
 ## Basic Installation 
-Install Loads Kernel as a python package with core dependencies via:
+Install Loads Kernel as a python package with its core dependencies using a package manager (PyPI or Conda):
 
 ```
 pip install LoadsKernel
 ```
 
+or
+
+```
+conda install -c conda-forge LoadsKernel
+```
+
 ## How can I use it?
 
 Copy and adjust the launch script (launch.py, example located in the [scripts folder](https://github.com/DLR-AE/LoadsKernel/tree/master/scripts)) to your needs / for your aircraft configuration. Then, launch the python script with:
 
 ```
 python launch.py
 ```
@@ -70,31 +79,36 @@
 Alternatively, if ~/.local/bin is in your system PATH, you can use the following commands from the command line:
 
 ```
 loads-kernel --job_name jcl_xy --pre True --main True --post True --path_input /path/to/JCLs --path_output /path/to/output
 ```
 
 ## Advanced Installation 
-
-As above, but with access to the code (keep the code where it is so that you can explore and modify):
+As above, but with access to the code (download and keep the code where it is so that you can explore and modify):
 
 ```
 git clone https://github.com/DLR-AE/LoadsKernel.git
 cd <local_repo_path>
 pip install -e . 
 ```
 
 To use the graphical tools and other features, optional libraries definded as extras are necessary:
 
 ```
 pip install -e .[extras]
 ```
 
-Note: Especially with mpi or the graphical libraries, pip frequently fails. In that case, try to install the failing packages using a
-package manager such as conda.
+or
+
+```
+conda install -c conda-forge loadskernel-extras
+```
+
+Note: Especially with mpi or the graphical libraries, pip frequently fails. In that case, try to install the missing/failing packages using a
+package manager such as conda, which is the more robust solution.
 
 There are two GUIs to visualize a simulation model (the Model Viewer) and to compare different sets of loads (Loads Compare), which can be started from the command line as well.
 
 ```
 model-viewer
 loads-compare
 ```
```

### Comparing `LoadsKernel-2024.2/README.md` & `loadskernel-2024.5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,32 +2,38 @@
 
 <p align="left">
 <img width="200" src="./graphics/LK_logo2.png">
 </p>
 
 The Loads Kernel Software allows for the calculation of quasi-steady and dynamic maneuver loads, unsteady gust loads in the time and frequency domain as well as dynamic landing loads based on a generic landing gear module.
 
-[![DOI](https://zenodo.org/badge/537500844.svg)](https://zenodo.org/badge/latestdoi/537500844)
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8341566.svg)](https://doi.org/10.5281/zenodo.8341566)
 
 # Theorectical Background & References
 
-[1] Voß, A., “Loads Kernel User Guide, Version 1.01,” Institut für Aeroelastik, Deutsches Zentrum für Luft- und Raumfahrt, Göttingen, Germany, Technical Report DLR-IB-AE-GO-2020-136, Nov. 2021, https://elib.dlr.de/140268/.
+[1] Voß, A., “Loads Kernel User Guide,” Institut für Aeroelastik, Deutsches Zentrum für Luft- und Raumfahrt, Göttingen, Germany, Technical Report DLR-IB-AE-GO-2020-136, Nov. 2021, https://elib.dlr.de/140268/.
 
 [2] Voß, A., “An Implementation of the Vortex Lattice and the Doublet Lattice Method,” Institut für Aeroelastik, Deutsches Zentrum für Luft- und Raumfahrt, Göttingen, Germany, Technical Report DLR-IB-AE-GO-2020-137, Oktober 2020, https://elib.dlr.de/136536/.
 
 If you use this software for your scientific work, we kindly ask you to include a reference [1,2] in your publications. Thank you!
 
 # Installation & Use
 ## Basic Installation 
-Install Loads Kernel as a python package with core dependencies via:
+Install Loads Kernel as a python package with its core dependencies using a package manager (PyPI or Conda):
 
 ```
 pip install LoadsKernel
 ```
 
+or
+
+```
+conda install -c conda-forge LoadsKernel
+```
+
 ## How can I use it?
 
 Copy and adjust the launch script (launch.py, example located in the [scripts folder](https://github.com/DLR-AE/LoadsKernel/tree/master/scripts)) to your needs / for your aircraft configuration. Then, launch the python script with:
 
 ```
 python launch.py
 ```
@@ -35,31 +41,36 @@
 Alternatively, if ~/.local/bin is in your system PATH, you can use the following commands from the command line:
 
 ```
 loads-kernel --job_name jcl_xy --pre True --main True --post True --path_input /path/to/JCLs --path_output /path/to/output
 ```
 
 ## Advanced Installation 
-
-As above, but with access to the code (keep the code where it is so that you can explore and modify):
+As above, but with access to the code (download and keep the code where it is so that you can explore and modify):
 
 ```
 git clone https://github.com/DLR-AE/LoadsKernel.git
 cd <local_repo_path>
 pip install -e . 
 ```
 
 To use the graphical tools and other features, optional libraries definded as extras are necessary:
 
 ```
 pip install -e .[extras]
 ```
 
-Note: Especially with mpi or the graphical libraries, pip frequently fails. In that case, try to install the failing packages using a
-package manager such as conda.
+or
+
+```
+conda install -c conda-forge loadskernel-extras
+```
+
+Note: Especially with mpi or the graphical libraries, pip frequently fails. In that case, try to install the missing/failing packages using a
+package manager such as conda, which is the more robust solution.
 
 There are two GUIs to visualize a simulation model (the Model Viewer) and to compare different sets of loads (Loads Compare), which can be started from the command line as well.
 
 ```
 model-viewer
 loads-compare
 ```
```

### Comparing `LoadsKernel-2024.2/loadscompare/compare.py` & `loadskernel-2024.5/loadscompare/compare.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -*- coding: utf-8 -*-
 import os
+from itertools import compress
 
 from pyface.qt import QtCore
 from pyface.qt.QtGui import (QApplication, QWidget, QTabWidget, QSizePolicy, QGridLayout, QMainWindow, QAction, QListWidget,
                              QListWidgetItem, QAbstractItemView, QFileDialog, QComboBox, QCheckBox, QLabel)
 import matplotlib
 from matplotlib.backends.backend_qt5agg import FigureCanvasQTAgg, NavigationToolbar2QT
 from matplotlib.figure import Figure
@@ -202,36 +203,39 @@
 
     def update_desc(self, *args):
         self.datasets['desc'][self.lb_dataset.currentRow()] = self.lb_dataset.currentItem().text()
         self.update_plot()
 
     def update_plot(self):
         if self.lb_dataset.currentItem() is not None and self.lb_mon.currentItem() is not None:
-            # Reverse current selection of datasets for plotting. The dataset added/created last is plotted first.
-            # This is useful for example after merging different datasets. The resulting dataset would obscure the view if
-            # plotted last.
-            current_selection = [item.row() for item in self.lb_dataset.selectedIndexes()]
-            dataset_sel = [self.datasets['dataset'][i] for i in current_selection]
-            color_sel = [self.datasets['color'][i] for i in current_selection]
-            desc_sel = [self.datasets['desc'][i] for i in current_selection]
+            # Get the items selected by the user.
             mon_sel = self.common_monstations[self.lb_mon.currentRow()]
-            n_subcases = [len(dataset[mon_sel]['subcases']) for dataset in dataset_sel]
-
-            self.plotting.potato_plots(dataset_sel,
+            dataset_sel = [item.row() for item in self.lb_dataset.selectedIndexes()]
+            # Check that monitoring stations exists in all selected datasets.
+            mon_existing = [mon_sel in self.datasets['dataset'][i] for i in dataset_sel]
+            dataset_sel = list(compress(dataset_sel, mon_existing))
+            # Get the selected datasets, colors and a description.
+            datasets = [self.datasets['dataset'][i] for i in dataset_sel]
+            colors = [self.datasets['color'][i] for i in dataset_sel]
+            desciptions = [self.datasets['desc'][i] for i in dataset_sel]
+            # Call the plotting function.
+            self.plotting.potato_plots(datasets,
                                        mon_sel,
-                                       desc_sel,
-                                       color_sel,
+                                       desciptions,
+                                       colors,
                                        self.cb_xaxis.currentIndex(),
                                        self.cb_yaxis.currentIndex(),
                                        self.cb_xaxis.currentText(),
                                        self.cb_yaxis.currentText(),
                                        self.cb_hull.isChecked(),
                                        self.cb_labels.isChecked(),
                                        self.cb_minmax.isChecked(),
                                        )
+            # Update the text box with number of plotted load cases.
+            n_subcases = [len(dataset[mon_sel]['subcases']) for dataset in datasets]
             self.label_n_loadcases.setText('Selected load case: {}'.format(np.sum(n_subcases)))
         else:
             self.plotting.plot_nothing()
         self.canvas.draw()
 
     def merge_monstation(self):
         if len(self.lb_dataset.selectedItems()) > 1:
@@ -302,15 +306,17 @@
     def update_fields(self):
         self.lb_dataset.clear()
         for desc in self.datasets['desc']:
             item = QListWidgetItem(desc)
             item.setFlags(item.flags() | QtCore.Qt.ItemIsEditable)
             self.lb_dataset.addItem(item)
 
-        keys = [list(dataset) for dataset in self.datasets['dataset']]
+        keys = []
+        for dataset in self.datasets['dataset']:
+            keys += dataset.keys()
         self.common_monstations = np.unique(keys)
         self.lb_mon.clear()
         for x in self.common_monstations:
             self.lb_mon.addItem(QListWidgetItem(x))
 
 
 def command_line_interface():
```

### Comparing `LoadsKernel-2024.2/loadscompare/graphics/LK_logo2.png` & `loadskernel-2024.5/loadscompare/graphics/LK_logo2.png`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadscompare/plotting.py` & `loadskernel-2024.5/loadscompare/plotting.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/atmosphere.py` & `loadskernel-2024.5/loadskernel/atmosphere.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/auxiliary_output.py` & `loadskernel-2024.5/loadskernel/auxiliary_output.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/build_aero_functions.py` & `loadskernel-2024.5/loadskernel/build_aero_functions.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/build_splinegrid.py` & `loadskernel-2024.5/loadskernel/build_splinegrid.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/cfd_interfaces/meshdefo.py` & `loadskernel-2024.5/loadskernel/cfd_interfaces/meshdefo.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/cfd_interfaces/mpi_helper.py` & `loadskernel-2024.5/loadskernel/cfd_interfaces/mpi_helper.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/cfd_interfaces/su2_interface.py` & `loadskernel-2024.5/loadskernel/cfd_interfaces/su2_interface.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/cfd_interfaces/tau_interface.py` & `loadskernel-2024.5/loadskernel/cfd_interfaces/tau_interface.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/engine_interfaces/engine.py` & `loadskernel-2024.5/loadskernel/engine_interfaces/engine.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/engine_interfaces/propeller.py` & `loadskernel-2024.5/loadskernel/engine_interfaces/propeller.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/equations/cfd.py` & `loadskernel-2024.5/loadskernel/equations/cfd.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,14 @@
                         'Pk_idrag': Pk_idrag,
                         'q_dyn': np.array([q_dyn]),
                         'Pb': Pb,
                         'Pmac': self.PHIcg_mac.T.dot(self.PHIcfd_cg.T).dot(Pcfd),
                         'Pf': Pf,
                         'alpha': np.array([alpha]),
                         'beta': np.array([beta]),
-                        # 'Pg_aero': np.dot(PHIk_strc.T, Pk_aero),
                         'Ux2': Ux2,
                         'dUcg_dt': dUcg_dt,
                         'd2Ucg_dt2': d2Ucg_dt2,
                         'Uf': Uf,
                         'dUf_dt': dUf_dt,
                         'd2Uf_dt2': d2Uf_dt2,
                         'Nxyz': Nxyz,
```

### Comparing `LoadsKernel-2024.2/loadskernel/equations/common.py` & `loadskernel-2024.5/loadskernel/equations/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -266,34 +266,34 @@
             # supersonic aero with NP at 50% (ZONA51)
             Pk = Pl
         else:
             # subsonic aero with NP at 25% (VLM/DLM)
             Pk = self.PHIlk.T.dot(Pl)
         return Pk
 
-    def rbm_nonlin(self, dUcg_dt, alpha, Vtas):
+    def rbm_nonlin(self, dUcg_dt):
         dUmac_dt = np.dot(self.PHImac_cg, dUcg_dt)  # auch bodyfixed
         Ujx1 = np.dot(self.Djx1, dUmac_dt)
         # der downwash wj ist nur die Komponente von Uj, welche senkrecht zum Panel steht!
         # --> mit N multiplizieren und danach die Norm bilden
         wj = np.sum(self.aerogrid['N'][:] * Ujx1[self.aerogrid['set_j'][:, (0, 1, 2)]], axis=1)
         Pk = self.calc_Pk_nonlin(dUmac_dt, wj)
         return Pk, wj
 
-    def rbm(self, dUcg_dt, alpha, q_dyn, Vtas):
+    def rbm(self, dUcg_dt, q_dyn, Vtas):
         dUmac_dt = np.dot(self.PHImac_cg, dUcg_dt)  # auch bodyfixed
         Ujx1 = np.dot(self.Djx1, dUmac_dt)
         # der downwash wj ist nur die Komponente von Uj, welche senkrecht zum Panel steht!
         # --> mit N multiplizieren und danach die Norm bilden
         wj = np.sum(self.aerogrid['N'][:] * Ujx1[self.aerogrid['set_j'][:, (0, 1, 2)]], axis=1) / Vtas * -1
         Pk = self.calc_Pk(q_dyn, wj)
         return Pk, wj
 
-    def camber_twist_nonlin(self, dUcg_dt):
-        wj = np.sin(self.cam_rad) * -1.0
+    def camber_twist_nonlin(self, dUcg_dt, Vtas):
+        wj = np.sin(self.cam_rad) * np.sign(self.aerogrid['N'][:, 2]) * -Vtas
         dUmac_dt = np.dot(self.PHImac_cg, dUcg_dt)  # auch bodyfixed
         Pk = self.calc_Pk_nonlin(dUmac_dt, wj)
         return Pk, wj
 
     def camber_twist(self, q_dyn):
         """
         Multiplication with the sign of the z-direction of the panel normal vector ensures compatibility
@@ -610,21 +610,21 @@
                 * self.jcl.general['A_ref'] * self.jcl.general['b_ref'] * beta
         return Pb_corr
 
     def vdrag(self, alpha, q_dyn):
         Pmac = np.zeros(6)
         if 'viscous_drag' in self.jcl.aero and self.jcl.aero['viscous_drag'] == 'coefficients':
             if 'Cd_0' in self.jcl.aero:
-                Cd0 = self.aero['Cd_0']
+                Cd0 = self.jcl.aero['Cd_0']
             else:
-                Cd0 = 0.012
-            if 'Cd_0' in self.jcl.aero:
-                Cd_alpha_sq = self.aero['Cd_alpha^2']
+                Cd0 = 0.0
+            if 'Cd_alpha^2' in self.jcl.aero:
+                Cd_alpha_sq = self.jcl.aero['Cd_alpha^2']
             else:
-                Cd_alpha_sq = 0.018
+                Cd_alpha_sq = 0.0
             Pmac[0] = q_dyn * self.jcl.general['A_ref'] * (Cd0 + Cd_alpha_sq * alpha ** 2.0)
         return Pmac
 
     def landinggear(self, X, Tbody2geo):
         Pextra = np.zeros(self.extragrid['n'] * 6)
         F1 = np.zeros(self.extragrid['n'])
         F2 = np.zeros(self.extragrid['n'])
```

### Comparing `LoadsKernel-2024.2/loadskernel/equations/frequency_domain.py` & `loadskernel-2024.5/loadskernel/equations/frequency_domain.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/equations/landing.py` & `loadskernel-2024.5/loadskernel/equations/landing.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,23 +12,22 @@
         dUcg_dt, Uf, dUf_dt = self.recover_states(X)
         Vtas, q_dyn = self.recover_Vtas(X)
         onflow = self.recover_onflow(X)
         alpha, beta, gamma = self.windsensor(X, Vtas, Uf, dUf_dt)
         Ux2 = self.get_Ux2(X)
 
         # aerodynamics
-        Pk_rbm, wj_rbm = self.rbm(onflow, alpha, q_dyn, Vtas)
+        Pk_rbm, wj_rbm = self.rbm(onflow, q_dyn, Vtas)
         Pk_cam, wj_cam = self.camber_twist(q_dyn)
         Pk_cs, wj_cs = self.cs(X, Ux2, q_dyn)
         Pk_f, wj_f = self.flexible(Uf, dUf_dt, onflow, q_dyn, Vtas)
         Pk_gust, wj_gust = self.gust(X, q_dyn)
 
         wj = wj_rbm + wj_cam + wj_cs + wj_f + wj_gust
         Pk_idrag = self.idrag(wj, q_dyn)
-
         Pk_unsteady = Pk_rbm * 0.0
 
         # correction coefficients
         Pb_corr = self.correctioon_coefficients(alpha, beta, q_dyn)
 
         # landing gear
         Pextra, _, dp2, ddp2, F1, F2 = self.landinggear(X, Tbody2geo)
@@ -100,15 +99,14 @@
                         'Pk_idrag': Pk_idrag,
                         'q_dyn': np.array([q_dyn]),
                         'Pb': Pb,
                         'Pmac': Pmac,
                         'Pf': Pf,
                         'alpha': np.array([alpha]),
                         'beta': np.array([beta]),
-                        # 'Pg_aero': np.dot(PHIk_strc.T, Pk_aero),
                         'Ux2': Ux2,
                         'dUcg_dt': dUcg_dt,
                         'd2Ucg_dt2': d2Ucg_dt2,
                         'Uf': Uf,
                         'dUf_dt': dUf_dt,
                         'd2Uf_dt2': d2Uf_dt2,
                         'Nxyz': Nxyz,
```

### Comparing `LoadsKernel-2024.2/loadskernel/equations/nonlin_steady.py` & `loadskernel-2024.5/loadskernel/equations/nonlin_steady.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,39 +13,41 @@
         dUcg_dt, Uf, dUf_dt = self.recover_states(X)
         Vtas, q_dyn = self.recover_Vtas(X)
         onflow = self.recover_onflow(X)
         alpha, beta, gamma = self.windsensor(X, Vtas, Uf, dUf_dt)
         Ux2 = self.get_Ux2(X)
 
         # aerodynamics
-        Pk_rbm, wj_rbm = self.rbm_nonlin(onflow, alpha, Vtas)
+        Pk_rbm, wj_rbm = self.rbm_nonlin(onflow)
+        Pk_cam, wj_cam = self.camber_twist_nonlin(onflow, Vtas)
         Pk_cs, wj_cs = self.cs_nonlin(onflow, X, Ux2, Vtas)
         Pk_f, wj_f = self.flexible_nonlin(onflow, Uf, dUf_dt, Vtas)
-        Pk_cam, wj_cam = self.camber_twist_nonlin(onflow)
+        Pk_gust = Pk_rbm * 0.0
 
-        wj = (wj_rbm + wj_cs + wj_f + wj_cam) / Vtas
+        wj = (wj_rbm + wj_cam + wj_cs + wj_f) / Vtas
         Pk_idrag = self.idrag(wj, q_dyn)
 
-        Pk_gust = Pk_rbm * 0.0
         Pk_unsteady = Pk_rbm * 0.0
 
+        Pextra, Pb_ext, Pf_ext = self.engine(X, Vtas, q_dyn, Uf, dUf_dt, t)
+
         # correction coefficients
         Pb_corr = self.correctioon_coefficients(alpha, beta, q_dyn)
         Pmac_vdrag = self.vdrag(alpha, q_dyn)
 
         # summation of forces
         Pk_aero = Pk_rbm + Pk_cam + Pk_cs + Pk_f + Pk_gust + Pk_idrag + Pk_unsteady
         Pmac = np.dot(self.Dkx1.T, Pk_aero) + Pmac_vdrag
-        Pb = np.dot(self.PHImac_cg.T, Pmac) + Pb_corr
+        Pb = np.dot(self.PHImac_cg.T, Pmac) + Pb_corr + Pb_ext
 
         g_cg = gravitation_on_earth(self.PHInorm_cg, Tgeo2body)
 
         # EoM
         d2Ucg_dt2, Nxyz = self.rigid_EoM(dUcg_dt, Pb, g_cg, modus)
-        Pf = np.dot(self.PHIkf.T, Pk_aero) + self.Mfcg.dot(np.hstack((d2Ucg_dt2[0:3] - g_cg, d2Ucg_dt2[3:6])))
+        Pf = np.dot(self.PHIkf.T, Pk_aero) + self.Mfcg.dot(np.hstack((d2Ucg_dt2[0:3] - g_cg, d2Ucg_dt2[3:6]))) + Pf_ext
         d2Uf_dt2 = self.flexible_EoM(dUf_dt, Uf, Pf)
 
         # CS derivatives
         dcommand = self.get_command_derivatives(t, X, Vtas, gamma, alpha, beta, Nxyz, np.dot(Tbody2geo, X[6:12])[0:3])
 
         # output
         Y = np.hstack((np.dot(Tbody2geo, X[6:12]),
@@ -75,19 +77,18 @@
                         'Pmac_vdrag': Pmac_vdrag,
                         'q_dyn': np.array([q_dyn]),
                         'Pb': Pb,
                         'Pmac': Pmac,
                         'Pf': Pf,
                         'alpha': np.array([alpha]),
                         'beta': np.array([beta]),
-                        # 'Pg_aero': np.dot(PHIk_strc.T, Pk_aero),
                         'Ux2': Ux2,
                         'dUcg_dt': dUcg_dt,
                         'd2Ucg_dt2': d2Ucg_dt2,
                         'Uf': Uf,
                         'dUf_dt': dUf_dt,
                         'd2Uf_dt2': d2Uf_dt2,
                         'Nxyz': Nxyz,
                         'g_cg': g_cg,
-                        'Pextra': [],
+                        'Pextra': Pextra,
                         }
             return response
```

### Comparing `LoadsKernel-2024.2/loadskernel/equations/state_space.py` & `loadskernel-2024.5/loadskernel/equations/state_space.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/equations/steady.py` & `loadskernel-2024.5/loadskernel/equations/steady.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,23 +15,22 @@
         dUcg_dt, Uf, dUf_dt = self.recover_states(X)
         Vtas, q_dyn = self.recover_Vtas(X)
         onflow = self.recover_onflow(X)
         alpha, beta, gamma = self.windsensor(X, Vtas, Uf, dUf_dt)
         Ux2 = self.get_Ux2(X)
 
         # aerodynamics
-        Pk_rbm, wj_rbm = self.rbm(onflow, alpha, q_dyn, Vtas)
+        Pk_rbm, wj_rbm = self.rbm(onflow, q_dyn, Vtas)
         Pk_cam, wj_cam = self.camber_twist(q_dyn)
         Pk_cs, wj_cs = self.cs(X, Ux2, q_dyn)
         Pk_f, wj_f = self.flexible(Uf, dUf_dt, onflow, q_dyn, Vtas)
         Pk_gust, wj_gust = self.gust(X, q_dyn)
 
         wj = wj_rbm + wj_cam + wj_cs + wj_f + wj_gust
         Pk_idrag = self.idrag(wj, q_dyn)
-
         Pk_unsteady = Pk_rbm * 0.0
 
         Pextra, Pb_ext, Pf_ext = self.engine(X, Vtas, q_dyn, Uf, dUf_dt, t)
 
         # correction coefficients
         Pb_corr = self.correctioon_coefficients(alpha, beta, q_dyn)
```

### Comparing `LoadsKernel-2024.2/loadskernel/equations/unsteady.py` & `loadskernel-2024.5/loadskernel/equations/unsteady.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,60 +11,59 @@
         Tgeo2body, Tbody2geo = self.geo2body(X)
         dUcg_dt, Uf, dUf_dt = self.recover_states(X)
         Vtas, q_dyn = self.recover_Vtas(self.X0)
         onflow = self.recover_onflow(X)
         alpha, beta, gamma = self.windsensor(X, Vtas, Uf, dUf_dt)
         Ux2 = self.get_Ux2(X)
 
-        # --- aerodynamics ---
-        Pk_rbm, wj_rbm = self.rbm(onflow, alpha, q_dyn, Vtas)
+        # aerodynamics
+        Pk_rbm, wj_rbm = self.rbm(onflow, q_dyn, Vtas)
         Pk_cam, wj_cam = self.camber_twist(q_dyn)
         Pk_cs, wj_cs = self.cs(X, Ux2, q_dyn)
         Pk_f, wj_f = self.flexible(Uf, dUf_dt, onflow, q_dyn, Vtas)
         Pk_gust, wj_gust = self.gust(X, q_dyn)
 
         wj = wj_rbm + wj_cam + wj_cs + wj_f + wj_gust
         Pk_idrag = self.idrag(wj, q_dyn)
         Pk_unsteady, dlag_states_dt = self.unsteady(X, t, wj, Uf, dUf_dt, onflow, q_dyn, Vtas)
 
         Pextra, Pb_ext, Pf_ext = self.engine(X, Vtas, q_dyn, Uf, dUf_dt, t)
 
-        # --- correction coefficients ---
+        # correction coefficients
         Pb_corr = self.correctioon_coefficients(alpha, beta, q_dyn)
 
-        # --- summation of forces ---
+        # summation of forces
         Pk_aero = Pk_rbm + Pk_cam + Pk_cs + Pk_f + Pk_gust + Pk_idrag + Pk_unsteady
         Pmac = np.dot(self.Dkx1.T, Pk_aero)
         Pb = np.dot(self.PHImac_cg.T, Pmac) + Pb_corr + Pb_ext
 
         g_cg = gravitation_on_earth(self.PHInorm_cg, Tgeo2body)
 
-        # --- EoM ---
+        # EoM
         d2Ucg_dt2, Nxyz = self.rigid_EoM(dUcg_dt, Pb, g_cg, modus)
         Pf = np.dot(self.PHIkf.T, Pk_aero) + self.Mfcg.dot(np.hstack((d2Ucg_dt2[0:3] - g_cg, d2Ucg_dt2[3:6]))) + Pf_ext
         d2Uf_dt2 = self.flexible_EoM(dUf_dt, Uf, Pf)
 
-        # --- CS derivatives ---
+        # CS derivatives
         dcommand = self.get_command_derivatives(t, X, Vtas, gamma, alpha, beta, Nxyz, np.dot(Tbody2geo, X[6:12])[0:3])
 
-        # --- output ---
+        # output
         Y = np.hstack((np.dot(Tbody2geo, X[6:12]),
                        np.dot(self.PHIcg_norm, d2Ucg_dt2),
                        dUf_dt,
                        d2Uf_dt2,
                        dcommand,
                        dlag_states_dt,
                        Nxyz[2],
                        Vtas,
                        beta,
                        ))
 
         if modus in ['trim', 'sim']:
             return Y
-
         elif modus in ['trim_full_output']:
             response = {'X': X,
                         'Y': Y,
                         't': np.array([t]),
                         'Pk_rbm': Pk_rbm,
                         'Pk_cam': Pk_cam,
                         'Pk_aero': Pk_aero,
@@ -86,15 +85,14 @@
                         'dUf_dt': dUf_dt,
                         'd2Uf_dt2': d2Uf_dt2,
                         'Nxyz': Nxyz,
                         'g_cg': g_cg,
                         'Pextra': Pextra,
                         }
             return response
-
         elif modus in ['sim_full_output']:
             # For time domain simulations, typically not all results are required. To reduce the amount of data while
             # maintaining compatibility with the trim, empty arrays are used.
             response = {'X': X,
                         'Y': Y,
                         't': np.array([t]),
                         'Pk_aero': Pk_aero,
```

### Comparing `LoadsKernel-2024.2/loadskernel/fem_interfaces/b2000_interface.py` & `loadskernel-2024.5/loadskernel/fem_interfaces/b2000_interface.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/fem_interfaces/cofe_interface.py` & `loadskernel-2024.5/loadskernel/fem_interfaces/cofe_interface.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/fem_interfaces/nastran_f06_interface.py` & `loadskernel-2024.5/loadskernel/fem_interfaces/nastran_f06_interface.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/fem_interfaces/nastran_interface.py` & `loadskernel-2024.5/loadskernel/fem_interfaces/nastran_interface.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/gather_loads.py` & `loadskernel-2024.5/loadskernel/gather_loads.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/graphics/LK_logo2.png` & `loadskernel-2024.5/loadskernel/graphics/LK_logo2.png`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/grid_trafo.py` & `loadskernel-2024.5/loadskernel/grid_trafo.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/integrate.py` & `loadskernel-2024.5/loadskernel/integrate.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/interpolate.py` & `loadskernel-2024.5/loadskernel/interpolate.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/io_functions/bdf_cards.py` & `loadskernel-2024.5/loadskernel/io_functions/bdf_cards.py`

 * *Files 6% similar despite different names*

```diff
@@ -91,14 +91,39 @@
                 card[name].append(nastran_number_converter(my_field, field_type, default_value))
                 i += 1
             else:
                 break
         return card
 
 
+class StringCard(SimpleCard):
+
+    @classmethod
+    def parse(cls, card_as_string, _):
+        card = cls.parse_string(cls, card_as_string)
+        return card
+
+    def parse_string(self, card_as_string):
+        # create an empty dictionary to store the card
+        card = {}
+        name = self.field_names[0]
+        """
+        This is the decision logic to parse fields:
+        Case 1: See if the card is suffiently long --> the field exists
+        Case 2: The field is missing --> issue a warning
+        """
+        if len(card_as_string) > 0:
+            # convert field and store in dictionary
+            tmp = card_as_string.strip("'*, ")
+            card[name] = tmp.replace(" ", "")
+        else:
+            logging.error('Field {} expected but missing in {} card: {}'.format(name, type(self).__name__, card_as_string))
+        return card
+
+
 class GRID(SimpleCard):
     expected_lines = 1
     # field of interest (any other fields are not implemented)
     field_names = ['ID', 'CP', 'X1', 'X2', 'X3', 'CD']
     field_positions = [0, 1, 2, 3, 4, 5]
     field_types = ['int', 'int', 'float', 'float', 'float', 'int']
     optional_fields = ['CP', 'CD']
@@ -229,7 +254,14 @@
     field_names = ['ID', 'values']
     field_positions = [0, 1]
     # Due to the mixture of integers and strings ('THRU') in a SET1 card, all list items are parsed as strings.
     field_types = ['int', 'str']
     # Blank strings (e.g. trailing spaces) shall be replaced with None.
     optional_fields = ['ID', 'values']
     optional_defaults = [123456, None]
+
+
+class INCLUDE(StringCard):
+    expected_lines = None
+    # field of interest (any other fields are not implemented)
+    field_names = ['filename']
+    field_types = ['str']
```

### Comparing `LoadsKernel-2024.2/loadskernel/io_functions/data_handling.py` & `loadskernel-2024.5/loadskernel/io_functions/data_handling.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/io_functions/read_bdf.py` & `loadskernel-2024.5/loadskernel/io_functions/read_bdf.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 This is a simple and light-weight BDF reader which consist of only two scripts (read_bdf.py & bdf_cards.py),
 and parses Nastran BDF files to Pandas data frames. It considers only those cards and fields actually needed
 for a loads analysis using Loads Kernel, providing maximum compatibility and speed and comes without further
 dependencies.
 Some ideas and concepts are inspired by pyBDF, a comprehensive DLR in-house BDF reader by Markus Zimmer.
 """
 
-import copy
 import logging
 import os
 
 import pandas as pd
 
 from loadskernel.io_functions import bdf_cards
 
@@ -27,23 +26,22 @@
                          'SET1': bdf_cards.SET1,
                          'AEFACT': bdf_cards.AEFACT,
                          'CAERO1': bdf_cards.CAERO1,
                          'CAERO7': bdf_cards.CAERO7,
                          'AESURF': bdf_cards.AESURF,
                          'AELIST': bdf_cards.AELIST,
                          'ASET1': bdf_cards.ASET1,
+                         'INCLUDE': bdf_cards.INCLUDE,
                          }
 
     def __init__(self):
         # This is the storage for processed files
         self.processed_files = []
         # This is the line storage
         self.lines = []
-        # This is the include storage
-        self.includes = []
         # This is a list of all known / implemented cards
         self.known_cards = self.card_interpreters.keys()
         # The cards are stored in a Pandas data frames, one frame per type of card.
         # The data frames themselfes are stored in a dictionary.
         self.cards = {}
         for card_name in self.known_cards:
             # Make sure the colums of the data frame have the correct type (int or float)
@@ -53,58 +51,68 @@
             df_definition = {}
             for c, t in zip(card_class.field_names, card_class.field_types):
                 df_definition[c] = pd.Series(dtype=t)
             # Create the data frame
             self.cards[card_name] = pd.DataFrame(df_definition)
 
     def process_deck(self, deck):
-        # Make sure deck is a list of filenames, not a single string
-        if isinstance(deck, str):
-            self.filenames = [deck]
-        else:
-            self.filenames = deck
         """
-        This is the iterative loop to capture all include statements.
+        This function parses a whole 'deck' of files and captures all include statements.
         Step 1: In case include statements are found, move them to filenames.
         Step 2: Re-run process_deck()
         Step 3: This loop terminates when the include list is empty, i.e. no more includes are found.
         """
-        self.read_lines_from_files()
-        self.read_cards_from_lines()
-
-        if self.includes:
-            logging.info('Found include(s):')
-            self.filenames = copy.deepcopy(self.includes)
-            self.includes = []
-            self.process_deck(self.filenames)
+        # Make sure the deck is a list of filenames, not a single string
+        if isinstance(deck, str):
+            filenames = [deck]
+        else:
+            filenames = deck
 
+        for filename in filenames:
+            # Parse all lines.
+            self.read_lines_from_file(filename)
+            # Interprete all lines.
+            self.read_cards_from_lines()
+            # In case include statements are found, move them to self.includes.
+            # At the same time, establish the path to the included file.
+            root = os.path.dirname(filename)
+            includes = []
+            for filename_include in self.cards['INCLUDE'].squeeze().to_list():
+                if os.path.isabs(filename_include):
+                    includes += [filename_include]
+                else:
+                    includes += [os.path.join(root, filename_include)]
+            self.cards['INCLUDE'].drop(self.cards['INCLUDE'].index, inplace=True)
+            # Re-run process_deck()
+            if includes:
+                logging.info('Found include(s):')
+                self.process_deck(includes)
+        # Do some post-processing
         self.aggregate_cards(['ASET1'])
         self.remove_duplicate_cards()
         return
 
-    def read_lines_from_files(self):
+    def read_lines_from_file(self, filename):
         # reset the line storage before reading new files
         self.lines = []
-        # loop over all filenames and read all lines
-        for filename in self.filenames:
-            # to save time, make sure the same file is not parsed twice
-            if filename in self.processed_files:
-                logging.info('File already processed: {}'.format(filename))
-            # make sure the given filename exists, if not, skip that file
-            elif os.path.exists(filename):
-                logging.info('Read from file: {}'.format(filename))
-                with open(filename, 'r') as fid:
-                    self.lines += fid.readlines()
-                self.processed_files += [filename]
-            else:
-                logging.warning('File NOT found: {}'.format(filename))
+        # to save time, make sure the same file is not parsed twice
+        if filename in self.processed_files:
+            logging.info('File already processed: {}'.format(filename))
+        # make sure the given filename exists, if not, skip that file
+        elif os.path.exists(filename):
+            logging.info('Read from file: {}'.format(filename))
+            with open(filename, 'r') as fid:
+                self.lines += fid.readlines()
+        else:
+            logging.warning('File NOT found: {}'.format(filename))
+        self.processed_files += [filename]
 
     def read_cards_from_lines(self):
         if self.lines:
-            logging.info('Read BDF cards from {} lines...'.format(len(self.lines)))
+            logging.debug('Read BDF cards from {} lines...'.format(len(self.lines)))
         # loop over all lines until empty
         while self.lines:
             # test the first 8 characters of the line for a known card
             card_name = self.lines[0][:8].strip('*, ').upper()
             if card_name in self.known_cards:
                 # get the corresponding interpeter
                 card_class = self.card_interpreters[card_name]
```

### Comparing `LoadsKernel-2024.2/loadskernel/io_functions/read_cfdgrids.py` & `loadskernel-2024.5/loadskernel/io_functions/read_cfdgrids.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/io_functions/read_h5.py` & `loadskernel-2024.5/loadskernel/io_functions/read_h5.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/io_functions/read_mona.py` & `loadskernel-2024.5/loadskernel/io_functions/read_mona.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/io_functions/read_op2.py` & `loadskernel-2024.5/loadskernel/io_functions/read_op2.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/io_functions/read_op4.py` & `loadskernel-2024.5/loadskernel/io_functions/read_op4.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/io_functions/write_mona.py` & `loadskernel-2024.5/loadskernel/io_functions/write_mona.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/jcl_helper.py` & `loadskernel-2024.5/loadskernel/jcl_helper.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/model.py` & `loadskernel-2024.5/loadskernel/model.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/plotting_extra.py` & `loadskernel-2024.5/loadskernel/plotting_extra.py`

 * *Files 13% similar despite different names*

```diff
@@ -88,33 +88,34 @@
         # Loop over responses and fill plots with data
         for response in self.responses:
             trimcase = self.jcl.trimcase[response['i'][()]]
             logging.info('plotting for simulation {:s}'.format(trimcase['desc']))
 
             self.n_modes = self.model['mass'][trimcase['mass']]['n_modes'][()]
 
-            Cl = response['Pmac'][:, 2] / response['q_dyn'][:].T / self.jcl.general['A_ref']
-            ax11.plot(response['t'], response['Pmac'][:, 2], 'b-')
-            ax12.plot(response['t'], Cl.T, 'b-')
+            if self.jcl.aero['method'] in ['mona_steady', 'mona_unsteady']:
+                Cl = response['Pmac'][:, 2] / response['q_dyn'][:].T / self.jcl.general['A_ref']
+                ax11.plot(response['t'], response['Pmac'][:, 2], 'b-')
+                ax12.plot(response['t'], Cl.T, 'b-')
+
+                ax21.plot(response['t'], response['q_dyn'], 'k-')
+                ax22.plot(response['t'], response['alpha'][:] / np.pi * 180.0, 'r-')
+                ax22.plot(response['t'], response['beta'][:] / np.pi * 180.0, 'c-')
+                ax23.plot(response['t'], response['Nxyz'][:, 1], 'g-')
+                ax23.plot(response['t'], response['Nxyz'][:, 2], 'b-')
 
             if self.jcl.aero['method'] in ['mona_unsteady']:
                 Pb_gust = []
                 Pb_unsteady = []
                 for i_step in range(len(response['t'])):
                     Pb_gust.append(np.dot(Dkx1.T, response['Pk_gust'][i_step, :])[2])
                     Pb_unsteady.append(np.dot(Dkx1.T, response['Pk_unsteady'][i_step, :])[2])
                 ax11.plot(response['t'], Pb_gust, 'k-')
                 ax11.plot(response['t'], Pb_unsteady, 'r-')
 
-            ax21.plot(response['t'], response['q_dyn'], 'k-')
-            ax22.plot(response['t'], response['alpha'][:] / np.pi * 180.0, 'r-')
-            ax22.plot(response['t'], response['beta'][:] / np.pi * 180.0, 'c-')
-            ax23.plot(response['t'], response['Nxyz'][:, 1], 'g-')
-            ax23.plot(response['t'], response['Nxyz'][:, 2], 'b-')
-
             ax32.plot(response['t'], response['X'][:, 3] / np.pi * 180.0, 'b-')
             ax32.plot(response['t'], response['X'][:, 4] / np.pi * 180.0, 'g-')
             ax32.plot(response['t'], response['X'][:, 5] / np.pi * 180.0, 'r-')
 
             ax41.plot(response['t'], response['X'][:, 6], 'b-')
             ax41.plot(response['t'], response['X'][:, 7], 'g-')
             ax41.plot(response['t'], response['X'][:, 8], 'r-')
@@ -209,14 +210,91 @@
             ax72.set_xlabel('t [s]')
             ax72.set_ylabel('F1 [N]')
             ax72.grid(True)
 
         # Show plots
         plt.show()
 
+    def plot_forces_deformation_interactive(self):
+
+        # loop over all responses
+        for response in self.responses:
+            trimcase = self.jcl.trimcase[response['i'][()]]
+            logging.info('interactive plotting of forces and deformations for trim {:s}'.format(trimcase['desc']))
+
+            # plot aerodynamic forces
+            x = self.aerogrid['offset_k'][:, 0]
+            y = self.aerogrid['offset_k'][:, 1]
+            z = self.aerogrid['offset_k'][:, 2]
+            fscale = 0.5 * self.model_size / np.max(np.abs(response['Pk_aero'][0][self.aerogrid['set_k'][:, (0, 1, 2)]]))
+            for name in ['Pk_aero', 'Pk_rbm', 'Pk_cam', 'Pk_cs', 'Pk_f', 'Pk_idrag']:
+                if response[name][0].sum() != 0.0:
+                    fx = response[name][0][self.aerogrid['set_k'][:, 0]]
+                    fy = response[name][0][self.aerogrid['set_k'][:, 1]]
+                    fz = response[name][0][self.aerogrid['set_k'][:, 2]]
+                    mlab.figure()
+                    mlab.points3d(x, y, z, scale_factor=self.pscale)
+                    mlab.quiver3d(x, y, z, fx, fy, fz, color=(0, 1, 0), scale_factor=fscale)
+                    mlab.title(name, size=0.5, height=0.9)
+                else:
+                    logging.info('Forces {} are zero, skip plotting'.format(name))
+
+            # plot structural deformations
+            x = self.strcgrid['offset'][:, 0]
+            y = self.strcgrid['offset'][:, 1]
+            z = self.strcgrid['offset'][:, 2]
+            x_r = self.strcgrid['offset'][:, 0] + response['Ug_r'][0][self.strcgrid['set'][:, 0]]
+            y_r = self.strcgrid['offset'][:, 1] + response['Ug_r'][0][self.strcgrid['set'][:, 1]]
+            z_r = self.strcgrid['offset'][:, 2] + response['Ug_r'][0][self.strcgrid['set'][:, 2]]
+            x_f = self.strcgrid['offset'][:, 0] + response['Ug'][0][self.strcgrid['set'][:, 0]]
+            y_f = self.strcgrid['offset'][:, 1] + response['Ug'][0][self.strcgrid['set'][:, 1]]
+            z_f = self.strcgrid['offset'][:, 2] + response['Ug'][0][self.strcgrid['set'][:, 2]]
+
+            mlab.figure()
+            mlab.points3d(x_r, y_r, z_r, color=(0, 1, 0), scale_factor=self.pscale)
+            mlab.points3d(x_f, y_f, z_f, color=(0, 0, 1), scale_factor=self.pscale)
+            mlab.title('rbm (green) and flexible deformation (blue, true scale) in 9300 coord', size=0.5, height=0.9)
+
+            # plot structural forces
+            mlab.figure()
+            mlab.points3d(x, y, z, scale_factor=self.pscale)
+            fscale = 0.5 * self.model_size / np.max(np.abs(response['Pg'][0][self.strcgrid['set'][:, (0, 1, 2)]]))
+            fx = response['Pg'][0][self.strcgrid['set'][:, 0]]
+            fy = response['Pg'][0][self.strcgrid['set'][:, 1]]
+            fz = response['Pg'][0][self.strcgrid['set'][:, 2]]
+            mlab.quiver3d(x, y, z, fx * fscale, fy * fscale, fz * fscale, color=(1, 1, 0), mode='2ddash', opacity=0.4,
+                          scale_mode='vector', scale_factor=1.0)
+            mlab.quiver3d(x + fx * fscale, y + fy * fscale, z + fz * fscale, fx * fscale, fy * fscale, fz * fscale,
+                          color=(1, 1, 0), mode='cone', scale_mode='vector', scale_factor=0.1, resolution=16)
+            mlab.points3d(self.splinegrid['offset'][:, 0], self.splinegrid['offset'][:, 1], self.splinegrid['offset'][:, 2],
+                          color=(1, 1, 0), scale_factor=self.pscale * 1.5)
+            mlab.title('Pg', size=0.5, height=0.9)
+
+            if response['Pg_cfd'][0].sum() != 0.0:
+                mlab.figure()
+                mlab.points3d(x, y, z, scale_factor=self.pscale)
+                fscale = 0.5 * self.model_size / np.max(np.abs(response['Pg_cfd'][0][self.strcgrid['set'][:, (0, 1, 2)]]))
+                fx = response['Pg_cfd'][0][self.strcgrid['set'][:, 0]]
+                fy = response['Pg_cfd'][0][self.strcgrid['set'][:, 1]]
+                fz = response['Pg_cfd'][0][self.strcgrid['set'][:, 2]]
+                mlab.quiver3d(x, y, z, fx * fscale, fy * fscale, fz * fscale, color=(1, 1, 0), mode='2ddash',
+                              opacity=0.4, scale_mode='vector', scale_factor=1.0)
+                mlab.quiver3d(x + fx * fscale, y + fy * fscale, z + fz * fscale, fx * fscale, fy * fscale, fz * fscale,
+                              color=(1, 1, 0), mode='cone', scale_mode='vector', scale_factor=0.1, resolution=16)
+                mlab.points3d(self.splinegrid['offset'][:, 0],
+                              self.splinegrid['offset'][:, 1],
+                              self.splinegrid['offset'][:, 2],
+                              color=(1, 1, 0), scale_factor=self.pscale * 1.5)
+                mlab.title('Pg_cfd', size=0.5, height=0.9)
+            else:
+                logging.info('Forces Pg_cfd are zero, skip plotting')
+
+            # Render all plots
+            mlab.show()
+
 
 class Animations(plotting_standard.LoadPlots):
 
     def make_movie(self, path_output, speedup_factor=1.0):
         for response in self.responses:
             self.plot_time_animation_3d(response, path_output, speedup_factor=speedup_factor, make_movie=True)
 
@@ -333,20 +411,20 @@
                 shells = []
                 for shell in self.strcshell['cornerpoints']:
                     shells.append([np.where(self.strcgrid['ID'] == id)[0][0]
                                   for id in shell(np.isfinite(shell))])
                 shell_type = tvtk.Polygon().cell_type
                 self.strc_ug.set_cells(shell_type, shells)
                 src_points = mlab.pipeline.add_dataset(self.strc_ug)
-                mlab.pipeline.glyph(src_points, colormap='viridis', scale_factor=self.p_scale, scale_mode='none')
+                mlab.pipeline.glyph(src_points, colormap='viridis', scale_factor=self.pscale, scale_mode='none')
                 mlab.pipeline.surface(src_points, colormap='viridis')
             else:
                 # plot points as glyphs
                 src_points = mlab.pipeline.add_dataset(self.strc_ug)
-                mlab.pipeline.glyph(src_points, colormap='viridis', scale_factor=self.p_scale, scale_mode='none')
+                mlab.pipeline.glyph(src_points, colormap='viridis', scale_factor=self.pscale, scale_mode='none')
 
         def update_strc_display(self, points, scalars):
             self.strc_ug.points.from_array(points)
             self.strc_ug.point_data.scalars.from_array(scalars)
             self.strc_ug.modified()
 
         def setup_text_display(self):
```

### Comparing `LoadsKernel-2024.2/loadskernel/plotting_standard.py` & `loadskernel-2024.5/loadskernel/plotting_standard.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,19 +5,14 @@
 import numpy as np
 from scipy.spatial import ConvexHull
 
 from matplotlib import pyplot as plt
 from matplotlib.backends.backend_pdf import PdfPages
 from mpl_toolkits.axes_grid1.axes_divider import make_axes_locatable
 
-try:
-    from mayavi import mlab
-except ImportError:
-    pass
-
 from loadskernel.units import tas2eas, eas2tas
 from loadskernel.io_functions.data_handling import load_hdf5_dict
 
 plt.rcParams.update({'font.size': 16,
                      'svg.fonttype': 'none',
                      'savefig.dpi': 300, })
 
@@ -82,91 +77,15 @@
 
     def calc_parameters_from_model_size(self):
         # Calculate the overall size of the model.
         self.model_size = ((self.strcgrid['offset'][:, 0].max() - self.strcgrid['offset'][:, 0].min()) ** 2
                            + (self.strcgrid['offset'][:, 1].max() - self.strcgrid['offset'][:, 1].min()) ** 2
                            + (self.strcgrid['offset'][:, 2].max() - self.strcgrid['offset'][:, 2].min()) ** 2) ** 0.5
         # Set some parameters which typically give a good view.
-        self.pscale = np.min([self.model_size / 400.0, 0.04])
-
-    def plot_forces_deformation_interactive(self):
-        # loop over all responses
-        for response in self.responses:
-            trimcase = self.jcl.trimcase[response['i'][()]]
-            logging.info('interactive plotting of forces and deformations for trim {:s}'.format(trimcase['desc']))
-
-            # plot aerodynamic forces
-            x = self.aerogrid['offset_k'][:, 0]
-            y = self.aerogrid['offset_k'][:, 1]
-            z = self.aerogrid['offset_k'][:, 2]
-            fscale = 0.5 * self.model_size / np.max(np.abs(response['Pk_aero'][0][self.aerogrid['set_k'][:, (0, 1, 2)]]))
-            for name in ['Pk_aero', 'Pk_rbm', 'Pk_cam', 'Pk_cs', 'Pk_f', 'Pk_idrag']:
-                if response[name][0].sum() != 0.0:
-                    fx = response[name][0][self.aerogrid['set_k'][:, 0]]
-                    fy = response[name][0][self.aerogrid['set_k'][:, 1]]
-                    fz = response[name][0][self.aerogrid['set_k'][:, 2]]
-                    mlab.figure()
-                    mlab.points3d(x, y, z, scale_factor=self.pscale)
-                    mlab.quiver3d(x, y, z, fx, fy, fz, color=(0, 1, 0), scale_factor=fscale)
-                    mlab.title(name, size=0.5, height=0.9)
-                else:
-                    logging.info('Forces "{}" are zero, skip plotting')
-
-            # plot structural deformations
-            x = self.strcgrid['offset'][:, 0]
-            y = self.strcgrid['offset'][:, 1]
-            z = self.strcgrid['offset'][:, 2]
-            x_r = self.strcgrid['offset'][:, 0] + response['Ug_r'][0][self.strcgrid['set'][:, 0]]
-            y_r = self.strcgrid['offset'][:, 1] + response['Ug_r'][0][self.strcgrid['set'][:, 1]]
-            z_r = self.strcgrid['offset'][:, 2] + response['Ug_r'][0][self.strcgrid['set'][:, 2]]
-            x_f = self.strcgrid['offset'][:, 0] + response['Ug'][0][self.strcgrid['set'][:, 0]]
-            y_f = self.strcgrid['offset'][:, 1] + response['Ug'][0][self.strcgrid['set'][:, 1]]
-            z_f = self.strcgrid['offset'][:, 2] + response['Ug'][0][self.strcgrid['set'][:, 2]]
-
-            mlab.figure()
-            mlab.points3d(x_r, y_r, z_r, color=(0, 1, 0), scale_factor=self.pscale)
-            mlab.points3d(x_f, y_f, z_f, color=(0, 0, 1), scale_factor=self.pscale)
-            mlab.title('rbm (green) and flexible deformation (blue, true scale) in 9300 coord', size=0.5, height=0.9)
-
-            # plot structural forces
-            mlab.figure()
-            mlab.points3d(x, y, z, scale_factor=self.pscale)
-            fscale = 0.5 * self.model_size / np.max(np.abs(response['Pg'][0][self.strcgrid['set'][:, (0, 1, 2)]]))
-            fx = response['Pg'][0][self.strcgrid['set'][:, 0]]
-            fy = response['Pg'][0][self.strcgrid['set'][:, 1]]
-            fz = response['Pg'][0][self.strcgrid['set'][:, 2]]
-            mlab.quiver3d(x, y, z, fx * fscale, fy * fscale, fz * fscale, color=(1, 1, 0), mode='2ddash', opacity=0.4,
-                          scale_mode='vector', scale_factor=1.0)
-            mlab.quiver3d(x + fx * fscale, y + fy * fscale, z + fz * fscale, fx * fscale, fy * fscale, fz * fscale,
-                          color=(1, 1, 0), mode='cone', scale_mode='vector', scale_factor=0.1, resolution=16)
-            mlab.points3d(self.splinegrid['offset'][:, 0], self.splinegrid['offset'][:, 1], self.splinegrid['offset'][:, 2],
-                          color=(1, 1, 0), scale_factor=self.pscale * 1.5)
-            mlab.title('Pg', size=0.5, height=0.9)
-
-            if response['Pg_cfd'][0].sum() != 0.0:
-                mlab.figure()
-                mlab.points3d(x, y, z, scale_factor=self.pscale)
-                fscale = 0.5 * self.model_size / np.max(np.abs(response['Pg_cfd'][0][self.strcgrid['set'][:, (0, 1, 2)]]))
-                fx = response['Pg_cfd'][0][self.strcgrid['set'][:, 0]]
-                fy = response['Pg_cfd'][0][self.strcgrid['set'][:, 1]]
-                fz = response['Pg_cfd'][0][self.strcgrid['set'][:, 2]]
-                mlab.quiver3d(x, y, z, fx * fscale, fy * fscale, fz * fscale, color=(1, 1, 0), mode='2ddash',
-                              opacity=0.4, scale_mode='vector', scale_factor=1.0)
-                mlab.quiver3d(x + fx * fscale, y + fy * fscale, z + fz * fscale, fx * fscale, fy * fscale, fz * fscale,
-                              color=(1, 1, 0), mode='cone', scale_mode='vector', scale_factor=0.1, resolution=16)
-                mlab.points3d(self.splinegrid['offset'][:, 0],
-                              self.splinegrid['offset'][:, 1],
-                              self.splinegrid['offset'][:, 2],
-                              color=(1, 1, 0), scale_factor=self.pscale * 1.5)
-                mlab.title('Pg_cfd', size=0.5, height=0.9)
-            else:
-                logging.info('CFD forces are zero, skip plotting')
-
-            # Render all plots
-            mlab.show()
+        self.pscale = np.min([self.model_size / 400.0, 0.1])
 
     def plot_monstations(self, filename_pdf):
         # launch plotting
         self.pp = PdfPages(filename_pdf, keep_empty=False)
         self.potato_plots()
         if self.cuttingforces_wing:
             self.cuttingforces_along_wing_plots()
@@ -284,57 +203,80 @@
                 dof_xaxis = 4
                 dof_yaxis = 5
                 self.potato_plot_nicely(station, station, dof_xaxis, dof_yaxis, var_xaxis, var_yaxis)
         plt.close()
 
     def cuttingforces_along_wing_plots(self):
         logging.info('start plotting cutting forces along wing...')
-        self.subplot = self.create_axes()
-        cuttingforces = ['Fx [N]', 'Fy [N]', 'Fz [N]', 'Mx [Nm]', 'My [Nm]', 'Mz [Nm]']
+        # Read the data required for plotting.
         loads = []
         offsets = []
+        subcases = []
         for station in self.cuttingforces_wing:
             # trigger to read the data now with [:]
             loads.append(list(self.monstations[station]['loads'][:]))
             offsets.append(list(self.monstations[station]['offset'][:]))
+            # Get subcase description at monitoring station
+            if isinstance(self.monstations[station]['subcases'], list):
+                # This is an exception if source is not a hdf5 file.
+                # For example, the monstations have been pre-processed by a merge script and are lists already.
+                subcases.append(self.monstations[station]['subcases'])
+            else:
+                # make sure this is a list of strings
+                subcases.append(list(self.monstations[station]['subcases'].asstr()[:]))
         loads = np.array(loads)
         offsets = np.array(offsets)
 
-        for i_cuttingforce in range(len(cuttingforces)):
-            i_max = np.argmax(loads[:, :, i_cuttingforce], 1)
-            i_min = np.argmin(loads[:, :, i_cuttingforce], 1)
-            self.subplot.cla()
+        # Loop over all six components of the cutting loads.
+        label_loads = ['Fx [N]', 'Fy [N]', 'Fz [N]', 'Mx [Nm]', 'My [Nm]', 'Mz [Nm]']
+        subplot = self.create_axes()
+        for idx_load in range(6):
+            # Recycle the existing subplot.
+            subplot.cla()
+
+            # Plot loads.
             if loads.shape[1] > 50:
-                logging.debug(
-                    'plotting of every load case skipped due to large number (>50) of cases')
+                logging.debug('plotting of every load case skipped due to large number (>50) of cases')
             else:
-                self.subplot.plot(offsets[:, 1], loads[:, :, i_cuttingforce], color='cornflowerblue',
-                                  linestyle='-', marker='.', zorder=-2)
-            for i_station in range(len(self.cuttingforces_wing)):
-                # verticalalignment or va 	[ 'center' | 'top' | 'bottom' | 'baseline' ]
-                # max
-                self.subplot.scatter(offsets[i_station, 1], loads[i_station, i_max[i_station], i_cuttingforce], color='r')
-                self.subplot.text(offsets[i_station, 1], loads[i_station, i_max[i_station], i_cuttingforce],
-                                  str(self.monstations[list(self.monstations)[0]]['subcases'][i_max[i_station]]),
-                                  fontsize=4, verticalalignment='bottom')
-                # min
-                self.subplot.scatter(offsets[i_station, 1], loads[i_station, i_min[i_station], i_cuttingforce], color='r')
-                self.subplot.text(offsets[i_station, 1], loads[i_station, i_min[i_station], i_cuttingforce],
-                                  str(self.monstations[list(self.monstations)[0]]['subcases'][i_min[i_station]]),
-                                  fontsize=4, verticalalignment='top')
-
-            self.subplot.set_title('Wing')
-            self.subplot.ticklabel_format(style='sci', axis='y', scilimits=(-2, 2))
-            self.subplot.grid(visible=True, which='major', axis='both')
-            self.subplot.minorticks_on()
-            yax = self.subplot.get_yaxis()
+                subplot.plot(offsets[:, 1], loads[:, :, idx_load], color='cornflowerblue',
+                             linestyle='-', marker='.', zorder=-2)
+
+            # Loop over all stations and label min and max loads.
+            for idx_station in range(len(self.cuttingforces_wing)):
+                # Identifiy min and max loads
+                idx_max_loads = np.argmax(loads[idx_station, :, idx_load])
+                idx_min_loads = np.argmin(loads[idx_station, :, idx_load])
+
+                # Highlight max loads with red dot and print subcase description.
+                subplot.scatter(offsets[idx_station, 1],
+                                loads[idx_station, idx_max_loads, idx_load],
+                                color='r')
+                subplot.text(offsets[idx_station, 1],
+                             loads[idx_station, idx_max_loads, idx_load],
+                             str(subcases[idx_station][idx_max_loads]),
+                             fontsize=4, verticalalignment='bottom')
+
+                # Highlight min loads with red dot and print subcase description.
+                subplot.scatter(offsets[idx_station, 1],
+                                loads[idx_station, idx_min_loads, idx_load],
+                                color='r')
+                subplot.text(offsets[idx_station, 1],
+                             loads[idx_station, idx_min_loads, idx_load],
+                             str(subcases[idx_station][idx_min_loads]),
+                             fontsize=4, verticalalignment='top')
+
+            subplot.set_title('Wing')
+            subplot.ticklabel_format(style='sci', axis='y', scilimits=(-2, 2))
+            subplot.grid(visible=True, which='major', axis='both')
+            subplot.minorticks_on()
+            yax = subplot.get_yaxis()
             yax.set_label_coords(x=-0.18, y=0.5)
-            self.subplot.set_xlabel('y [m]')
-            self.subplot.set_ylabel(cuttingforces[i_cuttingforce])
-            self.subplot.set_rasterization_zorder(-1)
+            subplot.set_xlabel('y [m]')
+            subplot.set_ylabel(label_loads[idx_load])
+            subplot.set_rasterization_zorder(-1)
             self.pp.savefig()
         plt.close()
 
     def plot_monstations_time(self, filename_pdf):
         logging.info('start plotting cutting forces over time ...')
         pp = PdfPages(filename_pdf)
         potato = np.sort(np.unique(self.potatos_fz_mx + self.potatos_mx_my + self.potatos_fz_my + self.potatos_fy_mx
```

### Comparing `LoadsKernel-2024.2/loadskernel/post_processing.py` & `loadskernel-2024.5/loadskernel/post_processing.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/program_flow.py` & `loadskernel-2024.5/loadskernel/program_flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import time
 
 try:
     from mpi4py import MPI
 except ImportError:
     pass
 
-from loadskernel import solution_sequences, post_processing, gather_loads, auxiliary_output, plotting_standard, plotting_extra
+from loadskernel import solution_sequences, post_processing, gather_loads, auxiliary_output, plotting_standard
 from loadskernel.io_functions import data_handling
 import loadskernel.model as model_modul
 from loadskernel.cfd_interfaces.mpi_helper import setup_mpi
 
 
 class ProgramFlowHelper():
 
@@ -380,14 +380,18 @@
         """
         This section shall be used for code that is not part of standard post-processing procedures.
         Below, some useful plotting functions are given that might be helpful, for example
         - to identify if a new model is working correctly
         - to get extra time data plots
         - to animate a time domain simulation
         """
+        # Import plotting_extra not before here, as the import of graphical libraries such as mayavi takes a long time and
+        # fails of systems without graphical display (such as HPS clusters).
+        from loadskernel import plotting_extra
+
         # Load the model and the response as usual
         model = data_handling.load_hdf5(self.path_output + 'model_' + self.job_name + '.hdf5')
         responses = data_handling.load_hdf5_responses(self.job_name, self.path_output)
 
         logging.info('--> Drawing some more detailed plots.')
         plt = plotting_extra.DetailedPlots(self.jcl, model)
         plt.add_responses(responses)
```

### Comparing `LoadsKernel-2024.2/loadskernel/solution_sequences.py` & `loadskernel-2024.5/loadskernel/solution_sequences.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/solution_tools.py` & `loadskernel-2024.5/loadskernel/solution_tools.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/spline_functions.py` & `loadskernel-2024.5/loadskernel/spline_functions.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/spline_rules.py` & `loadskernel-2024.5/loadskernel/spline_rules.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/trim_conditions.py` & `loadskernel-2024.5/loadskernel/trim_conditions.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/units.py` & `loadskernel-2024.5/loadskernel/units.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/utils/PID.py` & `loadskernel-2024.5/loadskernel/utils/PID.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/utils/filter.py` & `loadskernel-2024.5/loadskernel/utils/filter.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/loadskernel/utils/sparse_matrices.py` & `loadskernel-2024.5/loadskernel/utils/sparse_matrices.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/modelviewer/cfdgrid.py` & `loadskernel-2024.5/modelviewer/cfdgrid.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/modelviewer/iges.py` & `loadskernel-2024.5/modelviewer/iges.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/modelviewer/plotting.py` & `loadskernel-2024.5/modelviewer/plotting.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     def calc_parameters_from_model_size(self):
         # Calculate the overall size of the model.
         model_size = ((self.strcgrid['offset'][:, 0].max() - self.strcgrid['offset'][:, 0].min()) ** 2
                       + (self.strcgrid['offset'][:, 1].max() - self.strcgrid['offset'][:, 1].min()) ** 2
                       + (self.strcgrid['offset'][:, 2].max() - self.strcgrid['offset'][:, 2].min()) ** 2) ** 0.5
         # Set some parameters which typically give a good view.
         self.distance = model_size * 1.5
-        self.pscale = np.min([model_size / 400.0, 0.04])
+        self.pscale = np.min([model_size / 400.0, 0.1])
         self.macscale = np.min([model_size / 10.0, 1.0])
 
     def calc_focalpoint(self):
         self.focalpoint = (self.strcgrid['offset'].min(
             axis=0) + self.strcgrid['offset'].max(axis=0)) / 2.0
 
     def set_view_left_above(self):
```

### Comparing `LoadsKernel-2024.2/modelviewer/pytran.py` & `loadskernel-2024.5/modelviewer/pytran.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/modelviewer/view.py` & `loadskernel-2024.5/modelviewer/view.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/setup.py` & `loadskernel-2024.5/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 """
 
 from setuptools import setup, find_packages
 
 
 def my_setup():
     setup(name='LoadsKernel',
-          version='2024.02',
+          version='2024.05',
           description="""The Loads Kernel Software allows for the calculation of quasi-steady and dynamic maneuver loads,
           unsteady gust loads in the time and frequency domain as well as dynamic landing loads based on a generic landing
           gear module.""",
           long_description=open('README.md', encoding='utf8').read(),
           long_description_content_type='text/markdown',
           url='https://github.com/DLR-AE/LoadsKernel',
           author='Arne Voß',
@@ -26,36 +26,39 @@
           packages=find_packages(),
           entry_points={'console_scripts': ['loads-kernel=loadskernel.program_flow:command_line_interface',
                                             'model-viewer=modelviewer.view:command_line_interface',
                                             'loads-compare=loadscompare.compare:command_line_interface']},
           include_package_data=True,
           package_data={'loadskernel': ['graphics/*.*'],
                         'loadscompare': ['graphics/*.*'], },
-          python_requires='>=3.8',
+          python_requires='>=3.10',
           install_requires=['PanelAero',
                             'matplotlib',
                             'numpy',
                             'scipy',
                             'psutil',
                             'h5py',
                             'tables',
                             'pyyaml',
                             'pandas',
                             ],
           extras_require={'extras': ['mpi4py',
-                                     'pyfmi',
                                      'mayavi',
                                      'traits',
                                      'traitsui',
                                      'pyface',
-                                     'pyiges',
+                                     'jupyter',
+                                     'pyiges',  # only available with pip, not with conda
                                      ],
+                          'difficult': ['pyfmi',  # frequent version conflicts
+                                        ],
                           'test': ['pytest',
                                    'pytest-cov',
-                                   'jupyter',
                                    'jupyter-book==0.15.1',  # version 1.0.0 fails, wait for updates
+                                   'flake8',
+                                   'pylint',
                                    ]},
           )
 
 
 if __name__ == '__main__':
     my_setup()
```

### Comparing `LoadsKernel-2024.2/tests/helper_functions.py` & `loadskernel-2024.5/tests/helper_functions.py`

 * *Files identical despite different names*

### Comparing `LoadsKernel-2024.2/tests/test_integration.py` & `loadskernel-2024.5/tests/test_integration.py`

 * *Files identical despite different names*

