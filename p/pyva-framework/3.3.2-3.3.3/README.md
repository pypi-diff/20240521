# Comparing `tmp/pyva_framework-3.3.2.tar.gz` & `tmp/pyva_framework-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyva_framework-3.3.2.tar", last modified: Thu Apr 18 14:00:47 2024, max compression
+gzip compressed data, was "pyva_framework-3.3.3.tar", last modified: Tue May 21 07:18:55 2024, max compression
```

## Comparing `pyva_framework-3.3.2.tar` & `pyva_framework-3.3.3.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.226403 pyva_framework-3.3.2/
--rw-r--r--   0 szq        (501) staff       (20)     1073 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/LICENSE
--rw-r--r--   0 szq        (501) staff       (20)     2417 2024-04-18 14:00:47.225611 pyva_framework-3.3.2/PKG-INFO
--rw-r--r--   0 szq        (501) staff       (20)     1303 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/README.md
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.177483 pyva_framework-3.3.2/pyva/
--rw-r--r--   0 szq        (501) staff       (20)     1455 2024-04-17 10:15:56.000000 pyva_framework-3.3.2/pyva/Application.py
--rw-r--r--   0 szq        (501) staff       (20)      708 2023-11-28 12:16:55.000000 pyva_framework-3.3.2/pyva/Global.py
--rw-r--r--   0 szq        (501) staff       (20)     1010 2024-04-17 10:15:56.000000 pyva_framework-3.3.2/pyva/GlobalInit.py
--rw-r--r--   0 szq        (501) staff       (20)        0 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.179100 pyva_framework-3.3.2/pyva/cli/
--rw-r--r--   0 szq        (501) staff       (20)       18 2023-11-26 01:27:02.000000 pyva_framework-3.3.2/pyva/cli/__init__.py
--rw-r--r--   0 szq        (501) staff       (20)     1464 2023-11-26 11:30:11.000000 pyva_framework-3.3.2/pyva/cli/main.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.180205 pyva_framework-3.3.2/pyva/client/
--rw-r--r--   0 szq        (501) staff       (20)       21 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/client/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.184832 pyva_framework-3.3.2/pyva/client/dingtalk/
--rw-r--r--   0 szq        (501) staff       (20)     2563 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkContactClient.py
--rw-r--r--   0 szq        (501) staff       (20)     3239 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkOauth2Client.py
--rw-r--r--   0 szq        (501) staff       (20)     6758 2023-11-28 14:43:59.000000 pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkRobotClient.py
--rw-r--r--   0 szq        (501) staff       (20)     5526 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkYidaClient.py
--rw-r--r--   0 szq        (501) staff       (20)       31 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/client/dingtalk/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.187862 pyva_framework-3.3.2/pyva/common/
--rw-r--r--   0 szq        (501) staff       (20)      999 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/common/FastapiEvents.py
--rw-r--r--   0 szq        (501) staff       (20)     1911 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/common/FastapiException.py
--rw-r--r--   0 szq        (501) staff       (20)     1229 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/common/LoggerHandler.py
--rw-r--r--   0 szq        (501) staff       (20)       21 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/common/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.195212 pyva_framework-3.3.2/pyva/config/
--rw-r--r--   0 szq        (501) staff       (20)      963 2023-11-26 17:09:44.000000 pyva_framework-3.3.2/pyva/config/AppConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      893 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/config/DbConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      525 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/config/DingtalkConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      128 2023-11-28 14:45:03.000000 pyva_framework-3.3.2/pyva/config/DingtalkRobotConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      729 2023-11-26 17:08:07.000000 pyva_framework-3.3.2/pyva/config/FastapiConfig.py
--rw-r--r--   0 szq        (501) staff       (20)     3524 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/config/LoggingConfig.py
--rw-r--r--   0 szq        (501) staff       (20)       88 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/config/MongoConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      894 2023-11-28 10:52:03.000000 pyva_framework-3.3.2/pyva/config/NacosConfig.py
--rw-r--r--   0 szq        (501) staff       (20)      392 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/config/RedisConfig.py
--rw-r--r--   0 szq        (501) staff       (20)       21 2023-11-28 08:22:32.000000 pyva_framework-3.3.2/pyva/config/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.198005 pyva_framework-3.3.2/pyva/dao/
--rw-r--r--   0 szq        (501) staff       (20)     1401 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/dao/BaseDao.py
--rw-r--r--   0 szq        (501) staff       (20)     5952 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/dao/ListDao.py
--rw-r--r--   0 szq        (501) staff       (20)       18 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/dao/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.200779 pyva_framework-3.3.2/pyva/dto/
--rw-r--r--   0 szq        (501) staff       (20)     1360 2023-11-26 13:59:29.000000 pyva_framework-3.3.2/pyva/dto/BaseDto.py
--rw-r--r--   0 szq        (501) staff       (20)     1395 2023-11-22 14:07:26.000000 pyva_framework-3.3.2/pyva/dto/ListDto.py
--rw-r--r--   0 szq        (501) staff       (20)       18 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/dto/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.204362 pyva_framework-3.3.2/pyva/entity/
--rw-r--r--   0 szq        (501) staff       (20)     1190 2023-11-26 13:33:29.000000 pyva_framework-3.3.2/pyva/entity/BaseEntity.py
--rw-r--r--   0 szq        (501) staff       (20)     1073 2023-11-26 13:27:10.000000 pyva_framework-3.3.2/pyva/entity/GeneralHumpEntity.py
--rw-r--r--   0 szq        (501) staff       (20)      441 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/entity/HumpEntity.py
--rw-r--r--   0 szq        (501) staff       (20)        0 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/entity/__init__.py
--rw-r--r--   0 szq        (501) staff       (20)     1047 2024-04-17 13:46:37.000000 pyva_framework-3.3.2/pyva/startupApp.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.218524 pyva_framework-3.3.2/pyva/util/
--rw-r--r--   0 szq        (501) staff       (20)     5269 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/util/ConfigUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     9245 2023-11-29 07:09:53.000000 pyva_framework-3.3.2/pyva/util/DbUtil.py
--rw-r--r--   0 szq        (501) staff       (20)      581 2023-11-27 15:58:15.000000 pyva_framework-3.3.2/pyva/util/DictUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2780 2023-11-21 10:17:20.000000 pyva_framework-3.3.2/pyva/util/EntityUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1081 2024-04-17 10:13:18.000000 pyva_framework-3.3.2/pyva/util/FileUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1807 2023-11-22 13:57:36.000000 pyva_framework-3.3.2/pyva/util/IpUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2006 2024-04-17 10:15:56.000000 pyva_framework-3.3.2/pyva/util/JsonUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2034 2024-04-17 10:15:56.000000 pyva_framework-3.3.2/pyva/util/LockerUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1985 2024-04-17 10:15:56.000000 pyva_framework-3.3.2/pyva/util/MongoUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     6692 2023-11-28 13:44:28.000000 pyva_framework-3.3.2/pyva/util/NacosUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     1608 2023-11-26 15:13:28.000000 pyva_framework-3.3.2/pyva/util/PathUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     4136 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/util/QrcodeUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     2180 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/util/RedisUtil.py
--rw-r--r--   0 szq        (501) staff       (20)     6613 2024-04-17 10:15:56.000000 pyva_framework-3.3.2/pyva/util/TimeUtil.py
--rw-r--r--   0 szq        (501) staff       (20)       21 2023-10-17 09:37:11.000000 pyva_framework-3.3.2/pyva/util/__init__.py
-drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-04-18 14:00:47.224640 pyva_framework-3.3.2/pyva_framework.egg-info/
--rw-r--r--   0 szq        (501) staff       (20)     2417 2024-04-18 14:00:47.000000 pyva_framework-3.3.2/pyva_framework.egg-info/PKG-INFO
--rw-r--r--   0 szq        (501) staff       (20)     1578 2024-04-18 14:00:47.000000 pyva_framework-3.3.2/pyva_framework.egg-info/SOURCES.txt
--rw-r--r--   0 szq        (501) staff       (20)        1 2024-04-18 14:00:47.000000 pyva_framework-3.3.2/pyva_framework.egg-info/dependency_links.txt
--rw-r--r--   0 szq        (501) staff       (20)       43 2024-04-18 14:00:47.000000 pyva_framework-3.3.2/pyva_framework.egg-info/entry_points.txt
--rw-r--r--   0 szq        (501) staff       (20)      306 2024-04-18 14:00:47.000000 pyva_framework-3.3.2/pyva_framework.egg-info/requires.txt
--rw-r--r--   0 szq        (501) staff       (20)        5 2024-04-18 14:00:47.000000 pyva_framework-3.3.2/pyva_framework.egg-info/top_level.txt
--rw-r--r--   0 szq        (501) staff       (20)       38 2024-04-18 14:00:47.226549 pyva_framework-3.3.2/setup.cfg
--rw-r--r--   0 szq        (501) staff       (20)     1092 2024-04-17 14:40:02.000000 pyva_framework-3.3.2/setup.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.998657 pyva_framework-3.3.3/
+-rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/LICENSE
+-rw-r--r--   0 szq        (501) staff       (20)     2464 2024-05-21 07:18:55.998376 pyva_framework-3.3.3/PKG-INFO
+-rw-r--r--   0 szq        (501) staff       (20)     1349 2024-05-21 06:47:59.000000 pyva_framework-3.3.3/README.md
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.989681 pyva_framework-3.3.3/pyva/
+-rw-r--r--   0 szq        (501) staff       (20)     1455 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/Application.py
+-rw-r--r--   0 szq        (501) staff       (20)      708 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/Global.py
+-rw-r--r--   0 szq        (501) staff       (20)     1010 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/GlobalInit.py
+-rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.989934 pyva_framework-3.3.3/pyva/cli/
+-rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/cli/__init__.py
+-rw-r--r--   0 szq        (501) staff       (20)     1464 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/cli/main.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.990054 pyva_framework-3.3.3/pyva/client/
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/client/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.991561 pyva_framework-3.3.3/pyva/client/dingtalk/
+-rw-r--r--   0 szq        (501) staff       (20)     2563 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkContactClient.py
+-rw-r--r--   0 szq        (501) staff       (20)     3239 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkOauth2Client.py
+-rw-r--r--   0 szq        (501) staff       (20)     6758 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkRobotClient.py
+-rw-r--r--   0 szq        (501) staff       (20)     5526 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkYidaClient.py
+-rw-r--r--   0 szq        (501) staff       (20)       31 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/client/dingtalk/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.992264 pyva_framework-3.3.3/pyva/common/
+-rw-r--r--   0 szq        (501) staff       (20)      999 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/common/FastapiEvents.py
+-rw-r--r--   0 szq        (501) staff       (20)     1911 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/common/FastapiException.py
+-rw-r--r--   0 szq        (501) staff       (20)     1229 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/common/LoggerHandler.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/common/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.993634 pyva_framework-3.3.3/pyva/config/
+-rw-r--r--   0 szq        (501) staff       (20)     1069 2024-05-21 06:55:20.000000 pyva_framework-3.3.3/pyva/config/AppConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      893 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/config/DbConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      525 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/config/DingtalkConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      128 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/config/DingtalkRobotConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      729 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/config/FastapiConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)     3524 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/config/LoggingConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)       88 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/config/MongoConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      894 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/config/NacosConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)      392 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/config/RedisConfig.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/config/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.994125 pyva_framework-3.3.3/pyva/dao/
+-rw-r--r--   0 szq        (501) staff       (20)     1401 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/dao/BaseDao.py
+-rw-r--r--   0 szq        (501) staff       (20)     5952 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/dao/ListDao.py
+-rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/dao/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.994524 pyva_framework-3.3.3/pyva/dto/
+-rw-r--r--   0 szq        (501) staff       (20)     1360 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/dto/BaseDto.py
+-rw-r--r--   0 szq        (501) staff       (20)     1395 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/dto/ListDto.py
+-rw-r--r--   0 szq        (501) staff       (20)       18 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/dto/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.995029 pyva_framework-3.3.3/pyva/entity/
+-rw-r--r--   0 szq        (501) staff       (20)     1190 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/entity/BaseEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)     1073 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/entity/GeneralHumpEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)      441 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/entity/HumpEntity.py
+-rw-r--r--   0 szq        (501) staff       (20)        0 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/entity/__init__.py
+-rw-r--r--   0 szq        (501) staff       (20)     1047 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/startupApp.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.997274 pyva_framework-3.3.3/pyva/util/
+-rw-r--r--   0 szq        (501) staff       (20)     5269 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/ConfigUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     9245 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/DbUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)      581 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/DictUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2780 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/EntityUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1081 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/FileUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1807 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/IpUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2006 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/JsonUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2034 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/LockerUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1985 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/MongoUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     6692 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/NacosUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     1608 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/PathUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     4136 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/util/QrcodeUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     2180 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/util/RedisUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)     6613 2024-05-21 06:54:51.000000 pyva_framework-3.3.3/pyva/util/TimeUtil.py
+-rw-r--r--   0 szq        (501) staff       (20)       21 2024-05-21 06:24:11.000000 pyva_framework-3.3.3/pyva/util/__init__.py
+drwxr-xr-x   0 szq        (501) staff       (20)        0 2024-05-21 07:18:55.998026 pyva_framework-3.3.3/pyva_framework.egg-info/
+-rw-r--r--   0 szq        (501) staff       (20)     2464 2024-05-21 07:18:55.000000 pyva_framework-3.3.3/pyva_framework.egg-info/PKG-INFO
+-rw-r--r--   0 szq        (501) staff       (20)     1578 2024-05-21 07:18:55.000000 pyva_framework-3.3.3/pyva_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 szq        (501) staff       (20)        1 2024-05-21 07:18:55.000000 pyva_framework-3.3.3/pyva_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 szq        (501) staff       (20)       43 2024-05-21 07:18:55.000000 pyva_framework-3.3.3/pyva_framework.egg-info/entry_points.txt
+-rw-r--r--   0 szq        (501) staff       (20)      307 2024-05-21 07:18:55.000000 pyva_framework-3.3.3/pyva_framework.egg-info/requires.txt
+-rw-r--r--   0 szq        (501) staff       (20)        5 2024-05-21 07:18:55.000000 pyva_framework-3.3.3/pyva_framework.egg-info/top_level.txt
+-rw-r--r--   0 szq        (501) staff       (20)       38 2024-05-21 07:18:55.998706 pyva_framework-3.3.3/setup.cfg
+-rw-r--r--   0 szq        (501) staff       (20)     1092 2024-05-21 07:02:29.000000 pyva_framework-3.3.3/setup.py
```

### Comparing `pyva_framework-3.3.2/LICENSE` & `pyva_framework-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/PKG-INFO` & `pyva_framework-3.3.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: pyva-framework
-Version: 3.3.2
+Version: 3.3.3
 Summary: PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
 Home-page: https://github.com/zhenqiang-sun/pyva
 Author: Zhenqiang Sun
 Author-email: zhenqiang.sun@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fastapi==0.104.1
