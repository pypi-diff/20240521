# Comparing `tmp/ts3l-0.40.tar.gz` & `tmp/ts3l-0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ts3l-0.40.tar", last modified: Thu May  2 05:42:34 2024, max compression
+gzip compressed data, was "ts3l-0.41.tar", last modified: Tue May 21 17:51:40 2024, max compression
```

## Comparing `ts3l-0.40.tar` & `ts3l-0.41.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 05:42:25.000000 ts3l-0.40/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21158 2024-05-02 05:42:34.098232 ts3l-0.40/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20542 2024-05-02 05:42:25.000000 ts3l-0.40/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 05:42:34.098232 ts3l-0.40/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-02 05:42:25.000000 ts3l-0.40/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.090232 ts3l-0.40/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-02 05:42:25.000000 ts3l-0.40/test/test_dae.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-02 05:42:25.000000 ts3l-0.40/test/test_scarf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-02 05:42:25.000000 ts3l-0.40/test/test_subtab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-02 05:42:25.000000 ts3l-0.40/test/test_switchtab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-02 05:42:25.000000 ts3l-0.40/test/test_vime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.090232 ts3l-0.40/ts3l/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.090232 ts3l-0.40/ts3l/models/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.090232 ts3l-0.40/ts3l/models/common/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/common/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/common/mlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/models/dae/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/dae/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/dae/dae.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/models/scarf/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/scarf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/scarf/scarf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/models/subtab/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/subtab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/subtab/subtab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/models/switchtab/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/switchtab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/switchtab/ft_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/switchtab/switchtab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/models/vime/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/vime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/vime/vime.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/vime/vime_self.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/models/vime/vime_semi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/pl_modules/
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/base_module.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/dae_lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/scarf_lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/subtab_lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/switchtab_lightning.py
--rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/pl_modules/vime_lightning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.094232 ts3l-0.40/ts3l/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/base_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/ts3l/utils/dae_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/dae_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/dae_utils/dae_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/dae_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/ts3l/utils/scarf_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/scarf_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/scarf_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/scarf_utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/scarf_utils/scarf_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/ts3l/utils/subtab_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/subtab_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/subtab_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/subtab_utils/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/subtab_utils/subtab_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/ts3l/utils/switchtab_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/switchtab_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/switchtab_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/switchtab_utils/switchtab_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/ts3l/utils/vime_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/vime_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/vime_utils/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-02 05:42:25.000000 ts3l-0.40/ts3l/utils/vime_utils/vime_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 05:42:34.098232 ts3l-0.40/ts3l.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21158 2024-05-02 05:42:34.000000 ts3l-0.40/ts3l.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-02 05:42:34.000000 ts3l-0.40/ts3l.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 05:42:34.000000 ts3l-0.40/ts3l.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 05:42:34.000000 ts3l-0.40/ts3l.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 05:42:34.000000 ts3l-0.40/ts3l.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.553675 ts3l-0.41/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-21 17:51:32.000000 ts3l-0.41/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21158 2024-05-21 17:51:40.553675 ts3l-0.41/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20542 2024-05-21 17:51:32.000000 ts3l-0.41/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 17:51:40.553675 ts3l-0.41/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1577 2024-05-21 17:51:32.000000 ts3l-0.41/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.545675 ts3l-0.41/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-21 17:51:32.000000 ts3l-0.41/test/test_dae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-21 17:51:32.000000 ts3l-0.41/test/test_scarf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-21 17:51:32.000000 ts3l-0.41/test/test_subtab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1296 2024-05-21 17:51:32.000000 ts3l-0.41/test/test_switchtab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-21 17:51:32.000000 ts3l-0.41/test/test_vime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.545675 ts3l-0.41/ts3l/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.545675 ts3l-0.41/ts3l/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.545675 ts3l-0.41/ts3l/models/common/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/common/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/common/mlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.545675 ts3l-0.41/ts3l/models/dae/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/dae/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/dae/dae.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.545675 ts3l-0.41/ts3l/models/scarf/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/scarf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2581 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/scarf/scarf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.545675 ts3l-0.41/ts3l/models/subtab/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/subtab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3950 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/subtab/subtab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.545675 ts3l-0.41/ts3l/models/switchtab/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/switchtab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/switchtab/ft_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/switchtab/switchtab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.549675 ts3l-0.41/ts3l/models/vime/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/vime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/vime/vime.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/vime/vime_self.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/models/vime/vime_semi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.549675 ts3l-0.41/ts3l/pl_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/pl_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9000 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/pl_modules/base_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/pl_modules/dae_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/pl_modules/scarf_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/pl_modules/subtab_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3638 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/pl_modules/switchtab_lightning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4296 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/pl_modules/vime_lightning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.549675 ts3l-0.41/ts3l/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/base_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.549675 ts3l-0.41/ts3l/utils/dae_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/dae_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4440 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/dae_utils/dae_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6070 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/dae_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3486 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/misc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.553675 ts3l-0.41/ts3l/utils/scarf_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/scarf_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5033 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/scarf_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/scarf_utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2852 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/scarf_utils/scarf_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.553675 ts3l-0.41/ts3l/utils/subtab_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/subtab_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7786 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/subtab_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4947 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/subtab_utils/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/subtab_utils/subtab_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.553675 ts3l-0.41/ts3l/utils/switchtab_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/switchtab_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/switchtab_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/switchtab_utils/switchtab_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.553675 ts3l-0.41/ts3l/utils/vime_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/vime_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10356 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/vime_utils/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-21 17:51:32.000000 ts3l-0.41/ts3l/utils/vime_utils/vime_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 17:51:40.553675 ts3l-0.41/ts3l.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21158 2024-05-21 17:51:40.000000 ts3l-0.41/ts3l.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-21 17:51:40.000000 ts3l-0.41/ts3l.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 17:51:40.000000 ts3l-0.41/ts3l.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 17:51:40.000000 ts3l-0.41/ts3l.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 17:51:40.000000 ts3l-0.41/ts3l.egg-info/top_level.txt
```

### Comparing `ts3l-0.40/LICENSE` & `ts3l-0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/PKG-INFO` & `ts3l-0.41/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts3l
-Version: 0.40
+Version: 0.41
 Summary: A PyTorch Lightning-based library for self- and semi-supervised learning on tabular data.
 Home-page: https://github.com/Alcoholrithm/TabularS3L
 Author: Minwook Kim
 Author-email: kmiiiaa@pusan.ac.kr
 Keywords: tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF Denoising-AutoEncoder SwitchTab
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ts3l-0.40/README.md` & `ts3l-0.41/README.md`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/setup.py` & `ts3l-0.41/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         str(requirement)
         for requirement
         in pkg_resources.parse_requirements(requirements_txt)
     ]
 
 setup(
     name='ts3l',
-    version='v0.40',
+    version='v0.41',
     description='A PyTorch Lightning-based library for self- and semi-supervised learning on tabular data.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/Alcoholrithm/TabularS3L',
     author='Minwook Kim',
     author_email='kmiiiaa@pusan.ac.kr',
```

