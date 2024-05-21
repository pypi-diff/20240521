# Comparing `tmp/aonet-1.0.2.tar.gz` & `tmp/aonet-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aonet-1.0.2.tar", last modified: Wed May 15 06:17:48 2024, max compression
+gzip compressed data, was "aonet-1.0.3.tar", last modified: Tue May 21 06:04:05 2024, max compression
```

## Comparing `aonet-1.0.2.tar` & `aonet-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-15 06:17:48.221433 aonet-1.0.2/
--rw-r--r--   0 brent      (501) staff       (20)      126 2024-05-15 06:17:48.221166 aonet-1.0.2/PKG-INFO
--rw-rw-r--   0 brent      (501) staff       (20)     1577 2024-05-15 06:16:49.000000 aonet-1.0.2/README.md
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-15 06:17:48.218608 aonet-1.0.2/aonet/
--rw-r--r--   0 brent      (501) staff       (20)       23 2024-05-15 06:16:41.000000 aonet-1.0.2/aonet/__init__.py
--rw-r--r--   0 brent      (501) staff       (20)     2283 2024-05-15 06:16:43.000000 aonet-1.0.2/aonet/aonet.py
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-15 06:17:48.220899 aonet-1.0.2/aonet.egg-info/
--rw-r--r--   0 brent      (501) staff       (20)      126 2024-05-15 06:17:48.000000 aonet-1.0.2/aonet.egg-info/PKG-INFO
--rw-r--r--   0 brent      (501) staff       (20)      209 2024-05-15 06:17:48.000000 aonet-1.0.2/aonet.egg-info/SOURCES.txt
--rw-r--r--   0 brent      (501) staff       (20)        1 2024-05-15 06:17:48.000000 aonet-1.0.2/aonet.egg-info/dependency_links.txt
--rw-r--r--   0 brent      (501) staff       (20)       12 2024-05-15 06:17:48.000000 aonet-1.0.2/aonet.egg-info/requires.txt
--rw-r--r--   0 brent      (501) staff       (20)        6 2024-05-15 06:17:48.000000 aonet-1.0.2/aonet.egg-info/top_level.txt
--rw-r--r--   0 brent      (501) staff       (20)       38 2024-05-15 06:17:48.221597 aonet-1.0.2/setup.cfg
--rw-r--r--   0 brent      (501) staff       (20)      283 2024-05-15 06:17:20.000000 aonet-1.0.2/setup.py
-drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-15 06:17:48.220647 aonet-1.0.2/tests/
--rw-r--r--   0 brent      (501) staff       (20)      660 2024-05-15 06:16:46.000000 aonet-1.0.2/tests/test.py
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-21 06:04:05.597226 aonet-1.0.3/
+-rw-r--r--   0 brent      (501) staff       (20)      126 2024-05-21 06:04:05.596940 aonet-1.0.3/PKG-INFO
+-rw-rw-r--   0 brent      (501) staff       (20)     1575 2024-05-21 06:02:23.000000 aonet-1.0.3/README.md
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-21 06:04:05.595221 aonet-1.0.3/aonet/
+-rw-r--r--   0 brent      (501) staff       (20)       23 2024-05-21 06:01:07.000000 aonet-1.0.3/aonet/__init__.py
+-rw-r--r--   0 brent      (501) staff       (20)     2282 2024-05-21 06:01:49.000000 aonet-1.0.3/aonet/aonet.py
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-21 06:04:05.596651 aonet-1.0.3/aonet.egg-info/
+-rw-r--r--   0 brent      (501) staff       (20)      126 2024-05-21 06:04:05.000000 aonet-1.0.3/aonet.egg-info/PKG-INFO
+-rw-r--r--   0 brent      (501) staff       (20)      209 2024-05-21 06:04:05.000000 aonet-1.0.3/aonet.egg-info/SOURCES.txt
+-rw-r--r--   0 brent      (501) staff       (20)        1 2024-05-21 06:04:05.000000 aonet-1.0.3/aonet.egg-info/dependency_links.txt
+-rw-r--r--   0 brent      (501) staff       (20)       12 2024-05-21 06:04:05.000000 aonet-1.0.3/aonet.egg-info/requires.txt
+-rw-r--r--   0 brent      (501) staff       (20)        6 2024-05-21 06:04:05.000000 aonet-1.0.3/aonet.egg-info/top_level.txt
+-rw-r--r--   0 brent      (501) staff       (20)       38 2024-05-21 06:04:05.597288 aonet-1.0.3/setup.cfg
+-rw-r--r--   0 brent      (501) staff       (20)      283 2024-05-21 06:03:56.000000 aonet-1.0.3/setup.py
+drwxr-xr-x   0 brent      (501) staff       (20)        0 2024-05-21 06:04:05.596243 aonet-1.0.3/tests/
+-rw-r--r--   0 brent      (501) staff       (20)      653 2024-05-21 06:02:07.000000 aonet-1.0.3/tests/test.py
```

### Comparing `aonet-1.0.2/README.md` & `aonet-1.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 ```python
 from aonet import aonet
 
 #get your api key or jwt token from https://console.aonet.ai
 api_key = "my api key or jwt token"
 
-aonet_instance = aonet.AON(api_key)
+aonet_instance = aonet.AI(api_key)
 
 data = {
     "input":{
         "seed": 36446545872,
         "width": 768,
         "height": 768,
         "prompt": "with smoke, half ice and half fire and ultra realistic in detail.wolf, typography, dark fantasy, wildlife photography, vibrant, cinematic and on a black background",
@@ -53,15 +53,15 @@
 ## API
 
 All URIs are relative to *https://api.aonet.ai*
 
 ### Constructor
 
 ```javascript
-aonet_instance = aonet.AON(auth,host,headers)
+aonet_instance = aonet.AI(auth,host,headers)
 ```
 
 name | type | Description
 ------------ | ------------- | -------------
 *host* | string | The request host
 *auth* | string | **Required**.You can choose either API key or JWT token for authentication.
```

### Comparing `aonet-1.0.2/aonet/aonet.py` & `aonet-1.0.3/aonet/aonet.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     JWT = 2
     NONE = 3
 
 
 default_path = {AuthType.API: "/api", AuthType.JWT: "/jwt"}
 
 
-class AON:
+class AI:
     def __init__(self,
                  auth:str,
                  host:str = None,
                  headers:Optional[Dict[str,Any]] = None) -> None:
         super().__init__()
 
         if auth is None or auth == "":
```

### Comparing `aonet-1.0.2/tests/test.py` & `aonet-1.0.3/tests/test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import aonet.aonet as aonet
+import aonet as aonet
 
 api_key = "4oipB83LZCpkrVN3i12f38WcBUYH5MR9"
 
-aonet_instance = aonet.AON(api_key)
+aonet_instance = aonet.AI(api_key)
 
 data = {
     "input":{
         "seed": 36446545872,
         "width": 768,
         "height": 768,
         "prompt": "with smoke, half ice and half fire and ultra realistic in detail.wolf, typography, dark fantasy, wildlife photography, vibrant, cinematic and on a black background",
```

