# Comparing `tmp/openxlab-0.0.9.tar.gz` & `tmp/openxlab-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openxlab-0.0.9.tar", last modified: Fri May 19 05:40:41 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `openxlab-0.0.9.tar` & `openxlab-0.1.0.tar`

### file list

```diff
@@ -1,80 +1,106 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.621049 openxlab-0.0.9/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     4030 2023-05-19 05:40:41.620401 openxlab-0.0.9/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3632 2023-05-19 05:11:41.000000 openxlab-0.0.9/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.581540 openxlab-0.0.9/openxlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       46 2023-04-10 09:49:22.000000 openxlab-0.0.9/openxlab/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3207 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/cli.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.586497 openxlab-0.0.9/openxlab/config/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 09:49:22.000000 openxlab-0.0.9/openxlab/config/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      331 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/config/const.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/config/version.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.587260 openxlab-0.0.9/openxlab/demo_cmd/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1057 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/demo_cmd/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.587856 openxlab-0.0.9/openxlab/model/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      397 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.590928 openxlab-0.0.9/openxlab/model/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/clients/model_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     7757 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/clients/openapi_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      853 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/clients/oss_client.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1877 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/clients/upload_service_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.597310 openxlab-0.0.9/openxlab/model/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      875 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      705 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/create.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1021 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/download.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      365 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      541 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/init.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      689 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      536 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/remove.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1105 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/upload.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      765 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/commands/visibility.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.599615 openxlab-0.0.9/openxlab/model/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1747 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/common/constants.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1698 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/common/meta_file_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      831 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.606814 openxlab-0.0.9/openxlab/model/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        3 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/common.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1401 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/create_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     4328 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/download_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       26 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/model_inference.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       56 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/model_list.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1070 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/query_repo_model.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1023 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/remove_repo_or_file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1094 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/update_repository.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3711 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/model/handler/upload_file.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.608183 openxlab-0.0.9/openxlab/types/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-04-10 11:25:41.000000 openxlab-0.0.9/openxlab/types/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      951 2023-04-10 10:02:47.000000 openxlab-0.0.9/openxlab/types/command_type.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.612691 openxlab-0.0.9/openxlab/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)       20 2023-04-10 10:02:47.000000 openxlab-0.0.9/openxlab/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      201 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/utils/auth.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      151 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/utils/env_util.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 openxlab-0.0.9/openxlab/utils/file.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      688 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/utils/time_util.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.613639 openxlab-0.0.9/openxlab/xlab/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      488 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/__init__.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.614826 openxlab-0.0.9/openxlab/xlab/clients/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/clients/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     2381 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/clients/auth_client.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.615979 openxlab-0.0.9/openxlab/xlab/commands/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/commands/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      679 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/commands/config_command.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.617166 openxlab-0.0.9/openxlab/xlab/common/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/common/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)      851 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/common/response_dto.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.619354 openxlab-0.0.9/openxlab/xlab/handler/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/handler/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1802 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/handler/user_config.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3880 2023-05-19 05:11:41.000000 openxlab-0.0.9/openxlab/xlab/handler/user_token.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-19 05:40:41.584961 openxlab-0.0.9/openxlab.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)     4030 2023-05-19 05:40:41.000000 openxlab-0.0.9/openxlab.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1999 2023-05-19 05:40:41.000000 openxlab-0.0.9/openxlab.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-19 05:40:41.000000 openxlab-0.0.9/openxlab.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       48 2023-05-19 05:40:41.000000 openxlab-0.0.9/openxlab.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)      117 2023-05-19 05:40:41.000000 openxlab-0.0.9/openxlab.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        9 2023-05-19 05:40:41.000000 openxlab-0.0.9/openxlab.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1426 2023-05-19 05:11:01.000000 openxlab-0.0.9/pyproject.toml
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-19 05:40:41.621236 openxlab-0.0.9/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1173 2023-05-19 05:11:41.000000 openxlab-0.0.9/setup.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 openxlab-0.1.0/CHANGES.md
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 openxlab-0.1.0/README.md
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/__init__.py
+-rw-r--r--   0        0        0     3689 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/config/__init__.py
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/config/const.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/config/version.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/constants.py
+-rw-r--r--   0        0        0     1478 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/exception.py
+-rw-r--r--   0        0        0     7121 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/utils.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/client/__init__.py
+-rw-r--r--   0        0        0    14315 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/client/api.py
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/client/client.py
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/client/uaa.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/commands/__init__.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/commands/commit.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/commands/create.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/commands/download.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/commands/get.py
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/commands/info.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/commands/ls.py
+-rw-r--r--   0        0        0     1012 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/commands/remove.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/commands/upload_file.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/commands/upload_folder.py
+-rw-r--r--   0        0        0     1845 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/commands/utility.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/commands/visibility.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/handler/__init__.py
+-rw-r--r--   0        0        0      828 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/handler/commit_dataset_info.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/handler/create_dataset_repository.py
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/handler/download_dataset_repository.py
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/handler/get_dataset_repository.py
+-rw-r--r--   0        0        0     2624 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/handler/info_dataset_repository.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/handler/list_dataset_repository.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/handler/remove_dataset_repository.py
+-rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/handler/upload_dataset_file.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/handler/upload_dataset_folder.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/handler/visible_dataset_repository.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/io/__init__.py
+-rw-r--r--   0        0        0    16550 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/io/downloader.py
+-rw-r--r--   0        0        0    12303 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/io/upload.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/utility/__init__.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/dataset/utility/concurrency.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/demo_cmd/__init__.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/clients/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/clients/model_client.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/clients/modelapi_client.py
+-rw-r--r--   0        0        0     9664 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/clients/openapi_client.py
+-rw-r--r--   0        0        0     4676 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/clients/oss_client.py
+-rw-r--r--   0        0        0     1921 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/clients/upload_service_client.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/commands/__init__.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/commands/create.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/commands/download.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/commands/inference.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/commands/init.py
+-rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/commands/list.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/commands/remove.py
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/commands/upload.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/commands/visibility.py
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/commands/wget.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/common/__init__.py
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/common/bury.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/common/constants.py
+-rw-r--r--   0        0        0     3346 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/common/meta_file_util.py
+-rw-r--r--   0        0        0      858 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/common/response_dto.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/common/thread_pool.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/handler/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/handler/common.py
+-rw-r--r--   0        0        0     1950 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/handler/create_repository.py
+-rw-r--r--   0        0        0   224615 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/handler/demo_text_ocr.jpg
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/handler/download_file.py
+-rw-r--r--   0        0        0     2876 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/handler/model_inference.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/handler/model_list.py
+-rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/handler/query_repo_model.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/handler/remove_repo_or_file.py
+-rw-r--r--   0        0        0     1176 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/handler/update_repository.py
+-rw-r--r--   0        0        0     4097 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/model/handler/upload_file.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/types/__init__.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/types/command_type.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/utils/__init__.py
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/utils/auth.py
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/utils/directory_util.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/utils/env_util.py
+-rw-r--r--   0        0        0     3202 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/utils/file.py
+-rw-r--r--   0        0        0      192 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/utils/id_util.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/utils/local_cache.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/utils/time_util.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/clients/__init__.py
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/clients/auth_client.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/clients/version_client.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/commands/__init__.py
+-rw-r--r--   0        0        0      717 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/commands/config_command.py
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/commands/login_command.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/commands/token_command.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/commands/version_command.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/common/__init__.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/common/response_dto.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/handler/__init__.py
+-rw-r--r--   0        0        0     2798 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/handler/user_config.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/handler/user_login.py
+-rw-r--r--   0        0        0    14809 2020-02-02 00:00:00.000000 openxlab-0.1.0/openxlab/xlab/handler/user_token.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 openxlab-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 openxlab-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3829 2020-02-02 00:00:00.000000 openxlab-0.1.0/PKG-INFO
```

