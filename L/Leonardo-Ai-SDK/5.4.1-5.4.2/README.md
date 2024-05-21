# Comparing `tmp/Leonardo-Ai-SDK-5.4.1.tar.gz` & `tmp/Leonardo-Ai-SDK-5.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Leonardo-Ai-SDK-5.4.1.tar", last modified: Thu May 16 04:28:39 2024, max compression
+gzip compressed data, was "Leonardo-Ai-SDK-5.4.2.tar", last modified: Tue May 21 03:12:40 2024, max compression
```

## Comparing `Leonardo-Ai-SDK-5.4.1.tar` & `Leonardo-Ai-SDK-5.4.2.tar`

### file list

```diff
@@ -1,93 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:28:39.851511 Leonardo-Ai-SDK-5.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-16 04:28:39.851511 Leonardo-Ai-SDK-5.4.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     9922 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 04:28:39.851511 Leonardo-Ai-SDK-5.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:28:39.835511 Leonardo-Ai-SDK-5.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:28:39.839511 Leonardo-Ai-SDK-5.4.1/src/Leonardo_Ai_SDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-16 04:28:39.000000 Leonardo-Ai-SDK-5.4.1/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-16 04:28:39.000000 Leonardo-Ai-SDK-5.4.1/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 04:28:39.000000 Leonardo-Ai-SDK-5.4.1/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-16 04:28:39.000000 Leonardo-Ai-SDK-5.4.1/src/Leonardo_Ai_SDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-16 04:28:39.000000 Leonardo-Ai-SDK-5.4.1/src/Leonardo_Ai_SDK.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:28:39.839511 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:28:39.843511 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/element.py
--rw-r--r--   0 runner    (1001) docker     (127)    45413 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/initimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    27431 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:28:39.843511 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:28:39.843511 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:28:39.847511 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     6591 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15101 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/creategeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createlcmgeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createtexturegeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createvariationnobg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createvariationunzoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createvariationupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/deletedatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/deletegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/deletemodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/get3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getdatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getgenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getuserself.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getvariationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/listelements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/listplatformmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/performinpaintinglcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/performinstantrefine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/promptimprove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/promptrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/uploaddatasetimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/uploadinitimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/uploadmodelasset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:28:39.851511 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/controlnet_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/custom_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/lcm_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/model_asset_texture_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/sd_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/sd_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/strength.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/universal_upscaler_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/variation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 04:28:39.851511 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32647 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-05-16 04:28:29.000000 Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/variation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.922219 Leonardo-Ai-SDK-5.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16049 2024-05-21 03:12:40.922219 Leonardo-Ai-SDK-5.4.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10092 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 03:12:40.922219 Leonardo-Ai-SDK-5.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.910219 Leonardo-Ai-SDK-5.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.910219 Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16049 2024-05-21 03:12:40.000000 Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-21 03:12:40.000000 Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 03:12:40.000000 Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-21 03:12:40.000000 Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 03:12:40.000000 Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.914219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.914219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17541 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45413 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10155 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/initimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27431 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.914219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.914219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.922219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7196 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15102 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/creategeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createlcmgeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createtexturegeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4351 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createvariationnobg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createvariationunzoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createvariationupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletedatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletemodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/get3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getdatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getgenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getuserself.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getvariationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/listelements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/listplatformmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/performinpaintinglcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/performinstantrefine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13322 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/pricingcalculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/promptimprove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/promptrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploaddatasetimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploadinitimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploadmodelasset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.922219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/controlnet_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/custom_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/lcm_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/model_asset_texture_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/pricingcalculatorservices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/sd_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/sd_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/strength.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/universal_upscaler_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/variation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3977 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/pricing_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6869 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 03:12:40.922219 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32647 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17499 2024-05-21 03:12:33.000000 Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/variation.py
```

### Comparing `Leonardo-Ai-SDK-5.4.1/LICENSE.md` & `Leonardo-Ai-SDK-5.4.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/PKG-INFO` & `Leonardo-Ai-SDK-5.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.4.1
+Version: 5.4.2
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
@@ -89,14 +89,18 @@
         * [delete_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#delete_model_by_id) - Delete a Single Custom Model by ID
         * [get3_d_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#get3_d_model_by_id) - Get 3D Model by ID
         * [get3_d_models_by_user_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#get3_d_models_by_user_id) - Get 3D models by user ID
         * [get_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#get_model_by_id) - Get a Single Custom Model by ID
         * [list_platform_models](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#list_platform_models) - List Platform Models
         * [upload_model_asset](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#upload_model_asset) - Upload 3D Model
         
+        ### [pricing_calculator](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/pricingcalculator/README.md)
+        
+        * [pricing_calculator](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/pricingcalculator/README.md#pricing_calculator) - Calculating API Cost
+        
         ### [prompt](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md)
         
         * [prompt_improve](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_improve) - Improve a Prompt
         * [prompt_random](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_random) - Generate a Random prompt
         
         ### [variation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.4.1 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.4.2 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) res = s.dataset.create_dataset
 (request=operations.CreateDatasetRequestBody( name='', )) if res.object is not
@@ -89,24 +89,28 @@
 sdks/model/README.md#get3_d_models_by_user_id) - Get 3D models by user ID *
 [get_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/
 blob/master/docs/sdks/model/README.md#get_model_by_id) - Get a Single Custom
 Model by ID * [list_platform_models](https://github.com/Leonardo-Interactive/
 leonardo-python-sdk/blob/master/docs/sdks/model/README.md#list_platform_models)
 - List Platform Models * [upload_model_asset](https://github.com/Leonardo-
 Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/
-README.md#upload_model_asset) - Upload 3D Model ### [prompt](https://
+README.md#upload_model_asset) - Upload 3D Model ### [pricing_calculator](https:
+//github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
+pricingcalculator/README.md) * [pricing_calculator](https://github.com/
+Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
+pricingcalculator/README.md#pricing_calculator) - Calculating API Cost ###
+[prompt](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/
+master/docs/sdks/prompt/README.md) * [prompt_improve](https://github.com/
+Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/
+README.md#prompt_improve) - Improve a Prompt * [prompt_random](https://
 github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-prompt/README.md) * [prompt_improve](https://github.com/Leonardo-Interactive/
-leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_improve) -
-Improve a Prompt * [prompt_random](https://github.com/Leonardo-Interactive/
-leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_random) -
-Generate a Random prompt ### [variation](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md) *
-[create_universal_upscaler_job](https://github.com/Leonardo-Interactive/
-leonardo-python-sdk/blob/master/docs/sdks/variation/
+prompt/README.md#prompt_random) - Generate a Random prompt ### [variation]
+(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
+sdks/variation/README.md) * [create_universal_upscaler_job](https://github.com/
+Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/
 README.md#create_universal_upscaler_job) - Create using Universal Upscaler *
 [create_variation_no_bg](https://github.com/Leonardo-Interactive/leonardo-
 python-sdk/blob/master/docs/sdks/variation/README.md#create_variation_no_bg) -
 Create no background * [create_variation_unzoom](https://github.com/Leonardo-
 Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/
 README.md#create_variation_unzoom) - Create unzoom * [create_variation_upscale]
 (https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
```

### Comparing `Leonardo-Ai-SDK-5.4.1/README.md` & `Leonardo-Ai-SDK-5.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -82,14 +82,18 @@
 * [delete_model_by_id](docs/sdks/model/README.md#delete_model_by_id) - Delete a Single Custom Model by ID
 * [get3_d_model_by_id](docs/sdks/model/README.md#get3_d_model_by_id) - Get 3D Model by ID
 * [get3_d_models_by_user_id](docs/sdks/model/README.md#get3_d_models_by_user_id) - Get 3D models by user ID
 * [get_model_by_id](docs/sdks/model/README.md#get_model_by_id) - Get a Single Custom Model by ID
 * [list_platform_models](docs/sdks/model/README.md#list_platform_models) - List Platform Models
 * [upload_model_asset](docs/sdks/model/README.md#upload_model_asset) - Upload 3D Model
 
+### [pricing_calculator](docs/sdks/pricingcalculator/README.md)
+
+* [pricing_calculator](docs/sdks/pricingcalculator/README.md#pricing_calculator) - Calculating API Cost
+
 ### [prompt](docs/sdks/prompt/README.md)
 
 * [prompt_improve](docs/sdks/prompt/README.md#prompt_improve) - Improve a Prompt
 * [prompt_random](docs/sdks/prompt/README.md#prompt_random) - Generate a Random prompt
 
 ### [variation](docs/sdks/variation/README.md)
```

#### html2text {}

```diff
@@ -50,23 +50,25 @@
 (docs/sdks/model/README.md#delete_model_by_id) - Delete a Single Custom Model
 by ID * [get3_d_model_by_id](docs/sdks/model/README.md#get3_d_model_by_id) -
 Get 3D Model by ID * [get3_d_models_by_user_id](docs/sdks/model/
 README.md#get3_d_models_by_user_id) - Get 3D models by user ID *
 [get_model_by_id](docs/sdks/model/README.md#get_model_by_id) - Get a Single
 Custom Model by ID * [list_platform_models](docs/sdks/model/
 README.md#list_platform_models) - List Platform Models * [upload_model_asset]
-(docs/sdks/model/README.md#upload_model_asset) - Upload 3D Model ### [prompt]
-(docs/sdks/prompt/README.md) * [prompt_improve](docs/sdks/prompt/
-README.md#prompt_improve) - Improve a Prompt * [prompt_random](docs/sdks/
-prompt/README.md#prompt_random) - Generate a Random prompt ### [variation]
-(docs/sdks/variation/README.md) * [create_universal_upscaler_job](docs/sdks/
-variation/README.md#create_universal_upscaler_job) - Create using Universal
-Upscaler * [create_variation_no_bg](docs/sdks/variation/
-README.md#create_variation_no_bg) - Create no background *
-[create_variation_unzoom](docs/sdks/variation/
+(docs/sdks/model/README.md#upload_model_asset) - Upload 3D Model ###
+[pricing_calculator](docs/sdks/pricingcalculator/README.md) *
+[pricing_calculator](docs/sdks/pricingcalculator/README.md#pricing_calculator)
+- Calculating API Cost ### [prompt](docs/sdks/prompt/README.md) *
+[prompt_improve](docs/sdks/prompt/README.md#prompt_improve) - Improve a Prompt
+* [prompt_random](docs/sdks/prompt/README.md#prompt_random) - Generate a Random
+prompt ### [variation](docs/sdks/variation/README.md) *
+[create_universal_upscaler_job](docs/sdks/variation/
+README.md#create_universal_upscaler_job) - Create using Universal Upscaler *
+[create_variation_no_bg](docs/sdks/variation/README.md#create_variation_no_bg)
+- Create no background * [create_variation_unzoom](docs/sdks/variation/
 README.md#create_variation_unzoom) - Create unzoom * [create_variation_upscale]
 (docs/sdks/variation/README.md#create_variation_upscale) - Create upscale *
 [get_variation_by_id](docs/sdks/variation/README.md#get_variation_by_id) - Get
 variation by ID ## Error Handling Handling errors in this SDK should largely
 match your expectations. All operations return a response object or raise an
 error. If Error objects are specified in your OpenAPI Spec, the SDK will raise
 the appropriate Error type. | Error Object | Status Code | Content Type | | ---
```

### Comparing `Leonardo-Ai-SDK-5.4.1/setup.py` & `Leonardo-Ai-SDK-5.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='Leonardo-Ai-SDK',
-    version='5.4.1',
+    version='5.4.2',
     author='Leonardo-Ai',
     description='Leonardo AI Python Client SDK',
     url='https://github.com/Leonardo-Interactive/leonardo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `Leonardo-Ai-SDK-5.4.1/src/Leonardo_Ai_SDK.egg-info/PKG-INFO` & `Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.4.1
+Version: 5.4.2
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
@@ -89,14 +89,18 @@
         * [delete_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#delete_model_by_id) - Delete a Single Custom Model by ID
         * [get3_d_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#get3_d_model_by_id) - Get 3D Model by ID
         * [get3_d_models_by_user_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#get3_d_models_by_user_id) - Get 3D models by user ID
         * [get_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#get_model_by_id) - Get a Single Custom Model by ID
         * [list_platform_models](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#list_platform_models) - List Platform Models
         * [upload_model_asset](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/README.md#upload_model_asset) - Upload 3D Model
         
+        ### [pricing_calculator](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/pricingcalculator/README.md)
+        
+        * [pricing_calculator](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/pricingcalculator/README.md#pricing_calculator) - Calculating API Cost
+        
         ### [prompt](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md)
         
         * [prompt_improve](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_improve) - Improve a Prompt
         * [prompt_random](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_random) - Generate a Random prompt
         
         ### [variation](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.4.1 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.4.2 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) res = s.dataset.create_dataset
 (request=operations.CreateDatasetRequestBody( name='', )) if res.object is not
@@ -89,24 +89,28 @@
 sdks/model/README.md#get3_d_models_by_user_id) - Get 3D models by user ID *
 [get_model_by_id](https://github.com/Leonardo-Interactive/leonardo-python-sdk/
 blob/master/docs/sdks/model/README.md#get_model_by_id) - Get a Single Custom
 Model by ID * [list_platform_models](https://github.com/Leonardo-Interactive/
 leonardo-python-sdk/blob/master/docs/sdks/model/README.md#list_platform_models)
 - List Platform Models * [upload_model_asset](https://github.com/Leonardo-
 Interactive/leonardo-python-sdk/blob/master/docs/sdks/model/
-README.md#upload_model_asset) - Upload 3D Model ### [prompt](https://
+README.md#upload_model_asset) - Upload 3D Model ### [pricing_calculator](https:
+//github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
+pricingcalculator/README.md) * [pricing_calculator](https://github.com/
+Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
+pricingcalculator/README.md#pricing_calculator) - Calculating API Cost ###
+[prompt](https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/
+master/docs/sdks/prompt/README.md) * [prompt_improve](https://github.com/
+Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/prompt/
+README.md#prompt_improve) - Improve a Prompt * [prompt_random](https://
 github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/
-prompt/README.md) * [prompt_improve](https://github.com/Leonardo-Interactive/
-leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_improve) -
-Improve a Prompt * [prompt_random](https://github.com/Leonardo-Interactive/
-leonardo-python-sdk/blob/master/docs/sdks/prompt/README.md#prompt_random) -
-Generate a Random prompt ### [variation](https://github.com/Leonardo-
-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/README.md) *
-[create_universal_upscaler_job](https://github.com/Leonardo-Interactive/
-leonardo-python-sdk/blob/master/docs/sdks/variation/
+prompt/README.md#prompt_random) - Generate a Random prompt ### [variation]
+(https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
+sdks/variation/README.md) * [create_universal_upscaler_job](https://github.com/
+Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/
 README.md#create_universal_upscaler_job) - Create using Universal Upscaler *
 [create_variation_no_bg](https://github.com/Leonardo-Interactive/leonardo-
 python-sdk/blob/master/docs/sdks/variation/README.md#create_variation_no_bg) -
 Create no background * [create_variation_unzoom](https://github.com/Leonardo-
 Interactive/leonardo-python-sdk/blob/master/docs/sdks/variation/
 README.md#create_variation_unzoom) - Create unzoom * [create_variation_upscale]
 (https://github.com/Leonardo-Interactive/leonardo-python-sdk/blob/master/docs/
```

### Comparing `Leonardo-Ai-SDK-5.4.1/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt` & `Leonardo-Ai-SDK-5.4.2/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 src/Leonardo_Ai_SDK.egg-info/top_level.txt
 src/leonardoaisdk/__init__.py
 src/leonardoaisdk/dataset.py
 src/leonardoaisdk/element.py
 src/leonardoaisdk/generation.py
 src/leonardoaisdk/initimage.py
 src/leonardoaisdk/model.py
+src/leonardoaisdk/pricing_calculator.py
 src/leonardoaisdk/prompt.py
 src/leonardoaisdk/sdk.py
 src/leonardoaisdk/sdkconfiguration.py
 src/leonardoaisdk/user.py
 src/leonardoaisdk/variation.py
 src/leonardoaisdk/_hooks/__init__.py
 src/leonardoaisdk/_hooks/sdkhooks.py
@@ -52,27 +53,29 @@
 src/leonardoaisdk/models/operations/getuserself.py
 src/leonardoaisdk/models/operations/getvariationbyid.py
 src/leonardoaisdk/models/operations/listelements.py
 src/leonardoaisdk/models/operations/listplatformmodels.py
 src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
 src/leonardoaisdk/models/operations/performinpaintinglcm.py
 src/leonardoaisdk/models/operations/performinstantrefine.py
+src/leonardoaisdk/models/operations/pricingcalculator.py
 src/leonardoaisdk/models/operations/promptimprove.py
 src/leonardoaisdk/models/operations/promptrandom.py
 src/leonardoaisdk/models/operations/uploaddatasetimage.py
 src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
 src/leonardoaisdk/models/operations/uploadinitimage.py
 src/leonardoaisdk/models/operations/uploadmodelasset.py
 src/leonardoaisdk/models/shared/__init__.py
 src/leonardoaisdk/models/shared/controlnet_type.py
 src/leonardoaisdk/models/shared/custom_model_type.py
 src/leonardoaisdk/models/shared/element_input.py
 src/leonardoaisdk/models/shared/job_status.py
 src/leonardoaisdk/models/shared/lcm_generation_style.py
 src/leonardoaisdk/models/shared/model_asset_texture_types.py
+src/leonardoaisdk/models/shared/pricingcalculatorservices.py
 src/leonardoaisdk/models/shared/sd_generation_schedulers.py
 src/leonardoaisdk/models/shared/sd_generation_style.py
 src/leonardoaisdk/models/shared/sd_versions.py
 src/leonardoaisdk/models/shared/security.py
 src/leonardoaisdk/models/shared/strength.py
 src/leonardoaisdk/models/shared/universal_upscaler_style.py
 src/leonardoaisdk/models/shared/variation_type.py
```

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/_hooks/sdkhooks.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/_hooks/types.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/dataset.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/dataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/element.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/element.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/generation.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/generation.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/initimage.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/initimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/model.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/model.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/errors/sdkerror.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/__init__.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,16 @@
 from .getuserself import *
 from .getvariationbyid import *
 from .listelements import *
 from .listplatformmodels import *
 from .performalchemyupscalelcm import *
 from .performinpaintinglcm import *
 from .performinstantrefine import *
+from .pricingcalculator import *
 from .promptimprove import *
 from .promptrandom import *
 from .uploaddatasetimage import *
 from .uploaddatasetimagefromgen import *
 from .uploadinitimage import *
 from .uploadmodelasset import *
 
-__all__ = ["CreateDatasetRequestBody","CreateDatasetResponse","CreateDatasetResponseBody","CreateGenerationRequestBody","CreateGenerationResponse","CreateGenerationResponseBody","CreateLCMGenerationRequestBody","CreateLCMGenerationResponse","CreateLCMGenerationResponseBody","CreateModelRequestBody","CreateModelResponse","CreateModelResponseBody","CreateSVDMotionGenerationRequestBody","CreateSVDMotionGenerationResponse","CreateSVDMotionGenerationResponseBody","CreateTextureGenerationRequestBody","CreateTextureGenerationResponse","CreateTextureGenerationResponseBody","CreateUniversalUpscalerJobRequestBody","CreateUniversalUpscalerJobResponse","CreateUniversalUpscalerJobResponseBody","CreateVariationNoBGRequestBody","CreateVariationNoBGResponse","CreateVariationNoBGResponseBody","CreateVariationUnzoomRequestBody","CreateVariationUnzoomResponse","CreateVariationUnzoomResponseBody","CreateVariationUpscaleRequestBody","CreateVariationUpscaleResponse","CreateVariationUpscaleResponseBody","CreateVariationUpscaleSDUpscaleJobOutput","CustomModels","DatasetGenUploadOutput","DatasetImages","DatasetUploadOutput","Datasets","Delete3DModelByIDRequest","Delete3DModelByIDRequestBody","Delete3DModelByIDResponse","Delete3DModelByIDResponseBody","DeleteDatasetByIDDatasets","DeleteDatasetByIDRequest","DeleteDatasetByIDResponse","DeleteDatasetByIDResponseBody","DeleteGenerationByIDRequest","DeleteGenerationByIDResponse","DeleteGenerationByIDResponseBody","DeleteInitImageByIDRequest","DeleteInitImageByIDResponse","DeleteInitImageByIDResponseBody","DeleteModelByIDRequest","DeleteModelByIDResponse","DeleteModelByIDResponseBody","DeleteTextureGenerationByIDRequest","DeleteTextureGenerationByIDRequestBody","DeleteTextureGenerationByIDResponse","DeleteTextureGenerationByIDResponseBody","Elements","GeneratedImageVariationGeneric","GeneratedImages","GenerationElements","Generations","Get3DModelByIDModelAssets","Get3DModelByIDRequest","Get3DModelByIDRequestBody","Get3DModelByIDResponse","Get3DModelByIDResponseBody","Get3DModelsByUserIDModelAssets","Get3DModelsByUserIDRequest","Get3DModelsByUserIDRequestBody","Get3DModelsByUserIDResponse","Get3DModelsByUserIDResponseBody","GetDatasetByIDDatasets","GetDatasetByIDRequest","GetDatasetByIDResponse","GetDatasetByIDResponseBody","GetGenerationByIDGeneratedImageVariationGeneric","GetGenerationByIDGenerations","GetGenerationByIDLoras","GetGenerationByIDRequest","GetGenerationByIDResponse","GetGenerationByIDResponseBody","GetGenerationsByUserIDGeneratedImageVariationGeneric","GetGenerationsByUserIDGeneratedImages","GetGenerationsByUserIDGenerationElements","GetGenerationsByUserIDGenerations","GetGenerationsByUserIDRequest","GetGenerationsByUserIDResponse","GetGenerationsByUserIDResponseBody","GetInitImageByIDInitImages","GetInitImageByIDRequest","GetInitImageByIDResponse","GetInitImageByIDResponseBody","GetModelByIDCustomModels","GetModelByIDRequest","GetModelByIDResponse","GetModelByIDResponseBody","GetTextureGenerationByIDModelAssetTextureGenerations","GetTextureGenerationByIDRequest","GetTextureGenerationByIDRequestBody","GetTextureGenerationByIDResponse","GetTextureGenerationByIDResponseBody","GetTextureGenerationsByModelIDModelAssetTextureGenerations","GetTextureGenerationsByModelIDModelAssetTextureImages","GetTextureGenerationsByModelIDRequest","GetTextureGenerationsByModelIDRequestBody","GetTextureGenerationsByModelIDResponse","GetTextureGenerationsByModelIDResponseBody","GetUserSelfResponse","GetUserSelfResponseBody","GetVariationByIDRequest","GetVariationByIDResponse","GetVariationByIDResponseBody","InitImageUploadOutput","InitImages","LcmGenerationOutput","ListElementsResponse","ListElementsResponseBody","ListPlatformModelsCustomModels","ListPlatformModelsGeneratedImages","ListPlatformModelsResponse","ListPlatformModelsResponseBody","Loras","ModelAssetTextureGenerations","ModelAssetTextureImages","ModelAssetUploadOutput","ModelAssets","MotionSvdGenerationOutput","PerformAlchemyUpscaleLCMLCMGenerationOutput","PerformAlchemyUpscaleLCMRequestBody","PerformAlchemyUpscaleLCMResponse","PerformAlchemyUpscaleLCMResponseBody","PerformInpaintingLCMLCMGenerationOutput","PerformInpaintingLCMRequestBody","PerformInpaintingLCMResponse","PerformInpaintingLCMResponseBody","PerformInstantRefineLcmGenerationOutput","PerformInstantRefineRequestBody","PerformInstantRefineResponse","PerformInstantRefineResponseBody","PromptGenerationOutput","PromptImproveRequestBody","PromptImproveResponse","PromptImproveResponseBody","PromptRandomPromptGenerationOutput","PromptRandomResponse","PromptRandomResponseBody","SDGenerationOutput","SDTrainingOutput","SDUnzoomOutput","SDUpscaleJobOutput","TextureGenerationJobOutput","TransparencyType","UniversalUpscalerOutput","UploadDatasetImageFromGenRequest","UploadDatasetImageFromGenRequestBody","UploadDatasetImageFromGenResponse","UploadDatasetImageFromGenResponseBody","UploadDatasetImageRequest","UploadDatasetImageRequestBody","UploadDatasetImageResponse","UploadDatasetImageResponseBody","UploadInitImageRequestBody","UploadInitImageResponse","UploadInitImageResponseBody","UploadModelAssetRequestBody","UploadModelAssetResponse","UploadModelAssetResponseBody","UserDetails","Users"]
+__all__ = ["CalculateProductionAPIServiceCost","CreateDatasetRequestBody","CreateDatasetResponse","CreateDatasetResponseBody","CreateGenerationRequestBody","CreateGenerationResponse","CreateGenerationResponseBody","CreateLCMGenerationRequestBody","CreateLCMGenerationResponse","CreateLCMGenerationResponseBody","CreateModelRequestBody","CreateModelResponse","CreateModelResponseBody","CreateSVDMotionGenerationRequestBody","CreateSVDMotionGenerationResponse","CreateSVDMotionGenerationResponseBody","CreateTextureGenerationRequestBody","CreateTextureGenerationResponse","CreateTextureGenerationResponseBody","CreateUniversalUpscalerJobRequestBody","CreateUniversalUpscalerJobResponse","CreateUniversalUpscalerJobResponseBody","CreateVariationNoBGRequestBody","CreateVariationNoBGResponse","CreateVariationNoBGResponseBody","CreateVariationUnzoomRequestBody","CreateVariationUnzoomResponse","CreateVariationUnzoomResponseBody","CreateVariationUpscaleRequestBody","CreateVariationUpscaleResponse","CreateVariationUpscaleResponseBody","CreateVariationUpscaleSDUpscaleJobOutput","CustomModels","DatasetGenUploadOutput","DatasetImages","DatasetUploadOutput","Datasets","Delete3DModelByIDRequest","Delete3DModelByIDRequestBody","Delete3DModelByIDResponse","Delete3DModelByIDResponseBody","DeleteDatasetByIDDatasets","DeleteDatasetByIDRequest","DeleteDatasetByIDResponse","DeleteDatasetByIDResponseBody","DeleteGenerationByIDRequest","DeleteGenerationByIDResponse","DeleteGenerationByIDResponseBody","DeleteInitImageByIDRequest","DeleteInitImageByIDResponse","DeleteInitImageByIDResponseBody","DeleteModelByIDRequest","DeleteModelByIDResponse","DeleteModelByIDResponseBody","DeleteTextureGenerationByIDRequest","DeleteTextureGenerationByIDRequestBody","DeleteTextureGenerationByIDResponse","DeleteTextureGenerationByIDResponseBody","Elements","GeneratedImageVariationGeneric","GeneratedImages","GenerationElements","Generations","Get3DModelByIDModelAssets","Get3DModelByIDRequest","Get3DModelByIDRequestBody","Get3DModelByIDResponse","Get3DModelByIDResponseBody","Get3DModelsByUserIDModelAssets","Get3DModelsByUserIDRequest","Get3DModelsByUserIDRequestBody","Get3DModelsByUserIDResponse","Get3DModelsByUserIDResponseBody","GetDatasetByIDDatasets","GetDatasetByIDRequest","GetDatasetByIDResponse","GetDatasetByIDResponseBody","GetGenerationByIDGeneratedImageVariationGeneric","GetGenerationByIDGenerations","GetGenerationByIDLoras","GetGenerationByIDRequest","GetGenerationByIDResponse","GetGenerationByIDResponseBody","GetGenerationsByUserIDGeneratedImageVariationGeneric","GetGenerationsByUserIDGeneratedImages","GetGenerationsByUserIDGenerationElements","GetGenerationsByUserIDGenerations","GetGenerationsByUserIDRequest","GetGenerationsByUserIDResponse","GetGenerationsByUserIDResponseBody","GetInitImageByIDInitImages","GetInitImageByIDRequest","GetInitImageByIDResponse","GetInitImageByIDResponseBody","GetModelByIDCustomModels","GetModelByIDRequest","GetModelByIDResponse","GetModelByIDResponseBody","GetTextureGenerationByIDModelAssetTextureGenerations","GetTextureGenerationByIDRequest","GetTextureGenerationByIDRequestBody","GetTextureGenerationByIDResponse","GetTextureGenerationByIDResponseBody","GetTextureGenerationsByModelIDModelAssetTextureGenerations","GetTextureGenerationsByModelIDModelAssetTextureImages","GetTextureGenerationsByModelIDRequest","GetTextureGenerationsByModelIDRequestBody","GetTextureGenerationsByModelIDResponse","GetTextureGenerationsByModelIDResponseBody","GetUserSelfResponse","GetUserSelfResponseBody","GetVariationByIDRequest","GetVariationByIDResponse","GetVariationByIDResponseBody","InitImageUploadOutput","InitImages","LcmGenerationOutput","ListElementsResponse","ListElementsResponseBody","ListPlatformModelsCustomModels","ListPlatformModelsGeneratedImages","ListPlatformModelsResponse","ListPlatformModelsResponseBody","Loras","ModelAssetTextureGenerations","ModelAssetTextureImages","ModelAssetUploadOutput","ModelAssets","MotionSvdGenerationOutput","Object","PerformAlchemyUpscaleLCMLCMGenerationOutput","PerformAlchemyUpscaleLCMRequestBody","PerformAlchemyUpscaleLCMResponse","PerformAlchemyUpscaleLCMResponseBody","PerformInpaintingLCMLCMGenerationOutput","PerformInpaintingLCMRequestBody","PerformInpaintingLCMResponse","PerformInpaintingLCMResponseBody","PerformInstantRefineLcmGenerationOutput","PerformInstantRefineRequestBody","PerformInstantRefineResponse","PerformInstantRefineResponseBody","PricingCalculatorObject","PricingCalculatorPricingCalculatorObject","PricingCalculatorPricingCalculatorRequestObject","PricingCalculatorPricingCalculatorRequestRequestBodyObject","PricingCalculatorPricingCalculatorRequestRequestBodyServiceParamsObject","PricingCalculatorPricingCalculatorRequestRequestBodyServiceParamsTEXTUREGENERATIONObject","PricingCalculatorPricingCalculatorRequestRequestBodyServiceParamsUNIVERSALUPSCALERObject","PricingCalculatorRequestBody","PricingCalculatorResponse","PricingCalculatorResponseBody","PromptGenerationOutput","PromptImproveRequestBody","PromptImproveResponse","PromptImproveResponseBody","PromptRandomPromptGenerationOutput","PromptRandomResponse","PromptRandomResponseBody","SDGenerationOutput","SDTrainingOutput","SDUnzoomOutput","SDUpscaleJobOutput","TextureGenerationJobOutput","TransparencyType","UniversalUpscalerOutput","UploadDatasetImageFromGenRequest","UploadDatasetImageFromGenRequestBody","UploadDatasetImageFromGenResponse","UploadDatasetImageFromGenResponseBody","UploadDatasetImageRequest","UploadDatasetImageRequestBody","UploadDatasetImageResponse","UploadDatasetImageResponseBody","UploadInitImageRequestBody","UploadInitImageResponse","UploadInitImageResponseBody","UploadModelAssetRequestBody","UploadModelAssetResponse","UploadModelAssetResponseBody","UserDetails","Users"]
```

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createdataset.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createdataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/creategeneration.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/creategeneration.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from ...models.shared import sd_generation_style as shared_sd_generation_style
 from ...models.shared import sd_versions as shared_sd_versions
 from dataclasses_json import Undefined, dataclass_json
 from enum import Enum
 from leonardoaisdk import utils
 from typing import List, Optional
 
+
 class TransparencyType(str, Enum):
     r"""Which type of transparency this image should use"""
     DISABLED = 'disabled'
     FOREGROUND_ONLY = 'foreground_only'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
```

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createlcmgeneration.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createlcmgeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createmodel.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createmodel.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createtexturegeneration.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createtexturegeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createuniversalupscalerjob.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createvariationnobg.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createvariationnobg.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createvariationunzoom.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createvariationunzoom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/createvariationupscale.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/createvariationupscale.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/delete3dmodelbyid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/delete3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/deletedatasetbyid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletedatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/deletegenerationbyid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/deleteinitimagebyid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deleteinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/deletemodelbyid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletemodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/get3dmodelbyid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/get3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getdatasetbyid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getdatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getgenerationbyid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getgenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getinitimagebyid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getmodelbyid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getuserself.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getuserself.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/getvariationbyid.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/getvariationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/listelements.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/listelements.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/listplatformmodels.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/listplatformmodels.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/performinpaintinglcm.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/performinpaintinglcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/performinstantrefine.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/performinstantrefine.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/promptimprove.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/promptimprove.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/promptrandom.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/promptrandom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/uploaddatasetimage.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploaddatasetimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/uploadinitimage.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploadinitimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/operations/uploadmodelasset.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/operations/uploadmodelasset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/__init__.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 
 from .controlnet_type import *
 from .custom_model_type import *
 from .element_input import *
 from .job_status import *
 from .lcm_generation_style import *
 from .model_asset_texture_types import *
+from .pricingcalculatorservices import *
 from .sd_generation_schedulers import *
 from .sd_generation_style import *
 from .sd_versions import *
 from .security import *
 from .strength import *
 from .universal_upscaler_style import *
 from .variation_type import *
 
-__all__ = ["ControlnetType","CustomModelType","ElementInput","JobStatus","LcmGenerationStyle","ModelAssetTextureTypes","SdGenerationSchedulers","SdGenerationStyle","SdVersions","Security","Strength","UniversalUpscalerStyle","VariationType"]
+__all__ = ["ControlnetType","CustomModelType","ElementInput","JobStatus","LcmGenerationStyle","ModelAssetTextureTypes","PricingCalculatorServices","SdGenerationSchedulers","SdGenerationStyle","SdVersions","Security","Strength","UniversalUpscalerStyle","VariationType"]
```

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/custom_model_type.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/custom_model_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class CustomModelType(str, Enum):
     r"""The category the most accurately reflects the model."""
     GENERAL = 'GENERAL'
     BUILDINGS = 'BUILDINGS'
     CHARACTERS = 'CHARACTERS'
     ENVIRONMENTS = 'ENVIRONMENTS'
     FASHION = 'FASHION'
```

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/element_input.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/element_input.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/lcm_generation_style.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/lcm_generation_style.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class LcmGenerationStyle(str, Enum):
     r"""The style to generate LCM images with."""
     ANIME = 'ANIME'
     CINEMATIC = 'CINEMATIC'
     DIGITAL_ART = 'DIGITAL_ART'
     DYNAMIC = 'DYNAMIC'
     ENVIRONMENT = 'ENVIRONMENT'
```

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/sd_generation_style.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/sd_generation_style.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class SdGenerationStyle(str, Enum):
     r"""The style to generate images with. When photoReal is enabled, refer to the Guide section for a full list. When alchemy is disabled, use LEONARDO or NONE. When alchemy is enabled, use ANIME, CREATIVE, DYNAMIC, ENVIRONMENT, GENERAL, ILLUSTRATION, PHOTOGRAPHY, RAYTRACED, RENDER_3D, SKETCH_BW, SKETCH_COLOR, or NONE."""
     ANIME = 'ANIME'
     BOKEH = 'BOKEH'
     CINEMATIC = 'CINEMATIC'
     CINEMATIC_CLOSEUP = 'CINEMATIC_CLOSEUP'
     CREATIVE = 'CREATIVE'
```

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/models/shared/sd_versions.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/models/shared/sd_versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 from enum import Enum
 
+
 class SdVersions(str, Enum):
     r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5. Also includes SDXL and SDXL Lightning models"""
     V1_5 = 'v1_5'
     V2 = 'v2'
     V3 = 'v3'
     SDXL_0_8 = 'SDXL_0_8'
     SDXL_0_9 = 'SDXL_0_9'
```

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/prompt.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/prompt.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/sdk.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/sdk.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import requests as requests_http
 from .dataset import Dataset
 from .element import Element
 from .generation import Generation
 from .initimage import InitImage
 from .model import Model
+from .pricing_calculator import PricingCalculator
 from .prompt import Prompt
 from .sdkconfiguration import SDKConfiguration
 from .user import User
 from .utils.retries import RetryConfig
 from .variation import Variation
 from leonardoaisdk import utils
 from leonardoaisdk._hooks import SDKHooks
@@ -20,14 +21,15 @@
     r"""Rest Endpoints: Leonardo.Ai API OpenAPI specification."""
     dataset: Dataset
     element: Element
     generation: Generation
     init_image: InitImage
     user: User
     model: Model
+    pricing_calculator: PricingCalculator
     prompt: Prompt
     variation: Variation
 
     sdk_configuration: SDKConfiguration
 
     def __init__(self,
                  bearer_auth: Union[str, Callable[[], str]],
@@ -90,9 +92,10 @@
     def _init_sdks(self):
         self.dataset = Dataset(self.sdk_configuration)
         self.element = Element(self.sdk_configuration)
         self.generation = Generation(self.sdk_configuration)
         self.init_image = InitImage(self.sdk_configuration)
         self.user = User(self.sdk_configuration)
         self.model = Model(self.sdk_configuration)
+        self.pricing_calculator = PricingCalculator(self.sdk_configuration)
         self.prompt = Prompt(self.sdk_configuration)
         self.variation = Variation(self.sdk_configuration)
```

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/sdkconfiguration.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/sdkconfiguration.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = 'v1.0.0'
-    sdk_version: str = '5.4.1'
-    gen_version: str = '2.326.3'
-    user_agent: str = 'speakeasy-sdk/python 5.4.1 2.326.3 v1.0.0 Leonardo-Ai-SDK'
+    sdk_version: str = '5.4.2'
+    gen_version: str = '2.332.4'
+    user_agent: str = 'speakeasy-sdk/python 5.4.2 2.332.4 v1.0.0 Leonardo-Ai-SDK'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/user.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/user.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/utils/retries.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/utils/utils.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.4.1/src/leonardoaisdk/variation.py` & `Leonardo-Ai-SDK-5.4.2/src/leonardoaisdk/variation.py`

 * *Files identical despite different names*

