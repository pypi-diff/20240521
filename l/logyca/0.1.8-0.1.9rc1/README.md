# Comparing `tmp/logyca-0.1.8.tar.gz` & `tmp/logyca-0.1.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "logyca-0.1.9rc1.tar", last modified: Tue May 21 19:54:14 2024, max compression
```

## Comparing `logyca-0.1.8.tar` & `logyca-0.1.9rc1.tar`

### file list

```diff
@@ -1,20 +1,52 @@
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 logyca-0.1.8/.pypirc-sample
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 logyca-0.1.8/Pipfile
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 logyca-0.1.8/logyca/__init__.py
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 logyca-0.1.8/logyca/common/constants.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 logyca-0.1.8/logyca/data/enums/healthenum.py
--rw-r--r--   0        0        0     7697 2020-02-02 00:00:00.000000 logyca-0.1.8/logyca/data/enums/logycastatusenum.py
--rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 logyca-0.1.8/logyca/data/schemas/dtos/apIresultdto.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 logyca-0.1.8/logyca/data/schemas/dtos/apifilterexceptiondto.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 logyca-0.1.8/logyca/data/schemas/dtos/healthdto.py
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 logyca-0.1.8/logyca/data/schemas/dtos/httpexceptiondto.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 logyca-0.1.8/logyca/data/schemas/dtos/tokensdto.py
--rw-r--r--   0        0        0      619 2020-02-02 00:00:00.000000 logyca-0.1.8/logyca/helpers/datetimehelpers.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 logyca-0.1.8/logyca/helpers/stringshelpers.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 logyca-0.1.8/tests/test_data_schemes.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 logyca-0.1.8/tests/test_helpers.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 logyca-0.1.8/.gitignore
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 logyca-0.1.8/LICENSE.txt
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 logyca-0.1.8/README.md
--rw-r--r--   0        0        0     2054 2020-02-02 00:00:00.000000 logyca-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     8632 2020-02-02 00:00:00.000000 logyca-0.1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.722838 logyca-0.1.9rc1/
+-rw-rw-rw-   0        0        0     1092 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/LICENSE.txt
+-rw-rw-rw-   0        0        0    12569 2024-05-21 19:54:14.721836 logyca-0.1.9rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     9559 2024-05-21 19:42:54.000000 logyca-0.1.9rc1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.653241 logyca-0.1.9rc1/logyca/
+-rw-rw-rw-   0        0        0     1727 2024-04-26 23:10:10.000000 logyca-0.1.9rc1/logyca/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.667597 logyca-0.1.9rc1/logyca/dependencies/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/dependencies/__init__.py
+-rw-rw-rw-   0        0        0     1380 2024-04-29 13:53:22.000000 logyca-0.1.9rc1/logyca/dependencies/api_key_simple_auth.py
+-rw-rw-rw-   0        0        0     3728 2024-04-29 13:53:26.000000 logyca-0.1.9rc1/logyca/dependencies/oauth_token.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.668597 logyca-0.1.9rc1/logyca/schemas/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.678270 logyca-0.1.9rc1/logyca/schemas/input/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/input/__init__.py
+-rw-rw-rw-   0        0        0      288 2024-04-23 21:48:51.000000 logyca-0.1.9rc1/logyca/schemas/input/api_key.py
+-rw-rw-rw-   0        0        0      279 2024-04-24 01:52:56.000000 logyca-0.1.9rc1/logyca/schemas/input/claimsdto.py
+-rw-rw-rw-   0        0        0      111 2024-04-24 01:42:50.000000 logyca-0.1.9rc1/logyca/schemas/input/jwt.py
+-rw-rw-rw-   0        0        0      553 2024-04-24 00:49:40.000000 logyca-0.1.9rc1/logyca/schemas/input/oauth_token.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.688834 logyca-0.1.9rc1/logyca/schemas/output/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/output/__init__.py
+-rw-rw-rw-   0        0        0      954 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/output/apIresultdto.py
+-rw-rw-rw-   0        0        0      896 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/output/apifilterexceptiondto.py
+-rw-rw-rw-   0        0        0      628 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/output/healthdto.py
+-rw-rw-rw-   0        0        0      138 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/output/httpexceptiondto.py
+-rw-rw-rw-   0        0        0      472 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/schemas/output/tokensdto.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.690837 logyca-0.1.9rc1/logyca/utils/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.697836 logyca-0.1.9rc1/logyca/utils/constants/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/constants/__init__.py
+-rw-rw-rw-   0        0        0      128 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/constants/app.py
+-rw-rw-rw-   0        0        0      724 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/constants/healthenum.py
+-rw-rw-rw-   0        0        0     7697 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/constants/logycastatusenum.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.702837 logyca-0.1.9rc1/logyca/utils/handlers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/handlers/__init__.py
+-rw-rw-rw-   0        0        0     4689 2024-04-23 15:28:59.000000 logyca-0.1.9rc1/logyca/utils/handlers/exception_handlers.py
+-rw-rw-rw-   0        0        0     2436 2024-04-23 15:22:15.000000 logyca-0.1.9rc1/logyca/utils/handlers/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.707839 logyca-0.1.9rc1/logyca/utils/helpers/
+-rw-rw-rw-   0        0        0        0 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/logyca/utils/helpers/__init__.py
+-rw-rw-rw-   0        0        0      531 2024-04-26 17:40:26.000000 logyca-0.1.9rc1/logyca/utils/helpers/datetimehelpers.py
+-rw-rw-rw-   0        0        0      634 2024-04-24 02:55:02.000000 logyca-0.1.9rc1/logyca/utils/helpers/stringshelpers.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.716837 logyca-0.1.9rc1/logyca.egg-info/
+-rw-rw-rw-   0        0        0    12569 2024-05-21 19:54:14.000000 logyca-0.1.9rc1/logyca.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1204 2024-05-21 19:54:14.000000 logyca-0.1.9rc1/logyca.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 19:54:14.000000 logyca-0.1.9rc1/logyca.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      335 2024-05-21 19:54:14.000000 logyca-0.1.9rc1/logyca.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-21 19:54:14.000000 logyca-0.1.9rc1/logyca.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 19:54:14.724836 logyca-0.1.9rc1/setup.cfg
+-rw-rw-rw-   0        0        0     2481 2024-05-21 19:50:21.000000 logyca-0.1.9rc1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 19:54:14.713837 logyca-0.1.9rc1/tests/
+-rw-rw-rw-   0        0        0     2324 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/tests/test_data_schemes.py
+-rw-rw-rw-   0        0        0      221 2024-04-26 17:45:47.000000 logyca-0.1.9rc1/tests/test_functions.py
+-rw-rw-rw-   0        0        0      226 2024-04-23 14:32:08.000000 logyca-0.1.9rc1/tests/test_helpers.py
```

### Comparing `logyca-0.1.8/logyca/data/enums/healthenum.py` & `logyca-0.1.9rc1/logyca/utils/constants/healthenum.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.8/logyca/data/enums/logycastatusenum.py` & `logyca-0.1.9rc1/logyca/utils/constants/logycastatusenum.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.8/logyca/data/schemas/dtos/apIresultdto.py` & `logyca-0.1.9rc1/logyca/schemas/output/apIresultdto.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-from logyca.data.schemas.dtos.tokensdto import TokensDTO
-from logyca.data.schemas.dtos.apifilterexceptiondto import ApiFilterExceptionDTO
+from logyca.schemas.output.tokensdto import TokensDTO
+from logyca.schemas.output.apifilterexceptiondto import ApiFilterExceptionDTO
 from typing import Any
 from pydantic import BaseModel,Field
 
 class APIResultDTO(BaseModel):
         resultToken:TokensDTO=Field(default=TokensDTO(),description="Gets or sets object with result")
         resultObject:Any=Field(default=None,description="Gets or sets object with result")
         apiException:ApiFilterExceptionDTO=Field(description="Gets or sets error")
         resultMessage:str=Field(default='',description="Gets or sets result of negative or positive message")
         dataError:bool=Field(default=True,description="Gets or sets a value indicating whether gets or sets a value if it is data error")
