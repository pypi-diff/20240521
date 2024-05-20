# Comparing `tmp/chipstream-0.2.2.tar.gz` & `tmp/chipstream-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chipstream-0.2.2.tar", last modified: Tue Apr 16 08:41:40 2024, max compression
+gzip compressed data, was "chipstream-0.3.0.tar", last modified: Mon May 20 22:33:27 2024, max compression
```

## Comparing `chipstream-0.2.2.tar` & `chipstream-0.3.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.254051 chipstream-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.242051 chipstream-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.242051 chipstream-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-04-16 08:41:34.000000 chipstream-0.2.2/.github/workflows/check.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-16 08:41:34.000000 chipstream-0.2.2/.github/workflows/deploy_github.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-16 08:41:34.000000 chipstream-0.2.2/.github/workflows/deploy_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-04-16 08:41:34.000000 chipstream-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-16 08:41:34.000000 chipstream-0.2.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-16 08:41:34.000000 chipstream-0.2.2/CHANGELOG
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 08:41:34.000000 chipstream-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-16 08:41:40.254051 chipstream-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-16 08:41:34.000000 chipstream-0.2.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.246050 chipstream-0.2.2/build-recipes/
--rw-r--r--   0 runner    (1001) docker     (127)    75281 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/ChipStream.icns
--rw-r--r--   0 runner    (1001) docker     (127)   353118 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/ChipStream.ico
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/ChipStreamLauncher.py
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/ChipStreamLauncherCLI.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/Readme.md
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/hook-chipstream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/macos_ChipStream.spec
--rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/macos_build_app.sh
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/macos_build_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/win_ChipStream.spec
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/win_build_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/win_chipstream.iss_dummy
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-16 08:41:34.000000 chipstream-0.2.2/build-recipes/win_make_iss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.246050 chipstream-0.2.2/chipstream/
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.250050 chipstream-0.2.2/chipstream/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/cli/cli_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6462 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/cli/cli_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3859 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/cli/cli_proc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4014 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/cli/cli_valid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.250050 chipstream-0.2.2/chipstream/gui/
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.250050 chipstream-0.2.2/chipstream/gui/img/
--rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/gui/img/chipstream_icon.png
--rw-r--r--   0 runner    (1001) docker     (127)    13292 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/gui/main_window.py
--rw-r--r--   0 runner    (1001) docker     (127)    13667 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/gui/main_window.ui
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/gui/splash.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/gui/table_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-16 08:41:34.000000 chipstream-0.2.2/chipstream/path_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.254051 chipstream-0.2.2/chipstream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 08:41:40.000000 chipstream-0.2.2/chipstream.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.250050 chipstream-0.2.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.250050 chipstream-0.2.2/docs/artwork/
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-16 08:41:34.000000 chipstream-0.2.2/docs/artwork/chipstream_icon.svg
--rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-04-16 08:41:34.000000 chipstream-0.2.2/docs/artwork/chipstream_splash.png
--rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-04-16 08:41:34.000000 chipstream-0.2.2/docs/artwork/chipstream_splash.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-04-16 08:41:34.000000 chipstream-0.2.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-16 08:41:34.000000 chipstream-0.2.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 08:41:34.000000 chipstream-0.2.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-04-16 08:41:34.000000 chipstream-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 08:41:40.254051 chipstream-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.254051 chipstream-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:41:40.254051 chipstream-0.2.2/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/helper_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/requirements-full.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/test_gui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-04-16 08:41:34.000000 chipstream-0.2.2/tests/test_path_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.313227 chipstream-0.3.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.313227 chipstream-0.3.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-20 22:33:21.000000 chipstream-0.3.0/.github/workflows/check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-20 22:33:21.000000 chipstream-0.3.0/.github/workflows/deploy_github.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-05-20 22:33:21.000000 chipstream-0.3.0/.github/workflows/deploy_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3113 2024-05-20 22:33:21.000000 chipstream-0.3.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-20 22:33:21.000000 chipstream-0.3.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-20 22:33:21.000000 chipstream-0.3.0/CHANGELOG
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-20 22:33:21.000000 chipstream-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-20 22:33:27.321227 chipstream-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-20 22:33:21.000000 chipstream-0.3.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.317227 chipstream-0.3.0/build-recipes/
+-rw-r--r--   0 runner    (1001) docker     (127)    75281 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/ChipStream.icns
+-rw-r--r--   0 runner    (1001) docker     (127)   353118 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/ChipStream.ico
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/ChipStreamLauncher.py
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/ChipStreamLauncherCLI.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/hook-chipstream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/macos_ChipStream.spec
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1981 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/macos_build_app.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/macos_build_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/win_ChipStream.spec
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/win_build_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/win_chipstream.iss_dummy
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-20 22:33:21.000000 chipstream-0.3.0/build-recipes/win_make_iss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.317227 chipstream-0.3.0/chipstream/
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.317227 chipstream-0.3.0/chipstream/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/cli/cli_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8194 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/cli/cli_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4120 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/cli/cli_proc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4736 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/cli/cli_valid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/chipstream/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/chipstream/gui/img/
+-rw-r--r--   0 runner    (1001) docker     (127)    14396 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/img/chipstream_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13478 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/main_window.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/main_window.ui
+-rw-r--r--   0 runner    (1001) docker     (127)     9702 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/splash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/gui/table_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-20 22:33:21.000000 chipstream-0.3.0/chipstream/path_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/chipstream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-20 22:33:27.000000 chipstream-0.3.0/chipstream.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/docs/artwork/
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-05-20 22:33:21.000000 chipstream-0.3.0/docs/artwork/chipstream_icon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    10628 2024-05-20 22:33:21.000000 chipstream-0.3.0/docs/artwork/chipstream_splash.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5390 2024-05-20 22:33:21.000000 chipstream-0.3.0/docs/artwork/chipstream_splash.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1652 2024-05-20 22:33:21.000000 chipstream-0.3.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-20 22:33:21.000000 chipstream-0.3.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 22:33:21.000000 chipstream-0.3.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1397 2024-05-20 22:33:21.000000 chipstream-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:33:27.321227 chipstream-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:33:27.321227 chipstream-0.3.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   154010 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/helper_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/requirements-full.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/test_gui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/test_gui_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-20 22:33:21.000000 chipstream-0.3.0/tests/test_path_cache.py
```

### Comparing `chipstream-0.2.2/.github/workflows/check.yml` & `chipstream-0.3.0/.github/workflows/check.yml`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/.github/workflows/deploy_github.yml` & `chipstream-0.3.0/.github/workflows/deploy_github.yml`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.10"]
         os: [macos-latest, windows-latest]
     steps:
     - name: Set env
