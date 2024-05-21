# Comparing `tmp/tencentcloud-sdk-python-vcg-3.0.1150.tar.gz` & `tmp/tencentcloud-sdk-python-vcg-3.0.1151.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-vcg-3.0.1150.tar", last modified: Sun May 19 21:44:10 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-vcg-3.0.1151.tar", last modified: Mon May 20 21:07:13 2024, max compression
```

## Comparing `tencentcloud-sdk-python-vcg-3.0.1150.tar` & `tencentcloud-sdk-python-vcg-3.0.1151.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud/vcg/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud/vcg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud/vcg/v20240404/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud/vcg/v20240404/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2341 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud/vcg/v20240404/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     6212 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud/vcg/v20240404/models.py
--rw-r--r--   0 root         (0) root         (0)     3266 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud/vcg/v20240404/vcg_client.py
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud_sdk_python_vcg.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud_sdk_python_vcg.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud_sdk_python_vcg.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud_sdk_python_vcg.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud_sdk_python_vcg.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud_sdk_python_vcg.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/README.rst
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-19 21:44:10.000000 tencentcloud-sdk-python-vcg-3.0.1150/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud/vcg/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud/vcg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud/vcg/v20240404/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud/vcg/v20240404/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2341 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud/vcg/v20240404/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     6212 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud/vcg/v20240404/models.py
+-rw-r--r--   0 root         (0) root         (0)     3266 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud/vcg/v20240404/vcg_client.py
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud_sdk_python_vcg.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud_sdk_python_vcg.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud_sdk_python_vcg.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud_sdk_python_vcg.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud_sdk_python_vcg.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud_sdk_python_vcg.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2024-05-20 21:07:12.000000 tencentcloud-sdk-python-vcg-3.0.1151/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-20 21:07:12.000000 tencentcloud-sdk-python-vcg-3.0.1151/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-20 21:07:13.000000 tencentcloud-sdk-python-vcg-3.0.1151/PKG-INFO
```

### Comparing `tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud/vcg/v20240404/errorcodes.py` & `tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud/vcg/v20240404/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud/vcg/v20240404/models.py` & `tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud/vcg/v20240404/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud/vcg/v20240404/vcg_client.py` & `tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud/vcg/v20240404/vcg_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud/__init__.py` & `tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1150'
+__version__ = '3.0.1151'
```

### Comparing `tencentcloud-sdk-python-vcg-3.0.1150/tencentcloud_sdk_python_vcg.egg-info/PKG-INFO` & `tencentcloud-sdk-python-vcg-3.0.1151/tencentcloud_sdk_python_vcg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vcg
-Version: 3.0.1150
+Version: 3.0.1151
 Summary: Tencent Cloud Vcg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-vcg-3.0.1150/README.rst` & `tencentcloud-sdk-python-vcg-3.0.1151/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-vcg-3.0.1150/setup.py` & `tencentcloud-sdk-python-vcg-3.0.1151/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-vcg',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1150"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1151"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Vcg SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-vcg-3.0.1150/PKG-INFO` & `tencentcloud-sdk-python-vcg-3.0.1151/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-vcg
-Version: 3.0.1150
+Version: 3.0.1151
 Summary: Tencent Cloud Vcg SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```