### Comparing `openxlab-0.0.9/PKG-INFO` & `openxlab-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,63 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: openxlab
-Version: 0.0.9
-Summary: openxlab
-Home-page: https://github.com/xxx/xxxx
+Version: 0.1.0
+Summary: openxlab tools
+Project-URL: repository, https://github.com/xxx/xxxx
 Author: Openxlab Contributors
-Author-email: myname@example.com
+Author-email: openxlab@example.com
 License: Apache License 2.0
-Keywords: openxlab,xxxx
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Keywords: ai,openxlab
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Python: >=3.8
+Requires-Dist: filelock~=3.14.0
+Requires-Dist: oss2~=2.17.0
+Requires-Dist: packaging~=24.0
+Requires-Dist: pytz~=2023.3
+Requires-Dist: pyyaml~=6.0
+Requires-Dist: requests~=2.28.2
+Requires-Dist: rich~=13.4.2
+Requires-Dist: setuptools~=60.2.0
+Requires-Dist: tqdm~=4.65.0
+Provides-Extra: test
 Description-Content-Type: text/markdown
-Provides-Extra: tests
-Provides-Extra: build
-Provides-Extra: optional
 
 # openxlab-cli
 
 ## Getting started
 
 ### 代码结构
 
 ```
 ├─openxlab
 │  ├─config                存放通用配置
 │  ├─demo                  给出的一个demo，模型中心，应用中心可以创建自己的文件夹
-│  ├─types		   通用参数定义
-│  ├─utils		   存放通用方法
-│  ├─xlab		   主站逻辑
+│  ├─types     通用参数定义
+│  ├─utils     存放通用方法
+│  ├─xlab     主站逻辑
 ```
 
 ### 架构说明
 
 types 中定义定义命令基类
 
-- sub_command_list 	填入下一级命令对应的类定义
-- add_args        		用于添加当前命令的参数  --xxx
-- take_action 		用于定义当前命令的行为，未实现默认使用 argparse 的 help
+- sub_command_list  填入下一级命令对应的类定义
+- add_args          用于添加当前命令的参数  --xxx
+- take_action   用于定义当前命令的行为，未实现默认使用 argparse 的 help
 
 命令继承基类实现，通过 sub_command_list 实现多级子命令
 
+### 安装依赖环境
+
+```
+python -m pip install .
+```
+
 ### 本地测试
 
 ```
  python -m openxlab.cli
  python -m openxlab.cli  demo help  
  python -m openxlab.cli  demo upload
 ```
@@ -56,57 +71,73 @@
 
 打包，  命令将生成一个 dist 目录
 python -m build
 
 本地安装
 pip install .\dist\openxlab-0.0.7-py3-none-any.whl
 