+      shell: bash
       run: echo "RELEASE_VERSION=${GITHUB_REF#refs/*/}" >> $GITHUB_ENV
     - uses: actions/checkout@v3
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install Python dependencies
```

### Comparing `chipstream-0.2.2/.github/workflows/deploy_pypi.yml` & `chipstream-0.3.0/.github/workflows/deploy_pypi.yml`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/.gitignore` & `chipstream-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/LICENSE` & `chipstream-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/PKG-INFO` & `chipstream-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chipstream
-Version: 0.2.2
+Version: 0.3.0
 Summary: GUI for DC data postprocessing
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL version 3.0 or later
 Project-URL: source, https://github.com/DC-Analysis/ChipStream
 Project-URL: tracker, https://github.com/DC-Analysis/ChipStream/issues
 Project-URL: documentation, https://chipstream.readthedocs.io/en/stable/
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Intended Audience :: Science/Research
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: dcnum>=0.17.2
+Requires-Dist: dcnum>=0.19.1
 Requires-Dist: h5py<4,>=3.0.0
 Requires-Dist: numpy<2,>=1.21
 Provides-Extra: cli
 Requires-Dist: click>=8; extra == "cli"
 Provides-Extra: gui
 Requires-Dist: pyqt6; extra == "gui"
```

### Comparing `chipstream-0.2.2/README.rst` & `chipstream-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/build-recipes/ChipStream.icns` & `chipstream-0.3.0/build-recipes/ChipStream.icns`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/build-recipes/ChipStream.ico` & `chipstream-0.3.0/build-recipes/ChipStream.ico`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/build-recipes/Readme.md` & `chipstream-0.3.0/build-recipes/Readme.md`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/build-recipes/hook-chipstream.py` & `chipstream-0.3.0/build-recipes/hook-chipstream.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/build-recipes/macos_ChipStream.spec` & `chipstream-0.3.0/build-recipes/macos_ChipStream.spec`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/build-recipes/macos_build_app.sh` & `chipstream-0.3.0/build-recipes/macos_build_app.sh`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/build-recipes/win_ChipStream.spec` & `chipstream-0.3.0/build-recipes/win_ChipStream.spec`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/build-recipes/win_chipstream.iss_dummy` & `chipstream-0.3.0/build-recipes/win_chipstream.iss_dummy`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/build-recipes/win_make_iss.py` & `chipstream-0.3.0/build-recipes/win_make_iss.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/chipstream/__init__.py` & `chipstream-0.3.0/chipstream/__init__.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/chipstream/cli/cli_common.py` & `chipstream-0.3.0/chipstream/cli/cli_common.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/chipstream/cli/cli_main.py` & `chipstream-0.3.0/chipstream/cli/cli_main.py`

 * *Files 23% similar despite different names*

