# Comparing `tmp/alibabacloud_umeng-apm20220214-1.1.2.tar.gz` & `tmp/alibabacloud_umeng-apm20220214-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/alibabacloud_umeng-apm20220214-1.1.2.tar", last modified: Wed Apr 10 07:15:00 2024, max compression
+gzip compressed data, was "dist/alibabacloud_umeng-apm20220214-1.1.3.tar", last modified: Tue May 21 07:22:20 2024, max compression
```

## Comparing `alibabacloud_umeng-apm20220214-1.1.2.tar` & `alibabacloud_umeng-apm20220214-1.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/
--rw-r--r--   0 root         (0) root         (0)      621 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/ChangeLog.md
--rw-r--r--   0 root         (0) root         (0)      600 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2443 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1119 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1204 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214/
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41744 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214/client.py
--rw-r--r--   0 root         (0) root         (0)    57230 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214/models.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2443 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      468 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      316 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2834 2024-04-10 07:15:00.000000 alibabacloud_umeng-apm20220214-1.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/
+-rw-r--r--   0 root         (0) root         (0)      704 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/ChangeLog.md
+-rw-r--r--   0 root         (0) root         (0)      600 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1119 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1204 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/alibabacloud_umeng_apm20220214/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/alibabacloud_umeng_apm20220214/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49722 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/alibabacloud_umeng_apm20220214/client.py
+-rw-r--r--   0 root         (0) root         (0)    58560 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/alibabacloud_umeng_apm20220214/models.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/alibabacloud_umeng_apm20220214.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2443 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/alibabacloud_umeng_apm20220214.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      468 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/alibabacloud_umeng_apm20220214.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/alibabacloud_umeng_apm20220214.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      316 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/alibabacloud_umeng_apm20220214.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/alibabacloud_umeng_apm20220214.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2834 2024-05-21 07:22:20.000000 alibabacloud_umeng-apm20220214-1.1.3/setup.py
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.2/ChangeLog.md` & `alibabacloud_umeng-apm20220214-1.1.3/ChangeLog.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+2024-04-10 Version: 1.1.2
+- Update API GetTodayStatTrend: update response param.
+
+
 2024-04-09 Version: 1.1.1
 - Update API GetStatTrend: update response param.
 
 
 2023-08-11 Version: 1.1.0
 - Generated python 2022-02-14 for umeng-apm.
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.2/LICENSE` & `alibabacloud_umeng-apm20220214-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214-1.1.2/PKG-INFO` & `alibabacloud_umeng-apm20220214-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud_umeng-apm20220214
-Version: 1.1.2
+Version: 1.1.3
 Summary: Alibaba Cloud umeng-apm (20220214) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.2/README-CN.md` & `alibabacloud_umeng-apm20220214-1.1.3/README-CN.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214-1.1.2/README.md` & `alibabacloud_umeng-apm20220214-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214/client.py` & `alibabacloud_umeng-apm20220214-1.1.3/alibabacloud_umeng_apm20220214/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,17 @@
 from alibabacloud_endpoint_util.client import Client as EndpointUtilClient
 from alibabacloud_umeng_apm20220214 import models as umeng_apm_20220214_models
 from alibabacloud_tea_util import models as util_models
 from alibabacloud_openapi_util.client import Client as OpenApiUtilClient
 from alibabacloud_openplatform20191219.client import Client as OpenPlatformClient
 from alibabacloud_openplatform20191219 import models as open_platform_models
 from alibabacloud_oss_sdk import models as oss_models
+from alibabacloud_oss_sdk.client import Client as OSSClient
 from alibabacloud_tea_fileform import models as file_form_models
 from alibabacloud_oss_util import models as ossutil_models
