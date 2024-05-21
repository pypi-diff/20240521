# Comparing `tmp/vss-cli-2023.9.0.dev8.tar.gz` & `tmp/vss-cli-2024.5.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vss-cli-2023.9.0.dev8.tar", last modified: Thu Sep 28 20:02:42 2023, max compression
+gzip compressed data, was "vss-cli-2024.5.0.dev0.tar", last modified: Tue May 21 00:53:26 2024, max compression
```

## Comparing `vss-cli-2023.9.0.dev8.tar` & `vss-cli-2024.5.0.dev0.tar`

### file list

```diff
@@ -1,90 +1,93 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 20:02:42.148371 vss-cli-2023.9.0.dev8/
--rw-rw-rw-   0 root         (0) root         (0)     1078 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    12302 2023-09-28 20:02:42.148371 vss-cli-2023.9.0.dev8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    10991 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/README.md
--rw-rw-rw-   0 root         (0) root         (0)       62 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1257 2023-09-28 20:02:42.152371 vss-cli-2023.9.0.dev8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     3827 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 20:02:42.132371 vss-cli-2023.9.0.dev8/vss_cli/
--rw-rw-rw-   0 root         (0) root         (0)       39 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    18320 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/autocompletion.py
--rw-rw-rw-   0 root         (0) root         (0)     7453 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/cli.py
--rw-rw-rw-   0 root         (0) root         (0)    62562 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/config.py
--rw-rw-rw-   0 root         (0) root         (0)    14070 2023-09-28 20:01:40.000000 vss-cli-2023.9.0.dev8/vss_cli/const.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 20:02:42.136371 vss-cli-2023.9.0.dev8/vss_cli/data/
--rw-rw-rw-   0 root         (0) root         (0)     4524 2023-09-28 20:01:40.000000 vss-cli-2023.9.0.dev8/vss_cli/data/clib.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4288 2023-09-28 20:01:40.000000 vss-cli-2023.9.0.dev8/vss_cli/data/clone.yaml
--rw-rw-rw-   0 root         (0) root         (0)      577 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/data/config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2892 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/data/image.yaml
--rw-rw-rw-   0 root         (0) root         (0)     2951 2023-09-28 20:01:40.000000 vss-cli-2023.9.0.dev8/vss_cli/data/shell.yaml
--rw-rw-rw-   0 root         (0) root         (0)     4200 2023-09-28 20:01:40.000000 vss-cli-2023.9.0.dev8/vss_cli/data/template.yaml
--rw-rw-rw-   0 root         (0) root         (0)    25848 2023-09-28 00:44:28.000000 vss-cli-2023.9.0.dev8/vss_cli/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)      227 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      819 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/hcio.py
--rw-rw-rw-   0 root         (0) root         (0)    12512 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 20:02:42.144371 vss-cli-2023.9.0.dev8/vss_cli/plugins/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-09-28 20:02:38.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    15976 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/account.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/completion.py
--rw-rw-rw-   0 root         (0) root         (0)      908 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 20:02:42.148371 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      196 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9105 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/callbacks.py
--rw-rw-rw-   0 root         (0) root         (0)     4015 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/contentlib.py
--rw-rw-rw-   0 root         (0) root         (0)     2813 2023-09-28 00:51:19.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/domain.py
--rw-rw-rw-   0 root         (0) root         (0)     3133 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/floppy.py
--rw-rw-rw-   0 root         (0) root         (0)     8680 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/helper.py
--rw-rw-rw-   0 root         (0) root         (0)     3287 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2841 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     3046 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/iso.py
--rw-rw-rw-   0 root         (0) root         (0)     3477 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/net.py
--rw-rw-rw-   0 root         (0) root         (0)     1665 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/os.py
--rw-rw-rw-   0 root         (0) root         (0)      644 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/rel_args.py
--rw-rw-rw-   0 root         (0) root         (0)     9402 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     3790 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/template.py
--rw-rw-rw-   0 root         (0) root         (0)   143327 2023-09-28 20:01:40.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/vm.py
--rw-rw-rw-   0 root         (0) root         (0)     1907 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/vmdks.py
--rw-rw-rw-   0 root         (0) root         (0)    10871 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/configure.py
--rw-rw-rw-   0 root         (0) root         (0)     3481 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/key.py
--rw-rw-rw-   0 root         (0) root         (0)     3010 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/message.py
--rw-rw-rw-   0 root         (0) root         (0)     1947 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/misc.py
--rw-rw-rw-   0 root         (0) root         (0)     4310 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/ovf.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/plugins.py
--rw-rw-rw-   0 root         (0) root         (0)     1263 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/raw.py
--rw-rw-rw-   0 root         (0) root         (0)      595 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/request.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 20:02:42.148371 vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/
--rw-rw-rw-   0 root         (0) root         (0)      204 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5330 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/change.py
--rw-rw-rw-   0 root         (0) root         (0)     2306 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/export.py
--rw-rw-rw-   0 root         (0) root         (0)     2372 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/folder.py
--rw-rw-rw-   0 root         (0) root         (0)     2362 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/image.py
--rw-rw-rw-   0 root         (0) root         (0)     2345 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/inventory.py
--rw-rw-rw-   0 root         (0) root         (0)     2860 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/new.py
--rw-rw-rw-   0 root         (0) root         (0)     3924 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/retirement.py
--rw-rw-rw-   0 root         (0) root         (0)     3307 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/snapshot.py
--rw-rw-rw-   0 root         (0) root         (0)     2246 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/vmdk.py
--rw-rw-rw-   0 root         (0) root         (0)     1614 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/service.py
--rw-rw-rw-   0 root         (0) root         (0)     1867 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/shell.py
--rw-rw-rw-   0 root         (0) root         (0)     2325 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/status.py
--rw-rw-rw-   0 root         (0) root         (0)     6761 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/stor.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/token.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/plugins/upgrade.py
--rw-rw-rw-   0 root         (0) root         (0)     1130 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/rel_opts.py
--rw-rw-rw-   0 root         (0) root         (0)     2864 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/sstatus.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 20:02:42.148371 vss-cli-2023.9.0.dev8/vss_cli/utils/
--rw-rw-rw-   0 root         (0) root         (0)       36 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    75203 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/utils/emoji.py
--rw-rw-rw-   0 root         (0) root         (0)     2929 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/utils/threading.py
--rw-rw-rw-   0 root         (0) root         (0)     4734 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/validators.py
--rw-rw-rw-   0 root         (0) root         (0)     1225 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/vss.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/vssconst.py
--rw-rw-rw-   0 root         (0) root         (0)      951 2023-09-26 18:05:50.000000 vss-cli-2023.9.0.dev8/vss_cli/yaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-28 20:02:42.136371 vss-cli-2023.9.0.dev8/vss_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)    12302 2023-09-28 20:02:42.000000 vss-cli-2023.9.0.dev8/vss_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2388 2023-09-28 20:02:42.000000 vss-cli-2023.9.0.dev8/vss_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-28 20:02:42.000000 vss-cli-2023.9.0.dev8/vss_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       66 2023-09-28 20:02:42.000000 vss-cli-2023.9.0.dev8/vss_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-28 20:02:42.000000 vss-cli-2023.9.0.dev8/vss_cli.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      663 2023-09-28 20:02:42.000000 vss-cli-2023.9.0.dev8/vss_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-09-28 20:02:42.000000 vss-cli-2023.9.0.dev8/vss_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.077841 vss-cli-2024.5.0.dev0/
+-rw-rw-rw-   0 root         (0) root         (0)     1078 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    13872 2024-05-21 00:53:26.077841 vss-cli-2024.5.0.dev0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    10991 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       62 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1257 2024-05-21 00:53:26.077841 vss-cli-2024.5.0.dev0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     3827 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.057841 vss-cli-2024.5.0.dev0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     5569 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/tests/test_vss_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.061841 vss-cli-2024.5.0.dev0/vss_cli/
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    19671 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/autocompletion.py
+-rw-rw-rw-   0 root         (0) root         (0)     7453 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)    64867 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    15369 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.065841 vss-cli-2024.5.0.dev0/vss_cli/data/
+-rw-rw-rw-   0 root         (0) root         (0)     4500 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data/clib.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4288 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data/clone.yaml
+-rw-rw-rw-   0 root         (0) root         (0)      577 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data/config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2892 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data/image.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     2926 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data/shell.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     4198 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data/template.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    25848 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)      819 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/hcio.py
+-rw-rw-rw-   0 root         (0) root         (0)    12512 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.069841 vss-cli-2024.5.0.dev0/vss_cli/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-21 00:53:21.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15976 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/account.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/completion.py
+-rw-rw-rw-   0 root         (0) root         (0)      908 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.073841 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      196 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8906 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/callbacks.py
+-rw-rw-rw-   0 root         (0) root         (0)     4015 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/contentlib.py
+-rw-rw-rw-   0 root         (0) root         (0)     2813 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/domain.py
+-rw-rw-rw-   0 root         (0) root         (0)     3133 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/floppy.py
+-rw-rw-rw-   0 root         (0) root         (0)     8680 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2488 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/helper.py
+-rw-rw-rw-   0 root         (0) root         (0)     3287 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2841 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     3046 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/iso.py
+-rw-rw-rw-   0 root         (0) root         (0)     3477 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/net.py
+-rw-rw-rw-   0 root         (0) root         (0)     1665 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/os.py
+-rw-rw-rw-   0 root         (0) root         (0)      644 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/rel_args.py
+-rw-rw-rw-   0 root         (0) root         (0)     9604 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     3790 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/template.py
+-rw-rw-rw-   0 root         (0) root         (0)   149779 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/vm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1907 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/vmdks.py
+-rw-rw-rw-   0 root         (0) root         (0)    10871 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/configure.py
+-rw-rw-rw-   0 root         (0) root         (0)     3481 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/key.py
+-rw-rw-rw-   0 root         (0) root         (0)     3010 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/message.py
+-rw-rw-rw-   0 root         (0) root         (0)     1947 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/misc.py
+-rw-rw-rw-   0 root         (0) root         (0)     4310 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/ovf.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/plugins.py
+-rw-rw-rw-   0 root         (0) root         (0)     1362 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/raw.py
+-rw-rw-rw-   0 root         (0) root         (0)      608 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.073841 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/
+-rw-rw-rw-   0 root         (0) root         (0)      204 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5330 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/change.py
+-rw-rw-rw-   0 root         (0) root         (0)     2306 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/export.py
+-rw-rw-rw-   0 root         (0) root         (0)     2372 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     2362 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/image.py
+-rw-rw-rw-   0 root         (0) root         (0)     2345 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/new.py
+-rw-rw-rw-   0 root         (0) root         (0)     2366 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/restore.py
+-rw-rw-rw-   0 root         (0) root         (0)     3924 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/retirement.py
+-rw-rw-rw-   0 root         (0) root         (0)     3307 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/snapshot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2246 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/vmdk.py
+-rw-rw-rw-   0 root         (0) root         (0)     1614 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1867 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/shell.py
+-rw-rw-rw-   0 root         (0) root         (0)     2325 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/status.py
+-rw-rw-rw-   0 root         (0) root         (0)     6761 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/stor.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/token.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/plugins/upgrade.py
+-rw-rw-rw-   0 root         (0) root         (0)     1130 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/rel_opts.py
+-rw-rw-rw-   0 root         (0) root         (0)     2864 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/sstatus.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.073841 vss-cli-2024.5.0.dev0/vss_cli/utils/
+-rw-rw-rw-   0 root         (0) root         (0)       36 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    75203 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/utils/emoji.py
+-rw-rw-rw-   0 root         (0) root         (0)     2929 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/utils/threading.py
+-rw-rw-rw-   0 root         (0) root         (0)     4734 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/validators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1225 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/vss.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/vssconst.py
+-rw-rw-rw-   0 root         (0) root         (0)      951 2024-05-21 00:52:44.000000 vss-cli-2024.5.0.dev0/vss_cli/yaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 00:53:26.065841 vss-cli-2024.5.0.dev0/vss_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    13872 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2453 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       66 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      683 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-05-21 00:53:26.000000 vss-cli-2024.5.0.dev0/vss_cli.egg-info/top_level.txt
```

### Comparing `vss-cli-2023.9.0.dev8/LICENSE` & `vss-cli-2024.5.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/PKG-INFO` & `vss-cli-2024.5.0.dev0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,7 @@
-Metadata-Version: 2.1
-Name: vss-cli
-Version: 2023.9.0.dev8
-Summary: ITS Private Cloud Command Line Interface
-Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2023.9.0-dev8.zip
-Author: University of Toronto
-Author-email: vss-apps@eis.utoronto.ca
-Maintainer-email: vss-py@eis.utoronto.ca
-License: MIT
-Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
-Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
-Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Platform: any
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: System Administrators
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Topic :: System :: Systems Administration
-Requires-Python: >=3.7.5
-Description-Content-Type: text/markdown
-Provides-Extra: test
-Provides-Extra: dev
-Provides-Extra: stor
-License-File: LICENSE
-
 # ITS Private Cloud Command Line Interface ``vss-cli``
 
 [![PyPI][pypi-img]](https://pypi.python.org/pypi/vss-cli)
 [![PyPI version][pyver-img]](https://pypi.python.org/pypi/vss-cli)
 
 
 The ITS Private Cloud Command-Line Interface ``vss-cli`` simplifies the interaction with the 
@@ -376,8 +344,8 @@
 [pypi-img]: https://img.shields.io/pypi/v/vss-cli.svg
 [pyver-img]: https://img.shields.io/pypi/pyversions/vss-cli.svg
 [docker-pulls-img]:  https://img.shields.io/docker/pulls/uofteis/vss-cli.svg
 [docker-image]: https://hub.docker.com/r/uofteis/vss-cli/
 [python-tabulate]: https://pypi.org/project/tabulate/
 [ITS Private Cloud RESTful API]: https://vss-wiki.eis.utoronto.ca/display/API
 [Pull Request #76]: https://github.com/click-contrib/click-repl/pull/76
-[Homebrew]: https://brew.sh/
+[Homebrew]: https://brew.sh/
```

### Comparing `vss-cli-2023.9.0.dev8/setup.cfg` & `vss-cli-2024.5.0.dev0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/setup.py` & `vss-cli-2024.5.0.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/autocompletion.py` & `vss-cli-2024.5.0.dev0/vss_cli/autocompletion.py`

 * *Files 4% similar despite different names*

```diff
@@ -567,14 +567,28 @@
         incomplete,
         attrs=['id', 'name'],
         f_kwargs={"sort": "created_on,desc", "per_page": 500},
     )
 
 
 @to_completion_item
+def vm_gpu_profiles(
+    ctx: Configuration, param: click.Option, incomplete: str
+) -> List[Tuple[str, str]]:
+    """Autocomplete VM gpu profiles."""
+    _init_ctx(ctx)
+    return _autocomplete(
+        ctx.client.get_supported_gpu_types,
+        incomplete,
+        attrs=['type', 'description'],
+        f_kwargs={"only_type": False},
+    )
+
+
+@to_completion_item
 def vm_firmware(
     ctx: Configuration, param: click.Option, incomplete: str
 ) -> List[Tuple[str, str]]:
     """Autocomplete VM firmware types."""
     _init_ctx(ctx)
     return _autocomplete(
         ctx.client.get_supported_firmware_types,
@@ -631,14 +645,27 @@
         ctx.client.get_retirement_requests,
         incomplete,
         attrs=['id', 'vm_moref', 'vm_name', 'retire_on'],
         f_kwargs={"sort": "created_on,desc", "per_page": 500},
     )
 
 
+def restore_requests(
+    ctx: Configuration, param: click.Option, incomplete: str
+) -> List[Tuple[str, str]]:
+    """Autocomplete VM restore requests."""
+    _init_ctx(ctx)
+    return _autocomplete(
+        ctx.client.get_restore_requests,
+        incomplete,
+        attrs=['id', 'vm_moref', 'vm_name', 'timestamp'],
+        f_kwargs={"sort": "created_on,desc", "per_page": 500},
+    )
+
+
 @to_completion_item
 def vm_retirement_requests(
     ctx: Configuration, param: click.Option, incomplete: str
 ) -> List[Tuple[str, str]]:
     """Autocomplete VM retirement requests by VM."""
     _init_ctx(ctx)
     args = ctx.params
@@ -650,7 +677,28 @@
                 incomplete,
                 attrs=['id', 'name', 'description'],
                 f_kwargs={'vm_id': vm_id},
             )
         except IndexError:
             return []
     return []
+
+
+@to_completion_item
+def vm_restore_points(
+    ctx: Configuration, param: click.Option, incomplete: str
+) -> List[Tuple[str, str]]:
+    """Autocomplete VM restore points."""
+    _init_ctx(ctx)
+    args = ctx.params
+    if 'vm_id' in args:
+        try:
+            vm_id = args['vm_id']
+            return _autocomplete(
+                ctx.client.get_vm_restore_points,
+                incomplete,
+                attrs=['id', 'timestamp'],
+                f_kwargs={'moref': vm_id, 'show_all': True, 'per_page': 120},
+            )
+        except KeyError:
+            return []
+    return []
```

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/cli.py` & `vss-cli-2024.5.0.dev0/vss_cli/cli.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/config.py` & `vss-cli-2024.5.0.dev0/vss_cli/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 """Configuration for VSS CLI (vss-cli)."""
-from base64 import b64decode, b64encode
 import functools
 import json
 import logging
 import os
-from pathlib import Path
 import platform
 import sys
+from base64 import b64decode, b64encode
+from pathlib import Path
 from time import sleep
 from typing import (  # noqa: F401
     Any, Callable, Dict, List, Optional, Tuple, Union, cast)
 
 import click
-from click_spinner import Spinner, spinner
 import jwt
+from click_spinner import Spinner, spinner
 from pick import pick
 from pyvss.const import __version__ as pyvss_version
 from pyvss.enums import RequestStatus
 from pyvss.exceptions import VssError
 from pyvss.manager import VssManager
 from ruamel.yaml import YAML
 
 import vss_cli.const as const
+import vss_cli.yaml as yaml
 from vss_cli.data_types import ConfigEndpoint, ConfigFile, ConfigFileGeneral
 from vss_cli.exceptions import VssCliError
 from vss_cli.helper import (
     bytes_to_str, debug_requests_on, format_output, get_hostname_from_url)
 from vss_cli.utils.emoji import EMOJI_UNICODE
 from vss_cli.utils.threading import WorkerQueue
 from vss_cli.validators import (
     validate_email, validate_json_file_or_type, validate_phone_number,
     validate_uuid, validate_vm_moref)
-import vss_cli.yaml as yaml
 
 _LOGGING = logging.getLogger(__name__)
 
 
 class Configuration(VssManager):
     """The configuration context for the VSS CLI."""
 
@@ -416,15 +416,19 @@
                         # check valid creds
                         if not (usr and pwd or getattr(ep, 'token', None)):
                             _LOGGING.warning(msg)
                             default_endpoint = const.DEFAULT_ENDPOINT_NAME
                             _LOGGING.warning(
                                 f'Falling back to {default_endpoint}'
                             )
-                            (ep, usr, pwd,) = self.load_profile(  # NOQA: E501
+                            (
+                                ep,
+                                usr,
+                                pwd,
+                            ) = self.load_profile(  # NOQA: E501
                                 endpoint=const.DEFAULT_ENDPOINT_NAME
                             )
                         # set config_path data
                         self.set_credentials(
                             usr,
                             pwd,
                             ep.token,
@@ -500,15 +504,15 @@
     def check_available_updates(self) -> None:
         """Check available update from PyPI."""
         try:
             _LOGGING.debug('Checking for available updates.')
             cmd_bin = sys.executable
             # create command with the right exec
             pip_cmd = f'{cmd_bin} -m pip list --outdated'.split(None)
-            from subprocess import Popen, PIPE
+            from subprocess import PIPE, Popen
 
             p = Popen(pip_cmd, stdin=PIPE, stdout=PIPE, stderr=PIPE)
             out, err = p.communicate()
             out_decoded = out.decode('utf-8')
             # verify if package name is in outdated string
             pkg_name = const.PACKAGE_NAME.replace('_', '-')
             if pkg_name in out_decoded:
@@ -822,19 +826,26 @@
         """
         _objs = []
         for attr in attrs:
             attr_name = attr[0]
             attr_type = attr[1]
             try:
                 if attr_type in [str]:
-                    f = filter(
-                        lambda i: attr_type(value).lower()
-                        in i[attr_name].lower(),
-                        objects,
-                    )
+                    if attr_name in ['moref', 'uuid']:
+                        f = filter(
+                            lambda i: attr_type(value).lower()
+                            == i[attr_name].lower(),
+                            objects,
+                        )
+                    else:
+                        f = filter(
+                            lambda i: attr_type(value).lower()
+                            in i[attr_name].lower(),
+                            objects,
+                        )
                 elif attr_type in [int]:
                     f = filter(
                         lambda i: attr_type(value) == i[attr_name], objects
                     )
                 else:
                     f = filter(
                         lambda i: attr_type(value) in i[attr_name], objects
@@ -945,14 +956,31 @@
         if d_count > 1:
             return self.pick(
                 objs,
                 options=[f"{i['name']} ({i['description']})" for i in objs],
             )
         return objs
 
+    def get_vm_restore_points_by_id_or_timestamp(
+        self, vm_id: str, id_or_timestamp: str
+    ) -> List[Dict]:
+        """Get vm restore points by id or timestamp."""
+        rps = self.get_vm_restore_points(vm_id)
+        attributes = [('id', int), ('timestamp', str)]
+        objs = self._filter_objects_by_attrs(id_or_timestamp, rps, attributes)
+        if not objs:
+            raise click.BadParameter(f'{id_or_timestamp} could not be found')
+        d_count = len(objs)
+        if d_count > 1:
+            return self.pick(
+                objs,
+                options=[f"{i['id']} ({i['timestamp']})" for i in objs],
+            )
+        return objs
+
     def get_domain_by_name_or_moref(self, name_or_moref: str) -> List[Dict]:
         """Get domain by name or mo reference."""
         g_domains = self.get_domains()
         attributes = [('name', str), ('moref', str)]
         objs = self._filter_objects_by_attrs(
             name_or_moref, g_domains, attributes
         )
@@ -1184,14 +1212,22 @@
         """Get VM firmware by name."""
         return self._get_types_by_name(
             name,
             self.get_supported_firmware_types,
             attrs=[('type', str), ('description', str)],
         )
 
+    def get_vm_gpu_profiles_by_name_or_desc(self, name: Union[str, int]):
+        """Get VM gpu by name or desc."""
+        return self._get_types_by_name(
+            name,
+            self.get_supported_gpu_types,
+            attrs=[('type', str), ('description', str)],
+        )
+
     def get_vm_storage_type_by_type_or_desc(self, name: Union[str, int]):
         """Get VM supported storage types by name."""
         return self._get_types_by_name(
             name,
             self.get_supported_storage_types,
             attrs=[('type', str), ('description', str)],
         )
@@ -1349,14 +1385,15 @@
                 raw_dparams = value.get('Configuration') or value.get(
                     'ovf:Configuration', []
                 )
                 dparams = []
                 for x in raw_dparams:
                     _desc = x.get('Description') or x.get('ovf:Description')
                     _label = x.get('Label') or x.get('ovf:Label')
+                    label = ''
                     description = _desc
                     if isinstance(_desc, dict):
                         if '@ovf:msgid' in _desc or 'msgid' in _desc:
                             description = ovf_strings.get(
                                 _desc.get('@ovf:msgid') or _desc.get('msgid')
                             )
                     if isinstance(_label, dict):
@@ -1375,35 +1412,53 @@
             # ovf:VirtualSystem
             elif key in ['VirtualSystem', 'ovf:VirtualSystem']:
                 output['Name'] = value.get('ovf:Name') or value.get('Name')
                 if 'ovf:ProductSection' in value or 'ProductSection' in value:
                     prod_sect = value.get('ProductSection') or value.get(
                         'ovf:ProductSection'
                     )
-                    output['Product'] = prod_sect.get(
-                        'Product'
-                    ) or prod_sect.get('ovf:FullVersion')
-                    output['Version'] = prod_sect.get(
-                        'Version'
-                    ) or prod_sect.get('ovf:Version')
-                    if 'Property' in prod_sect or 'ovf:Property' in prod_sect:
+                    prod_props = []
+                    if isinstance(prod_sect, list):
+                        for item in prod_sect:
+                            if 'Product' in item:
+                                output['Product'] = item.get('Product')
+                            if 'Vendor' in item:
+                                output['Vendor'] = item.get('Vendor')
+                            if 'Property' in item:
+                                prod_props.extend(item.get('Property', []))
+                    elif isinstance(prod_sect, dict):
+                        output['Product'] = prod_sect.get(
+                            'Product'
+                        ) or prod_sect.get('ovf:FullVersion')
+                        output['Version'] = prod_sect.get(
+                            'Version'
+                        ) or prod_sect.get('ovf:Version')
+                    if (
+                        'Property' in prod_sect
+                        or 'ovf:Property' in prod_sect
+                        or prod_props
+                    ):
                         pparams = []
-                        properties = prod_sect.get(
-                            'Property'
-                        ) or prod_sect.get('ovf:Property', [])
+                        properties = (
+                            prod_props
+                            or prod_sect.get('Property')
+                            or prod_sect.get('ovf:Property', [])
+                        )
                         for prop in properties:
                             if (
                                 prop.get('@ovf:userConfigurable', None)
                                 == 'true'
                             ):
                                 prop = {
                                     'key': prop['@ovf:key'],
                                     'type': prop['@ovf:type'],
                                     'description': prop.get('Description')
-                                    or prop.get('ovf:Description'),
+                                    or prop.get('ovf:Description')
+                                    or prop.get('Label')
+                                    or prop.get('ovf:Label'),
                                     'default': prop.get('@ovf:value'),
                                 }
                                 pparams.append(prop)
                         output['PropertyParams'] = pparams
         return output
 
     def yaml(self) -> YAML:
```

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/const.py` & `vss-cli-2024.5.0.dev0/vss_cli/const.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Constants used by VSS CLI (vss-cli)."""
 import os
 
 import pkg_resources
 
 PACKAGE_NAME = "vss_cli"
 
-__version__ = "2023.9.0-dev8"
+__version__ = "2024.5.0-dev0"
 
 
 DEFAULT_TIMEOUT = 30
 DEFAULT_ENDPOINT = "https://cloud-api.eis.utoronto.ca"
 DEFAULT_ENDPOINT_NAME = "cloud-api"
 DEFAULT_S3_SERVER = "https://vskey-stor.eis.utoronto.ca"
 _LEGACY_CONFIG = ("~", ".vss-cli", "config.json")
@@ -83,29 +83,58 @@
 DEFAULT_STATE_MSG = (
     "Host Name:\t{hostname} ({os[full_name]})\n"
     "IP Address:\t{ip_addresses}\n"
     "Are you sure you want to change the state from "
     '"{guest_state} to {state}" '
     "of the above VM?"
 )
-
+_DEFAULT_VM_INFO = (
+    "Moref:\t\t{vm[moref]}\n"
+    "UUID:\t\t{vm[uuid]}\n"
+    "Name:\t\t{vm[name]}\n"
+    "Folder:\t\t{vm[folder][path]}\n"
+    "Host Name:\t{vm[hostname]} "
+    "({vm[guest_full_name]})\n"
+    "IP Address:\t{vm[ip_address]}\n"
+    "MAC Address:\t{vm[mac_address]}\n"
+    "Create Date:\t{vm[create_date]}\n"
+)
+DEFAULT_VM_DISK_CP_MSG = (
+    f"{_DEFAULT_VM_INFO}"
+    "Are you sure you want to copy the "
+    "following disk(s) "
+    "the above VM?\n\n"
+    "{msg}"
+)
 DEFAULT_VM_DEL_MSG = (
+    f"{_DEFAULT_VM_INFO}" "Are you sure you want to delete " "the above VM?"
+)
+DEFAULT_VM_RESTORE_MSG = (
     "Moref:\t\t{vm[moref]}\n"
     "UUID:\t\t{vm[uuid]}\n"
     "Name:\t\t{vm[name]}\n"
     "Folder:\t\t{vm[folder][path]}\n"
     "Host Name:\t{vm[hostname]} "
     "({vm[guest_full_name]})\n"
     "IP Address:\t{vm[ip_address]}\n"
     "MAC Address:\t{vm[mac_address]}\n"
     "Create Date:\t{vm[create_date]}\n"
-    "Are you sure you want to delete "
-    "the above VM?"
+    "Storage (GB):\t{vm[provisioned_gb]}\n"
+    "Storage Type:\t{vm[storage_type]}\n\n"
+    "Are you sure you want to restore "
+    "the above VM to timestamp {rp[timestamp]}?"
+)
+VM_RESTORE_PRICE_GB = {'ssd': 0.60, 'hdd': 0.3}
+CONFIRM_VM_RESTORE_MSG = (
+    '\nYou are requesting a service that is immediately '
+    'billable at ${ssd} per GB for SSD \n'
+    'and ${hdd} per GB for HDD, which will appear in your next bill.\n\n'
+    'This VM is {provisioned_gb:.2f}GB and Restoring will cost '
+    '${total_gb:.2f}.\n\nDo you agree?'
 )
-
 COLUMNS_TWO_FMT = "{0:<20}: {1:<20}"
 
 COLUMNS_DEFAULT = [("all", "*")]
 COLUMNS_MFA_MIN = [("message",), ("type",)]
 COLUMNS_VM_MIN = [("moref",), ("name",)]
 COLUMNS_VIM_REQUEST = [("vm_moref",), ("vm_name",)]
 COLUMNS_MOREF = [("moref",), ("name",)]
@@ -165,14 +194,21 @@
 ]
 COLUMNS_REQUEST_MULT_SUBMITTED = [
     ("id", "request.id[*]"),
     ("status", "request.status[*]"),
     ("task_id", "request.task_id[*]"),
     ("message",),
 ]
+COLUMNS_REQUEST_RESTORE = [
+    *COLUMNS_REQUEST,
+    *COLUMNS_VIM_REQUEST,
+    ("timestamp",),
+    ("result_vm_name",),
+    ("result_vm_moref",),
+]
 COLUMNS_REQUEST_RETIRE = [
     *COLUMNS_REQUEST,
     *COLUMNS_VIM_REQUEST,
     ("retire_on",),
     ("warning",),
     ("warning_on",),
 ]
@@ -326,17 +362,18 @@
 COLUMNS_VM_OS = [
     ("cfg.full_name",),
     ("cfg.guest_id",),
     ("guest.guest_full_name",),
     ("guest.guest_id",),
     ("guest.guest_family",),
 ]
-COLUMNS_VM_HAGROUP = [*COLUMNS_VM_MIN, ("VALID", "valid")]
+COLUMNS_VM_HAGROUP = [*COLUMNS_VM_MIN, ("domain.name",), ("group", "group[*]")]
 COLUMNS_VM_MEMORY = [
     ("memory_gb",),
+    ("memory_gb_reserved", "reservation.memory_gb_reserved"),
     ("hot_add.enabled",),
     ("hot_add.limit_gb",),
     ("ballooned_memory_mb", "quick_stats.ballooned_memory_mb"),
     ("guest_memory_usage_mb", "quick_stats.guest_memory_usage_mb"),
 ]
 COLUMNS_VM_NIC_MIN = [
     ("label",),
```

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/data/clib.yaml` & `vss-cli-2024.5.0.dev0/vss_cli/data/clib.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from CLib 2023.9.0-dev8             #
+#     VSS-CLI Spec from CLib 2024.5.0-dev0             #
 ####################################################
 built: clib               # Required: Do not remove.
 machine:
   item: ubuntu-22.04      # Required: Source content library id OVF.
   cpu: 1                  # Optional: CPU count (Default: 1).
   memory: 1               # Optional: Memory in GB (Default: 1GB).
   name: &name Vm-Name     # Required: Target virtual machine name.
@@ -29,15 +29,15 @@
 # metadata required
 metadata:
   client: Department     # Required: Client department
   # Required: Description of virtual machine
   description: >
     nginx and database server for a very important service.
   usage: Test             # Optional: Usage between Prod | Dev | QA | Test (default: Test)
-  inform:                 # Optional: list of additional contact email addresses (default: user account)
+  inform:                 # Required: list of additional contact email addresses
     - email@utoronto.ca
 #  admin:                  # Optional: VM Administrator (Default: user submitting request)
 #    name:                 # (Admin) Required: VM Administrator full name
 #    email:                # (Admin) Required: VM Administrator email i.e. user@utoronto.ca
 #    phone:                # (Admin) Required: VM Administrator phone i.e. 416-123-2341
 # Recommended Metadata (Uncomment to enable)
 #   notes:                  # Optional: list of key-value items to be set in Key: value form.
```

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/data/clone.yaml` & `vss-cli-2024.5.0.dev0/vss_cli/data/clone.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Clone 2023.9.0-dev8             #
+#     VSS-CLI Spec from Clone 2024.5.0-dev0             #
 ####################################################
 built: clone              # Required: Do not remove.
 machine:
   source: SourceVM        # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   disks:                  # Optional: Disks (Default: source vm disk layout)
     - capacity_gb: 40     # Optional: Disk capacity in GB (Default: source vm disk capacity)
@@ -42,15 +42,15 @@
 #      - 10.6.0.1
 # Metadata required
 metadata:                 # Optional: Description of virtual machine
   description: >
     nginx and database server for a very important service.
   usage: Test             # Optional: Usage between Prod | Dev | QA | Test (default: source vm usage)
   client: Department      # Optional: Client department (default: source vm client)
-  inform:                 # Optional: list of email addresses. (default: source vm inform)
+  inform:                 # Required: list of email addresses. (default: source vm inform)
     - email@utoronto.ca
   admin:                  # Optional: VM Administrator (Default: source vm admin)
     name:                 # (Admin) Required: VM Administrator full name
     email:                # (Admin) Required: VM Administrator email i.e. user@utoronto.ca
     phone:                # (Admin) Required: VM Administrator phone i.e. 416-123-2341
 #  vss_service: N/A        # Optional: VSS Service name or service id
 # Recommended Metadata (Uncomment to enable)
```

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/data/config.yaml` & `vss-cli-2024.5.0.dev0/vss_cli/data/config.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/data/image.yaml` & `vss-cli-2024.5.0.dev0/vss_cli/data/image.yaml`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/data/shell.yaml` & `vss-cli-2024.5.0.dev0/vss_cli/data/shell.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec shell VM v2023.9.0-dev8             #
+#     VSS-CLI Spec shell VM 2024.5.0-dev0             #
 ####################################################
 built: os_install         # Required: Do not remove.
 machine:
   name: Vm-Name            # Required: Target virtual machine name.
   os: ubuntu64Guest              # Required: Guest Operating System name or Id.
   cpu: 1                   # Optional: CPU count (Default: 1).
   memory: 1                # Optional: Memory in GB (Default: 1GB).
@@ -31,15 +31,15 @@
 # metadata required
 metadata:
   client: Department     # Required: Client department
   # Required: Description of virtual machine
   description: >
     nginx and database server for a very important service.
   usage: Test             # Optional: Usage between Prod | Dev | QA | Test (default: Test)
-  inform:                 # Optional: list of additional contact email addresses (default: user account)
+  inform:                 # Required: list of additional contact email addresses
     - email@utoronto.ca
 #  admin:                  # Optional: VM Administrator (Default: user submitting request)
 #    name:                 # (Admin) Required: VM Administrator full name
 #    email:                # (Admin) Required: VM Administrator email i.e. user@utoronto.ca
 #    phone:                # (Admin) Required: VM Administrator phone i.e. 416-123-2341
 # Recommended Metadata (Uncomment to enable)
 # notes:                  # Optional: list of key-value items to be set in Key: value form.
```

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/data/template.yaml` & `vss-cli-2024.5.0.dev0/vss_cli/data/template.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ####################################################
-#     VSS-CLI Spec from Template v2023.9.0-dev8         #
+#     VSS-CLI Spec from Template 2024.5.0-dev0        #
 ####################################################
 built: template           # Required: Do not remove.
 machine:
   source: NixSource                # Required: Can be a vm name or a vm id.
   name: &name Vm-Name     # Required: Target virtual machine name
   folder: MyFolder       # Optional: Folder name, path or ID (Default: source vm folder)
   disks:                  # Optional: Disks (Default: source vm disk layout)
@@ -41,15 +41,15 @@
 #      - 10.6.0.1
 # Metadata required
 metadata:                 # Optional: Description of virtual machine
   description: >
     nginx and database server for a very important service.
   usage: Test             # Optional: Usage between Prod | Dev | QA | Test (default: source vm usage)
   client: Department      # Optional: Client department (default: source vm client)
-  inform:                 # Optional: list of email addresses. (default: source vm inform)
+  inform:                 # Required: list of email addresses. (default: source vm inform)
     - email@utoronto.ca
   admin:                  # Optional: VM Administrator (Default: source vm admin)
     name:                 # (Admin) Required: VM Administrator full name
     email:                # (Admin) Required: VM Administrator email i.e. user@utoronto.ca
     phone:                # (Admin) Required: VM Administrator phone i.e. 416-123-2341
 #  vss_service: N/A        # Optional: VSS Service name or service id
 # Recommended Metadata (Uncomment to enable)
```

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/data_types.py` & `vss-cli-2024.5.0.dev0/vss_cli/data_types.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/hcio.py` & `vss-cli-2024.5.0.dev0/vss_cli/hcio.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/helper.py` & `vss-cli-2024.5.0.dev0/vss_cli/helper.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/account.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/account.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/completion.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/completion.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/callbacks.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/callbacks.py`

 * *Files 8% similar despite different names*

```diff
@@ -142,25 +142,26 @@
                     _backing_mode = (
                         ctx.client.get_vm_disk_backing_mode_by_name(  # NOQA:
                             _dev.get('backing_mode')
                         )
                     )
                     _backing_mode = _backing_mode[0]['type']
                     disk['backing_mode'] = _backing_mode
+                else:
+                    disk['backing_mode'] = _backing_mode
                 if _dev.get('backing_sharing'):
                     _sharing_mode = ctx.client.get_vm_disk_backing_sharing_by_name(  # NOQA:
                         _dev.get('backing_sharing')
                     )
                     _sharing_mode = _sharing_mode[0]['type']
                     disk['backing_sharing'] = _sharing_mode
+                else:
+                    disk['backing_sharing'] = _sharing_mode
                 if _dev.get('backing_vmdk'):
-                    _backing_vmdk = ctx.client.get_vmdk_by_name_path_or_id(
-                        _dev.get('backing_vmdk')
-                    )
-                    disk['backing_vmdk'] = _backing_vmdk[0]['path']
+                    disk['backing_vmdk'] = _dev.get('backing_vmdk')
                 if _dev.get('scsi') is not None:
                     try:
                         _scsi_crllr = int(_dev.get('scsi'))
                     except ValueError:
                         raise BadParameter('scsi must be a number')
                     disk['scsi'] = _scsi_crllr
             else:
@@ -176,19 +177,15 @@
                         _spec = to_tuples(_spec[1])[0]
                         _sharing_mode = ctx.client.get_vm_disk_backing_sharing_by_name(  # NOQA
                             _spec[0]
                         )
                         _sharing_mode = _sharing_mode[0]['type']
                         disk['backing_sharing'] = _sharing_mode
                     if len(_spec) > 1:
-                        _backing_vmdk = ctx.client.get_vmdk_by_name_path_or_id(
-                            _spec[1]
-                        )
-                        _backing_vmdk = _backing_vmdk[0]['path']
-                        disk['backing_vmdk'] = _backing_vmdk
+                        disk['backing_vmdk'] = _spec[1]
             devices.append(disk)
         return devices
 
 
 def process_options(ctx: Configuration, param, key_value):
     """Process options."""
     _init_ctx(ctx)
```

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/contentlib.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/contentlib.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/domain.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/domain.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/floppy.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/floppy.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/folder.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/image.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/inventory.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/iso.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/iso.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/net.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/net.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/os.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/os.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/rel_args.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/rel_args.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/rel_opts.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/rel_opts.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,15 @@
     multiple=True,
     required=False,
     callback=callbacks.process_disk_opt,
 )
 disk_opt = click.option(
     '--disk',
     '-i',
-    help='Disk spec <capacity>=<backing_mode>=<backing_sharing>. '
+    help='Disk spec <capacity>=<backing_mode>=<backing_sharing>=<backing_vmdk>. '  # NOQA:
     'optional: backing_mode, backing_sharing',
     type=click.STRING,
     multiple=True,
     required=True,
     callback=callbacks.process_disk_opt,
 )
 domain_opt = click.option(
@@ -318,14 +318,22 @@
 )
 vss_options_opt = click.option(
     '--vss-option',
     help='VSS Option to enable',
     shell_complete=autocompletion.vss_options,
     required=False,
 )
+gpu_profile_opt = click.option(
+    '--profile',
+    '-p',
+    type=click.STRING,
+    help='GPU Profile',
+    shell_complete=autocompletion.vm_gpu_profiles,
+    required=True,
+)
 firmware_nr_opt = click.option(
     '--firmware',
     '-w',
     help='Firmware type.',
     shell_complete=autocompletion.vm_firmware,
     required=False,
 )
```

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/template.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/template.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/vm.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/vm.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,24 +5,27 @@
 from pathlib import Path
 from typing import Optional
 
 import click
 from click_plugins import with_plugins
 from pkg_resources import iter_entry_points
 
-from vss_cli import const, rel_opts as so
 import vss_cli.autocompletion as autocompletion
+from vss_cli import const
+from vss_cli import rel_opts as so
 from vss_cli.cli import pass_context
 from vss_cli.config import Configuration
 from vss_cli.data_types import VmApiSpec, VmCliSpec
 from vss_cli.exceptions import VssCliError
 from vss_cli.helper import format_output, raw_format_output, to_tuples
 from vss_cli.plugins.compute import cli
-from vss_cli.plugins.compute_plugins import rel_args as c_sa, rel_opts as c_so
-from vss_cli.plugins.compute_plugins.helper import process_retirement_new
+from vss_cli.plugins.compute_plugins import rel_args as c_sa
+from vss_cli.plugins.compute_plugins import rel_opts as c_so
+from vss_cli.plugins.compute_plugins.helper import (
+    get_restore_user_confirmation, process_retirement_new)
 from vss_cli.validators import (
     flexible_email_args, retirement_value, validate_email, validate_json_type,
     validate_phone_number)
 
 _LOGGING = logging.getLogger(__name__)
 
 
@@ -771,15 +774,15 @@
 
 @compute_vm_get.command('gpu', short_help='GPU configuration')
 @pass_context
 def compute_vm_get_gpu(ctx: Configuration):
     """Virtual machine gpu configuration."""
     columns = ctx.columns or const.COLUMNS_VM_GPU
     objs = ctx.get_vm_gpu(ctx.moref)
-    ctx.echo(format_output(ctx, objs, columns=columns, single=True))
+    ctx.echo(format_output(ctx, objs, columns=columns))
 
 
 @compute_vm_get.group('restore-point', short_help='Restore Points')
 @pass_context
 def compute_vm_get_rp(ctx: Configuration):
     """Virtual machine restore points configuration."""
 
@@ -1599,14 +1602,76 @@
     columns = ctx.columns or const.COLUMNS_REQUEST_SUBMITTED
     ctx.echo(format_output(ctx, [obj], columns=columns, single=True))
     # wait for request
     if ctx.wait_for_requests:
         ctx.wait_for_request_to(obj)
 
 
+@compute_vm_set.group('gpu', short_help='vGPU management')
+@pass_context
+def compute_vm_set_gpu(ctx: Configuration):
+    """Manage virtual Graphics Processing Unit."""
+    pass
+
+
+@compute_vm_set_gpu.command('mk', short_help='Create vGPU')
+@c_so.gpu_profile_opt
+@pass_context
+def compute_vm_set_gpu_mk(ctx: Configuration, profile):
+    """Create GPU based on given profile."""
+    _profile = ctx.get_vm_gpu_profiles_by_name_or_desc(profile)[0]['type']
+    payload = dict(vm_id=ctx.moref, profile=_profile)
+    # add common options
+    payload.update(ctx.payload_options)
+    # submit task
+    obj = ctx.create_vm_gpu(**payload)
+    # print
+    columns = ctx.columns or const.COLUMNS_REQUEST_SUBMITTED
+    ctx.echo(format_output(ctx, [obj], columns=columns, single=True))
+    # wait for request
+    if ctx.wait_for_requests:
+        ctx.wait_for_request_to(obj)
+
+
+@compute_vm_set_gpu.command('up', short_help='Update vGPU')
+@c_so.gpu_profile_opt
+@pass_context
+def compute_vm_set_gpu_up(ctx: Configuration, profile):
+    """Update vm gpu profile."""
+    _profile = ctx.get_vm_gpu_profiles_by_name_or_desc(profile)[0]['type']
+    payload = dict(vm_id=ctx.moref, profile=_profile)
+    # add common options
+    payload.update(ctx.payload_options)
+    # submit task
+    obj = ctx.update_vm_gpu(**payload)
+    # print
+    columns = ctx.columns or const.COLUMNS_REQUEST_SUBMITTED
+    ctx.echo(format_output(ctx, [obj], columns=columns, single=True))
+    # wait for request
+    if ctx.wait_for_requests:
+        ctx.wait_for_request_to(obj)
+
+
+@compute_vm_set_gpu.command('rm', short_help='Delete vGPU')
+@pass_context
+def compute_vm_set_gpu_rm(ctx: Configuration):
+    """Delete VM GPU."""
+    payload = dict(vm_id=ctx.moref)
+    # add common options
+    payload.update(ctx.payload_options)
+    # submit task
+    obj = ctx.delete_vm_gpu(**payload)
+    # print
+    columns = ctx.columns or const.COLUMNS_REQUEST_SUBMITTED
+    ctx.echo(format_output(ctx, [obj], columns=columns, single=True))
+    # wait for request
+    if ctx.wait_for_requests:
+        ctx.wait_for_request_to(obj)
+
+
 @compute_vm_set.group('tpm', short_help='TPM management')
 @pass_context
 def compute_vm_set_tpm(ctx: Configuration):
     """Manage Trusted Platform Module.
 
     Add and remove vTPM.
     """
@@ -1653,14 +1718,58 @@
     """Manage virtual machine disks.
 
     Add, expand and remove virtual disks.
     """
     pass
 
 
+@compute_vm_set_disk.command('cp', short_help='Copy disk(s)')
+@c_so.disk_opt
+@click.option(
+    '-c', '--confirm', is_flag=True, default=False, help='Confirm disk copy'
+)
+@pass_context
+def compute_vm_set_disk_cp(ctx: Configuration, disk, confirm):
+    """Copy given disk from another VM and add it to the current VM.
+
+    vss-cli compute vm set <name-or-vm_id> disk cp
+    -i "<capacity>=<backing_mode>=<backing_sharing>=<backing_file>"
+
+    """
+    payload = dict(vm_id=ctx.moref, disks=disk)
+    # look for backing_file as required
+    rv = list(filter(lambda x: 'backing_vmdk' in x, disk))
+    if not rv:
+        raise click.BadParameter('Missing backing_vmdk')
+    strs = [
+        (
+            f'{d["backing_vmdk"]} - {d["capacity_gb"]} '
+            f'({d["backing_mode"]}:{d["backing_sharing"]})'
+        )
+        for d in disk
+    ]
+    msg = '\n'.join(strs)
+    _vm = ctx.get_vm_by_id_or_name(ctx.moref)
+    if _vm:
+        c_str = const.DEFAULT_VM_DISK_CP_MSG.format(vm=_vm[0], msg=msg)
+        confirm = confirm or click.confirm(c_str)
+        if not confirm:
+            raise click.ClickException('Cancelled by user.')
+    # add common options
+    payload.update(ctx.payload_options)
+    # request
+    obj = ctx.create_vm_disk(**payload)
+    # print
+    columns = ctx.columns or const.COLUMNS_REQUEST_SUBMITTED
+    ctx.echo(format_output(ctx, [obj], columns=columns, single=True))
+    # wait for request
+    if ctx.wait_for_requests:
+        ctx.wait_for_request_to(obj)
+
+
 @compute_vm_set_disk.command('mk', short_help='Create disk(s)')
 @c_so.disk_opt
 @pass_context
 def compute_vm_set_disk_mk(ctx: Configuration, disk):
     """Create virtual machine disk.
 
     vss-cli compute vm set <name-or-vm_id> disk mk
@@ -2349,14 +2458,38 @@
 @compute_vm_set.group('memory')
 @pass_context
 def compute_vm_set_memory(ctx: Configuration):
     """Update virtual machine Memory count and settings."""
     pass
 
 
+@compute_vm_set_memory.command(
+    'reservation', short_help='Update memory reservation in GB'
+)
+@click.argument('memory_gb', type=click.INT, required=True)
+@pass_context
+def compute_vm_set_memory_reservation(ctx: Configuration, memory_gb):
+    """Update virtual machine memory reservation in GB.
+
+    vss-cli compute vm set <name-or-vm_id> memory reservation <memory_gb>
+    """
+    # create payload
+    payload = dict(size=memory_gb, vm_id=ctx.moref)
+    # add common options
+    payload.update(ctx.payload_options)
+    # request
+    obj = ctx.set_vm_memory_reservation(**payload)
+    # print
+    columns = ctx.columns or const.COLUMNS_REQUEST_SUBMITTED
+    ctx.echo(format_output(ctx, [obj], columns=columns, single=True))
+    # wait for request
+    if ctx.wait_for_requests:
+        ctx.wait_for_request_to(obj)
+
+
 @compute_vm_set_memory.command('size', short_help='Update memory size in GB')
 @click.argument('memory_gb', type=click.INT, required=True)
 @pass_context
 def compute_vm_set_memory_size(ctx: Configuration, memory_gb):
     """Update virtual machine memory size in GB.
 
     vss-cli compute vm set <name-or-vm_id> memory size <memory_gb>
@@ -3415,14 +3548,73 @@
     columns = ctx.columns or const.COLUMNS_REQUEST_SUBMITTED
     ctx.echo(format_output(ctx, [obj], columns=columns, single=True))
     # wait for request
     if ctx.wait_for_requests:
         ctx.wait_for_request_to(obj)
 
 
+@compute_vm.command(
+    'res',
+    help='Restore virtual machine from available restore points.',
+)
+@click.option(
+    '-t',
+    '--timestamp',
+    required=True,
+    help='Restore point timestamp or id.',
+    shell_complete=autocompletion.vm_restore_points,
+)
+@click.option(
+    '--reason', type=click.STRING, required=False, help='Restore reason.'
+)
+@click.argument(
+    'vm_id',
+    type=click.STRING,
+    required=True,
+    shell_complete=autocompletion.virtual_machines,
+)
+@pass_context
+def compute_vm_restore(
+    ctx: Configuration, vm_id: str, timestamp: str, reason: str = None
+):
+    """Restore virtual machine from restore point."""
+    _LOGGING.debug(f'Attempting to restore {vm_id}')
+    _vm = ctx.get_vm_by_id_or_name(vm_id)
+    # get moref from reference
+    moref = _vm[0]['moref']
+    # get id from reference
+    _rp = ctx.get_vm_restore_points_by_id_or_timestamp(moref, timestamp)
+    rp_timestamp = _rp[0]['timestamp']
+    #
+    _LOGGING.debug(f'Attempting to restore: {moref} -> {rp_timestamp}')
+    if _vm and _rp:
+        (
+            confirmation,
+            confirmation_2,
+            reason_payload,
+        ) = get_restore_user_confirmation(ctx, _vm, _rp, reason)
+        if not (confirmation and confirmation_2):
+            _LOGGING.warning('No requests have been submitted.')
+            raise click.ClickException('Cancelled by user.')
+        # add user meta.
+        ctx.user_meta = reason_payload
+        # set payload options
+        ctx.payload_options['user_meta'] = ctx.user_meta
+        payload = dict(moref=moref, timestamp=rp_timestamp)
+        payload.update(ctx.payload_options)
+        _LOGGING.debug(f'Using payload: {payload}')
+        obj = ctx.restore_vm(**payload)
+        # submit request
+        columns = ctx.columns or const.COLUMNS_REQUEST_SUBMITTED
+        ctx.echo(format_output(ctx, [obj], columns=columns, single=True))
+        # wait for request
+        if ctx.wait_for_requests:
+            ctx.wait_for_request_to(obj)
+
+
 @compute_vm.group(
     'rm', help='Delete given virtual machines', invoke_without_command=True
 )
 @click.option(
     '-f',
     '--force',
     is_flag=True,
@@ -3578,14 +3770,15 @@
 
     Edit vm.yaml file and deploy as follows:
 
     vss-cli compute vm mk from-file <cli-spec>.json|yaml
 
     """
     import time
+
     from pick import pick
 
     if file_spec:
         raw = file_spec.read()
     else:
         # load default configuration
         if not spec_template:
```

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/compute_plugins/vmdks.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/compute_plugins/vmdks.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/configure.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/configure.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/key.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/key.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/message.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/message.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/misc.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/misc.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/ovf.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/ovf.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/plugins.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/change.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/change.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/export.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/export.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/folder.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/folder.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/image.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/image.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/inventory.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/inventory.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/new.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/new.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/retirement.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/retirement.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/snapshot.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/snapshot.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/request_plugins/vmdk.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/request_plugins/vmdk.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/service.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/service.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/shell.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/shell.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/status.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/status.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/stor.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/stor.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/token.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/token.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/plugins/upgrade.py` & `vss-cli-2024.5.0.dev0/vss_cli/plugins/upgrade.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/rel_opts.py` & `vss-cli-2024.5.0.dev0/vss_cli/rel_opts.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/sstatus.py` & `vss-cli-2024.5.0.dev0/vss_cli/sstatus.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/utils/emoji.py` & `vss-cli-2024.5.0.dev0/vss_cli/utils/emoji.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/utils/threading.py` & `vss-cli-2024.5.0.dev0/vss_cli/utils/threading.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/validators.py` & `vss-cli-2024.5.0.dev0/vss_cli/validators.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/vss.py` & `vss-cli-2024.5.0.dev0/vss_cli/vss.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli/yaml.py` & `vss-cli-2024.5.0.dev0/vss_cli/yaml.py`

 * *Files identical despite different names*

### Comparing `vss-cli-2023.9.0.dev8/vss_cli.egg-info/PKG-INFO` & `vss-cli-2024.5.0.dev0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: vss-cli
-Version: 2023.9.0.dev8
+Version: 2024.5.0.dev0
 Summary: ITS Private Cloud Command Line Interface
 Home-page: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
-Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2023.9.0-dev8.zip
+Download-URL: https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/archive/2024.5.0-dev0.zip
 Author: University of Toronto
 Author-email: vss-apps@eis.utoronto.ca
 Maintainer-email: vss-py@eis.utoronto.ca
 License: MIT
 Project-URL: Bug Reports, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli/issues
 Project-URL: Documentation, https://eis.utoronto.ca/~vss/vss-cli/
 Project-URL: Source, https://gitlab-ee.eis.utoronto.ca/vss/vss-cli
@@ -21,18 +21,57 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: System :: Systems Administration
 Requires-Python: >=3.7.5
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyvss==2023.12.0
+Requires-Dist: click==8.1.7
+Requires-Dist: click-log==0.4.0
+Requires-Dist: click-plugins==1.1.1
+Requires-Dist: click-repl==0.2.0
+Requires-Dist: click-threading==0.5.0
+Requires-Dist: tabulate==0.9.0
+Requires-Dist: jsonpath-ng<2,>=1.5.1
+Requires-Dist: jinja2>=2.10
+Requires-Dist: dateparser==1.1.8
+Requires-Dist: Pygments>=2.13.0
+Requires-Dist: pick==2.2.0
+Requires-Dist: dataclasses-json==0.5.7
+Requires-Dist: validators==0.20.0
+Requires-Dist: click-spinner==0.1.10
+Requires-Dist: ruamel.yaml==0.17.21
+Requires-Dist: qrcode==7.3.1
+Requires-Dist: pyjwt==2.6.0
+Requires-Dist: xmltodict==0.13.0
+Requires-Dist: setuptools==68.2.2
 Provides-Extra: test
+Requires-Dist: flake8==6.0.0; extra == "test"
+Requires-Dist: nose==1.3.7; extra == "test"
+Requires-Dist: coverage==6.5.0; extra == "test"
+Requires-Dist: pytz==2022.6; extra == "test"
+Requires-Dist: wheel==0.38.4; extra == "test"
+Requires-Dist: minio==7.1.17; extra == "test"
 Provides-Extra: dev
+Requires-Dist: flake8==6.0.0; extra == "dev"
+Requires-Dist: nose==1.3.7; extra == "dev"
+Requires-Dist: coverage==6.5.0; extra == "dev"
+Requires-Dist: pytz==2022.6; extra == "dev"
+Requires-Dist: wheel==0.38.4; extra == "dev"
+Requires-Dist: minio==7.1.17; extra == "dev"
+Requires-Dist: minio==7.1.17; extra == "dev"
+Requires-Dist: sphinx-rtd-theme==1.3.0; extra == "dev"
+Requires-Dist: Sphinx==7.2.2; extra == "dev"
+Requires-Dist: bump2version==1.0.1; extra == "dev"
+Requires-Dist: sphinxcontrib-jquery==4.1; extra == "dev"
+Requires-Dist: sphinxcontrib-confluencebuilder==2.2.0; extra == "dev"
 Provides-Extra: stor
-License-File: LICENSE
+Requires-Dist: minio==7.1.17; extra == "stor"
 
 # ITS Private Cloud Command Line Interface ``vss-cli``
 
 [![PyPI][pypi-img]](https://pypi.python.org/pypi/vss-cli)
 [![PyPI version][pyver-img]](https://pypi.python.org/pypi/vss-cli)
```

### Comparing `vss-cli-2023.9.0.dev8/vss_cli.egg-info/SOURCES.txt` & `vss-cli-2024.5.0.dev0/vss_cli.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+tests/test_vss_cli.py
 vss_cli/__init__.py
 vss_cli/autocompletion.py
 vss_cli/cli.py
 vss_cli/config.py
 vss_cli/const.py
 vss_cli/data_types.py
 vss_cli/exceptions.py
@@ -69,13 +70,14 @@
 vss_cli/plugins/request_plugins/__init__.py
 vss_cli/plugins/request_plugins/change.py
 vss_cli/plugins/request_plugins/export.py
 vss_cli/plugins/request_plugins/folder.py
 vss_cli/plugins/request_plugins/image.py
 vss_cli/plugins/request_plugins/inventory.py
 vss_cli/plugins/request_plugins/new.py
+vss_cli/plugins/request_plugins/restore.py
 vss_cli/plugins/request_plugins/retirement.py
 vss_cli/plugins/request_plugins/snapshot.py
 vss_cli/plugins/request_plugins/vmdk.py
 vss_cli/utils/__init__.py
 vss_cli/utils/emoji.py
 vss_cli/utils/threading.py
```

### Comparing `vss-cli-2023.9.0.dev8/vss_cli.egg-info/requires.txt` & `vss-cli-2024.5.0.dev0/vss_cli.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-pyvss==2023.9.0
+pyvss==2023.12.0
 click==8.1.7
 click-log==0.4.0
 click-plugins==1.1.1
 click-repl==0.2.0
 click-threading==0.5.0
 tabulate==0.9.0
 jsonpath-ng<2,>=1.5.1
@@ -13,14 +13,15 @@
 dataclasses-json==0.5.7
 validators==0.20.0
 click-spinner==0.1.10
 ruamel.yaml==0.17.21
 qrcode==7.3.1
 pyjwt==2.6.0
 xmltodict==0.13.0
+setuptools==68.2.2
 
 [dev]
 flake8==6.0.0
 nose==1.3.7
 coverage==6.5.0
 pytz==2022.6
 wheel==0.38.4
```