-        class Config():
-                orm_mode = True
         def __init__(self, **kwargs):
                 kwargs['dataError'] = False
                 kwargs['apiException'] = ApiFilterExceptionDTO()
                 super().__init__(**kwargs)
```

### Comparing `logyca-0.1.8/logyca/data/schemas/dtos/apifilterexceptiondto.py` & `logyca-0.1.9rc1/logyca/schemas/output/apifilterexceptiondto.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pydantic import BaseModel,Field
-from logyca.data.enums.logycastatusenum import LogycaStatusEnum
+from logyca.utils.constants.logycastatusenum import LogycaStatusEnum
 from typing import Any
 from http import HTTPStatus
 
 class ApiFilterExceptionDTO(BaseModel):
         message:str=Field(default='',description="Gets or sets error message")
         isError:bool=Field(default=True,description="Gets or sets a value indicating whether api has error")
         detail:Any=Field(default=None,description="Gets or sets error detail")
```

### Comparing `logyca-0.1.8/logyca/data/schemas/dtos/healthdto.py` & `logyca-0.1.9rc1/logyca/schemas/output/healthdto.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from logyca.data.enums.healthenum import HealthEnum
+from logyca.utils.constants.healthenum import HealthEnum
 
 class HealthDTO():
     '''Description
     LOGYCA HTTP Custom States
     :param name:str Gets or sets health status name
     :param status:HealthEnum Gets or sets health check status response code
     :param description:str Gets or sets description of the monitoring process
```

### Comparing `logyca-0.1.8/tests/test_data_schemes.py` & `logyca-0.1.9rc1/tests/test_data_schemes.py`

 * *Files identical despite different names*

### Comparing `logyca-0.1.8/LICENSE.txt` & `logyca-0.1.9rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `logyca-0.1.8/PKG-INFO` & `logyca-0.1.9rc1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,288 +1,304 @@
-Metadata-Version: 2.1
-Name: logyca
-Version: 0.1.8
-Summary: This package name is reserved by LOGYCA company
-Project-URL: Homepage, https://github.com/ccc/ccc
-Project-URL: Documentation, https://ccc/
-Author-email: Jaime Andres Cardona Carrillo <tecnologiaeinformacion@logyca.com>
-Maintainer-email: Jaime Andres Cardona Carrillo <tecnologiaeinformacion@logyca.com>
-License: MIT
-License-File: LICENSE.txt
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Pydantic
-Classifier: Framework :: Pydantic :: 1
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: System Administrators
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet
-Classifier: Topic :: Internet :: WWW/HTTP
-Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Libraries
-Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Typing :: Typed
-Requires-Python: >=3.7
-Requires-Dist: pydantic>=1.8
-Requires-Dist: pytz>=2022.1
-Provides-Extra: logycafeaturesample
-Requires-Dist: sqlalchemy<2.0.8,>=1.3.18; extra == 'logycafeaturesample'
-Provides-Extra: test
-Requires-Dist: pytest<8.0.0,>=7.1.3; extra == 'test'
-Description-Content-Type: text/markdown
-
-<p align="center">
-  <a href="https://logyca.com/"><img src="https://logyca.com/sites/default/files/logyca.png" alt="Logyca"></a>
-</p>
-<p align="center">
-    <em>LOGYCA public libraries</em>
-</p>
-
-<p align="center">
-<a href="https://pypi.org/project/logyca" target="_blank">
-    <img src="https://img.shields.io/pypi/v/logyca?color=orange&label=PyPI%20Package" alt="Package version">
-</a>
-<a href="(https://www.python.org" target="_blank">
-    <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.7%2C%3C%3D3.11%5D-orange" alt="Python">
-</a>
-</p>
-
-
----
-
-# About us
-
-* <a href="http://logyca.com" target="_blank">LOGYCA Company</a>
-* <a href="https://www.youtube.com/channel/UCzcJtxfScoAtwFbxaLNnEtA" target="_blank">LOGYCA Youtube Channel</a>
-* <a href="https://www.linkedin.com/company/logyca" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="Linkedin"></a>
-* <a href="https://twitter.com/LOGYCA_Org" target="_blank"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter"></a>
-* <a href="https://www.facebook.com/OrganizacionLOGYCA/" target="_blank"><img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" alt="Facebook"></a>
-
----
-
-# What's libraries
-
-* **Traversal libraries**: Standard methods to be used by microservices.
-* **Return codes**: Standard methods to report result status codes.
-* **Monitoring**: Standard methods to report check health status codes.
-* **Helpers**: Standard methods to be used. *
-
----
-
-# Semantic Versioning
-
-logyca <MAJOR>.<MINOR>.<PATCH>
-
-* **MAJOR**: version when you make incompatible API changes
-* **MINOR**: version when you add functionality in a backwards compatible manner
-* **PATCH**: version when you make backwards compatible bug fixes
-
-# Quick install
-
-```console
-# Windows
-python -m pip install logyca
-# Linux
-pip install logyca
-```
-
----
-
-# Example of concepts using library APIResult
-
-```python
-# Example output from ApiResult:
-result={
-  "resultToken": {
-    "token": "",
-    "refreshToken": "",
-    "result": "",
-    "emailActiveDirectory": "",
-    "message": ""
-  },
-  "resultObject": [
-    {
-      "name": "Database server",
-      "status": 0,
-      "description": "Connection status fine"
-    },
-    {
-      "name": "Redis server",
-      "status": 0,
-      "description": "Connection status fine"
-    }
-  ],
-  "apiException": {
-    "message": "",
-    "isError": false,
-    "detail": null,
-    "status": 200,
-    "logycaStatus": 0
-  },
-  "resultMessage": "",
-  "dataError": false
-}
-```
-
-## Use cases: you must catch de exception
-
-1. if you get data only the token:
-```json
-{
-"dataError":false,
-"resultObject":null,
-"resultToken":"Not Null"
-}
-```
-
-2. if you get data correctly
-```json
-{
-"dataError":false,
-"resultObject"="Not Null"
-"resultToken"=null
-}
-```
-
-3. if you don't get because the operation was cancelled
-```json
-{
-"dataError":true,
-"resultObject":null,
-"resultToken":null,
-"apiException.logycaStatus":1,
-"apiException.status"=404,
-"resultMessage":"exception messages: the operation was cancelled"
-}
-```
-[optional]apiException.message="if needed, return an object with structured failure data other than exception messages"
-
-
-# Example of using library APIResult + Health Check
-
-```python
-
-from logyca import HealthEnum, LogycaStatusEnum, APIResultDTO, ApiFilterExceptionDTO, HTTPExceptionDTO, HealthDTO, TokensDTO
-
-tokensDTO=TokensDTO()
-tokensDTO.token='Token Example'
-
-apiFilterExceptionDTO=ApiFilterExceptionDTO()
-apiFilterExceptionDTO.isError=False
-apiFilterExceptionDTO.logycaStatus=LogycaStatusEnum.Already_Exists
-apiFilterExceptionDTO.status=LogycaStatusEnum.Already_Exists.mappingHttpStatusCode
-
-httpExceptionDTO=HTTPExceptionDTO()
-httpExceptionDTO.detail='No Problem'
-
-listHealth=[]
-
-listHealth.append(HealthDTO(name='Check CPU',status=HealthEnum.Ok,description='OK'))
-listHealth.append(HealthDTO(name='Check Connect DB',status=HealthEnum.Warning,description='Warning'))
-listHealth.append(HealthDTO(name='Check Connect Storage',status=HealthEnum.Critical,description='Critical'))
-
-
-apiResultDTO=APIResultDTO()
-apiResultDTO.resultMessage=httpExceptionDTO.detail
-apiResultDTO.resultObject=listHealth
-apiResultDTO.dataError=False
-apiResultDTO.resultToken=tokensDTO
-apiResultDTO.apiException=apiFilterExceptionDTO
-
-print(apiResultDTO.resultToken)
-for item in apiResultDTO.resultObject:
-    print(f'name={item.name},status={item.status},description={item.description}')
-print(apiResultDTO.resultToken)
-
-# output
-# token='Token Example' refreshToken='' result='' emailActiveDirectory='' message=''
-# name=Check CPU,status=0,description=OK
-# name=Check Connect DB,status=1,description=Warning
-# name=Check Connect Storage,status=2,description=Critical
-# token='Token Example' refreshToken='' result='' emailActiveDirectory='' message=''
-```
-
----
-
-# Example of using helpers
-
-```python
-from logyca import buildUrl,convertDateTimeStampUTCtoUTCColombia
-
-url1='https://domain.com'
-url2='api/get'
-print(f'buildUrl={buildUrl(url1,url2)}')
-# ouput
-# buildUrl=https://domain.com/api/get
-
-datetimestampUTC=1679729109
-print(f'datetimeUTCColombia={convertDateTimeStampUTCtoUTCColombia(datetimestampUTC)}')
-# output
-# datetimeUTCColombia=2023-03-25 02:25:09-05:00
-```
-
----
-
-# Current library test
-
-```console
-# Library installation
-
-# Windows
-python -m pip install logyca[test]
-# Linux
-pip install logyca
-
-# Run it
-pytest -s
-```
-
----
-
-# Changelog
-
-All notable changes to this project will be documented in this file.
-
-The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
-and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
-
-## Types of changes
-
-- Added for new features.
-- Changed for changes in existing functionality.
-- Deprecated for soon-to-be removed features.
-- Removed for now removed features.
-- Fixed for any bug fixes.
-- Security in case of vulnerabilities.
-
-## [0.1.8] - 2023-10-03
-### Fixed
-- Due to a link error in the readme to internal documents in pypi, we chose to leave the changelog at the end of the readme. 
-
-## [0.1.7] - 2023-10-02
-### Fixed
-- The url address for the logyca logo is corrected
-- Adjust return code for LogycaStatusEnum class: LogycaStatusEnum.Created==HTTPStatus.CREATED
-- Adjust return code for LogycaStatusEnum class: LogycaStatusEnum.InProcess==HTTPStatus.ACCEPTED
-- Adjust return code for LogycaStatusEnum class: LogycaStatusEnum.Partial==HTTPStatus.ACCEPTED
-- Empty files __init__.py removed
-
-## [0.1.6] - 2023-09-11
-### Fixed
-- Pydantic restriction for versions lower than 2.0 is removed
-
-## [0.1.5] - 2023-03-27
-### Added
-- Release ready for production
-
+<p align="center">
+  <a href="https://logyca.com/"><img src="https://logyca.com/sites/default/files/logyca.png" alt="Logyca"></a>
+</p>
+<p align="center">
+    <em>LOGYCA public libraries</em>
+</p>
+
+<p align="center">
+<a href="https://pypi.org/project/logyca" target="_blank">
+    <img src="https://img.shields.io/pypi/v/logyca?color=orange&label=PyPI%20Package" alt="Package version">
+</a>
+<a href="(https://www.python.org" target="_blank">
+    <img src="https://img.shields.io/badge/Python-%5B%3E%3D3.7%2C%3C%3D3.11%5D-orange" alt="Python">
+</a>
+</p>
+
+
+---
+
+# About us
+
+* <a href="http://logyca.com" target="_blank">LOGYCA Company</a>
+* <a href="https://www.youtube.com/channel/UCzcJtxfScoAtwFbxaLNnEtA" target="_blank">LOGYCA Youtube Channel</a>
+* <a href="https://www.linkedin.com/company/logyca" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="Linkedin"></a>
+* <a href="https://twitter.com/LOGYCA_Org" target="_blank"><img src="https://img.shields.io/badge/Twitter-1DA1F2?style=for-the-badge&logo=twitter&logoColor=white" alt="Twitter"></a>
+* <a href="https://www.facebook.com/OrganizacionLOGYCA/" target="_blank"><img src="https://img.shields.io/badge/Facebook-1877F2?style=for-the-badge&logo=facebook&logoColor=white" alt="Facebook"></a>
+
+---
+
+# What's libraries
+
+* **Traversal libraries**: Standard methods to be used by microservices.
+* **Return codes**: Standard methods for reporting result status codes using APIResult.
+* **Monitoring**: Standard methods to report check health status codes.
+* **Helpers**: Standard methods to be used. *
+
+---
+
+---
+
+# "pip install" dependency check
+The user must select the required libraries and versions for the project that uses this library, which validates that they are pre-installed in order to be installed.
+
+To install the libraries of the logyca package (APIResult,Health) verifying the pydantic,pytz prerequisite without validating other packages, use the following command:
+
+```Python
+# Check pydantic dependency that is installed
+pip install logyca
+```
+
+To install the fastapi package libraries and logyca authentication dependency injection, use the following command:
+
+```Python
+# Check the aiohttp dependency that is installed, for use with oauth authentication, e.g. single sign-on (SSO).
+pip install logyca[oauth_token]
+# Check the fastapi dependency that is installed, for use with Api-key authentication.
+pip install logyca[api_key_simple_auth]
+# Check the fastapi dependency that is installed, for use with Api-key and oauth authentication.
+pip install logyca[oauth_token-api_key_simple_auth]
+```
+
+---
+
+# Semantic Versioning
+
+logyca < MAJOR >.< MINOR >.< PATCH >
+
+* **MAJOR**: version when you make incompatible API changes
+* **MINOR**: version when you add functionality in a backwards compatible manner
+* **PATCH**: version when you make backwards compatible bug fixes
+
+## Definitions for releasing versions
+* https://peps.python.org/pep-0440/
+
+    - X.YaN (Alpha release): Identify and fix early-stage bugs. Not suitable for production use.
+    - X.YbN (Beta release): Stabilize and refine features. Address reported bugs. Prepare for official release.
+    - X.YrcN (Release candidate): Final version before official release. Assumes all major features are complete and stable. Recommended for testing in non-critical environments.
+    - X.Y (Final release/Stable/Production): Completed, stable version ready for use in production. Full release for public use.
+
+# Quick install
+
+```console
+# Windows
+python -m pip install logyca
+# Linux
+pip install logyca
+```
+
+---
+
+# Example of concepts using library APIResult
+
+```python
+# Example output from ApiResult:
+result={
+  "resultToken": {
+    "token": "",
+    "refreshToken": "",
+    "result": "",
+    "emailActiveDirectory": "",
+    "message": ""
+  },
+  "resultObject": [
+    {
+      "name": "Database server",
+      "status": 0,
+      "description": "Connection status fine"
+    },
+    {
+      "name": "Redis server",
+      "status": 0,
+      "description": "Connection status fine"
+    }
+  ],
+  "apiException": {
+    "message": "",
+    "isError": false,
+    "detail": null,
+    "status": 200,
+    "logycaStatus": 0
+  },
+  "resultMessage": "",
+  "dataError": false
+}
+```
+
+## Use cases: you must catch de exception
+
+1. if you get data only the token:
+```json
+{
+"dataError":false,
+"resultObject":null,
+"resultToken":"Not Null"
+}
+```
+
+2. if you get data correctly
+```json
+{
+"dataError":false,
+"resultObject"="Not Null"
+"resultToken"=null
+}
+```
+
+3. if you don't get because the operation was cancelled
+```json
+{
+"dataError":true,
+"resultObject":null,
+"resultToken":null,
+"apiException.logycaStatus":1,
+"apiException.status"=404,
+"resultMessage":"exception messages: the operation was cancelled"
+}
+```
+[optional]apiException.message="if needed, return an object with structured failure data other than exception messages"
+
+
+# Example of using library APIResult + Health Check
+
+```python
+
+from logyca import HealthEnum, LogycaStatusEnum, APIResultDTO, ApiFilterExceptionDTO, HTTPExceptionDTO, HealthDTO, TokensDTO
+
+tokensDTO=TokensDTO()
+tokensDTO.token='Token Example'
+
+apiFilterExceptionDTO=ApiFilterExceptionDTO()
+apiFilterExceptionDTO.isError=False
+apiFilterExceptionDTO.logycaStatus=LogycaStatusEnum.Already_Exists
+apiFilterExceptionDTO.status=LogycaStatusEnum.Already_Exists.mappingHttpStatusCode
+
+httpExceptionDTO=HTTPExceptionDTO()
+httpExceptionDTO.detail='No Problem'
+
+listHealth=[]
+
+listHealth.append(HealthDTO(name='Check CPU',status=HealthEnum.Ok,description='OK'))
+listHealth.append(HealthDTO(name='Check Connect DB',status=HealthEnum.Warning,description='Warning'))
+listHealth.append(HealthDTO(name='Check Connect Storage',status=HealthEnum.Critical,description='Critical'))
+
+
+apiResultDTO=APIResultDTO()
+apiResultDTO.resultMessage=httpExceptionDTO.detail
+apiResultDTO.resultObject=listHealth
+apiResultDTO.dataError=False
+apiResultDTO.resultToken=tokensDTO
+apiResultDTO.apiException=apiFilterExceptionDTO
+
+print(apiResultDTO.resultToken)
+for item in apiResultDTO.resultObject:
+    print(f'name={item.name},status={item.status},description={item.description}')
+print(apiResultDTO.resultToken)
+
+# output
+# token='Token Example' refreshToken='' result='' emailActiveDirectory='' message=''
+# name=Check CPU,status=0,description=OK
+# name=Check Connect DB,status=1,description=Warning
+# name=Check Connect Storage,status=2,description=Critical
+# token='Token Example' refreshToken='' result='' emailActiveDirectory='' message=''
+```
+
+---
+
+# Example of using helpers
+
+```python
+from logyca import buildUrl,convertDateTimeStampUTCtoUTCColombia
+
+url1='https://domain.com'
+url2='api/get'
+print(f'buildUrl={buildUrl(url1,url2)}')
+# ouput
+# buildUrl=https://domain.com/api/get
+
+datetimestampUTC=1679729109
+print(f'datetimeUTCColombia={convertDateTimeStampUTCtoUTCColombia(datetimestampUTC)}')
+# output
+# datetimeUTCColombia=2023-03-25 02:25:09-05:00
+```
+
+---
+
+# Example of using Logger
+At the root of the project, the logs folder is created and the types of errors are differentiated by different files.
+```python
+
+# main.py
+from logyca import Logger, ConstantsLogger
+logger = Logger(logger_name=ConstantsLogger.NAME,log_dir=FOLDER_LOGS,log_file_name=f"{App.Settings.NAME}")
+logger.info(f"message")
+
+# Other files.py
+from logyca import Logger, ConstantsLogger
+import logging
+logger = logging.getLogger(ConstantsLogger.NAME)
+
+logger.info(f"message")
+logger.error(f"message")
+
+```
+---
+
+# Current library test
+
+```console
+# Library installation
+
+# Windows
+python -m pip install logyca[test]
+# Linux
+pip install logyca
+
+# Run it
+pytest -s
+```
+
+---
+
+# Changelog
+
+All notable changes to this project will be documented in this file.
+
+The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
+and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
+
+## Types of changes
+
+- Added for new features.
+- Changed for changes in existing functionality.
+- Deprecated for soon-to-be removed features.
+- Removed for now removed features.
+- Fixed for any bug fixes.
+- Security in case of vulnerabilities.
+
+## [0.1.9] - 2023-10-03
+### Added
+- New logger functionality.
+- new authentication functionality in fastapi by dependency injection with api-key, to be used on endpoints.
+- new authentication functionality in fastapi by dependency injection with oauth (single sign on), to be used on endpoints.
+- In the samples folder of this library, there are complete working examples of using the code.
+
+## [0.1.8] - 2023-10-03
+### Fixed
+- Due to a link error in the readme to internal documents in pypi, we chose to leave the changelog at the end of the readme. 
+
+## [0.1.7] - 2023-10-02
+### Fixed
+- The url address for the logyca logo is corrected
+- Adjust return code for LogycaStatusEnum class: LogycaStatusEnum.Created==HTTPStatus.CREATED
+- Adjust return code for LogycaStatusEnum class: LogycaStatusEnum.InProcess==HTTPStatus.ACCEPTED
+- Adjust return code for LogycaStatusEnum class: LogycaStatusEnum.Partial==HTTPStatus.ACCEPTED
+- Empty files __init__.py removed
+
+## [0.1.6] - 2023-09-11
+### Fixed
+- Pydantic restriction for versions lower than 2.0 is removed
+
+## [0.1.5] - 2023-03-27
+### Added
+- Release ready for production
+
```

#### html2text {}

```diff
@@ -1,60 +1,55 @@
-Metadata-Version: 2.1 Name: logyca Version: 0.1.8 Summary: This package name is
-reserved by LOGYCA company Project-URL: Homepage, https://github.com/ccc/ccc
-Project-URL: Documentation, https://ccc/ Author-email: Jaime Andres Cardona
-Carrillo
-logyca.com> Maintainer-email: Jaime Andres Cardona Carrillo
-logyca.com> License: MIT License-File: LICENSE.txt Classifier: Development
-Status :: 4 - Beta Classifier: Environment :: Web Environment Classifier:
-Framework :: Pydantic Classifier: Framework :: Pydantic :: 1 Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Information
-Technology Classifier: Intended Audience :: System Administrators Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Classifier: Programming Language :: Python Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Topic :: Internet Classifier: Topic ::
-Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
-Classifier: Topic :: Software Development Classifier: Topic :: Software
-Development :: Libraries Classifier: Topic :: Software Development :: Libraries
-:: Application Frameworks Classifier: Topic :: Software Development ::
-Libraries :: Python Modules Classifier: Typing :: Typed Requires-Python: >=3.7
-Requires-Dist: pydantic>=1.8 Requires-Dist: pytz>=2022.1 Provides-Extra:
-logycafeaturesample Requires-Dist: sqlalchemy<2.0.8,>=1.3.18; extra ==
-'logycafeaturesample' Provides-Extra: test Requires-Dist: pytest<8.0.0,>=7.1.3;
-extra == 'test' Description-Content-Type: text/markdown
                                    _[_L_o_g_y_c_a_]
                             LLOOGGYYCCAA ppuubblliicc lliibbrraarriieess
                            _[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_y_t_h_o_n_]
 --- # About us * _L_O_G_Y_C_A_ _C_o_m_p_a_n_y * _L_O_G_Y_C_A_ _Y_o_u_t_u_b_e_ _C_h_a_n_n_e_l * _[_L_i_n_k_e_d_i_n_]*
 _[_T_w_i_t_t_e_r_]* _[_F_a_c_e_b_o_o_k_]--- # What's libraries * **Traversal libraries**: Standard
-methods to be used by microservices. * **Return codes**: Standard methods to
-report result status codes. * **Monitoring**: Standard methods to report check
-health status codes. * **Helpers**: Standard methods to be used. * --- #
-Semantic Versioning logyca .. * **MAJOR**: version when you make incompatible
-API changes * **MINOR**: version when you add functionality in a backwards
-compatible manner * **PATCH**: version when you make backwards compatible bug
-fixes # Quick install ```console # Windows python -m pip install logyca # Linux
-pip install logyca ``` --- # Example of concepts using library APIResult
-```python # Example output from ApiResult: result={ "resultToken": { "token":
-"", "refreshToken": "", "result": "", "emailActiveDirectory": "", "message": ""
-}, "resultObject": [ { "name": "Database server", "status": 0, "description":
-"Connection status fine" }, { "name": "Redis server", "status": 0,
-"description": "Connection status fine" } ], "apiException": { "message": "",
-"isError": false, "detail": null, "status": 200, "logycaStatus": 0 },
-"resultMessage": "", "dataError": false } ``` ## Use cases: you must catch de
-exception 1. if you get data only the token: ```json { "dataError":false,
-"resultObject":null, "resultToken":"Not Null" } ``` 2. if you get data
-correctly ```json { "dataError":false, "resultObject"="Not Null"
-"resultToken"=null } ``` 3. if you don't get because the operation was
-cancelled ```json { "dataError":true, "resultObject":null, "resultToken":null,
-"apiException.logycaStatus":1, "apiException.status"=404, "resultMessage":
-"exception messages: the operation was cancelled" } ```
+methods to be used by microservices. * **Return codes**: Standard methods for
+reporting result status codes using APIResult. * **Monitoring**: Standard
+methods to report check health status codes. * **Helpers**: Standard methods to
+be used. * --- --- # "pip install" dependency check The user must select the
+required libraries and versions for the project that uses this library, which
+validates that they are pre-installed in order to be installed. To install the
+libraries of the logyca package (APIResult,Health) verifying the pydantic,pytz
+prerequisite without validating other packages, use the following command:
+```Python # Check pydantic dependency that is installed pip install logyca ```
+To install the fastapi package libraries and logyca authentication dependency
+injection, use the following command: ```Python # Check the aiohttp dependency
+that is installed, for use with oauth authentication, e.g. single sign-on
+(SSO). pip install logyca[oauth_token] # Check the fastapi dependency that is
+installed, for use with Api-key authentication. pip install logyca
+[api_key_simple_auth] # Check the fastapi dependency that is installed, for use
+with Api-key and oauth authentication. pip install logyca[oauth_token-
+api_key_simple_auth] ``` --- # Semantic Versioning logyca < MAJOR >.< MINOR >.<
+PATCH > * **MAJOR**: version when you make incompatible API changes *
+**MINOR**: version when you add functionality in a backwards compatible manner
+* **PATCH**: version when you make backwards compatible bug fixes ##
+Definitions for releasing versions * https://peps.python.org/pep-0440/ - X.YaN
+(Alpha release): Identify and fix early-stage bugs. Not suitable for production
+use. - X.YbN (Beta release): Stabilize and refine features. Address reported
+bugs. Prepare for official release. - X.YrcN (Release candidate): Final version
+before official release. Assumes all major features are complete and stable.
+Recommended for testing in non-critical environments. - X.Y (Final release/
+Stable/Production): Completed, stable version ready for use in production. Full
+release for public use. # Quick install ```console # Windows python -m pip
+install logyca # Linux pip install logyca ``` --- # Example of concepts using
+library APIResult ```python # Example output from ApiResult: result=
+{ "resultToken": { "token": "", "refreshToken": "", "result": "",
+"emailActiveDirectory": "", "message": "" }, "resultObject": [ { "name":
+"Database server", "status": 0, "description": "Connection status fine" },
+{ "name": "Redis server", "status": 0, "description": "Connection status fine"
+} ], "apiException": { "message": "", "isError": false, "detail": null,
+"status": 200, "logycaStatus": 0 }, "resultMessage": "", "dataError": false }
+``` ## Use cases: you must catch de exception 1. if you get data only the
+token: ```json { "dataError":false, "resultObject":null, "resultToken":"Not
+Null" } ``` 2. if you get data correctly ```json { "dataError":false,
+"resultObject"="Not Null" "resultToken"=null } ``` 3. if you don't get because
+the operation was cancelled ```json { "dataError":true, "resultObject":null,
+"resultToken":null, "apiException.logycaStatus":1, "apiException.status"=404,
+"resultMessage":"exception messages: the operation was cancelled" } ```
 [optional]apiException.message="if needed, return an object with structured
 failure data other than exception messages" # Example of using library
 APIResult + Health Check ```python from logyca import HealthEnum,
 LogycaStatusEnum, APIResultDTO, ApiFilterExceptionDTO, HTTPExceptionDTO,
 HealthDTO, TokensDTO tokensDTO=TokensDTO() tokensDTO.token='Token Example'
 apiFilterExceptionDTO=ApiFilterExceptionDTO()
 apiFilterExceptionDTO.isError=False
@@ -78,27 +73,40 @@
 Storage,status=2,description=Critical # token='Token Example' refreshToken=''
 result='' emailActiveDirectory='' message='' ``` --- # Example of using helpers
 ```python from logyca import buildUrl,convertDateTimeStampUTCtoUTCColombia
 url1='https://domain.com' url2='api/get' print(f'buildUrl={buildUrl
 (url1,url2)}') # ouput # buildUrl=https://domain.com/api/get
 datetimestampUTC=1679729109 print(f'datetimeUTCColombia=
 {convertDateTimeStampUTCtoUTCColombia(datetimestampUTC)}') # output #
-datetimeUTCColombia=2023-03-25 02:25:09-05:00 ``` --- # Current library test
-```console # Library installation # Windows python -m pip install logyca[test]
-# Linux pip install logyca # Run it pytest -s ``` --- # Changelog All notable
-changes to this project will be documented in this file. The format is based on
-[Keep a Changelog](https://keepachangelog.com/en/1.0.0/), and this project
-adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html). ## Types
-of changes - Added for new features. - Changed for changes in existing
-functionality. - Deprecated for soon-to-be removed features. - Removed for now
-removed features. - Fixed for any bug fixes. - Security in case of
-vulnerabilities. ## [0.1.8] - 2023-10-03 ### Fixed - Due to a link error in the
-readme to internal documents in pypi, we chose to leave the changelog at the
-end of the readme. ## [0.1.7] - 2023-10-02 ### Fixed - The url address for the
-logyca logo is corrected - Adjust return code for LogycaStatusEnum class:
+datetimeUTCColombia=2023-03-25 02:25:09-05:00 ``` --- # Example of using Logger
+At the root of the project, the logs folder is created and the types of errors
+are differentiated by different files. ```python # main.py from logyca import
+Logger, ConstantsLogger logger = Logger
+(logger_name=ConstantsLogger.NAME,log_dir=FOLDER_LOGS,log_file_name=f"
+{App.Settings.NAME}") logger.info(f"message") # Other files.py from logyca
+import Logger, ConstantsLogger import logging logger = logging.getLogger
+(ConstantsLogger.NAME) logger.info(f"message") logger.error(f"message") ``` --
+- # Current library test ```console # Library installation # Windows python -
+m pip install logyca[test] # Linux pip install logyca # Run it pytest -s ``` --
+- # Changelog All notable changes to this project will be documented in this
+file. The format is based on [Keep a Changelog](https://keepachangelog.com/en/
+1.0.0/), and this project adheres to [Semantic Versioning](https://semver.org/
+spec/v2.0.0.html). ## Types of changes - Added for new features. - Changed for
+changes in existing functionality. - Deprecated for soon-to-be removed
+features. - Removed for now removed features. - Fixed for any bug fixes. -
+Security in case of vulnerabilities. ## [0.1.9] - 2023-10-03 ### Added - New
+logger functionality. - new authentication functionality in fastapi by
+dependency injection with api-key, to be used on endpoints. - new
+authentication functionality in fastapi by dependency injection with oauth
+(single sign on), to be used on endpoints. - In the samples folder of this
+library, there are complete working examples of using the code. ## [0.1.8] -
+2023-10-03 ### Fixed - Due to a link error in the readme to internal documents
+in pypi, we chose to leave the changelog at the end of the readme. ## [0.1.7] -
+2023-10-02 ### Fixed - The url address for the logyca logo is corrected -
+Adjust return code for LogycaStatusEnum class:
 LogycaStatusEnum.Created==HTTPStatus.CREATED - Adjust return code for
 LogycaStatusEnum class: LogycaStatusEnum.InProcess==HTTPStatus.ACCEPTED -
 Adjust return code for LogycaStatusEnum class:
 LogycaStatusEnum.Partial==HTTPStatus.ACCEPTED - Empty files __init__.py removed
 ## [0.1.6] - 2023-09-11 ### Fixed - Pydantic restriction for versions lower
 than 2.0 is removed ## [0.1.5] - 2023-03-27 ### Added - Release ready for
 production
```