```diff
@@ -58,14 +58,25 @@
 @click.argument("path_out",
                 required=False,
                 type=click.Path(dir_okay=True,
                                 writable=True,
                                 resolve_path=True,
                                 path_type=pathlib.Path),
                 )
+@click.option("-b", "--background-method",
+              type=click.Choice(sorted(cm.bg_methods.keys()),
+                                case_sensitive=False),
+              default="sparsemed",
+              help="Background computation method to use.")
+@click.option("-kb", "background_kwargs",
+              multiple=True,
+              help="Optional ``KEY=VALUE`` argument for the specified "
+                   "background method",
+              metavar="KEY=VALUE",
+              )
 @click.option("-s", "--segmentation-method",
               type=click.Choice(sorted(cm.seg_methods.keys()),
                                 case_sensitive=False),
               default="thresh",
               help="Segmentation method to use.")
 @click.option("-ks", "segmentation_kwargs",
               multiple=True,
@@ -83,14 +94,20 @@
               multiple=True,
               help="Optional ``KEY=VALUE`` argument for event gating.",
               metavar="KEY=VALUE",
               )
 @click.option("-p", "--pixel-size", type=float, default=0,
               help="Set/override the pixel size for feature "
                    "extraction [µm].")
+@click.option("--limit-events", type=str, default="0",
+              help="Limit events of events to analyze. This can be either "
+                   "a number (e.g. '5000') or a range (e.g. '5000-7000'). "
+                   "You can also specify a step size (e.g. '5000-7000-2' for "
+                   "every second event). The convention follows Python slices "
+                   "with 'n' substituting for 'None'.")
 @click.option("-r", "--recursive", is_flag=True,
               help="Recurse into subdirectories.")
 @click.option("--num-cpus",
               type=click.IntRange(min=1, max=mp.cpu_count(), clamp=True),
               help="Number of processes to create."
               )
 @click.option("--dry-run", is_flag=True,
@@ -100,47 +117,70 @@
 @click.option("--debug", is_flag=True,
               help="Run chipstream in debugging mode. This disables "
                    "multiprocessing and yields a more verbose output.")
 @click.version_option(version)
 def chipstream_cli(
     path_in,
     path_out=None,
+    background_method="sparsemed",
+    background_kwargs=None,
     segmentation_method="thresh",
     segmentation_kwargs=None,
     feature_kwargs=None,
     gate_kwargs=None,
     pixel_size=0,
+    limit_events="0",
     recursive=False,
     num_cpus=None,
     dry_run=False,
     verbose=False,
     debug=False,
 ):
 
     if debug:
         click.secho("Running in debug mode (this will be slow)",
                     fg="yellow")
         verbose = True
 
+    # Parse limit_frames to get the HDF5Data index_mapping
+
+    if limit_events == "0":
+        index_mapping = None
+    elif limit_events.count("-"):
+        vals = limit_events.split("-")
+        assert len(vals) in [2, 3], "slice definition must have length 2 or 3"
+        start = None if vals[0] == "n" else int(vals[0])
+        stop = None if vals[1] == "n" else int(vals[1])
+        if len(vals) == 3:
+            step = None if vals[2] == "n" else int(vals[2])
+        else:
+            step = None
+        index_mapping = slice(start, stop, step)
+    else:
+        index_mapping = int(limit_events)
+
     # Tell the root logger to pretty-print logs
     root_logger = logging.getLogger()
     handler = logging.StreamHandler()
     handler.setFormatter(cm.PrettyFormatter())
     root_logger.addHandler(handler)
     handler.setLevel(logging.DEBUG if verbose else logging.WARNING)
 
     mp.freeze_support()
 
     process_kwargs = dict(
+        background_method=background_method,
+        background_kwargs=background_kwargs,
         segmentation_method=segmentation_method,
         segmentation_kwargs=segmentation_kwargs,
         feature_kwargs=feature_kwargs,
         gate_kwargs=gate_kwargs,
         pixel_size=pixel_size,
         # Below this line are arguments that do not define the pipeline ID
+        index_mapping=index_mapping,
         num_cpus=num_cpus or mp.cpu_count(),
         dry_run=dry_run,
         debug=debug,
         )
 
     if recursive:
         failed = 0  # keeps track of files that failed to process
```

