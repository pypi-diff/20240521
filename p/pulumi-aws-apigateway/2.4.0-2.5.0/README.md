# Comparing `tmp/pulumi_aws_apigateway-2.4.0.tar.gz` & `tmp/pulumi_aws_apigateway-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_aws_apigateway-2.4.0.tar", last modified: Wed Feb 28 12:07:19 2024, max compression
+gzip compressed data, was "pulumi_aws_apigateway-2.5.0.tar", last modified: Tue May 21 07:55:25 2024, max compression
```

## Comparing `pulumi_aws_apigateway-2.4.0.tar` & `pulumi_aws_apigateway-2.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 12:07:19.943712 pulumi_aws_apigateway-2.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-02-28 12:07:19.943712 pulumi_aws_apigateway-2.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-02-28 12:07:04.000000 pulumi_aws_apigateway-2.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 12:07:19.943712 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/
--rw-------   0 runner    (1001) docker     (127)      716 2024-02-28 12:07:04.000000 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1127 2024-02-28 12:07:04.000000 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/_enums.py
--rw-------   0 runner    (1001) docker     (127)    37712 2024-02-28 12:07:04.000000 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     9228 2024-02-28 12:07:04.000000 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/_utilities.py
--rw-------   0 runner    (1001) docker     (127)     2754 2024-02-28 12:07:04.000000 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/provider.py
--rw-------   0 runner    (1001) docker     (127)       51 2024-02-28 12:07:04.000000 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-02-28 12:07:04.000000 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/py.typed
--rw-------   0 runner    (1001) docker     (127)    19936 2024-02-28 12:07:04.000000 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/rest_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-28 12:07:19.943712 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-02-28 12:07:19.000000 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      523 2024-02-28 12:07:19.000000 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-28 12:07:19.000000 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-02-28 12:07:19.000000 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-02-28 12:07:19.000000 pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      722 2024-02-28 12:07:04.000000 pulumi_aws_apigateway-2.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-28 12:07:19.943712 pulumi_aws_apigateway-2.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:55:25.427430 pulumi_aws_apigateway-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-21 07:55:25.427430 pulumi_aws_apigateway-2.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2432 2024-05-21 07:55:18.000000 pulumi_aws_apigateway-2.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:55:25.423431 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/
+-rw-------   0 runner    (1001) docker     (127)      716 2024-05-21 07:55:18.000000 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1127 2024-05-21 07:55:18.000000 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    37712 2024-05-21 07:55:18.000000 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     9228 2024-05-21 07:55:18.000000 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/_utilities.py
+-rw-------   0 runner    (1001) docker     (127)     2754 2024-05-21 07:55:18.000000 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/provider.py
+-rw-------   0 runner    (1001) docker     (127)       51 2024-05-21 07:55:18.000000 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-05-21 07:55:18.000000 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/py.typed
+-rw-------   0 runner    (1001) docker     (127)    21385 2024-05-21 07:55:18.000000 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/rest_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:55:25.427430 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-21 07:55:25.000000 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-21 07:55:25.000000 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:55:25.000000 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-21 07:55:25.000000 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 07:55:25.000000 pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      722 2024-05-21 07:55:18.000000 pulumi_aws_apigateway-2.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 07:55:25.427430 pulumi_aws_apigateway-2.5.0/setup.cfg
```

### Comparing `pulumi_aws_apigateway-2.4.0/PKG-INFO` & `pulumi_aws_apigateway-2.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_aws_apigateway
-Version: 2.4.0
+Version: 2.5.0
 Summary: Pulumi Amazon Web Services (AWS) API Gateway Components.
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aws-apigateway
 Keywords: pulumi,aws,apigateway,category/cloud,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_aws_apigateway Version: 2.4.0 Summary:
+Metadata-Version: 2.1 Name: pulumi_aws_apigateway Version: 2.5.0 Summary:
 Pulumi Amazon Web Services (AWS) API Gateway Components. License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aws-apigateway
 Keywords: pulumi,aws,apigateway,category/cloud,kind/component Requires-Python:
 >=3.8 Description-Content-Type: text/markdown Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.0.0 Requires-Dist: pulumi-aws<7.0.0,>=6.0.0
 Requires-Dist: semver>=2.8.1 [![Actions Status](https://github.com/pulumi/
 pulumi-aws-apigateway/workflows/release/badge.svg)](https://github.com/pulumi/
```

### Comparing `pulumi_aws_apigateway-2.4.0/README.md` & `pulumi_aws_apigateway-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/__init__.py` & `pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/_enums.py` & `pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/_inputs.py` & `pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/_utilities.py` & `pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/provider.py` & `pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway/rest_api.py` & `pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway/rest_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,16 @@
                  description: Optional[pulumi.Input[str]] = None,
                  disable_execute_api_endpoint: Optional[pulumi.Input[bool]] = None,
                  gateway_responses: Optional[Mapping[str, pulumi.Input['SwaggerGatewayResponseArgs']]] = None,
                  request_validator: Optional['RequestValidator'] = None,
                  routes: Optional[Sequence['RouteArgs']] = None,
                  stage_name: Optional[pulumi.Input[str]] = None,
                  static_routes_bucket: Optional[pulumi.Input['pulumi_aws.s3.Bucket']] = None,
-                 swagger_string: Optional[pulumi.Input[str]] = None):
+                 swagger_string: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a RestAPI resource.
         :param 'APIKeySource' api_key_source: The source for the apikey. This can either be a HEADER or AUTHORIZER. If `apiKeyRequired` is
                set to true on a route, and this is not defined the value will default to HEADER.
         :param Sequence[pulumi.Input[str]] binary_media_types: List of binary media types supported by the REST API. By default, the REST API supports only UTF-8-encoded text payloads. 
                If importing an OpenAPI specification via the body argument, this corresponds to the x-amazon-apigateway-binary-media-types extension. 
                If the argument value is provided and is different than the OpenAPI value, the argument value will override the OpenAPI value.
@@ -50,14 +51,16 @@
         :param pulumi.Input['pulumi_aws.s3.Bucket'] static_routes_bucket: Bucket to use for placing resources for static resources.  If not provided a default one will
                be created on your behalf if any `StaticRoute`s are provided.
         :param pulumi.Input[str] swagger_string: A Swagger specification already in string form to use to initialize the APIGateway.  Note
                that you must manually provide permission for any route targets to be invoked by API Gateway
                when using `swaggerString`.
                
                Either `swaggerString` or `routes` must be specified.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: 'Map of tags to assign to the resource. If configured with a provider `defaultTags` configuration block present,
+               tags with matching keys will overwrite those defined at the provider-level.
         """
         if api_key_source is not None:
             pulumi.set(__self__, "api_key_source", api_key_source)
         if binary_media_types is not None:
             pulumi.set(__self__, "binary_media_types", binary_media_types)
         if description is not None:
             pulumi.set(__self__, "description", description)
@@ -71,14 +74,16 @@
             pulumi.set(__self__, "routes", routes)
         if stage_name is not None:
             pulumi.set(__self__, "stage_name", stage_name)
         if static_routes_bucket is not None:
             pulumi.set(__self__, "static_routes_bucket", static_routes_bucket)
         if swagger_string is not None:
             pulumi.set(__self__, "swagger_string", swagger_string)
+        if tags is not None:
+            pulumi.set(__self__, "tags", tags)
 
     @property
     @pulumi.getter(name="apiKeySource")
     def api_key_source(self) -> Optional['APIKeySource']:
         """
         The source for the apikey. This can either be a HEADER or AUTHORIZER. If `apiKeyRequired` is
         set to true on a route, and this is not defined the value will default to HEADER.
@@ -207,14 +212,27 @@
         """
         return pulumi.get(self, "swagger_string")
 
     @swagger_string.setter
     def swagger_string(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "swagger_string", value)
 
+    @property
+    @pulumi.getter
+    def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
+        """
+        'Map of tags to assign to the resource. If configured with a provider `defaultTags` configuration block present,
+        tags with matching keys will overwrite those defined at the provider-level.
+        """
+        return pulumi.get(self, "tags")
+
+    @tags.setter
+    def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
+        pulumi.set(self, "tags", value)
+
 
 class RestAPI(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  api_key_source: Optional['APIKeySource'] = None,
@@ -223,14 +241,15 @@
                  disable_execute_api_endpoint: Optional[pulumi.Input[bool]] = None,
                  gateway_responses: Optional[Mapping[str, pulumi.Input[pulumi.InputType['SwaggerGatewayResponseArgs']]]] = None,
                  request_validator: Optional['RequestValidator'] = None,
                  routes: Optional[Sequence[pulumi.InputType['RouteArgs']]] = None,
                  stage_name: Optional[pulumi.Input[str]] = None,
                  static_routes_bucket: Optional[pulumi.Input['pulumi_aws.s3.Bucket']] = None,
                  swagger_string: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
         """
         The RestAPI component offers a simple interface for creating a fully functional API Gateway REST API. The
         REST API can define any number of routes, each of which maps a path and HTTP method to one of (1) an event
         hander route that invokes a Lambda Function (2) a local path route which uploads local files into an S3 bucket
         and serves them or (3) an integration target such as an HTTP proxy or service integration.
 
