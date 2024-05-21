# Comparing `tmp/gammarers.aws-frontend-web-app-deploy-stack-1.2.4.tar.gz` & `tmp/gammarers.aws-frontend-web-app-deploy-stack-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gammarers.aws-frontend-web-app-deploy-stack-1.2.4.tar", last modified: Tue May 14 19:13:23 2024, max compression
+gzip compressed data, was "gammarers.aws-frontend-web-app-deploy-stack-1.2.5.tar", last modified: Tue May 21 19:16:34 2024, max compression
```

## Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.4.tar` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:13:23.103896 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-14 19:13:12.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-14 19:13:12.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-14 19:13:23.103896 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-14 19:13:12.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-14 19:13:12.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 19:13:23.103896 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-14 19:13:12.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:13:23.099896 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:13:23.099896 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:13:23.103896 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers/aws_frontend_web_app_deploy_stack/
--rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-05-14 19:13:12.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:13:23.103896 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-14 19:13:12.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36126 2024-05-14 19:13:12.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.4.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:13:12.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers/aws_frontend_web_app_deploy_stack/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 19:13:23.103896 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-14 19:13:23.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-14 19:13:23.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 19:13:23.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-14 19:13:23.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-14 19:13:23.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:16:34.701773 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-21 19:16:22.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 19:16:22.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-21 19:16:34.701773 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-21 19:16:22.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-21 19:16:22.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 19:16:34.701773 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-21 19:16:22.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:16:34.697773 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:16:34.697773 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:16:34.701773 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers/aws_frontend_web_app_deploy_stack/
+-rw-r--r--   0 runner    (1001) docker     (127)    27776 2024-05-21 19:16:22.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:16:34.701773 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      708 2024-05-21 19:16:22.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36129 2024-05-21 19:16:22.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.5.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:16:22.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers/aws_frontend_web_app_deploy_stack/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:16:34.701773 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-05-21 19:16:34.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-21 19:16:34.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:16:34.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-21 19:16:34.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 19:16:34.000000 gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.4/LICENSE` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.4/PKG-INFO` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-frontend-web-app-deploy-stack
-Version: 1.2.4
+Version: 1.2.5
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.4/README.md` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.4/setup.py` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "gammarers.aws-frontend-web-app-deploy-stack",
-    "version": "1.2.4",
+    "version": "1.2.5",
     "description": "This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.",
     "license": "Apache-2.0",
     "url": "https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git",
     "long_description_content_type": "text/markdown",
     "author": "yicr<yicr@users.noreply.github.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "gammarers.aws_frontend_web_app_deploy_stack",
         "gammarers.aws_frontend_web_app_deploy_stack._jsii"
     ],
     "package_data": {
         "gammarers.aws_frontend_web_app_deploy_stack._jsii": [
-            "aws-frontend-web-app-deploy-stack@1.2.4.jsii.tgz"
+            "aws-frontend-web-app-deploy-stack@1.2.5.jsii.tgz"
         ],
         "gammarers.aws_frontend_web_app_deploy_stack": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py`

 * *Files identical despite different names*

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
 import constructs._jsii
 import gammarers.aws_secure_bucket._jsii
 import gammarers.aws_secure_cloudfront_origin_bucket._jsii
 import gammarers.aws_secure_frontend_web_app_cloudfront_distribution._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "@gammarers/aws-frontend-web-app-deploy-stack",
-    "1.2.4",
+    "1.2.5",
     __name__[0:-6],
-    "aws-frontend-web-app-deploy-stack@1.2.4.jsii.tgz",
+    "aws-frontend-web-app-deploy-stack@1.2.5.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gammarers.aws-frontend-web-app-deploy-stack
-Version: 1.2.4
+Version: 1.2.5
 Summary: This is an AWS CDK Construct to make deploying a Frontend Web App (SPA) deploy to S3 behind CloudFront.
 Home-page: https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git
 Author: yicr<yicr@users.noreply.github.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/gammarers/aws-frontend-web-app-deploy-stack.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `gammarers.aws-frontend-web-app-deploy-stack-1.2.4/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt` & `gammarers.aws-frontend-web-app-deploy-stack-1.2.5/src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/SOURCES.txt
 src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/dependency_links.txt
 src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/requires.txt
 src/gammarers.aws_frontend_web_app_deploy_stack.egg-info/top_level.txt
 src/gammarers/aws_frontend_web_app_deploy_stack/__init__.py
 src/gammarers/aws_frontend_web_app_deploy_stack/py.typed
 src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/__init__.py
-src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.4.jsii.tgz
+src/gammarers/aws_frontend_web_app_deploy_stack/_jsii/aws-frontend-web-app-deploy-stack@1.2.5.jsii.tgz
```

