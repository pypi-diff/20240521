# Comparing `tmp/tencentcloud-sdk-python-hai-3.0.1149.tar.gz` & `tmp/tencentcloud-sdk-python-hai-3.0.1151.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-hai-3.0.1149.tar", last modified: Thu May 16 20:41:49 2024, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-hai-3.0.1151.tar", last modified: Mon May 20 20:42:17 2024, max compression
```

## Comparing `tencentcloud-sdk-python-hai-3.0.1149.tar` & `tencentcloud-sdk-python-hai-3.0.1151.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud_sdk_python_hai.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud_sdk_python_hai.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       13 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud_sdk_python_hai.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       40 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud_sdk_python_hai.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      495 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud_sdk_python_hai.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud_sdk_python_hai.egg-info/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      631 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud/hai/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud/hai/v20230812/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud/hai/v20230812/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10865 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud/hai/v20230812/hai_client.py
--rw-r--r--   0 root         (0) root         (0)     4636 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud/hai/v20230812/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    65206 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud/hai/v20230812/models.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/tencentcloud/hai/__init__.py
--rw-r--r--   0 root         (0) root         (0)      737 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/README.rst
--rw-r--r--   0 root         (0) root         (0)     1073 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/setup.py
--rw-r--r--   0 root         (0) root         (0)       88 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1660 2024-05-16 20:41:49.000000 tencentcloud-sdk-python-hai-3.0.1149/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud_sdk_python_hai.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud_sdk_python_hai.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud_sdk_python_hai.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud_sdk_python_hai.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      495 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud_sdk_python_hai.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud_sdk_python_hai.egg-info/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      631 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud/hai/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud/hai/v20230812/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud/hai/v20230812/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10865 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud/hai/v20230812/hai_client.py
+-rw-r--r--   0 root         (0) root         (0)     4636 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud/hai/v20230812/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    65206 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud/hai/v20230812/models.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/tencentcloud/hai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      737 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/README.rst
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/setup.py
+-rw-r--r--   0 root         (0) root         (0)       88 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1660 2024-05-20 20:42:17.000000 tencentcloud-sdk-python-hai-3.0.1151/PKG-INFO
```

### Comparing `tencentcloud-sdk-python-hai-3.0.1149/tencentcloud_sdk_python_hai.egg-info/PKG-INFO` & `tencentcloud-sdk-python-hai-3.0.1151/tencentcloud_sdk_python_hai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hai
-Version: 3.0.1149
+Version: 3.0.1151
 Summary: Tencent Cloud Hai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-hai-3.0.1149/tencentcloud/__init__.py` & `tencentcloud-sdk-python-hai-3.0.1151/tencentcloud/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.1149'
+__version__ = '3.0.1151'
```

### Comparing `tencentcloud-sdk-python-hai-3.0.1149/tencentcloud/hai/v20230812/hai_client.py` & `tencentcloud-sdk-python-hai-3.0.1151/tencentcloud/hai/v20230812/hai_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hai-3.0.1149/tencentcloud/hai/v20230812/errorcodes.py` & `tencentcloud-sdk-python-hai-3.0.1151/tencentcloud/hai/v20230812/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hai-3.0.1149/tencentcloud/hai/v20230812/models.py` & `tencentcloud-sdk-python-hai-3.0.1151/tencentcloud/hai/v20230812/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hai-3.0.1149/README.rst` & `tencentcloud-sdk-python-hai-3.0.1151/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-hai-3.0.1149/setup.py` & `tencentcloud-sdk-python-hai-3.0.1151/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-hai',
-    install_requires=["tencentcloud-sdk-python-common==3.0.1149"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.1151"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Hai SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```

### Comparing `tencentcloud-sdk-python-hai-3.0.1149/PKG-INFO` & `tencentcloud-sdk-python-hai-3.0.1151/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-hai
-Version: 3.0.1149
+Version: 3.0.1151
 Summary: Tencent Cloud Hai SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```
