# Comparing `tmp/octoxlabs-0.4.3.tar.gz` & `tmp/octoxlabs-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "octoxlabs-0.4.3.tar", last modified: Thu May 16 19:21:07 2024, max compression
+gzip compressed data, was "octoxlabs-0.4.4.tar", last modified: Tue May 21 21:33:38 2024, max compression
```

## Comparing `octoxlabs-0.4.3.tar` & `octoxlabs-0.4.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:07.724658 octoxlabs-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-16 19:21:07.720658 octoxlabs-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:21:07.724658 octoxlabs-0.4.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:07.716658 octoxlabs-0.4.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:07.720658 octoxlabs-0.4.3/src/octoxlabs/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:07.720658 octoxlabs-0.4.3/src/octoxlabs/constants/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/constants/paths.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:07.720658 octoxlabs-0.4.3/src/octoxlabs/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/models/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/models/companies.py
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/models/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/models/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/models/users.py
--rw-r--r--   0 runner    (1001) docker     (127)    20926 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/octoxlabs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/service.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-16 19:21:01.000000 octoxlabs-0.4.3/src/octoxlabs/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:21:07.720658 octoxlabs-0.4.3/src/octoxlabs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-16 19:21:07.000000 octoxlabs-0.4.3/src/octoxlabs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-16 19:21:07.000000 octoxlabs-0.4.3/src/octoxlabs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:21:07.000000 octoxlabs-0.4.3/src/octoxlabs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 19:21:07.000000 octoxlabs-0.4.3/src/octoxlabs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-16 19:21:07.000000 octoxlabs-0.4.3/src/octoxlabs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:33:38.022823 octoxlabs-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-21 21:33:38.018823 octoxlabs-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 21:33:38.022823 octoxlabs-0.4.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:33:38.014823 octoxlabs-0.4.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:33:38.018823 octoxlabs-0.4.4/src/octoxlabs/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/src/octoxlabs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:33:38.018823 octoxlabs-0.4.4/src/octoxlabs/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/src/octoxlabs/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/src/octoxlabs/constants/paths.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/src/octoxlabs/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:33:38.018823 octoxlabs-0.4.4/src/octoxlabs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/src/octoxlabs/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2346 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/src/octoxlabs/models/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/src/octoxlabs/models/companies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/src/octoxlabs/models/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/src/octoxlabs/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/src/octoxlabs/models/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20841 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/src/octoxlabs/octoxlabs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1510 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/src/octoxlabs/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-21 21:33:32.000000 octoxlabs-0.4.4/src/octoxlabs/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 21:33:38.018823 octoxlabs-0.4.4/src/octoxlabs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2448 2024-05-21 21:33:38.000000 octoxlabs-0.4.4/src/octoxlabs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-21 21:33:38.000000 octoxlabs-0.4.4/src/octoxlabs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 21:33:38.000000 octoxlabs-0.4.4/src/octoxlabs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-21 21:33:38.000000 octoxlabs-0.4.4/src/octoxlabs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-21 21:33:38.000000 octoxlabs-0.4.4/src/octoxlabs.egg-info/top_level.txt
```

### Comparing `octoxlabs-0.4.3/LICENSE` & `octoxlabs-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `octoxlabs-0.4.3/PKG-INFO` & `octoxlabs-0.4.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoxlabs
-Version: 0.4.3
+Version: 0.4.4
 Summary: py-octoxlabs is an API client for Octox Labs Cyber Security Asset Management platform on python programming language.
 Author-email: Octox Labs Development Team <development@octoxlabs.com>
 License: MIT License
         
         Copyright (c) 2022 Octox Labs Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `octoxlabs-0.4.3/README.md` & `octoxlabs-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `octoxlabs-0.4.3/pyproject.toml` & `octoxlabs-0.4.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "octoxlabs"
-version = "0.4.3"
+version = "0.4.4"
 authors = [
   { name="Octox Labs Development Team", email="development@octoxlabs.com" },
 ]
 description = "py-octoxlabs is an API client for Octox Labs Cyber Security Asset Management platform on python programming language."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `octoxlabs-0.4.3/src/octoxlabs/constants/paths.py` & `octoxlabs-0.4.4/src/octoxlabs/constants/paths.py`

 * *Files identical despite different names*

### Comparing `octoxlabs-0.4.3/src/octoxlabs/models/adapter.py` & `octoxlabs-0.4.4/src/octoxlabs/models/adapter.py`

 * *Files identical despite different names*

### Comparing `octoxlabs-0.4.3/src/octoxlabs/models/companies.py` & `octoxlabs-0.4.4/src/octoxlabs/models/companies.py`

 * *Files identical despite different names*

### Comparing `octoxlabs-0.4.3/src/octoxlabs/models/discovery.py` & `octoxlabs-0.4.4/src/octoxlabs/models/discovery.py`

 * *Files identical despite different names*

### Comparing `octoxlabs-0.4.3/src/octoxlabs/models/query.py` & `octoxlabs-0.4.4/src/octoxlabs/models/query.py`

 * *Files identical despite different names*

### Comparing `octoxlabs-0.4.3/src/octoxlabs/models/users.py` & `octoxlabs-0.4.4/src/octoxlabs/models/users.py`

 * *Files identical despite different names*

### Comparing `octoxlabs-0.4.3/src/octoxlabs/octoxlabs.py` & `octoxlabs-0.4.4/src/octoxlabs/octoxlabs.py`

 * *Files 0% similar despite different names*

```diff
@@ -202,20 +202,18 @@
             query = self.service.request_builder(method="POST", path=queries_path(), json=payload).json()
             return f"{query.get('name')} query created successfully"
 
         except Exception as e:
             return CantCreate(str(e))
 
     def update_query(
-        self, query_id: str, query_name: str, query_text: str, is_public: bool = None, tags: List[int] = None
+        self, query_id: str, query_name: str, query_text: str, is_public: bool = False, tags: List[int] = None
     ) -> Union[str, CantUpdate]:
-        payload = {"name": query_name, "text": query_text}
+        payload = {"name": query_name, "text": query_text, "is_public": is_public}
 
-        if is_public:
-            payload["is_public"] = is_public
         if tags:
             payload["tags"] = tags
 
         try:
             query = self.service.request_builder(
                 method="PUT", path=query_detail_path(query_id=query_id), json=payload
             ).json()
@@ -337,20 +335,18 @@
             domain = self.service.request_builder(method="POST", path=domains_path(), json=payload).json()
             return f"{domain.get('domain')} domain created successfully"
 
         except Exception as e:
             return CantCreate(str(e))
 
     def update_domain(
-        self, domain_id: int, company_id: int, domain_name: str, is_primary: bool = None
+        self, domain_id: int, company_id: int, domain_name: str, is_primary: bool = False
     ) -> Union[str, CantUpdate]:
-        payload = {"domain": domain_name, "tenant": company_id}
+        payload = {"domain": domain_name, "tenant": company_id, "is_primary": is_primary}
 
-        if is_primary:
-            payload["is_primary"] = is_primary
         try:
             domain = self.service.request_builder(
                 method="PUT", path=domain_detail_path(domain_id=domain_id), json=payload
             ).json()
             return f"{domain.get('domain')} domain successfully updated."
 
         except Exception as e:
```

### Comparing `octoxlabs-0.4.3/src/octoxlabs/service.py` & `octoxlabs-0.4.4/src/octoxlabs/service.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     def __init__(self, ip: str, token: str):
         self.set_ip(ip=ip)
         self.set_token(token=token)
 
     def set_ip(self, ip: str):
         self.ip = ip
-        self.base_url = os.getenv("OCTOXLABS_URL", None) or f"https://{self.ip}:8043"
+        self.base_url = os.getenv("OCTOXLABS_URL", None) or f"https://{self.ip}:8443"
 
     def set_token(self, token: str):
         self.token = token
         self.access_token = self.request_builder(
             method="POST", path=access_token_path(), json={"token": self.token}
         ).json()["access"]
         self.headers = {"Authorization": f"{self.token_prefix} {self.access_token}"}
```

### Comparing `octoxlabs-0.4.3/src/octoxlabs.egg-info/PKG-INFO` & `octoxlabs-0.4.4/src/octoxlabs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: octoxlabs
-Version: 0.4.3
+Version: 0.4.4
 Summary: py-octoxlabs is an API client for Octox Labs Cyber Security Asset Management platform on python programming language.
 Author-email: Octox Labs Development Team <development@octoxlabs.com>
 License: MIT License
         
         Copyright (c) 2022 Octox Labs Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `octoxlabs-0.4.3/src/octoxlabs.egg-info/SOURCES.txt` & `octoxlabs-0.4.4/src/octoxlabs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