### Comparing `chipstream-0.2.2/chipstream/cli/cli_proc.py` & `chipstream-0.3.0/chipstream/cli/cli_proc.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,28 +6,31 @@
 import dcnum.logic
 from dcnum.meta import ppid
 import dcnum.read
 
 
 from . import cli_common as cm
 from .cli_valid import (
-    validate_feature_kwargs, validate_gate_kwargs, validate_pixel_size,
-    validate_segmentation_kwargs
+    validate_background_kwargs, validate_feature_kwargs, validate_gate_kwargs,
+    validate_pixel_size, validate_segmentation_kwargs
 )
 
 
 def process_dataset(
     path_in: pathlib.Path,
     path_out: pathlib.Path,
+    background_method: str,
+    background_kwargs: List[str],
     segmentation_method: str,
     segmentation_kwargs: List[str],
     feature_kwargs: List[str],
     gate_kwargs: List[str],
     pixel_size: float,
     # Below this line are arguments that do not affect the pipeline ID
+    index_mapping: int | slice | None,
     num_cpus: int,
     dry_run: bool,
     debug: bool,
 ):
     # Make sure the pixel size makes sense
     if pixel_size == 0:
         pixel_size = validate_pixel_size(data_path=path_in)
@@ -38,17 +41,18 @@
 
     # data keyword arguments
     with dcnum.read.HDF5Data(path_in, pixel_size=pixel_size) as data:
         dat_id = data.get_ppid()
     click.echo(f"Data ID:\t{dat_id}")
 
     # background keyword arguments
-    bg_cls = cm.bg_methods["sparsemed"]
-    bg_kwargs = {}  # use defaults
-    bg_id = bg_cls.get_ppid_from_ppkw(bg_kwargs)  # use defaults
+    bg_kwargs = validate_background_kwargs(background_method,
+                                           background_kwargs)
+    bg_cls = cm.bg_methods[background_method]
+    bg_id = bg_cls.get_ppid_from_ppkw(bg_kwargs)
     click.echo(f"Background ID:\t{bg_id}")
 
     # segmenter keyword arguments
     seg_kwargs = validate_segmentation_kwargs(segmentation_method,
                                               segmentation_kwargs)
     seg_cls = cm.seg_methods[segmentation_method]
     seg_id = seg_cls.get_ppid_from_ppkw(seg_kwargs)