-from alibabacloud_oss_sdk.client import Client as OSSClient
 
 
 class Client(OpenApiClient):
     """
     *\
     """
     def __init__(
@@ -49,14 +49,22 @@
 
     def get_h5page_trend_with_options(
         self,
         request: umeng_apm_20220214_models.GetH5PageTrendRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetH5PageTrendResponse:
+        """
+        @summary 获取H5页面性能统计数据
+        
+        @param request: GetH5PageTrendRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetH5PageTrendResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.end_date):
@@ -87,14 +95,22 @@
 
     async def get_h5page_trend_with_options_async(
         self,
         request: umeng_apm_20220214_models.GetH5PageTrendRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetH5PageTrendResponse:
+        """
+        @summary 获取H5页面性能统计数据
+        
+        @param request: GetH5PageTrendRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetH5PageTrendResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.end_date):
@@ -123,32 +139,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_h5page_trend(
         self,
         request: umeng_apm_20220214_models.GetH5PageTrendRequest,
     ) -> umeng_apm_20220214_models.GetH5PageTrendResponse:
+        """
+        @summary 获取H5页面性能统计数据
+        
+        @param request: GetH5PageTrendRequest
+        @return: GetH5PageTrendResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_h5page_trend_with_options(request, headers, runtime)
 
     async def get_h5page_trend_async(
         self,
         request: umeng_apm_20220214_models.GetH5PageTrendRequest,
     ) -> umeng_apm_20220214_models.GetH5PageTrendResponse:
+        """
+        @summary 获取H5页面性能统计数据
+        
+        @param request: GetH5PageTrendRequest
+        @return: GetH5PageTrendResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_h5page_trend_with_options_async(request, headers, runtime)
 
     def get_launch_trend_with_options(
         self,
         request: umeng_apm_20220214_models.GetLaunchTrendRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetLaunchTrendResponse:
+        """
+        @summary 获取启动性能统计数据
+        
+        @param request: GetLaunchTrendRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetLaunchTrendResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.end_date):
@@ -179,14 +215,22 @@
 
     async def get_launch_trend_with_options_async(
         self,
         request: umeng_apm_20220214_models.GetLaunchTrendRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetLaunchTrendResponse:
+        """
+        @summary 获取启动性能统计数据
+        
+        @param request: GetLaunchTrendRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetLaunchTrendResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.end_date):
@@ -215,32 +259,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_launch_trend(
         self,
         request: umeng_apm_20220214_models.GetLaunchTrendRequest,
     ) -> umeng_apm_20220214_models.GetLaunchTrendResponse:
+        """
+        @summary 获取启动性能统计数据
+        
+        @param request: GetLaunchTrendRequest
+        @return: GetLaunchTrendResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_launch_trend_with_options(request, headers, runtime)
 
     async def get_launch_trend_async(
         self,
         request: umeng_apm_20220214_models.GetLaunchTrendRequest,
     ) -> umeng_apm_20220214_models.GetLaunchTrendResponse:
+        """
+        @summary 获取启动性能统计数据
+        
+        @param request: GetLaunchTrendRequest
+        @return: GetLaunchTrendResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_launch_trend_with_options_async(request, headers, runtime)
 
     def get_native_page_trend_with_options(
         self,
         request: umeng_apm_20220214_models.GetNativePageTrendRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetNativePageTrendResponse:
+        """
+        @summary 获取原生页面性能统计数据
+        
+        @param request: GetNativePageTrendRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetNativePageTrendResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.end_date):
@@ -271,14 +335,22 @@
 
     async def get_native_page_trend_with_options_async(
         self,
         request: umeng_apm_20220214_models.GetNativePageTrendRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetNativePageTrendResponse:
+        """
+        @summary 获取原生页面性能统计数据
+        
+        @param request: GetNativePageTrendRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetNativePageTrendResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.end_date):
@@ -307,32 +379,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_native_page_trend(
         self,
         request: umeng_apm_20220214_models.GetNativePageTrendRequest,
     ) -> umeng_apm_20220214_models.GetNativePageTrendResponse:
+        """
+        @summary 获取原生页面性能统计数据
+        
+        @param request: GetNativePageTrendRequest
+        @return: GetNativePageTrendResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_native_page_trend_with_options(request, headers, runtime)
 
     async def get_native_page_trend_async(
         self,
         request: umeng_apm_20220214_models.GetNativePageTrendRequest,
     ) -> umeng_apm_20220214_models.GetNativePageTrendResponse:
+        """
+        @summary 获取原生页面性能统计数据
+        
+        @param request: GetNativePageTrendRequest
+        @return: GetNativePageTrendResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_native_page_trend_with_options_async(request, headers, runtime)
 
     def get_network_trend_with_options(
         self,
         request: umeng_apm_20220214_models.GetNetworkTrendRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetNetworkTrendResponse:
+        """
+        @summary 获取网络性能统计数据
+        
+        @param request: GetNetworkTrendRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetNetworkTrendResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.end_date):
@@ -363,14 +455,22 @@
 
     async def get_network_trend_with_options_async(
         self,
         request: umeng_apm_20220214_models.GetNetworkTrendRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetNetworkTrendResponse:
+        """
+        @summary 获取网络性能统计数据
+        
+        @param request: GetNetworkTrendRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetNetworkTrendResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.end_date):
@@ -399,32 +499,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_network_trend(
         self,
         request: umeng_apm_20220214_models.GetNetworkTrendRequest,
     ) -> umeng_apm_20220214_models.GetNetworkTrendResponse:
+        """
+        @summary 获取网络性能统计数据
+        
+        @param request: GetNetworkTrendRequest
+        @return: GetNetworkTrendResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_network_trend_with_options(request, headers, runtime)
 
     async def get_network_trend_async(
         self,
         request: umeng_apm_20220214_models.GetNetworkTrendRequest,
     ) -> umeng_apm_20220214_models.GetNetworkTrendResponse:
+        """
+        @summary 获取网络性能统计数据
+        
+        @param request: GetNetworkTrendRequest
+        @return: GetNetworkTrendResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_network_trend_with_options_async(request, headers, runtime)
 
     def get_stat_trend_with_options(
         self,
         request: umeng_apm_20220214_models.GetStatTrendRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetStatTrendResponse:
+        """
+        @summary 获取离线统计数据
+        
+        @param request: GetStatTrendRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetStatTrendResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.end_date):
@@ -455,14 +575,22 @@
 
     async def get_stat_trend_with_options_async(
         self,
         request: umeng_apm_20220214_models.GetStatTrendRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetStatTrendResponse:
+        """
+        @summary 获取离线统计数据
+        
+        @param request: GetStatTrendRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetStatTrendResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.end_date):
@@ -491,32 +619,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_stat_trend(
         self,
         request: umeng_apm_20220214_models.GetStatTrendRequest,
     ) -> umeng_apm_20220214_models.GetStatTrendResponse:
+        """
+        @summary 获取离线统计数据
+        
+        @param request: GetStatTrendRequest
+        @return: GetStatTrendResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_stat_trend_with_options(request, headers, runtime)
 
     async def get_stat_trend_async(
         self,
         request: umeng_apm_20220214_models.GetStatTrendRequest,
     ) -> umeng_apm_20220214_models.GetStatTrendResponse:
+        """
+        @summary 获取离线统计数据
+        
+        @param request: GetStatTrendRequest
+        @return: GetStatTrendResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_stat_trend_with_options_async(request, headers, runtime)
 
     def get_sym_upload_param_with_options(
         self,
         request: umeng_apm_20220214_models.GetSymUploadParamRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetSymUploadParamResponse:
+        """
+        @summary 获取符号表文件上传参数
+        
+        @param request: GetSymUploadParamRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSymUploadParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.file_name):
@@ -547,14 +695,22 @@
 
     async def get_sym_upload_param_with_options_async(
         self,
         request: umeng_apm_20220214_models.GetSymUploadParamRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetSymUploadParamResponse:
+        """
+        @summary 获取符号表文件上传参数
+        
+        @param request: GetSymUploadParamRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetSymUploadParamResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.file_name):
@@ -583,32 +739,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_sym_upload_param(
         self,
         request: umeng_apm_20220214_models.GetSymUploadParamRequest,
     ) -> umeng_apm_20220214_models.GetSymUploadParamResponse:
+        """
+        @summary 获取符号表文件上传参数
+        
+        @param request: GetSymUploadParamRequest
+        @return: GetSymUploadParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_sym_upload_param_with_options(request, headers, runtime)
 
     async def get_sym_upload_param_async(
         self,
         request: umeng_apm_20220214_models.GetSymUploadParamRequest,
     ) -> umeng_apm_20220214_models.GetSymUploadParamResponse:
+        """
+        @summary 获取符号表文件上传参数
+        
+        @param request: GetSymUploadParamRequest
+        @return: GetSymUploadParamResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_sym_upload_param_with_options_async(request, headers, runtime)
 
     def get_today_stat_trend_with_options(
         self,
         request: umeng_apm_20220214_models.GetTodayStatTrendRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetTodayStatTrendResponse:
+        """
+        @summary 获取今日实时统计数据
+        
+        @param request: GetTodayStatTrendRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTodayStatTrendResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.type):
@@ -635,14 +811,22 @@
 
     async def get_today_stat_trend_with_options_async(
         self,
         request: umeng_apm_20220214_models.GetTodayStatTrendRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.GetTodayStatTrendResponse:
+        """
+        @summary 获取今日实时统计数据
+        
+        @param request: GetTodayStatTrendRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: GetTodayStatTrendResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.type):
@@ -667,32 +851,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def get_today_stat_trend(
         self,
         request: umeng_apm_20220214_models.GetTodayStatTrendRequest,
     ) -> umeng_apm_20220214_models.GetTodayStatTrendResponse:
+        """
+        @summary 获取今日实时统计数据
+        
+        @param request: GetTodayStatTrendRequest
+        @return: GetTodayStatTrendResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.get_today_stat_trend_with_options(request, headers, runtime)
 
     async def get_today_stat_trend_async(
         self,
         request: umeng_apm_20220214_models.GetTodayStatTrendRequest,
     ) -> umeng_apm_20220214_models.GetTodayStatTrendResponse:
+        """
+        @summary 获取今日实时统计数据
+        
+        @param request: GetTodayStatTrendRequest
+        @return: GetTodayStatTrendResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.get_today_stat_trend_with_options_async(request, headers, runtime)
 
     def update_alert_plan_with_options(
         self,
         request: umeng_apm_20220214_models.UpdateAlertPlanRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.UpdateAlertPlanResponse:
+        """
+        @summary 更新监控告警计划
+        
+        @param request: UpdateAlertPlanRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAlertPlanResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.plan_id):
             query['planId'] = request.plan_id
         if not UtilClient.is_unset(request.versions):
@@ -719,14 +923,22 @@
 
     async def update_alert_plan_with_options_async(
         self,
         request: umeng_apm_20220214_models.UpdateAlertPlanRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.UpdateAlertPlanResponse:
+        """
+        @summary 更新监控告警计划
+        
+        @param request: UpdateAlertPlanRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UpdateAlertPlanResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.plan_id):
             query['planId'] = request.plan_id
         if not UtilClient.is_unset(request.versions):
@@ -751,32 +963,52 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def update_alert_plan(
         self,
         request: umeng_apm_20220214_models.UpdateAlertPlanRequest,
     ) -> umeng_apm_20220214_models.UpdateAlertPlanResponse:
+        """
+        @summary 更新监控告警计划
+        
+        @param request: UpdateAlertPlanRequest
+        @return: UpdateAlertPlanResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.update_alert_plan_with_options(request, headers, runtime)
 
     async def update_alert_plan_async(
         self,
         request: umeng_apm_20220214_models.UpdateAlertPlanRequest,
     ) -> umeng_apm_20220214_models.UpdateAlertPlanResponse:
+        """
+        @summary 更新监控告警计划
+        
+        @param request: UpdateAlertPlanRequest
+        @return: UpdateAlertPlanResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.update_alert_plan_with_options_async(request, headers, runtime)
 
     def upload_symbol_file_with_options(
         self,
         request: umeng_apm_20220214_models.UploadSymbolFileRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.UploadSymbolFileResponse:
+        """
+        @summary 上传符号表文件
+        
+        @param request: UploadSymbolFileRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UploadSymbolFileResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.file_name):
@@ -809,14 +1041,22 @@
 
     async def upload_symbol_file_with_options_async(
         self,
         request: umeng_apm_20220214_models.UploadSymbolFileRequest,
         headers: Dict[str, str],
         runtime: util_models.RuntimeOptions,
     ) -> umeng_apm_20220214_models.UploadSymbolFileResponse:
+        """
+        @summary 上传符号表文件
+        
+        @param request: UploadSymbolFileRequest
+        @param headers: map
+        @param runtime: runtime options for this request RuntimeOptions
+        @return: UploadSymbolFileResponse
+        """
         UtilClient.validate_model(request)
         query = {}
         if not UtilClient.is_unset(request.app_version):
             query['appVersion'] = request.app_version
         if not UtilClient.is_unset(request.data_source_id):
             query['dataSourceId'] = request.data_source_id
         if not UtilClient.is_unset(request.file_name):
@@ -847,22 +1087,34 @@
             await self.call_api_async(params, req, runtime)
         )
 
     def upload_symbol_file(
         self,
         request: umeng_apm_20220214_models.UploadSymbolFileRequest,
     ) -> umeng_apm_20220214_models.UploadSymbolFileResponse:
+        """
+        @summary 上传符号表文件
+        
+        @param request: UploadSymbolFileRequest
+        @return: UploadSymbolFileResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return self.upload_symbol_file_with_options(request, headers, runtime)
 
     async def upload_symbol_file_async(
         self,
         request: umeng_apm_20220214_models.UploadSymbolFileRequest,
     ) -> umeng_apm_20220214_models.UploadSymbolFileResponse:
+        """
+        @summary 上传符号表文件
+        
+        @param request: UploadSymbolFileRequest
+        @return: UploadSymbolFileResponse
+        """
         runtime = util_models.RuntimeOptions()
         headers = {}
         return await self.upload_symbol_file_with_options_async(request, headers, runtime)
 
     def upload_symbol_file_advance(
         self,
         request: umeng_apm_20220214_models.UploadSymbolFileAdvanceRequest,
@@ -871,15 +1123,15 @@
     ) -> umeng_apm_20220214_models.UploadSymbolFileResponse:
         # Step 0: init client
         access_key_id = self._credential.get_access_key_id()
         access_key_secret = self._credential.get_access_key_secret()
         security_token = self._credential.get_security_token()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
+        if UtilClient.empty(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
         auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
@@ -891,20 +1143,21 @@
         auth_client = OpenPlatformClient(auth_config)
         auth_request = open_platform_models.AuthorizeFileUploadRequest(
             product='umeng-apm',
             region_id=self._region_id
         )
         auth_response = open_platform_models.AuthorizeFileUploadResponse()
         oss_config = oss_models.Config(
+            access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             type='access_key',
             protocol=self._protocol,
             region_id=self._region_id
         )
-        oss_client = None
+        oss_client = OSSClient(oss_config)
         file_obj = file_form_models.FileField()
         oss_header = oss_models.PostObjectRequestHeader()
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         upload_symbol_file_req = umeng_apm_20220214_models.UploadSymbolFileRequest()
         OpenApiUtilClient.convert(request, upload_symbol_file_req)
@@ -943,15 +1196,15 @@
     ) -> umeng_apm_20220214_models.UploadSymbolFileResponse:
         # Step 0: init client
         access_key_id = await self._credential.get_access_key_id_async()
         access_key_secret = await self._credential.get_access_key_secret_async()
         security_token = await self._credential.get_security_token_async()
         credential_type = self._credential.get_type()
         open_platform_endpoint = self._open_platform_endpoint
-        if UtilClient.is_unset(open_platform_endpoint):
+        if UtilClient.empty(open_platform_endpoint):
             open_platform_endpoint = 'openplatform.aliyuncs.com'
         if UtilClient.is_unset(credential_type):
             credential_type = 'access_key'
         auth_config = open_api_models.Config(
             access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             security_token=security_token,
@@ -963,20 +1216,21 @@
         auth_client = OpenPlatformClient(auth_config)
         auth_request = open_platform_models.AuthorizeFileUploadRequest(
             product='umeng-apm',
             region_id=self._region_id
         )
         auth_response = open_platform_models.AuthorizeFileUploadResponse()
         oss_config = oss_models.Config(
+            access_key_id=access_key_id,
             access_key_secret=access_key_secret,
             type='access_key',
             protocol=self._protocol,
             region_id=self._region_id
         )
-        oss_client = None
+        oss_client = OSSClient(oss_config)
         file_obj = file_form_models.FileField()
         oss_header = oss_models.PostObjectRequestHeader()
         upload_request = oss_models.PostObjectRequest()
         oss_runtime = ossutil_models.RuntimeOptions()
         OpenApiUtilClient.convert(runtime, oss_runtime)
         upload_symbol_file_req = umeng_apm_20220214_models.UploadSymbolFileRequest()
         OpenApiUtilClient.convert(request, upload_symbol_file_req)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214/models.py` & `alibabacloud_umeng-apm20220214-1.1.3/alibabacloud_umeng_apm20220214/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,21 @@
         app_version: str = None,
         data_source_id: str = None,
         end_date: str = None,
         start_date: str = None,
         time_unit: str = None,
     ):
         self.app_version = app_version
+        # This parameter is required.
         self.data_source_id = data_source_id
+        # This parameter is required.
         self.end_date = end_date
+        # This parameter is required.
         self.start_date = start_date
+        # This parameter is required.
         self.time_unit = time_unit
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -308,17 +312,21 @@
         app_version: str = None,
         data_source_id: str = None,
         end_date: str = None,
         start_date: str = None,
         time_unit: str = None,
     ):
         self.app_version = app_version
+        # This parameter is required.
         self.data_source_id = data_source_id
+        # This parameter is required.
         self.end_date = end_date
+        # This parameter is required.
         self.start_date = start_date
+        # This parameter is required.
         self.time_unit = time_unit
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -516,17 +524,21 @@
         app_version: str = None,
         data_source_id: str = None,
         end_date: str = None,
         start_date: str = None,
         time_unit: str = None,
     ):
         self.app_version = app_version