@@ -257,14 +276,16 @@
         :param pulumi.Input['pulumi_aws.s3.Bucket'] static_routes_bucket: Bucket to use for placing resources for static resources.  If not provided a default one will
                be created on your behalf if any `StaticRoute`s are provided.
         :param pulumi.Input[str] swagger_string: A Swagger specification already in string form to use to initialize the APIGateway.  Note
                that you must manually provide permission for any route targets to be invoked by API Gateway
                when using `swaggerString`.
                
                Either `swaggerString` or `routes` must be specified.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: 'Map of tags to assign to the resource. If configured with a provider `defaultTags` configuration block present,
+               tags with matching keys will overwrite those defined at the provider-level.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[RestAPIArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
@@ -295,14 +316,15 @@
                  disable_execute_api_endpoint: Optional[pulumi.Input[bool]] = None,
                  gateway_responses: Optional[Mapping[str, pulumi.Input[pulumi.InputType['SwaggerGatewayResponseArgs']]]] = None,
                  request_validator: Optional['RequestValidator'] = None,
                  routes: Optional[Sequence[pulumi.InputType['RouteArgs']]] = None,
                  stage_name: Optional[pulumi.Input[str]] = None,
                  static_routes_bucket: Optional[pulumi.Input['pulumi_aws.s3.Bucket']] = None,
                  swagger_string: Optional[pulumi.Input[str]] = None,
+                 tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
@@ -316,14 +338,15 @@
             __props__.__dict__["disable_execute_api_endpoint"] = disable_execute_api_endpoint
             __props__.__dict__["gateway_responses"] = gateway_responses
             __props__.__dict__["request_validator"] = request_validator
             __props__.__dict__["routes"] = routes
             __props__.__dict__["stage_name"] = stage_name
             __props__.__dict__["static_routes_bucket"] = static_routes_bucket
             __props__.__dict__["swagger_string"] = swagger_string
+            __props__.__dict__["tags"] = tags
             __props__.__dict__["api"] = None
             __props__.__dict__["api_policy"] = None
             __props__.__dict__["deployment"] = None
             __props__.__dict__["stage"] = None
             __props__.__dict__["url"] = None
         super(RestAPI, __self__).__init__(
             'aws-apigateway:index:RestAPI',
```

### Comparing `pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway.egg-info/PKG-INFO` & `pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_aws_apigateway
-Version: 2.4.0
+Version: 2.5.0
 Summary: Pulumi Amazon Web Services (AWS) API Gateway Components.
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aws-apigateway
 Keywords: pulumi,aws,apigateway,category/cloud,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pulumi_aws_apigateway Version: 2.4.0 Summary:
+Metadata-Version: 2.1 Name: pulumi_aws_apigateway Version: 2.5.0 Summary:
 Pulumi Amazon Web Services (AWS) API Gateway Components. License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-aws-apigateway
 Keywords: pulumi,aws,apigateway,category/cloud,kind/component Requires-Python:
 >=3.8 Description-Content-Type: text/markdown Requires-Dist: parver>=0.2.1
 Requires-Dist: pulumi<4.0.0,>=3.0.0 Requires-Dist: pulumi-aws<7.0.0,>=6.0.0
 Requires-Dist: semver>=2.8.1 [![Actions Status](https://github.com/pulumi/
 pulumi-aws-apigateway/workflows/release/badge.svg)](https://github.com/pulumi/
```

### Comparing `pulumi_aws_apigateway-2.4.0/pulumi_aws_apigateway.egg-info/SOURCES.txt` & `pulumi_aws_apigateway-2.5.0/pulumi_aws_apigateway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_aws_apigateway-2.4.0/pyproject.toml` & `pulumi_aws_apigateway-2.5.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_aws_apigateway"
   description = "Pulumi Amazon Web Services (AWS) API Gateway Components."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "pulumi-aws>=6.0.0,<7.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "aws", "apigateway", "category/cloud", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.4.0"
+  version = "2.5.0"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/pulumi/pulumi-aws-apigateway"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