### Comparing `ts3l-0.40/test/test_dae.py` & `ts3l-0.41/test/test_dae.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/test/test_scarf.py` & `ts3l-0.41/test/test_scarf.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/test/test_subtab.py` & `ts3l-0.41/test/test_subtab.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/test/test_switchtab.py` & `ts3l-0.41/test/test_switchtab.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/test/test_vime.py` & `ts3l-0.41/test/test_vime.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/models/common/misc.py` & `ts3l-0.41/ts3l/models/common/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,14 @@
         model (nn.Module): PyTorch model instance.
         initialization (str): Name of the initialization method.
             Options: 'xavier_uniform', 'xavier_normal', 'kaiming_uniform', 'kaiming_normal', 'uniform', 'normal'.
             Defaults to 'kaiming_normal'.
     """
 
     for name, param in model.named_parameters():
-        print(name)
         if any(layer_name.upper() in name.upper() for layer_name in exclude_layers):
             continue
         if 'weight' in name:
             if initialization == 'xavier_uniform':
                 init.xavier_uniform_(param)
             elif initialization == 'xavier_normal':
                 init.xavier_normal_(param)
```

### Comparing `ts3l-0.40/ts3l/models/common/mlp.py` & `ts3l-0.41/ts3l/models/common/mlp.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/models/dae/dae.py` & `ts3l-0.41/ts3l/models/dae/dae.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/models/scarf/scarf.py` & `ts3l-0.41/ts3l/models/scarf/scarf.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/models/subtab/subtab.py` & `ts3l-0.41/ts3l/models/subtab/subtab.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/models/switchtab/ft_transformer.py` & `ts3l-0.41/ts3l/models/switchtab/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/models/switchtab/switchtab.py` & `ts3l-0.41/ts3l/models/switchtab/switchtab.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/models/vime/vime.py` & `ts3l-0.41/ts3l/models/vime/vime.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/models/vime/vime_self.py` & `ts3l-0.41/ts3l/models/vime/vime_self.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/models/vime/vime_semi.py` & `ts3l-0.41/ts3l/models/vime/vime_semi.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/pl_modules/base_module.py` & `ts3l-0.41/ts3l/pl_modules/base_module.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/pl_modules/dae_lightning.py` & `ts3l-0.41/ts3l/pl_modules/dae_lightning.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/pl_modules/scarf_lightning.py` & `ts3l-0.41/ts3l/pl_modules/scarf_lightning.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/pl_modules/subtab_lightning.py` & `ts3l-0.41/ts3l/pl_modules/subtab_lightning.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/pl_modules/switchtab_lightning.py` & `ts3l-0.41/ts3l/pl_modules/switchtab_lightning.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/pl_modules/vime_lightning.py` & `ts3l-0.41/ts3l/pl_modules/vime_lightning.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/base_config.py` & `ts3l-0.41/ts3l/utils/base_config.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/dae_utils/dae_config.py` & `ts3l-0.41/ts3l/utils/dae_utils/dae_config.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/dae_utils/data_utils.py` & `ts3l-0.41/ts3l/utils/dae_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/datamodule.py` & `ts3l-0.41/ts3l/utils/datamodule.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/misc.py` & `ts3l-0.41/ts3l/utils/misc.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/scarf_utils/data_utils.py` & `ts3l-0.41/ts3l/utils/scarf_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/scarf_utils/loss.py` & `ts3l-0.41/ts3l/utils/scarf_utils/loss.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/scarf_utils/scarf_config.py` & `ts3l-0.41/ts3l/utils/scarf_utils/scarf_config.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/subtab_utils/data_utils.py` & `ts3l-0.41/ts3l/utils/subtab_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/subtab_utils/loss.py` & `ts3l-0.41/ts3l/utils/subtab_utils/loss.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/subtab_utils/subtab_config.py` & `ts3l-0.41/ts3l/utils/subtab_utils/subtab_config.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/switchtab_utils/data_utils.py` & `ts3l-0.41/ts3l/utils/switchtab_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/switchtab_utils/switchtab_config.py` & `ts3l-0.41/ts3l/utils/switchtab_utils/switchtab_config.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/vime_utils/data_utils.py` & `ts3l-0.41/ts3l/utils/vime_utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l/utils/vime_utils/vime_config.py` & `ts3l-0.41/ts3l/utils/vime_utils/vime_config.py`

 * *Files identical despite different names*

### Comparing `ts3l-0.40/ts3l.egg-info/PKG-INFO` & `ts3l-0.41/ts3l.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ts3l
-Version: 0.40
+Version: 0.41
 Summary: A PyTorch Lightning-based library for self- and semi-supervised learning on tabular data.
 Home-page: https://github.com/Alcoholrithm/TabularS3L
 Author: Minwook Kim
 Author-email: kmiiiaa@pusan.ac.kr
 Keywords: tabular-data semi-supervised-learning self-supervised-learning VIME SubTab SCARF Denoising-AutoEncoder SwitchTab
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `ts3l-0.40/ts3l.egg-info/SOURCES.txt` & `ts3l-0.41/ts3l.egg-info/SOURCES.txt`

 * *Files identical despite different names*