+        # This parameter is required.
         self.data_source_id = data_source_id
+        # This parameter is required.
         self.end_date = end_date
+        # This parameter is required.
         self.start_date = start_date
+        # This parameter is required.
         self.time_unit = time_unit
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -712,17 +724,21 @@
         app_version: str = None,
         data_source_id: str = None,
         end_date: str = None,
         start_date: str = None,
         time_unit: str = None,
     ):
         self.app_version = app_version
+        # This parameter is required.
         self.data_source_id = data_source_id
+        # This parameter is required.
         self.end_date = end_date
+        # This parameter is required.
         self.start_date = start_date
+        # This parameter is required.
         self.time_unit = time_unit
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -908,17 +924,19 @@
         app_version: str = None,
         data_source_id: str = None,
         end_date: str = None,
         start_date: str = None,
         type: int = None,
     ):
         self.app_version = app_version
+        # This parameter is required.
         self.data_source_id = data_source_id
         self.end_date = end_date
         self.start_date = start_date
+        # This parameter is required.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1103,17 +1121,21 @@
         self,
         app_version: str = None,
         data_source_id: str = None,
         file_name: str = None,
         file_type: int = None,
         flutter_name: str = None,
     ):
+        # This parameter is required.
         self.app_version = app_version
+        # This parameter is required.
         self.data_source_id = data_source_id