-上传 pip 包到 test pypi
+# 上传 pip 包到 test pypi
 twine upload --repository testpypi dist/*
 
-从 test pypi 下载
+# 从 test pypi 下载
 pip install -i https://test.pypi.org/simple/ openxlab==0.0.1
 
 从 test pypi 更新
 pip install -i https://test.pypi.org/simple/ -U openxlab
 ```
 
-### ak和sk的设置**（暂时只支持开发环境）**
+### ak和sk的设置
+
 设置ak，sk的有一下几种方法，任选一种即可：
+
 1. 本地使用python -m openxlab.cli config命令调试，按照提示输入对应的access key和secret access key。完成后会在~/.openxlab目录下生成config.json文件，格式如下：
+
     ```json
     {
-        "ak": "vmb1akg9w1xwdrxnyxlr",
-        "sk": "9gvpqrel6jez23ywerzvbz2dbpq4y8b1aow5nngx"
+        "ak": "xxx",
+        "sk": "xxx"
     }
     ```
+
 2. 直接在~/.openxlab目录下创建对应的config.json文件，格式如上。
 3. 设置环境变量。可以将access key设置到名为OPENXLAB_AK的环境变量下，secret access key设置到名为OPENXLAB_SK的环境变量下。
 
+### token的获取
 
-### token的获取**（暂时只支持开发环境）**
 在设置好ak和sk之后，业务方可以调用openxlab.xlab.handler.user_token.get_jwt方法获得token。
+
 ```python
 def get_jwt(ak=None, sk=None):
     return get_token(ak, sk).jwt
 ```
+
 该方法拥有ak和sk两个可选参数，允许业务方调用该方法时传递ak和sk。ak和sk生效的优先级如下：
+
 ```
 get_jwt方法中的ak和sk参数(如果不为空） > ~/.openxlab/config.json文件 > OPENXLAB_AK和OPENXLAB_SK环境变量。   
 ```
+
 如果上面三者都为空，则在调用get_jwt方法时会抛出异常如下：
+
 ```python
 ValueError("Local config must not be empty before get token via api. "
                          "Please use the 'openxlab config' command to set the config")
 ```
+
 get_jwt方法调用成功后，会在~/.openxlab目录下生成token.json文件，格式如下：
+
 ```json
 {
     "expiration": "2023-05-16 16:29:03",
-    "jwt": "Bearer eyJ0eXBlIjoiSldUIiwiYWxnIjoiSFM1MTIifQ.eyJqdGkiOiIwMDA1MjA2Iiwicm9sIjoiUk9MRV9BRE1JTiIsImlzcyI6Ik9wZW5YTGFiIiwiaWF0IjoxNjg0MjIyMTQzLCJwaG9uZSI6IjE1ODIxOTkyMzg1IiwiYWsiOiJ2bWIxYWtnOXcxeHdkcnhueXhsciIsImVtYWlsIjoiMjkwMjMyNDc1MUBxcS5jb20iLCJleHAiOjE2ODQyMjU3NDN9.YnM7oPgKubc6jSBvb07usgjjKnCUiNi3RB1SlJC4uMHZ52MWbAJE7PeB8VpUF0sDoi_VWvgfVyRcMRJkamSWig",
+    "jwt": "Bearer eyJxxx",
     "refresh_expiration": "2023-05-23 15:29:03",
     "refresh_time": "2023-05-16 15:29:03",
-    "refresh_token": "Bearer eyJ0eXBlIjoiSldUIiwiYWxnIjoiSFM1MTIifQ.eyJzc291aWQiOiIwMDA1MjA2IiwiaXNSZWZyZXNoVG9rZW4iOnRydWUsImFrIjoidm1iMWFrZzl3MXh3ZHJ4bnl4bHIiLCJleHAiOjE2ODQ4MjY5NDN9.jn6quSfxj5-198onX31GAeS024KZgDGDus2xosrakozd1f7hyvXTrh5DJHDdp6_foOQQcJSRxEUPfdkfXVRvoA",
-    "sso_uid": "0005206"
+    "refresh_token": "Bearer eyJxxx",
+    "sso_uid": "xxx"
 }
 ```
+# Change Log
+
+
+## v0.1.0 
 
+- Release the initial version
```

### Comparing `openxlab-0.0.9/openxlab/model/clients/openapi_client.py` & `openxlab-0.1.0/openxlab/model/clients/openapi_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,158 +1,191 @@
-import requests
-
-from openxlab.model.common.constants import paths
-from openxlab.model.common.response_dto import ReturnDto
-from openxlab.model.common.meta_file_util import get_meta_payload, get_filename_from_url
-import os
-from openxlab.xlab.handler.user_token import get_jwt
-
-
-class OpenapiClient(object):
-    def __init__(self, endpoint, token):
-        self.endpoint = endpoint
-        self.token = token
-
-    # def get_dataset_files(self, dataset_name:str, prefix:str):
-    def get_download_url(self, repository, file):
-        """
-        get file(model file|meta file|log file|readme file) download url
-        """
-        client_from = os.environ.get('CLIENT_FROM', '0')
-        payload = {"repositoryName": repository, "fileName": file, "clientFrom": client_from}
-        path = paths['file_download_path']
-        response_dto = self.http_post_response_dto(path, payload)
-        if response_dto.msg_code != '10000':
-            raise ValueError(f"Get download url error:{response_dto.msg}, traceId:{response_dto.trace_id}")
-        if response_dto.data['msgCode'] != '10000':
-            raise ValueError(f"Get download url error:{response_dto.data['msg']}, "
-                             f"traceId:{response_dto.data['traceId']}")
-        return response_dto.data['data']['url'], response_dto.data['data']['fileName'], \
-            response_dto.data['data']['hash'], response_dto.data['data']['weightRawSize']
-
-    def get_metafile_template_download_url(self, file=None):
-        """
-        get metafile template download url
-        """
-        payload = {}
-        path = paths['meta_file_template_download_path']
-        response_dto = self.http_post_response_dto(path, payload)
-        if response_dto.msg_code != '10000':
-            raise ValueError(f"Get download url error:{response_dto.msg}, traceId:{response_dto.trace_id}")
-        if response_dto.data['msgCode'] != '10000':
-            raise ValueError(f"Get download url error:{response_dto.data['msg']}, "
-                             f"traceId:{response_dto.data['traceId']}")
-        return response_dto.data['data']['url']
-
-    def create_repository(self, repository: str, private: bool, meta_data: dict):
-        """
-        create repository
-        """
-        payload = get_meta_payload(repository, private, meta_data)
-        path = paths['create_repository_path']
-        response_dto = self.http_post_response_dto(path, payload)
-        if response_dto.msg_code != '10000':
-            raise ValueError(f"Create repository error:{response_dto.msg}, traceId:{response_dto.trace_id}")
-        if response_dto.data['msgCode'] != '10000':
-            raise ValueError(f"Create repository error:{response_dto.data['msg']}, "
-                             f"traceId:{response_dto.data['traceId']}")
-        return response_dto.data
-
-    def update_repository(self, repository: str, private: bool):
-        """
-        update repository
-        """
-        public_status = 0 if private else 1
-        payload = {"repoName": repository, "publicStatus": public_status}
-        path = paths['update_repository_path']
-        response_dto = self.http_post_response_dto(path, payload)
-        if response_dto.msg_code != '10000':
-            raise ValueError(f"Create repository error:{response_dto.msg}, traceId:{response_dto.trace_id}")
-        if response_dto.data['msgCode'] != '10000':
-            raise ValueError(f"Create repository error:{response_dto.data['msg']}, "
-                             f"traceId:{response_dto.data['traceId']}")
-        return response_dto.data
-
-    def remove_repository(self, repository):
-        """
-        remove repository
-        """
-        payload = {"repoName": repository}
-        path = paths['delete_repository_path']
-        response_dto = self.http_post_response_dto(path, payload)
-        if response_dto.msg_code != '10000':
-            raise ValueError(f"Create repository error:{response_dto.msg}, traceId:{response_dto.trace_id}")
-        if response_dto.data['msgCode'] != '10000':
-            raise ValueError(f"Create repository error:{response_dto.data['msg']}, "
-                             f"traceId:{response_dto.data['traceId']}")
-        return response_dto.data
-
-    def query_models(self, repository, metafile=None):
-        """
-        query models
-        """
-        payload = {"repoName": repository}
-        path = paths['query_models_path']
-        response_dto = self.http_post_response_dto(path, payload)
-        if response_dto.msg_code != '10000':
-            raise ValueError(f"Create repository error:{response_dto.msg}, traceId:{response_dto.trace_id}")
-        if response_dto.data['msgCode'] != '10000':
-            raise ValueError(f"Create repository error:{response_dto.data['msg']}, "
-                             f"traceId:{response_dto.data['traceId']}")
-        return response_dto.data['data']
-
-    def update_upload_status(self, repository, file_names, new_models=None, update_models=None, upload_status=None):
-        """
-        update upload status
-        """
-        _new_models = None
-        if new_models is not None:
-            _new_models = [{"name": m['Name'], "weightName": get_filename_from_url(m['Weights']),
-                            "evaluations": [{"task": e['Task'], "dataset": e['Dataset']} for e in m['Results']]} for m
-                           in new_models]
-        payload = {"repoName": repository, "fileNames": file_names, "uploadStatus": upload_status,
-                   "models": _new_models}
-        path = paths['update_upload_status_path']
-        response_dto = self.http_post_response_dto(path, payload)
-        if response_dto.msg_code != '10000':
-            raise ValueError(f"Update upload status error:{response_dto.msg}, traceId:{response_dto.trace_id}")
-        if response_dto.data['msgCode'] != '10000':
-            raise ValueError(f"Update upload status error:{response_dto.data['msg']}, "
-                             f"traceId:{response_dto.data['traceId']}")
-        return response_dto.data['data']
-
-    def get_upload_signature(self, repository_id, uid, model, model_info):
-        payload = {"tag": "file", "key": "model-center", "type": 0, "fileType": "file/pth",
-                   "fileName": model_info['objectName'],
-                   "data": {"repositoryId": repository_id, "modelId": model_info['modelId'],
-                            "modelName": model_info['modelName'], "weightName": model_info['weightName'],
-                            "uid": uid}}
-        path = paths['get_upload_signature']
-        response_dto = self.http_post_response_dto(path, payload)
-        if response_dto.msg_code != '10000':
-            raise ValueError(f"Get upload signature error:{response_dto.msg}, traceId:{response_dto.trace_id}")
-        if response_dto.data['msgCode'] != '10000':
-            raise ValueError(f"Get upload signature error:{response_dto.data['msg']}, "
-                             f"traceId:{response_dto.data['traceId']}")
-        return response_dto.data['data']
-
-    def http_post_response_dto(self, path, payload):
-        headers = self.http_common_header()
-        print(f"headers:{headers}, body:{payload}")
-        response = requests.post(f"{self.endpoint}{path}", json=payload, headers=headers)
-        response.raise_for_status()
-        response_dict = response.json()
-        response_dto = ReturnDto.from_camel_case(response_dict)
-        return response_dto
-
-    def http_common_header(self):
-        try:
-            jwt = get_jwt()
-        except ValueError as e:
-            print(f"Error: {e}")
-            return
-        header_dict = {
-            "Content-Type": "application/json",
-            "accept": "application/json",
-            "Authorization": jwt
-        }
-        return header_dict
+import requests
+
+from openxlab.model.common.constants import paths
+from openxlab.model.common.response_dto import ReturnDto
+from openxlab.model.common.meta_file_util import get_meta_payload, get_filename_from_url
+import os
+from openxlab.xlab.handler.user_token import get_jwt
+
+
+class OpenapiClient(object):
+    def __init__(self, endpoint, token=None):
+        self.endpoint = endpoint
+        self.token = token
+
+    # def get_dataset_files(self, dataset_name:str, prefix:str):
+    def get_download_url(self, username, repository, model_name, filepath, ignore):
+        """
+        get file(model file|meta file|log file|readme file) download url
+        """
+        if isinstance(ignore, str):
+            ignore = [ignore]
+        client_from = os.environ.get('CLIENT_FROM', '0')
+        payload = {"userName": username, "repositoryName": repository, "modelNames": model_name, "filePaths": filepath,
+                   "clientFrom": client_from, "ignore": ignore}
+        path = paths['file_download_path']
+        response_dto = self.http_post_response_dto(path, payload)
+        if response_dto.msg_code != '10000':
+            raise ValueError(f"Get download url error:{response_dto.msg}, traceId:{response_dto.trace_id}")
+        if response_dto.data['msgCode'] != '10000':
+            raise ValueError(f"Get download url error:{response_dto.data['msg']}, "
+                             f"traceId:{response_dto.data['traceId']}")
+        return response_dto.data['data']['modelNames'], response_dto.data['data']['filePaths']
+
+    def get_metafile_template_download_url(self, file=None, all=False):
+        """
+        get metafile template download url
+        """
+        payload = {'all': all}
+        path = paths['meta_file_template_download_path']
+        response_dto = self.http_post_response_dto(path, payload, auth=False)
+        if response_dto.msg_code != '10000':
+            raise ValueError(f"Get download url error:{response_dto.msg}, traceId:{response_dto.trace_id}")
+        if response_dto.data['msgCode'] != '10000':
+            raise ValueError(f"Get download url error:{response_dto.data['msg']}, "
+                             f"traceId:{response_dto.data['traceId']}")
+        return response_dto.data['data']['url']
+
+    def create_repository(self, repository: str, private: bool, meta_data: dict):
+        """
+        create repository
+        """
+        payload = get_meta_payload(repository, private, meta_data)
+        path = paths['create_repository_path']
+        response_dto = self.http_post_response_dto(path, payload)
+        if response_dto.msg_code != '10000':
+            raise ValueError(f"Create repository error:{response_dto.msg}, traceId:{response_dto.trace_id}")
+        if response_dto.data['msgCode'] != '10000':
+            raise ValueError(f"Create repository error:{response_dto.data['msg']}, "
+                             f"traceId:{response_dto.data['traceId']}")
+        return response_dto.data
+
+    def update_repository(self, repository: str, private: bool):
+        """
+        update repository
+        """
+        public_status = 0 if private else 1
+        payload = {"repoName": repository, "publicStatus": public_status}
+        path = paths['update_repository_path']
+        response_dto = self.http_post_response_dto(path, payload)
+        if response_dto.msg_code != '10000':
+            raise ValueError(f"Update repository error:{response_dto.msg}, traceId:{response_dto.trace_id}")
+        if response_dto.data['msgCode'] != '10000':
+            raise ValueError(f"Update repository error:{response_dto.data['msg']}, "
+                             f"traceId:{response_dto.data['traceId']}")
+        return response_dto.data
+
+    def remove_repository(self, repository):
+        """
+        remove repository
+        """
+        payload = {"repoName": repository}
+        path = paths['delete_repository_path']
+        print(f'payload:{payload}')
+        response_dto = self.http_post_response_dto(path, payload)
+        if response_dto.msg_code != '10000':
+            raise ValueError(f"Delete repository error:{response_dto.msg}, traceId:{response_dto.trace_id}")
+        if response_dto.data['msgCode'] != '10000':
+            raise ValueError(f"Delete repository error:{response_dto.data['msg']}, "
+                             f"traceId:{response_dto.data['traceId']}")
+        return response_dto.data
+
+    def query_models(self, repository, metafile=None):
+        """
+        query models
+        """
+        payload = {"repoName": repository}
+        path = paths['query_models_path']
+        response_dto = self.http_post_response_dto(path, payload)
+        if response_dto.msg_code != '10000':
+            raise ValueError(f"Query models error:{response_dto.msg}, traceId:{response_dto.trace_id}")
+        if response_dto.data['msgCode'] != '10000':
+            raise ValueError(f"Query models error:{response_dto.data['msg']}, "
+                             f"traceId:{response_dto.data['traceId']}")
+        return response_dto.data['data']
+
+    def update_upload_status(self, repository, file_names, new_models=None, update_models=None, upload_status=None):
+        """
+        update upload status
+        """
+        _new_models = None
+        _update_models = None
+        if new_models is not None:
+            _new_models = [{"name": m['Name'], "weightName": get_filename_from_url(m['Weights']),
+                            "evaluations": [{"task": e['Task'], "dataset": e['Dataset']} for e in m['Results']]} for m
+                           in new_models]
+        if update_models is not None:
+            _update_models = [{"name": m['Name'], "weightName": get_filename_from_url(m['Weights'])} for m
+                              in update_models]
+
+        payload = {"repoName": repository, "fileNames": file_names, "uploadStatus": upload_status,
+                   "models": _new_models, "updateModels": _update_models}
+        path = paths['update_upload_status_path']
+        response_dto = self.http_post_response_dto(path, payload)
+        if response_dto.msg_code != '10000':
+            raise ValueError(f"Update upload status error:{response_dto.msg}, traceId:{response_dto.trace_id}")
+        if response_dto.data['msgCode'] != '10000':
+            raise ValueError(f"Update upload status error:{response_dto.data['msg']}, "
+                             f"traceId:{response_dto.data['traceId']}")
+        return response_dto.data['data']
+
+    def get_upload_signature(self, repository_id, uid, model, model_info):
+        payload = {"tag": "file", "key": "model-center", "type": 0, "fileType": "file/pth",
+                   "fileName": model_info['objectName'],
+                   "data": {"repositoryId": repository_id, "modelId": model_info['modelId'],
+                            "modelName": model_info['modelName'], "weightName": model_info['weightName'],
+                            "uid": uid}}
+        path = paths['get_upload_signature']
+        response_dto = self.http_post_response_dto(path, payload)
+        if response_dto.msg_code != '10000':
+            raise ValueError(f"Get upload signature error:{response_dto.msg}, traceId:{response_dto.trace_id}")
+        if response_dto.data['msgCode'] != '10000':
+            raise ValueError(f"Get upload signature error:{response_dto.data['msg']}, "
+                             f"traceId:{response_dto.data['traceId']}")
+        return response_dto.data['data']
+
+    def query_model_repo_info(self, username: str, repository: str):
+        """
+        query model repo info
+        """
+        payload = {"userName": username, "repoName": repository}
+        path = paths['query_model_repo_info_path']
+        response_dto = self.http_post_response_dto(path, payload)
+        if response_dto.msg_code != '10000':
+            raise ValueError(f"Get model repo info error:{response_dto.msg}, traceId:{response_dto.trace_id}")
+        if response_dto.data['msgCode'] != '10000':
+            raise ValueError(f"Get model repo info error:{response_dto.data['msg']}, "
+                             f"traceId:{response_dto.data['traceId']}")
+        return response_dto.data['data']
+
+    def bury_data_upload(self, payload):
+        """
+        query model repo info
+        """
+        path = paths['bury_upload']
+        response_dto = self.http_post_response_dto(path, payload, auth=False)
+        if response_dto.msg_code != '10000':
+            print(f"upload bury data error:{response_dto.msg}, traceId:{response_dto.trace_id}")
+        if response_dto.data['msgCode'] != '10000':
+            print(f"upload bury data error:{response_dto.data['msg']}, traceId:{response_dto.data['traceId']}")
+
+    def http_post_response_dto(self, path, payload, auth=True):
+        headers = self.http_common_header(auth)
+        # print(f"headers:{headers}, body:{payload}")
+        response = requests.post(f"{self.endpoint}{path}", json=payload, headers=headers)
+        response.raise_for_status()
+        response_dict = response.json()
+        response_dto = ReturnDto.from_camel_case(response_dict)
+        return response_dto
+
+    def http_common_header(self, auth=True):
+        header_dict = {
+            "Content-Type": "application/json",
+            "accept": "application/json"
+        }
+        if auth:
+            try:
+                jwt = get_jwt()
+                header_dict['Authorization'] = jwt
+            except ValueError as e:
+                print(f"warning: {e}")
+        return header_dict
```

### Comparing `openxlab-0.0.9/openxlab/model/clients/upload_service_client.py` & `openxlab-0.1.0/openxlab/model/clients/upload_service_client.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-import requests
-
-from openxlab.model.common.constants import paths
-from openxlab.model.common.response_dto import ReturnDto
-
-
-class UploadServiceClient(object):
-    def __init__(self, endpoint, token):
-        self.endpoint = endpoint
-        self.token = token
-
-    def get_upload_signature(self, repository_id, uid, model, model_info):
-        payload = {"tag": "file", "key": "model-center", "type": 0, "fileType": "file/pth",
-                   "fileName": model_info['objectName'],
-                   "data": {"repositoryId": repository_id, "modelId": model_info['modelId'],
-                            "modelName": model_info['modelName'], "weightName": model_info['weightName'],
-                            "uid": uid}}
-        response_dto = self.http_post_response_dto("", payload)
-        if response_dto.msg_code != '10000':
-            raise ValueError(f"Get upload signature error:{response_dto.msg}, traceId:{response_dto.trace_id}")
-        if response_dto.data['msgCode'] != '10000':
-            raise ValueError(f"Get upload signature error:{response_dto.data['msg']}, "
-                             f"traceId:{response_dto.data['traceId']}")
-        return response_dto.data['data']
-
-    def http_post_response_dto(self, path, payload):
-        headers = self.http_common_header()
-        print(f"headers:{headers}, body:{payload}")
-        response = requests.post(f"{self.endpoint}{path}", json=payload, headers=headers)
-        response.raise_for_status()
-        response_dict = response.json()
-        response_dto = ReturnDto.from_camel_case(response_dict)
-        return response_dto
-
-    def http_common_header(self):
-        header_dict = {
-            "Content-Type": "application/json",
-            "accept": "application/json",
-            "id": "597091",
-            "Authorization": f"Bearer {self.token}"
-        }
-        return header_dict
-
-
+import requests
+
+from openxlab.model.common.constants import paths
+from openxlab.model.common.response_dto import ReturnDto
+
+
+class UploadServiceClient(object):
+    def __init__(self, endpoint, token):
+        self.endpoint = endpoint
+        self.token = token
+
+    def get_upload_signature(self, repository_id, uid, model, model_info):
+        payload = {"tag": "file", "key": "model-center", "type": 0, "fileType": "file/pth",
+                   "fileName": model_info['objectName'],
+                   "data": {"repositoryId": repository_id, "modelId": model_info['modelId'],
+                            "modelName": model_info['modelName'], "weightName": model_info['weightName'],
+                            "uid": uid}}
+        response_dto = self.http_post_response_dto("", payload)
+        if response_dto.msg_code != '10000':
+            raise ValueError(f"Get upload signature error:{response_dto.msg}, traceId:{response_dto.trace_id}")
+        if response_dto.data['msgCode'] != '10000':
+            raise ValueError(f"Get upload signature error:{response_dto.data['msg']}, "
+                             f"traceId:{response_dto.data['traceId']}")
+        return response_dto.data['data']
+
+    def http_post_response_dto(self, path, payload):
+        headers = self.http_common_header()
+        print(f"headers:{headers}, body:{payload}")
+        response = requests.post(f"{self.endpoint}{path}", json=payload, headers=headers)
+        response.raise_for_status()
+        response_dict = response.json()
+        response_dto = ReturnDto.from_camel_case(response_dict)
+        return response_dto
+
+    def http_common_header(self):
+        header_dict = {
+            "Content-Type": "application/json",
+            "accept": "application/json",
+            "id": "597091",
+            "Authorization": f"Bearer {self.token}"
+        }
+        return header_dict
+
+
```

### Comparing `openxlab-0.0.9/openxlab/model/commands/download.py` & `openxlab-0.1.0/openxlab/model/commands/download.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,26 +1,35 @@
-"""
-download model file|meta file|log file|readme file-cli
-"""
-from openxlab.types.command_type import *
-from openxlab.model import download
-
-
-class Download(BaseCommand):
-    """download"""
-
-    def get_name(self) -> str:
-        return "download"
-
-    def add_arguments(self, parser: ArgumentParser) -> None:
-        parser.add_argument('-r', '--model-repo', required=True,
-                            help='model repository address. format:username/repository.')
-        parser.add_argument('-f', '--file', required=True,
-                            help='target file to be download.')
-        parser.add_argument('-p', '--path', required=False,
-                            help='setting download path.')
-        parser.add_argument('-o', '--overwrite', action='store_true',
-                            help='force overwriting local files.')
-
-    def take_action(self, parsed_args: Namespace) -> int:
-        download(parsed_args.model_repo, parsed_args.file, parsed_args.path, parsed_args.overwrite)
-        return 0
+"""
+download model file|meta file|log file|readme file-cli
+"""
+from openxlab.types.command_type import *
+from openxlab.model import download
+
+
+class Download(BaseCommand):
+    """Download model weight files."""
+
+    def get_name(self) -> str:
+        return "download"
+
+    def add_arguments(self, parser: ArgumentParser) -> None:
+        parser.usage = "openxlab model download [-h] -r MODEL_REPO -f FILE [-p PATH] [-o] {help} ...\n" \
+                       'Example:\n' \
+                       '> openxlab model download --model-repo=username/model_repo_name' \
+                       '  --model_name=faster_rcnn \n' \
+                       '  --output=/path/to/local/folder/\n' \
+                       '  --overwrite=True'
+        parser.add_argument('-r', '--model-repo', required=True,
+                            help='model repository address. format:username/repository.')
+        parser.add_argument('-m', '--model-name', required=False, nargs='+',
+                            help='target model to be download.')
+        parser.add_argument('-op', '--output', required=False,
+                            help='setting download path.')
+        parser.add_argument('-o', '--overwrite', default=False, type=bool,
+                            help='force overwriting local files.')
+        parser.add_argument('-i', '--ignore', required=False,
+                            help='ignore is used to filter files that do not need to be downloaded.')
+
+    def take_action(self, parsed_args: Namespace) -> int:
+        download(parsed_args.model_repo, model_name=parsed_args.model_name, output=parsed_args.output,
+                 overwrite=parsed_args.overwrite, ignore=parsed_args.ignore)
+        return 0
```

### Comparing `openxlab-0.0.9/openxlab/model/commands/list.py` & `openxlab-0.1.0/openxlab/model/commands/list.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,25 @@
-"""
-get model list of repository-cli
-"""
-from openxlab.types.command_type import *
-from openxlab.model import list
-
-
-class List(BaseCommand):
-    """list"""
-
-    def get_name(self) -> str:
-        return "list"
-
-    def add_arguments(self, parser: ArgumentParser) -> None:
-        parser.add_argument('-r', '--model-repo', required=True,
-                            help='model repository address. format:username/repository.')
-        parser.add_argument('-i', '--metafile', type=bool, required=False,
-                            help='get meta data.')
-
-    def take_action(self, parsed_args: Namespace) -> int:
-        list(parsed_args.model_repo, parsed_args.metafile)
-        return 0
+"""
+get model list of repository-cli
+"""
+from openxlab.types.command_type import *
+from openxlab.model import list
+
+
+class List(BaseCommand):
+    """To view model information and model meta information under the model repository."""
+
+    def get_name(self) -> str:
+        return "list"
+
+    def add_arguments(self, parser: ArgumentParser) -> None:
+        parser.usage = 'openxlab model list [-h] -r MODEL_REPO [-i METAFILE] {help} ...\n' \
+                       'Example:\n' \
+                       '> openxlab model list --model-repo=username/model_repo_name'
+        parser.add_argument('-r', '--model-repo', required=True,
+                            help='The name of model repository.[required]')
+        parser.add_argument('-i', '--metafile', type=bool, required=False,
+                            help='View model meta information, default is Fasle.')
+
+    def take_action(self, parsed_args: Namespace) -> int:
+        list(parsed_args.model_repo, parsed_args.metafile)
+        return 0
```

### Comparing `openxlab-0.0.9/openxlab/model/commands/visibility.py` & `openxlab-0.1.0/openxlab/model/commands/visibility.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-"""
-setting model repository visibility-cli
-"""
-from openxlab.types.command_type import *
-from openxlab.model import visibility
-
-
-class Visibility(BaseCommand):
-    """visibility"""
-
-    def get_name(self) -> str:
-        return "visibility"
-
-    def add_arguments(self, parser: ArgumentParser) -> None:
-        parser.add_argument('-r', '--model-repo', required=True,
-                            help='model repository address. format:username/repository.')
-        parser.add_argument('-prt', '--private', type=bool, default=False, required=False,
-                            help='set repository visibility.')
-
-    def take_action(self, parsed_args: Namespace) -> int:
-        private = False
-        visibility(parsed_args.model_repo, private)
-        return 0
+"""
+setting model repository visibility-cli
+"""
+from openxlab.types.command_type import *
+from openxlab.model import visibility
+
+
+class Visibility(BaseCommand):
+    """visibility"""
+
+    def get_name(self) -> str:
+        return "visibility"
+
+    def add_arguments(self, parser: ArgumentParser) -> None:
+        parser.add_argument('-r', '--model-repo', required=True,
+                            help='model repository address. format:username/repository.')
+        parser.add_argument('-prt', '--private', type=bool, default=False, required=False,
+                            help='set repository visibility.')
+
+    def take_action(self, parsed_args: Namespace) -> int:
+        private = False
+        visibility(parsed_args.model_repo, private)
+        return 0
```

### Comparing `openxlab-0.0.9/openxlab/model/common/response_dto.py` & `openxlab-0.1.0/openxlab/model/common/response_dto.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import re
-
-
-class ReturnDto:
-    def __init__(self, trace_id=None, msg_code=None, msg=None, data=None, total=None, success=None):
-        self.trace_id = trace_id
-        self.msg_code = msg_code
-        self.msg = msg
-        self.data = data
-        self.total = total
-        self.success = success
-
-    # 将驼峰型属性名转换为下划线型属性名
-    @classmethod
-    def from_camel_case(cls, camel_dict):
-        snake_dict = {}
-        for key, value in camel_dict.items():
-            snake_key = re.sub(r'(?<!^)(?=[A-Z])', '_', key).lower()
-            snake_dict[snake_key] = value
-        return cls(**snake_dict)
-
-
-class DownloadUrlDto:
-    def __int__(self, url=None, updating=None, updating_readme=None):
-        self.url = url
-        self.updating = updating
-        self.updating_readme = updating_readme
+import re
+
+
+class ReturnDto:
+    def __init__(self, trace_id=None, msg_code=None, msg=None, data=None, total=None, success=None):
+        self.trace_id = trace_id
+        self.msg_code = msg_code
+        self.msg = msg
+        self.data = data
+        self.total = total
+        self.success = success
+
+    # 将驼峰型属性名转换为下划线型属性名
+    @classmethod
+    def from_camel_case(cls, camel_dict):
+        snake_dict = {}
+        for key, value in camel_dict.items():
+            snake_key = re.sub(r'(?<!^)(?=[A-Z])', '_', key).lower()
+            snake_dict[snake_key] = value
+        return cls(**snake_dict)
+
+
+class DownloadUrlDto:
+    def __int__(self, url=None, updating=None, updating_readme=None):
+        self.url = url
+        self.updating = updating
+        self.updating_readme = updating_readme
```

### Comparing `openxlab-0.0.9/openxlab/model/handler/upload_file.py` & `openxlab-0.1.0/openxlab/model/handler/upload_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,83 +1,94 @@
-"""
-upload or update model file | log file | metafile
-"""
-import re
-import os
-
-from openxlab.model.clients.openapi_client import OpenapiClient
-from openxlab.model.clients.oss_client import OssClient
-from openxlab.model.clients.upload_service_client import UploadServiceClient
-from openxlab.model.common.constants import endpoint, token, oss_endpoint
-from openxlab.model.common.meta_file_util import MetafileParser
-
-
-def upload(model_repo, file_type, source, target=None) -> None:
-    """
-    upload model file | readme file | logfile | meta file
-    """
-    try:
-        # split params
-        username, repository = _split_repo(model_repo)
-        client = OpenapiClient(endpoint, token)
-        """
-        cli逻辑：
-        metafile-根据metafile全部覆盖上传
-        other-指定具体文件上传
-        web端逻辑如下：
-        1. 查询哪些待上传
-        2. 更新上传状态-开始上传
-        2. 遍历获取signature
-        3. 上传oss
-        4. 更新上传状态-上传完成
-        """
-        if file_type == 'metafile':
-            remote_model_list = client.query_models(repository)['models']
-
-            meta_parser = MetafileParser(source)
-            meta_data = meta_parser.parse_and_validate()
-            meta_file_model_list = meta_data['Models']
-            upload_model_list(client, repository, meta_file_model_list, remote_model_list)
-        elif file_type == 'other':
-            print('other way is designing')
-        else:
-            raise ValueError("file_type only support metafile/other")
-        print(f"file upload successfully.")
-    except ValueError as e:
-        print(f"Error: {e}")
-        return
-
-
-def _split_repo(model_repo) -> (str, str):
-    """
-    Split a full repository name into two separate strings: the username and the repository name.
-    """
-    # username/repository format check
-    pattern = r'^[a-zA-Z0-9]+\/[a-zA-Z0-9\-_]+$'
-    if not re.match(pattern, model_repo):
-        raise ValueError("The input string must be in the format 'didi12/test-d-1'")
-
-    values = model_repo.split('/')
-    return values[0], values[1]
-
-
-def upload_model_list(client: OpenapiClient, repository, meta_file_model_list, remote_model_list):
-    meta_file_model_need_upload_list = []
-    # 筛选出新增的models
-    new_models = [m_meta for m_meta in meta_file_model_list
-                  if m_meta['Name'] not in [m_remote['name'] for m_remote in remote_model_list]]
-    update_models = [m_meta for m_meta in meta_file_model_list for m_remote in remote_model_list
-                     if m_meta['Name'] == m_remote['name']]
-    # 加上更新的models
-    meta_file_model_need_upload_list = new_models + update_models
-    file_names = [os.path.basename(m['Weights']) for m in meta_file_model_need_upload_list]
-    models_data = client.update_upload_status(repository, file_names, new_models, update_models, 1)
-    model_info_list = models_data['objects']
-    for model in meta_file_model_need_upload_list:
-        model_info_filter_list = list(filter(lambda m: m['modelName'] == model['Name'], model_info_list))
-        signature = client.get_upload_signature(models_data['repositoryId'], models_data['uid'], model,
-                                                               model_info_filter_list[0])
-        oss_client = OssClient(oss_endpoint, signature['accessKeyId'], signature['accessKeySecret'],
-                               signature['stsToken'],
-                               signature['bucket'])
-        oss_client.upload_to_oss(model['Weights'], signature['object'], signature['callback'], signature['callbackVar'])
-        client.update_upload_status(repository, [os.path.basename(model['Weights'])], upload_status=2)
+"""
+upload or update model file | log file | metafile
+"""
+import os
+import re
+
+from openxlab.model.clients.openapi_client import OpenapiClient
+from openxlab.model.clients.oss_client import OssClient
+from openxlab.model.common.bury import bury_data
+from openxlab.model.common.constants import endpoint, token, oss_endpoint
+from openxlab.model.common.meta_file_util import MetafileParser
+
+
+@bury_data("upload_file")
+def upload(model_repo, file_type='metafile', source=None, target=None, domain='bucket') -> None:
+    """
+    upload model file | readme file | logfile | meta file
+    model_repo: model repo full name
+    file_type: upload method.
+    source: metafile location
+
+    """
+    try:
+        # split params
+        username, repository = _split_repo(model_repo)
+        client = OpenapiClient(endpoint, token)
+        """
+        cli逻辑：
+        metafile-根据metafile全部覆盖上传
+        other-指定具体文件上传
+        web端逻辑如下：
+        1. 查询哪些待上传
+        2. 更新上传状态-开始上传
+        2. 遍历获取signature
+        3. 上传oss
+        4. 更新上传状态-上传完成
+        """
+        if file_type == 'metafile':
+            remote_model_list = client.query_models(repository)['models']
+
+            meta_parser = MetafileParser(source)
+            meta_data = meta_parser.parse_and_validate()
+            meta_file_model_list = meta_data['Models']
+            upload_model_list(client, repository, meta_file_model_list, remote_model_list, domain)
+        elif file_type == 'other':
+            print('other way is designing')
+        else:
+            raise ValueError("file_type only support metafile/other")
+        print(f"file upload successfully.")
+    except ValueError as e:
+        print(f"Error: {e}")
+        return
+
+
+def _split_repo(model_repo) -> (str, str):
+    """
+    Split a full repository name into two separate strings: the username and the repository name.
+    """
+    # username/repository format check
+    pattern = r'.+/.+'
+    if not re.match(pattern, model_repo):
+        raise ValueError("The input string must be in the format 'username/model_repo'")
+
+    values = model_repo.split('/')
+    return values[0], values[1]
+
+
+def upload_model_list(client: OpenapiClient, repository, meta_file_model_list, remote_model_list, domain):
+    # 筛选出新增的models
+    new_models = [m_meta for m_meta in meta_file_model_list
+                  if m_meta['Name'] not in [m_remote['name'] for m_remote in remote_model_list]]
+
+    update_models = []
+    file_names = []
+    for m_meta in meta_file_model_list:
+        for m_remote in remote_model_list:
+            if m_meta['Name'] == m_remote['name'] and os.path.basename(m_meta['Weights']) != m_remote['weightName']:
+                file_names.append(m_remote['weightName'])
+            else:
+                file_names.append(os.path.basename(m_meta['Weights']))
+            update_models.append(m_meta)
+
+    models_data = client.update_upload_status(repository, file_names, new_models, update_models, 1)
+    model_info_list = models_data['objects']
+    for model in meta_file_model_list:
+        model_info_filter_list = list(filter(lambda m: m['modelName'] == model['Name'], model_info_list))
+        signature = client.get_upload_signature(models_data['repositoryId'], models_data['uid'], model,
+                                                model_info_filter_list[0])
+        oss_client = OssClient(oss_endpoint, signature['accessKeyId'], signature['accessKeySecret'],
+                               signature['stsToken'],
+                               signature['bucket'])
+        # oss_client.upload_to_oss(model['Weights'], signature['object'], signature['callback'], signature['callbackVar'])
+        oss_client.multipart_resume_upload(model['Weights'], signature['object'], signature['callback'], signature['callbackVar'], domain=domain)
+        client.update_upload_status(repository, [os.path.basename(model['Weights'])], upload_status=2)
```

### Comparing `openxlab-0.0.9/openxlab/utils/file.py` & `openxlab-0.1.0/openxlab/utils/file.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-import re
-import sys
-from os.path import exists
-
-
-def get_file_content(file_name):
-    with open(file_name, encoding='utf-8') as f:
-        content = f.read()
-    return content
-    
-    
-def parse_requirements(fname='requirements.txt', with_version=True):
-    """Parse the package dependencies listed in a requirements file but strips
-    specific versioning information.
-
-    Args:
-        fname (str): path to requirements file
-        with_version (bool, default=False): if True include version specs
-
-    Returns:
-        List[str]: list of requirements items
-
-    CommandLine:
-        python -c "import setup; print(setup.parse_requirements())"
-    """
-
-    require_fpath = fname
-
-    def parse_line(line):
-        """Parse information from a line in a requirements text file."""
-        if line.startswith('-r '):
-            # Allow specifying requirements in other files
-            target = line.split(' ')[1]
-            for info in parse_require_file(target):
-                yield info
-        else:
-            info = {'line': line}
-            if line.startswith('-e '):
-                info['package'] = line.split('#egg=')[1]
-            elif '@git+' in line:
-                info['package'] = line
-            else:
-                # Remove versioning from the package
-                pat = '(' + '|'.join(['>=', '==', '>']) + ')'
-                parts = re.split(pat, line, maxsplit=1)
-                parts = [p.strip() for p in parts]
-
-                info['package'] = parts[0]
-                if len(parts) > 1:
-                    op, rest = parts[1:]
-                    if ';' in rest:
-                        # Handle platform specific dependencies
-                        # http://setuptools.readthedocs.io/en/latest/setuptools.html#declaring-platform-specific-dependencies
-                        version, platform_deps = map(str.strip,
-                                                     rest.split(';'))
-                        info['platform_deps'] = platform_deps
-                    else:
-                        version = rest  # NOQA
-                    info['version'] = (op, version)
-            yield info
-
-    def parse_require_file(fpath):
-        with open(fpath, 'r') as f:
-            for line in f.readlines():
-                line = line.strip()
-                if line and not line.startswith('#'):
-                    for info in parse_line(line):
-                        yield info
-
-    def gen_packages_items():
-        if exists(require_fpath):
-            for info in parse_require_file(require_fpath):
-                parts = [info['package']]
-                if with_version and 'version' in info:
-                    parts.extend(info['version'])
-                if not sys.version.startswith('3.4'):
-                    # apparently package_deps are broken in 3.4
-                    platform_deps = info.get('platform_deps')
-                    if platform_deps is not None:
-                        parts.append(';' + platform_deps)
-                item = ''.join(parts)
-                yield item
-
-    packages = list(gen_packages_items())
+import re
+import sys
+from os.path import exists
+
+
+def get_file_content(file_name):
+    with open(file_name, encoding='utf-8') as f:
+        content = f.read()
+    return content
+    
+    
+def parse_requirements(fname='requirements.txt', with_version=True):
+    """Parse the package dependencies listed in a requirements file but strips
+    specific versioning information.
+
+    Args:
+        fname (str): path to requirements file
+        with_version (bool, default=False): if True include version specs
+
+    Returns:
+        List[str]: list of requirements items
+
+    CommandLine:
+        python -c "import setup; print(setup.parse_requirements())"
+    """
+
+    require_fpath = fname
+
+    def parse_line(line):
+        """Parse information from a line in a requirements text file."""
+        if line.startswith('-r '):
+            # Allow specifying requirements in other files
+            target = line.split(' ')[1]
+            for info in parse_require_file(target):
+                yield info
+        else:
+            info = {'line': line}
+            if line.startswith('-e '):
+                info['package'] = line.split('#egg=')[1]
+            elif '@git+' in line:
+                info['package'] = line
+            else:
+                # Remove versioning from the package
+                pat = '(' + '|'.join(['>=', '==', '>']) + ')'
+                parts = re.split(pat, line, maxsplit=1)
+                parts = [p.strip() for p in parts]
+
+                info['package'] = parts[0]
+                if len(parts) > 1:
+                    op, rest = parts[1:]
+                    if ';' in rest:
+                        # Handle platform specific dependencies
+                        # http://setuptools.readthedocs.io/en/latest/setuptools.html#declaring-platform-specific-dependencies
+                        version, platform_deps = map(str.strip,
+                                                     rest.split(';'))
+                        info['platform_deps'] = platform_deps
+                    else:
+                        version = rest  # NOQA
+                    info['version'] = (op, version)
+            yield info
+
+    def parse_require_file(fpath):
+        with open(fpath, 'r') as f:
+            for line in f.readlines():
+                line = line.strip()
+                if line and not line.startswith('#'):
+                    for info in parse_line(line):
+                        yield info
+
+    def gen_packages_items():
+        if exists(require_fpath):
+            for info in parse_require_file(require_fpath):
+                parts = [info['package']]
+                if with_version and 'version' in info:
+                    parts.extend(info['version'])
+                if not sys.version.startswith('3.4'):
+                    # apparently package_deps are broken in 3.4
+                    platform_deps = info.get('platform_deps')
+                    if platform_deps is not None:
+                        parts.append(';' + platform_deps)
+                item = ''.join(parts)
+                yield item
+
+    packages = list(gen_packages_items())
     return packages
```

### Comparing `openxlab-0.0.9/openxlab/utils/time_util.py` & `openxlab-0.1.0/openxlab/utils/time_util.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from datetime import datetime
-import pytz
-
-
-def get_current_formatted_time(timezone='Asia/Shanghai') -> str:
-    formatted_date = get_current_time(timezone).strftime("%Y-%m-%d %H:%M:%S")
-    return formatted_date
-
-
-def get_current_time(timezone='Asia/Shanghai') -> datetime:
-    now_utc = datetime.now(tz=pytz.utc)
-    tz = pytz.timezone(timezone)
-    return now_utc.astimezone(tz)
-
-
-def get_datetime_from_formatted_str(time_str, timezone='Asia/Shanghai') -> datetime:
-    if len(time_str) == 0:
-        raise ValueError("formatted time string must not be empty")
-    timezone = pytz.timezone(timezone)
-    return datetime.strptime(time_str, '%Y-%m-%d %H:%M:%S').replace(tzinfo=timezone)
+from datetime import datetime
+import pytz
+
+
+def get_current_formatted_time(timezone='Asia/Shanghai') -> str:
+    formatted_date = get_current_time(timezone).strftime("%Y-%m-%d %H:%M:%S")
+    return formatted_date
+
+
+def get_current_time(timezone='Asia/Shanghai') -> datetime:
+    now_utc = datetime.now(tz=pytz.utc)
+    tz = pytz.timezone(timezone)
+    return now_utc.astimezone(tz)
+
+
+def get_datetime_from_formatted_str(time_str, timezone='Asia/Shanghai') -> datetime:
+    if len(time_str) == 0:
+        raise ValueError("formatted time string must not be empty")
+    timezone = pytz.timezone(timezone)
+    return datetime.strptime(time_str, '%Y-%m-%d %H:%M:%S').replace(tzinfo=timezone)
```

### Comparing `openxlab-0.0.9/openxlab/xlab/common/response_dto.py` & `openxlab-0.1.0/openxlab/xlab/common/response_dto.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import json
-import re
-
-
-class ReturnDto:
-    def __init__(self, trace_id=None, msg_code=None, msg=None, data=None, total=None, success=None):
-        self.trace_id = trace_id
-        self.msg_code = msg_code
-        self.msg = msg
-        self.data = data
-        self.total = total
-        self.success = success
-
-    def is_success(self):
-        return self.msg_code == '10000'
-
-    def to_json(self):
-        return json.dumps(self, default=lambda o: o.__dict__,
-                          sort_keys=True, indent=4)
-
-    # 将驼峰型属性名转换为下划线型属性名
-    @classmethod
-    def from_camel_case(cls, camel_dict):
-        snake_dict = {}
-        for key, value in camel_dict.items():
-            snake_key = re.sub(r'(?<!^)(?=[A-Z])', '_', key).lower()
-            snake_dict[snake_key] = value
-        return cls(**snake_dict)
+import json
+import re
+
+
+class ReturnDto:
+    def __init__(self, trace_id=None, msg_code=None, msg=None, data=None, total=None, success=None):
+        self.trace_id = trace_id
+        self.msg_code = msg_code
+        self.msg = msg
+        self.data = data
+        self.total = total
+        self.success = success
+
+    def is_success(self):
+        return self.msg_code == '10000'
+
+    def to_json(self):
+        return json.dumps(self, default=lambda o: o.__dict__,
+                          sort_keys=True, indent=4)
+
+    # 将驼峰型属性名转换为下划线型属性名
+    @classmethod
+    def from_camel_case(cls, camel_dict):
+        snake_dict = {}
+        for key, value in camel_dict.items():
+            snake_key = re.sub(r'(?<!^)(?=[A-Z])', '_', key).lower()
+            snake_dict[snake_key] = value
+        return cls(**snake_dict)
```

### Comparing `openxlab-0.0.9/openxlab/xlab/handler/user_config.py` & `openxlab-0.1.0/openxlab/xlab/handler/user_config.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,60 +1,87 @@
-import json
-
-from openxlab.config import const
-from openxlab.utils.file import *
-from openxlab.utils.env_util import *
-
-
-def get_config_path() -> str:
-    return os.path.join(get_config_dir(), get_config_file_name())
-
-
-def get_token_path() -> str:
-    return os.path.join(get_config_dir(), get_token_file_name())
-
-
-def get_config_dir() -> str:
-    return const.DEFAULT_CONFIG_DIR
-
-
-def get_token_file_name() -> str:
-    return const.DEFAULT_CLI_TOKEN_FILE_NAME
-
-
-def get_config_file_name() -> str:
-    return const.DEFAULT_CLI_CONFIG_FILE_NAME
-
-
-def get_config(ak=None, sk=None):
-    if ak is not None and sk is not None:
-        return UserConfig(ak, sk)
-    if not os.path.exists(get_config_path()):
-        ak_env_value = get_env(const.AK_ENV_NAME)
-        sk_env_value = get_env(const.SK_ENV_NAME)
-        if ak_env_value is not None and sk_env_value is not None:
-            return UserConfig(ak_env_value, sk_env_value)
-        return None
-    config_json = get_file_content(get_config_path())
-    config_dict = json.loads(config_json)
-    return UserConfig(config_dict['ak'], config_dict['sk'])
-
-
-class UserConfig(object):
-    def __init__(self, ak, sk):
-        if ak is None or sk is None:
-            raise ValueError("ak and sk must not be empty")
-        self.ak = ak
-        self.sk = sk
-
-    def to_json(self):
-        return json.dumps(self, default=lambda o: o.__dict__,
-                          sort_keys=True, indent=4)
-
-    def store_to_local(self):
-        if not os.path.exists(get_config_dir()):
-            os.makedirs(get_config_dir(), mode=0o700)
-        config_json = self.to_json()
-        set_env(const.AK_ENV_NAME, self.ak)
-        set_env(const.SK_ENV_NAME, self.sk)
-        with open(get_config_path(), mode="w", encoding='utf-8') as f:
-            f.write(config_json)
+import json
+
+from openxlab.config import const
+from openxlab.utils.env_util import *
+from openxlab.utils.file import *
+
+
+def get_config_path() -> str:
+    return os.path.join(get_config_dir(), get_config_file_name())
+
+
+def get_token_path() -> str:
+    return os.path.join(get_config_dir(), get_token_file_name())
+
+
+def get_dataset_path() -> str:
+    return os.path.join(get_config_dir(), get_dataset_file_name())
+
+
+def get_version_path() -> str:
+    return os.path.join(get_config_dir(), get_version_file_name())
+
+def get_config_dir() -> str:
+    return const.DEFAULT_CONFIG_DIR
+
+def get_version_file_name() -> str:
+    return const.DEFAULT_CLI_VERSION_FILE_NAME
+
+def get_token_file_name() -> str:
+    return const.DEFAULT_CLI_TOKEN_FILE_NAME
+
+
+def get_config_file_name() -> str:
+    return const.DEFAULT_CLI_CONFIG_FILE_NAME
+
+
+def get_dataset_file_name() -> str:
+    return const.DEFAULT_CLI_DATASET_FILE_NAME
+
+
+def get_config(ak=None, sk=None, auth=False):
+    """@auth: utilized to check user's ak, if not, ask user to login"""
+    if ak is not None and sk is not None:
+        return UserConfig(ak, sk)
+    if not os.path.exists(get_config_path()):
+        ak_env_value = get_env(const.AK_ENV_NAME)
+        sk_env_value = get_env(const.SK_ENV_NAME)
+        if ak_env_value is not None and sk_env_value is not None:
+            return UserConfig(ak_env_value, sk_env_value)
+        # need login
+        if auth is True and not ak_env_value:
+            raise Exception(
+                "Please login openxlab and config ak/sk, try \"openxlab login\" and refer to https://openxlab.org.cn/docs/developers/鉴权管理.html"
+            )
+        return None
+    config_json = get_file_content(get_config_path())
+    config_dict = json.loads(config_json)
+    return UserConfig(config_dict['ak'], config_dict['sk'])
+
+
+def clear_dataset_json():
+    """clear the content in dataset.json file"""
+    try:
+        with open(get_dataset_path(), 'w') as f:
+            f.truncate(0)
+    except Exception as e:
+        raise (e)
+
+
+class UserConfig(object):
+    def __init__(self, ak, sk):
+        if ak is None or sk is None:
+            raise ValueError("ak and sk must not be empty")
+        self.ak = ak.strip()
+        self.sk = sk.strip()
+
+    def to_json(self):
+        return json.dumps(self, default=lambda o: o.__dict__, sort_keys=True, indent=4)
+
+    def store_to_local(self):
+        if not os.path.exists(get_config_dir()):
+            os.makedirs(get_config_dir(), mode=0o700)
+        config_json = self.to_json()
+        set_env(const.AK_ENV_NAME, self.ak)
+        set_env(const.SK_ENV_NAME, self.sk)
+        with open(get_config_path(), mode="w", encoding='utf-8') as f:
+            f.write(config_json)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