@@ -80,15 +84,16 @@
         click.echo("Dry run complete")
         return 0
 
     job = dcnum.logic.DCNumPipelineJob(
         path_in=path_in,
         path_out=path_out,
         data_code="hdf",
-        data_kwargs={"pixel_size": pixel_size},
+        data_kwargs={"pixel_size": pixel_size,
+                     "index_mapping": index_mapping},
         background_code=bg_cls.get_ppid_code(),
         background_kwargs=bg_kwargs,
         segmenter_code=seg_cls.get_ppid_code(),
         segmenter_kwargs=seg_kwargs,
         feature_code=feat_cls.get_ppid_code(),
         feature_kwargs=feat_kwargs,
         gate_code=gate_cls.get_ppid_code(),
```

### Comparing `chipstream-0.2.2/chipstream/cli/cli_valid.py` & `chipstream-0.3.0/chipstream/cli/cli_valid.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,14 +4,32 @@
 from dcnum.meta import ppid
 import dcnum.read
 import h5py
 
 from . import cli_common as cm
 
 
+def validate_background_kwargs(bg_method, args):
+    """Parse background keyword arguments"""
+    # Get list of valid keyword arguments
+    bg_cls = cm.bg_methods[bg_method]
+    spec = inspect.getfullargspec(bg_cls.check_user_kwargs)
+    valid_kw = spec.kwonlyargs
+    annot = spec.annotations
+    # Convert the input args to key-value pairs
+    kwargs = {}
+    for key, value in [a.split("=") for a in args]:
+        if key not in valid_kw:
+            raise ValueError(f"Invalid keyword '{key}' for {bg_method}. "
+                             + f"Allowed keywords are {valid_kw}!")
+        # Convert to correct dtype (default to string)
+        kwargs[key] = ppid.convert_to_dtype(value, annot[key])
+    return kwargs
+
+
 def validate_feature_kwargs(args):
     # Get list of valid keyword arguments
     feat_cls = cm.QueueEventExtractor
     feat_code = feat_cls.get_ppid_code()
     # extract_approach
     spec_appr = inspect.getfullargspec(feat_cls.get_events_from_masks)
     valid_kw_appr = spec_appr.kwonlyargs
```

### Comparing `chipstream-0.2.2/chipstream/gui/__init__.py` & `chipstream-0.3.0/chipstream/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/chipstream/gui/img/chipstream_icon.png` & `chipstream-0.3.0/chipstream/gui/img/chipstream_icon.png`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/chipstream/gui/main_window.py` & `chipstream-0.3.0/chipstream/gui/main_window.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,33 +146,37 @@
         if self.checkBox_pixel_size.isChecked():
             data_kwargs = {"pixel_size": self.doubleSpinBox_pixel_size.value()}
         else:
             data_kwargs = None
 
         # default background computer is "sparsemed"
         bg_default = feat_background.BackgroundSparseMed
+        bg_kwargs = inspect.getfullargspec(
+            bg_default.check_user_kwargs).kwonlydefaults
+        bg_kwargs["offset_correction"] = \
+            self.checkBox_bg_flickering.isChecked()
 
         # populate segmenter and its kwargs
         segmenter = self.comboBox_segmenter.currentData()
         segmenter_kwargs = {}
         if segmenter == "thresh":
             segmenter_kwargs["thresh"] = self.spinBox_thresh.value()
 
         job_kwargs = {
             "data_code": "hdf",
             "data_kwargs": data_kwargs,
             "background_code": bg_default.get_ppid_code(),
-            "background_kwargs": inspect.getfullargspec(
-                bg_default.check_user_kwargs).kwonlydefaults,
+            "background_kwargs": bg_kwargs,
             "segmenter_code": segmenter,
             "segmenter_kwargs": segmenter_kwargs,
             "feature_code": "legacy",
             "feature_kwargs": {
                 "brightness": self.checkBox_feat_bright.isChecked(),
                 "haralick": self.checkBox_feat_haralick.isChecked(),
+                "volume": self.checkBox_feat_volume.isChecked(),
                 },
             "gate_code": "norm",
             "gate_kwargs": {},
             "num_procs": self.spinBox_procs.value(),
         }
 
         # special case for copy-segmenter
```

### Comparing `chipstream-0.2.2/chipstream/gui/main_window.ui` & `chipstream-0.3.0/chipstream/gui/main_window.ui`

 * *Files 4% similar despite different names*

#### Comparing `chipstream-0.2.2/chipstream/gui/main_window.ui` & `chipstream-0.3.0/chipstream/gui/main_window.ui`

```diff
@@ -2,16 +2,16 @@
 <ui version="4.0">
   <class>MainWindow</class>
   <widget class="QMainWindow" name="MainWindow">
     <property name="geometry">
       <rect>
         <x>0</x>
         <y>0</y>
-        <width>1408</width>
-        <height>754</height>
+        <width>1120</width>
+        <height>680</height>
       </rect>
     </property>
     <property name="windowTitle">
       <string>MainWindow</string>
     </property>
     <widget class="QWidget" name="centralwidget">
       <layout class="QHBoxLayout" name="horizontalLayout" stretch="4,1">
@@ -119,14 +119,33 @@
                       <width>20</width>
                       <height>40</height>
                     </size>
                   </property>
                 </spacer>
               </item>
               <item>
+                <widget class="QGroupBox" name="groupBox">
+                  <property name="title">
+                    <string>Background Image</string>
+                  </property>
+                  <layout class="QVBoxLayout" name="verticalLayout_2">
+                    <item>
+                      <widget class="QCheckBox" name="checkBox_bg_flickering">
+                        <property name="text">
+                          <string>flickering correction</string>
+                        </property>
+                        <property name="checked">
+                          <bool>true</bool>
+                        </property>
+                      </widget>
+                    </item>
+                  </layout>
+                </widget>
+              </item>
+              <item>
                 <widget class="QGroupBox" name="groupBox_4">
                   <property name="sizePolicy">
                     <sizepolicy hsizetype="Preferred" vsizetype="Preferred">
                       <horstretch>0</horstretch>
                       <verstretch>0</verstretch>
                     </sizepolicy>
                   </property>
@@ -230,14 +249,24 @@
                         </property>
                         <property name="checked">
                           <bool>true</bool>
                         </property>
                       </widget>
                     </item>
                     <item>
+                      <widget class="QCheckBox" name="checkBox_feat_volume">
+                        <property name="text">
+                          <string>Volume</string>
+                        </property>
+                        <property name="checked">
+                          <bool>true</bool>
+                        </property>
+                      </widget>
+                    </item>
+                    <item>
                       <widget class="QCheckBox" name="checkBox_feat_haralick">
                         <property name="text">
                           <string>Haralick texture features</string>
                         </property>
                       </widget>
                     </item>
                     <item>
@@ -331,15 +360,15 @@
       </layout>
     </widget>
     <widget class="QMenuBar" name="menubar">
       <property name="geometry">
         <rect>
           <x>0</x>
           <y>0</y>
-          <width>1408</width>
+          <width>1120</width>
           <height>22</height>
         </rect>
       </property>
       <widget class="QMenu" name="menuHelp">
         <property name="title">
           <string>Help</string>
         </property>
```

### Comparing `chipstream-0.2.2/chipstream/gui/table_progress.py` & `chipstream-0.3.0/chipstream/gui/table_progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from PyQt6 import QtCore, QtWidgets
 
-from ..manager import ChipStreamJobManager
+from .manager import ChipStreamJobManager
 
 
 ItemProgressRole = QtCore.Qt.ItemDataRole.UserRole + 1001
 
 
 class ProgressDelegate(QtWidgets.QStyledItemDelegate):
     def paint(self, painter, option, index):
```

### Comparing `chipstream-0.2.2/chipstream/manager.py` & `chipstream-0.3.0/chipstream/gui/manager.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/chipstream/path_cache.py` & `chipstream-0.3.0/chipstream/path_cache.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/chipstream.egg-info/PKG-INFO` & `chipstream-0.3.0/chipstream.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chipstream
-Version: 0.2.2
+Version: 0.3.0
 Summary: GUI for DC data postprocessing
 Author: Paul Müller
 Maintainer-email: Paul Müller <dev@craban.de>
 License: GPL version 3.0 or later
 Project-URL: source, https://github.com/DC-Analysis/ChipStream
 Project-URL: tracker, https://github.com/DC-Analysis/ChipStream/issues
 Project-URL: documentation, https://chipstream.readthedocs.io/en/stable/
@@ -13,15 +13,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Intended Audience :: Science/Research
 Requires-Python: <4,>=3.10
 Description-Content-Type: text/x-rst
 License-File: LICENSE
-Requires-Dist: dcnum>=0.17.2
+Requires-Dist: dcnum>=0.19.1
 Requires-Dist: h5py<4,>=3.0.0
 Requires-Dist: numpy<2,>=1.21
 Provides-Extra: cli
 Requires-Dist: click>=8; extra == "cli"
 Provides-Extra: gui
 Requires-Dist: pyqt6; extra == "gui"
```

### Comparing `chipstream-0.2.2/chipstream.egg-info/SOURCES.txt` & `chipstream-0.3.0/chipstream.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 build-recipes/macos_build_requirements.txt
 build-recipes/win_ChipStream.spec
 build-recipes/win_build_requirements.txt
 build-recipes/win_chipstream.iss_dummy
 build-recipes/win_make_iss.py
 chipstream/__init__.py
 chipstream/_version.py
-chipstream/manager.py
 chipstream/path_cache.py
 chipstream.egg-info/PKG-INFO
 chipstream.egg-info/SOURCES.txt
 chipstream.egg-info/dependency_links.txt
 chipstream.egg-info/entry_points.txt
 chipstream.egg-info/requires.txt
 chipstream.egg-info/top_level.txt
@@ -34,14 +33,15 @@
 chipstream/cli/cli_common.py
 chipstream/cli/cli_main.py
 chipstream/cli/cli_proc.py
 chipstream/cli/cli_valid.py
 chipstream/gui/__init__.py
 chipstream/gui/main_window.py
 chipstream/gui/main_window.ui
+chipstream/gui/manager.py
 chipstream/gui/splash.py
 chipstream/gui/table_progress.py
 chipstream/gui/img/chipstream_icon.png
 docs/conf.py
 docs/index.rst
 docs/requirements.txt
 docs/artwork/chipstream_icon.svg
@@ -49,10 +49,10 @@
 docs/artwork/chipstream_splash.svg
 tests/conftest.py
 tests/helper_methods.py
 tests/requirements-full.txt
 tests/requirements.txt
 tests/test_cli.py
 tests/test_gui.py
-tests/test_manager.py
+tests/test_gui_manager.py
 tests/test_path_cache.py
 tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip
```

### Comparing `chipstream-0.2.2/docs/artwork/chipstream_icon.svg` & `chipstream-0.3.0/docs/artwork/chipstream_icon.svg`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/docs/artwork/chipstream_splash.png` & `chipstream-0.3.0/docs/artwork/chipstream_splash.png`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/docs/artwork/chipstream_splash.svg` & `chipstream-0.3.0/docs/artwork/chipstream_splash.svg`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/docs/conf.py` & `chipstream-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/pyproject.toml` & `chipstream-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     'Operating System :: OS Independent',
     'Programming Language :: Python :: 3',
     'Topic :: Scientific/Engineering :: Visualization',
     'Intended Audience :: Science/Research',
 ]
 license = {text = "GPL version 3.0 or later"}
 dependencies = [
-    "dcnum>=0.17.2",
+    "dcnum>=0.19.1",
     "h5py>=3.0.0, <4",
     "numpy>=1.21, <2",  # CVE-2021-33430
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 cli = ["click>=8"]
```

### Comparing `chipstream-0.2.2/tests/conftest.py` & `chipstream-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip` & `chipstream-0.3.0/tests/data/fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/tests/helper_methods.py` & `chipstream-0.3.0/tests/helper_methods.py`

 * *Files identical despite different names*

### Comparing `chipstream-0.2.2/tests/test_manager.py` & `chipstream-0.3.0/tests/test_gui_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import shutil
 
-from chipstream import manager
+from chipstream.gui import manager
 
 
 from helper_methods import retrieve_data
 
 
 def test_manager_get_paths_out(tmp_path):
     path = retrieve_data(
@@ -76,19 +76,19 @@
 
     assert mg[0]["progress"] == 1
     assert mg[0]["state"] == "done"
     assert mg[0]["path"] == str(path)
     assert mg.current_index == 0
     assert not mg.is_busy()
     # default pipeline may change in dcnum
-    assert mg.get_runner(0).ppid == ("7|"
-                                     "hdf:p=0.2645|"
-                                     "sparsemed:k=200^s=1^t=0^f=0.8|"
+    assert mg.get_runner(0).ppid == ("8|"
+                                     "hdf:p=0.2645^i=0|"
+                                     "sparsemed:k=200^s=1^t=0^f=0.8^o=1|"
                                      "thresh:t=-6:cle=1^f=1^clo=2|"
-                                     "legacy:b=1^h=1|"
+                                     "legacy:b=1^h=1^v=1|"
                                      "norm:o=0^s=10")
 
 
 def test_manager_run_with_path_out(tmp_path):
     path = retrieve_data(
         "fmt-hdf5_cytoshot_full-features_legacy_allev_2023.zip")
```

### Comparing `chipstream-0.2.2/tests/test_path_cache.py` & `chipstream-0.3.0/tests/test_path_cache.py`

 * *Files identical despite different names*