+        # This parameter is required.
         self.file_name = file_name
+        # This parameter is required.
         self.file_type = file_type
         self.flutter_name = flutter_name
 
     def validate(self):
         pass
 
     def to_map(self):
@@ -1306,15 +1328,17 @@
     def __init__(
         self,
         app_version: str = None,
         data_source_id: str = None,
         type: int = None,
     ):
         self.app_version = app_version
+        # This parameter is required.
         self.data_source_id = data_source_id
+        # This parameter is required.
         self.type = type
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1489,16 +1513,19 @@
 class UpdateAlertPlanRequest(TeaModel):
     def __init__(
         self,
         data_source_id: str = None,
         plan_id: int = None,
         versions: str = None,
     ):
+        # This parameter is required.
         self.data_source_id = data_source_id
+        # This parameter is required.
         self.plan_id = plan_id
+        # This parameter is required.
         self.versions = versions
 
     def validate(self):
         pass
 
     def to_map(self):
         _map = super().to_map()
@@ -1611,17 +1638,21 @@
         app_version: str = None,
         data_source_id: str = None,
         file_name: str = None,
         file_type: int = None,
         flutter_name: str = None,
         oss_url: str = None,
     ):
+        # This parameter is required.
         self.app_version = app_version
+        # This parameter is required.
         self.data_source_id = data_source_id