-Requires-Dist: uvicorn==0.24.0
-Requires-Dist: SQLAlchemy==2.0.23
+Requires-Dist: fastapi==0.111.0
+Requires-Dist: uvicorn==0.29.0
+Requires-Dist: SQLAlchemy==2.0.30
 Requires-Dist: PyMySQL==1.1.0
 Requires-Dist: sqlacodegen==2.3.0
-Requires-Dist: redis==5.0.1
-Requires-Dist: requests==2.31.0
+Requires-Dist: redis==5.0.4
+Requires-Dist: requests==2.32.1
 Requires-Dist: pyhumps==3.8.0
 Requires-Dist: nacos-sdk-python==0.1.14
 Requires-Dist: PyYAML==6.0.1
-Requires-Dist: python-multipart==0.0.6
-Requires-Dist: pymongo==4.6.0
-Requires-Dist: orjson==3.9.10
+Requires-Dist: python-multipart==0.0.9
+Requires-Dist: pymongo==4.7.2
+Requires-Dist: orjson==3.10.3
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: deprecated==1.2.14
-Requires-Dist: jinja2==3.1.2
-Requires-Dist: typer[all]==0.9.0
+Requires-Dist: jinja2==3.1.4
+Requires-Dist: typer[all]==0.12.3
 Requires-Dist: py-ulid==1.0.3
 
 # PyVa
 PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
 
 [Github: PyVa](https://github.com/zhenqiang-sun/pyva)
+[Gitee: PyVa](https://gitee.com/qiangai/pyva)
 
 ### 依赖组件：
 
 #### 1、FastAPI
 https://fastapi.tiangolo.com/
 * 快速：可与 NodeJS 和 Go 比肩的极高性能（归功于 Starlette 和 Pydantic）。最快的 Python web 框架之一。
 * 高效编码：提高功能开发速度约 200％ 至 300％。*
```

### Comparing `pyva_framework-3.3.2/README.md` & `pyva_framework-3.3.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # PyVa
 PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
 
 [Github: PyVa](https://github.com/zhenqiang-sun/pyva)
+[Gitee: PyVa](https://gitee.com/qiangai/pyva)
 
 ### 依赖组件：
 
 #### 1、FastAPI
 https://fastapi.tiangolo.com/
 * 快速：可与 NodeJS 和 Go 比肩的极高性能（归功于 Starlette 和 Pydantic）。最快的 Python web 框架之一。
 * 高效编码：提高功能开发速度约 200％ 至 300％。*
```

### Comparing `pyva_framework-3.3.2/pyva/Application.py` & `pyva_framework-3.3.3/pyva/Application.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/Global.py` & `pyva_framework-3.3.3/pyva/Global.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/GlobalInit.py` & `pyva_framework-3.3.3/pyva/GlobalInit.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/cli/main.py` & `pyva_framework-3.3.3/pyva/cli/main.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkContactClient.py` & `pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkContactClient.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkOauth2Client.py` & `pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkOauth2Client.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkRobotClient.py` & `pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkRobotClient.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/client/dingtalk/DingtalkYidaClient.py` & `pyva_framework-3.3.3/pyva/client/dingtalk/DingtalkYidaClient.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/common/FastapiEvents.py` & `pyva_framework-3.3.3/pyva/common/FastapiEvents.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/common/FastapiException.py` & `pyva_framework-3.3.3/pyva/common/FastapiException.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/common/LoggerHandler.py` & `pyva_framework-3.3.3/pyva/common/LoggerHandler.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/config/AppConfig.py` & `pyva_framework-3.3.3/pyva/config/AppConfig.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,16 @@
     pyva AppConfig 应用配置类
 
     :version: 3.0.1
     :createdDate: 2020-02-11
     :updatedDate: 2022-10-03
     """
 
+    # 应用ID，即服务唯一标识
+    id: str = ""
     # 应用名，即服务注册名
     name: str = "pava-demo"
     # 应用标题
     title: str = "pyva Demo"
     # 应用描述
     description: str = "PyVa项目示例，基于FastAPI。"
     # 应用版本
@@ -32,7 +34,9 @@
     workers: int = 2
     # token有效秒数
     tokenExpire: int = 86400
     # log输出至钉钉
     log2dingtalk: bool = False
     # 安全模式：是否启用HTTPS
     https = False
+    # 访问限制Token
+    accessToken: str = ""
```

### Comparing `pyva_framework-3.3.2/pyva/config/DbConfig.py` & `pyva_framework-3.3.3/pyva/config/DbConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/config/DingtalkConfig.py` & `pyva_framework-3.3.3/pyva/config/DingtalkConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/config/FastapiConfig.py` & `pyva_framework-3.3.3/pyva/config/FastapiConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/config/LoggingConfig.py` & `pyva_framework-3.3.3/pyva/config/LoggingConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/config/NacosConfig.py` & `pyva_framework-3.3.3/pyva/config/NacosConfig.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/dao/BaseDao.py` & `pyva_framework-3.3.3/pyva/dao/BaseDao.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/dao/ListDao.py` & `pyva_framework-3.3.3/pyva/dao/ListDao.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/dto/BaseDto.py` & `pyva_framework-3.3.3/pyva/dto/BaseDto.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/dto/ListDto.py` & `pyva_framework-3.3.3/pyva/dto/ListDto.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/entity/BaseEntity.py` & `pyva_framework-3.3.3/pyva/entity/BaseEntity.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/entity/GeneralHumpEntity.py` & `pyva_framework-3.3.3/pyva/entity/GeneralHumpEntity.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/startupApp.py` & `pyva_framework-3.3.3/pyva/startupApp.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/ConfigUtil.py` & `pyva_framework-3.3.3/pyva/util/ConfigUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/DbUtil.py` & `pyva_framework-3.3.3/pyva/util/DbUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/DictUtil.py` & `pyva_framework-3.3.3/pyva/util/DictUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/EntityUtil.py` & `pyva_framework-3.3.3/pyva/util/EntityUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/FileUtil.py` & `pyva_framework-3.3.3/pyva/util/FileUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/IpUtil.py` & `pyva_framework-3.3.3/pyva/util/IpUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/JsonUtil.py` & `pyva_framework-3.3.3/pyva/util/JsonUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/LockerUtil.py` & `pyva_framework-3.3.3/pyva/util/LockerUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/MongoUtil.py` & `pyva_framework-3.3.3/pyva/util/MongoUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/NacosUtil.py` & `pyva_framework-3.3.3/pyva/util/NacosUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/PathUtil.py` & `pyva_framework-3.3.3/pyva/util/PathUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/QrcodeUtil.py` & `pyva_framework-3.3.3/pyva/util/QrcodeUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/RedisUtil.py` & `pyva_framework-3.3.3/pyva/util/RedisUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva/util/TimeUtil.py` & `pyva_framework-3.3.3/pyva/util/TimeUtil.py`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/pyva_framework.egg-info/PKG-INFO` & `pyva_framework-3.3.3/pyva_framework.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 Metadata-Version: 2.1
 Name: pyva-framework
-Version: 3.3.2
+Version: 3.3.3
 Summary: PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
 Home-page: https://github.com/zhenqiang-sun/pyva
 Author: Zhenqiang Sun
 Author-email: zhenqiang.sun@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: fastapi==0.104.1
-Requires-Dist: uvicorn==0.24.0
-Requires-Dist: SQLAlchemy==2.0.23
+Requires-Dist: fastapi==0.111.0
+Requires-Dist: uvicorn==0.29.0
+Requires-Dist: SQLAlchemy==2.0.30
 Requires-Dist: PyMySQL==1.1.0
 Requires-Dist: sqlacodegen==2.3.0
-Requires-Dist: redis==5.0.1
-Requires-Dist: requests==2.31.0
+Requires-Dist: redis==5.0.4
+Requires-Dist: requests==2.32.1
 Requires-Dist: pyhumps==3.8.0
 Requires-Dist: nacos-sdk-python==0.1.14
 Requires-Dist: PyYAML==6.0.1
-Requires-Dist: python-multipart==0.0.6
-Requires-Dist: pymongo==4.6.0
-Requires-Dist: orjson==3.9.10
+Requires-Dist: python-multipart==0.0.9
+Requires-Dist: pymongo==4.7.2
+Requires-Dist: orjson==3.10.3
 Requires-Dist: openpyxl==3.1.2
 Requires-Dist: deprecated==1.2.14
-Requires-Dist: jinja2==3.1.2
-Requires-Dist: typer[all]==0.9.0
+Requires-Dist: jinja2==3.1.4
+Requires-Dist: typer[all]==0.12.3
 Requires-Dist: py-ulid==1.0.3
 
 # PyVa
 PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。
 
 [Github: PyVa](https://github.com/zhenqiang-sun/pyva)
+[Gitee: PyVa](https://gitee.com/qiangai/pyva)
 
 ### 依赖组件：
 
 #### 1、FastAPI
 https://fastapi.tiangolo.com/
 * 快速：可与 NodeJS 和 Go 比肩的极高性能（归功于 Starlette 和 Pydantic）。最快的 Python web 框架之一。
 * 高效编码：提高功能开发速度约 200％ 至 300％。*
```

### Comparing `pyva_framework-3.3.2/pyva_framework.egg-info/SOURCES.txt` & `pyva_framework-3.3.3/pyva_framework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyva_framework-3.3.2/setup.py` & `pyva_framework-3.3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
     requirements = re.sub(r'(?m)#.*$', '', requirements)
 
 setuptools.setup(
     name="pyva-framework",
-    version="3.3.2",
+    version="3.3.3",
     author="Zhenqiang Sun",
     author_email="zhenqiang.sun@gmail.com",
     description="PyVa = Python项目 + Java风格，这是一个工程框架库，包含DB、Redis、MongoDB、JSON等工具和基础服务类。",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhenqiang-sun/pyva",
     packages=setuptools.find_packages(),
```

