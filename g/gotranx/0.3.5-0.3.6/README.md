# Comparing `tmp/gotranx-0.3.5.tar.gz` & `tmp/gotranx-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gotranx-0.3.5.tar", last modified: Thu Apr  4 09:42:21 2024, max compression
+gzip compressed data, was "gotranx-0.3.6.tar", last modified: Tue May 21 07:01:11 2024, max compression
```

## Comparing `gotranx-0.3.5.tar` & `gotranx-0.3.6.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:21.246795 gotranx-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-04 09:42:21.246795 gotranx-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-04-04 09:42:14.000000 gotranx-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-04 09:42:14.000000 gotranx-0.3.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 09:42:21.246795 gotranx-0.3.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:21.234795 gotranx-0.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:21.238795 gotranx-0.3.5/src/gotranx/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/atoms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:21.238795 gotranx-0.3.5/src/gotranx/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/cli/cellml2ode.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/cli/gotran2c.py
--rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/cli/gotran2py.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:21.238795 gotranx-0.3.5/src/gotranx/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/codegen/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/codegen/c.py
--rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/codegen/ode.py
--rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/codegen/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/myokit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/ode.lark
--rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/ode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/ode_component.py
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/save.py
--rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/schemes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/sympytools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:21.238795 gotranx-0.3.5/src/gotranx/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/templates/c.py
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/templates/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-04 09:42:14.000000 gotranx-0.3.5/src/gotranx/units.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:21.242795 gotranx-0.3.5/src/gotranx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-04-04 09:42:21.000000 gotranx-0.3.5/src/gotranx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-04-04 09:42:21.000000 gotranx-0.3.5/src/gotranx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:42:21.000000 gotranx-0.3.5/src/gotranx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-04 09:42:21.000000 gotranx-0.3.5/src/gotranx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 09:42:21.000000 gotranx-0.3.5/src/gotranx.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-04 09:42:21.000000 gotranx-0.3.5/src/gotranx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-04 09:42:21.000000 gotranx-0.3.5/src/gotranx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 09:42:21.242795 gotranx-0.3.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_atoms.py
--rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_c_codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_conditionals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_myokit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_ode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_ode_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    20676 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_python_codegen.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_schemes.py
--rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_subodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_sympytools.py
--rw-r--r--   0 runner    (1001) docker     (127)    19349 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_transformer_assignments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_transformer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-04 09:42:14.000000 gotranx-0.3.5/tests/test_transformer_states.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:01:11.367250 gotranx-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-21 07:01:11.363250 gotranx-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-21 07:01:08.000000 gotranx-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-21 07:01:08.000000 gotranx-0.3.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 07:01:11.367250 gotranx-0.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:01:11.355250 gotranx-0.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:01:11.359250 gotranx-0.3.6/src/gotranx/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/atoms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:01:11.359250 gotranx-0.3.6/src/gotranx/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/cli/cellml2ode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/cli/gotran2c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/cli/gotran2py.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:01:11.359250 gotranx-0.3.6/src/gotranx/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/codegen/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/codegen/c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/codegen/ode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6008 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/codegen/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/myokit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2335 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/ode.lark
+-rw-r--r--   0 runner    (1001) docker     (127)    11529 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/ode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/ode_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5073 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/schemes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/sympytools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:01:11.359250 gotranx-0.3.6/src/gotranx/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2343 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/templates/c.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/templates/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-21 07:01:08.000000 gotranx-0.3.6/src/gotranx/units.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:01:11.363250 gotranx-0.3.6/src/gotranx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-21 07:01:11.000000 gotranx-0.3.6/src/gotranx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-21 07:01:11.000000 gotranx-0.3.6/src/gotranx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:01:11.000000 gotranx-0.3.6/src/gotranx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 07:01:11.000000 gotranx-0.3.6/src/gotranx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:01:11.000000 gotranx-0.3.6/src/gotranx.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-21 07:01:11.000000 gotranx-0.3.6/src/gotranx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 07:01:11.000000 gotranx-0.3.6/src/gotranx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:01:11.363250 gotranx-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_atoms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21269 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_c_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_conditionals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_myokit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4867 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_ode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_ode_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20676 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_python_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_schemes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7535 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_subodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_sympytools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19349 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_transformer_assignments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_transformer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-21 07:01:08.000000 gotranx-0.3.6/tests/test_transformer_states.py
```

### Comparing `gotranx-0.3.5/PKG-INFO` & `gotranx-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotranx
-Version: 0.3.5
+Version: 0.3.6
 Summary: A declarative language describing ordinary differential equations
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://github.com/finsberg/gotranx
 Keywords: parser,lark,gotran,ode
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gotranx-0.3.5/README.md` & `gotranx-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/pyproject.toml` & `gotranx-0.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gotranx"
-version = "0.3.5"
+version = "0.3.6"
 description = "A declarative language describing ordinary differential equations"
 authors = [{name = "Henrik Finsberg", email = "henriknf@simula.no"}]
 license = {text = "MIT"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
@@ -153,14 +153,14 @@
 allow_dirty = false
 commit = true
 message = "Bump version: {current_version} → {new_version}"
 tag = true
 sign_tags = false
 tag_name = "v{new_version}"
 tag_message = "Bump version: {current_version} → {new_version}"
-current_version = "0.3.5"
+current_version = "0.3.6"
 
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
```

### Comparing `gotranx-0.3.5/src/gotranx/__init__.py` & `gotranx-0.3.6/src/gotranx/__init__.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/atoms.py` & `gotranx-0.3.6/src/gotranx/atoms.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 def unit_from_string(unit_str: str | None) -> pint.Unit | None:
     if unit_str is not None:
         try:
             unit = ureg.Unit(unit_str)
         except pint.UndefinedUnitError:
             logger.warning(f"Undefined unit {unit_str!r}")
             unit = None
+        except ValueError:
+            try:
+                unit = ureg.Unit(unit_str.split(" ")[0])
+            except Exception:
+                logger.warning(f"Invalid unit {unit_str!r}")
+                unit = None
     else:
         unit = None
     return unit
 
 
 def _set_unit(instance, unit_str: str) -> None:
     object.__setattr__(instance, "unit", unit_from_string(unit_str))
```

### Comparing `gotranx-0.3.5/src/gotranx/cli/__init__.py` & `gotranx-0.3.6/src/gotranx/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/cli/cellml2ode.py` & `gotranx-0.3.6/src/gotranx/cli/cellml2ode.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/cli/gotran2c.py` & `gotranx-0.3.6/src/gotranx/cli/gotran2c.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/cli/gotran2py.py` & `gotranx-0.3.6/src/gotranx/cli/gotran2py.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/codegen/__init__.py` & `gotranx-0.3.6/src/gotranx/codegen/__init__.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/codegen/base.py` & `gotranx-0.3.6/src/gotranx/codegen/base.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/codegen/c.py` & `gotranx-0.3.6/src/gotranx/codegen/c.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/codegen/ode.py` & `gotranx-0.3.6/src/gotranx/codegen/ode.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/codegen/python.py` & `gotranx-0.3.6/src/gotranx/codegen/python.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/exceptions.py` & `gotranx-0.3.6/src/gotranx/exceptions.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/expressions.py` & `gotranx-0.3.6/src/gotranx/expressions.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/load.py` & `gotranx-0.3.6/src/gotranx/load.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/myokit.py` & `gotranx-0.3.6/src/gotranx/myokit.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/ode.lark` & `gotranx-0.3.6/src/gotranx/ode.lark`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/ode.py` & `gotranx-0.3.6/src/gotranx/ode.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/ode_component.py` & `gotranx-0.3.6/src/gotranx/ode_component.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/save.py` & `gotranx-0.3.6/src/gotranx/save.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/schemes.py` & `gotranx-0.3.6/src/gotranx/schemes.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/sympytools.py` & `gotranx-0.3.6/src/gotranx/sympytools.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/templates/__init__.py` & `gotranx-0.3.6/src/gotranx/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/templates/c.py` & `gotranx-0.3.6/src/gotranx/templates/c.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/templates/python.py` & `gotranx-0.3.6/src/gotranx/templates/python.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx/transformer.py` & `gotranx-0.3.6/src/gotranx/transformer.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/src/gotranx.egg-info/PKG-INFO` & `gotranx-0.3.6/src/gotranx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gotranx
-Version: 0.3.5
+Version: 0.3.6
 Summary: A declarative language describing ordinary differential equations
 Author-email: Henrik Finsberg <henriknf@simula.no>
 License: MIT
 Project-URL: Homepage, https://github.com/finsberg/gotranx
 Keywords: parser,lark,gotran,ode
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `gotranx-0.3.5/src/gotranx.egg-info/SOURCES.txt` & `gotranx-0.3.6/src/gotranx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_atoms.py` & `gotranx-0.3.6/tests/test_atoms.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_c_codegen.py` & `gotranx-0.3.6/tests/test_c_codegen.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_cli.py` & `gotranx-0.3.6/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_conditionals.py` & `gotranx-0.3.6/tests/test_conditionals.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_expressions.py` & `gotranx-0.3.6/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_load.py` & `gotranx-0.3.6/tests/test_load.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_myokit.py` & `gotranx-0.3.6/tests/test_myokit.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_ode.py` & `gotranx-0.3.6/tests/test_ode.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_ode_component.py` & `gotranx-0.3.6/tests/test_ode_component.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_python_codegen.py` & `gotranx-0.3.6/tests/test_python_codegen.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_save.py` & `gotranx-0.3.6/tests/test_save.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_schemes.py` & `gotranx-0.3.6/tests/test_schemes.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_subodes.py` & `gotranx-0.3.6/tests/test_subodes.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_sympytools.py` & `gotranx-0.3.6/tests/test_sympytools.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_transformer_assignments.py` & `gotranx-0.3.6/tests/test_transformer_assignments.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_transformer_parameters.py` & `gotranx-0.3.6/tests/test_transformer_parameters.py`

 * *Files identical despite different names*

### Comparing `gotranx-0.3.5/tests/test_transformer_states.py` & `gotranx-0.3.6/tests/test_transformer_states.py`

 * *Files identical despite different names*