+        # This parameter is required.
         self.file_name = file_name
+        # This parameter is required.
         self.file_type = file_type
         self.flutter_name = flutter_name
         self.oss_url = oss_url
 
     def validate(self):
         pass
 
@@ -1668,17 +1699,21 @@
         app_version: str = None,
         data_source_id: str = None,
         file_name: str = None,
         file_type: int = None,
         flutter_name: str = None,
         oss_url_object: BinaryIO = None,
     ):
+        # This parameter is required.
         self.app_version = app_version
+        # This parameter is required.
         self.data_source_id = data_source_id
+        # This parameter is required.
         self.file_name = file_name
+        # This parameter is required.
         self.file_type = file_type
         self.flutter_name = flutter_name
         self.oss_url_object = oss_url_object
 
     def validate(self):
         pass
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.2/alibabacloud_umeng_apm20220214.egg-info/PKG-INFO` & `alibabacloud_umeng-apm20220214-1.1.3/alibabacloud_umeng_apm20220214.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alibabacloud-umeng-apm20220214
-Version: 1.1.2
+Version: 1.1.3
 Summary: Alibaba Cloud umeng-apm (20220214) SDK Library for Python
 Home-page: https://github.com/aliyun/alibabacloud-python-sdk
 Author: Alibaba Cloud SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
         ![](https://aliyunsdk-pages.alicdn.com/icons/AlibabaCloud.svg)
```

### Comparing `alibabacloud_umeng-apm20220214-1.1.2/setup.py` & `alibabacloud_umeng-apm20220214-1.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,33 +20,33 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for alibabacloud_umeng-apm20220214.
 
-Created on 10/04/2024
+Created on 21/05/2024
 
 @author: Alibaba Cloud SDK
 """
 
 PACKAGE = "alibabacloud_umeng_apm20220214"
 NAME = "alibabacloud_umeng-apm20220214" or "alibabacloud-package"
 DESCRIPTION = "Alibaba Cloud umeng-apm (20220214) SDK Library for Python"
 AUTHOR = "Alibaba Cloud SDK"
 AUTHOR_EMAIL = "sdk-team@alibabacloud.com"
 URL = "https://github.com/aliyun/alibabacloud-python-sdk"
 VERSION = __import__(PACKAGE).__version__
 REQUIRES = [
-    "alibabacloud_tea_util>=0.3.11, <1.0.0",
+    "alibabacloud_tea_util>=0.3.12, <1.0.0",
     "alibabacloud_oss_sdk>=0.1.0, <1.0.0",
     "alibabacloud_openplatform20191219>=2.0.0, <3.0.0",
     "alibabacloud_oss_util>=0.0.5, <1.0.0",
     "alibabacloud_tea_fileform>=0.0.3, <1.0.0",
-    "alibabacloud_tea_openapi>=0.3.8, <1.0.0",
+    "alibabacloud_tea_openapi>=0.3.9, <1.0.0",
     "alibabacloud_openapi_util>=0.2.1, <1.0.0",
     "alibabacloud_endpoint_util>=0.0.3, <1.0.0"
 ]
 
 LONG_DESCRIPTION = ''
 if os.path.exists('./README.md'):
     with open("README.md", encoding='utf-8') as fp:
```

