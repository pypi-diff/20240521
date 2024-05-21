# Comparing `tmp/canonicalwebteam_store_api-4.8.0.tar.gz` & `tmp/canonicalwebteam_store_api-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "canonicalwebteam_store_api-4.8.0.tar", max compression
+gzip compressed data, was "canonicalwebteam_store_api-4.9.0.tar", max compression
```

## Comparing `canonicalwebteam_store_api-4.8.0.tar` & `canonicalwebteam_store_api-4.9.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     7652 2023-12-12 13:38:23.860580 canonicalwebteam_store_api-4.8.0/LICENSE
--rw-r--r--   0        0        0     1430 2023-12-12 13:38:23.860580 canonicalwebteam_store_api-4.8.0/README.md
--rw-r--r--   0        0        0       65 2023-12-12 13:38:23.860580 canonicalwebteam_store_api-4.8.0/canonicalwebteam/__init__.py
--rw-r--r--   0        0        0        0 2023-12-12 13:38:23.860580 canonicalwebteam_store_api-4.8.0/canonicalwebteam/store_api/__init__.py
--rw-r--r--   0        0        0     1517 2023-12-12 13:38:23.860580 canonicalwebteam_store_api-4.8.0/canonicalwebteam/store_api/exceptions.py
--rw-r--r--   0        0        0    10632 2023-12-12 13:38:23.860580 canonicalwebteam_store_api-4.8.0/canonicalwebteam/store_api/publisher.py
--rw-r--r--   0        0        0     6249 2023-12-12 13:38:23.860580 canonicalwebteam_store_api-4.8.0/canonicalwebteam/store_api/store.py
--rw-r--r--   0        0        0        0 2023-12-12 13:38:23.860580 canonicalwebteam_store_api-4.8.0/canonicalwebteam/store_api/stores/__init__.py
--rw-r--r--   0        0        0    11602 2023-12-12 13:38:23.860580 canonicalwebteam_store_api-4.8.0/canonicalwebteam/store_api/stores/charmstore.py
--rw-r--r--   0        0        0    14824 2023-12-12 13:38:23.860580 canonicalwebteam_store_api-4.8.0/canonicalwebteam/store_api/stores/snapstore.py
--rw-r--r--   0        0        0      493 2023-12-12 13:38:23.860580 canonicalwebteam_store_api-4.8.0/pyproject.toml
--rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 canonicalwebteam_store_api-4.8.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2024-01-24 13:30:55.408466 canonicalwebteam_store_api-4.9.0/LICENSE
+-rw-r--r--   0        0        0     1430 2024-01-24 13:30:55.408466 canonicalwebteam_store_api-4.9.0/README.md
+-rw-r--r--   0        0        0       65 2024-01-24 13:30:55.408466 canonicalwebteam_store_api-4.9.0/canonicalwebteam/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-24 13:30:55.408466 canonicalwebteam_store_api-4.9.0/canonicalwebteam/store_api/__init__.py
+-rw-r--r--   0        0        0     1517 2024-01-24 13:30:55.408466 canonicalwebteam_store_api-4.9.0/canonicalwebteam/store_api/exceptions.py
+-rw-r--r--   0        0        0    10632 2024-01-24 13:30:55.408466 canonicalwebteam_store_api-4.9.0/canonicalwebteam/store_api/publisher.py
+-rw-r--r--   0        0        0     6249 2024-01-24 13:30:55.408466 canonicalwebteam_store_api-4.9.0/canonicalwebteam/store_api/store.py
+-rw-r--r--   0        0        0        0 2024-01-24 13:30:55.408466 canonicalwebteam_store_api-4.9.0/canonicalwebteam/store_api/stores/__init__.py
+-rw-r--r--   0        0        0    11579 2024-01-24 13:30:55.408466 canonicalwebteam_store_api-4.9.0/canonicalwebteam/store_api/stores/charmstore.py
+-rw-r--r--   0        0        0    14824 2024-01-24 13:30:55.408466 canonicalwebteam_store_api-4.9.0/canonicalwebteam/store_api/stores/snapstore.py
+-rw-r--r--   0        0        0      493 2024-01-24 13:30:55.408466 canonicalwebteam_store_api-4.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2264 1970-01-01 00:00:00.000000 canonicalwebteam_store_api-4.9.0/PKG-INFO
```

### Comparing `canonicalwebteam_store_api-4.8.0/LICENSE` & `canonicalwebteam_store_api-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_api-4.8.0/README.md` & `canonicalwebteam_store_api-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_api-4.8.0/canonicalwebteam/store_api/exceptions.py` & `canonicalwebteam_store_api-4.9.0/canonicalwebteam/store_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_api-4.8.0/canonicalwebteam/store_api/publisher.py` & `canonicalwebteam_store_api-4.9.0/canonicalwebteam/store_api/publisher.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_api-4.8.0/canonicalwebteam/store_api/store.py` & `canonicalwebteam_store_api-4.9.0/canonicalwebteam/store_api/store.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_api-4.8.0/canonicalwebteam/store_api/stores/charmstore.py` & `canonicalwebteam_store_api-4.9.0/canonicalwebteam/store_api/stores/charmstore.py`

 * *Files 0% similar despite different names*

```diff
@@ -335,15 +335,15 @@
         response = self.session.post(
             url=self.get_endpoint_url(
                 f"charm/{name}/collaborators/invites/revoke"
             ),
             headers=self._get_authorization_header(publisher_auth),
             json=payload,
         )
-        return self.process_response(response)
+        return response
 
     def accept_invite(self, publisher_auth, name, token):
         """
         Accept a collaborator invite.
         """
         response = self.session.post(
             url=self.get_endpoint_url(
```

### Comparing `canonicalwebteam_store_api-4.8.0/canonicalwebteam/store_api/stores/snapstore.py` & `canonicalwebteam_store_api-4.9.0/canonicalwebteam/store_api/stores/snapstore.py`

 * *Files identical despite different names*

### Comparing `canonicalwebteam_store_api-4.8.0/PKG-INFO` & `canonicalwebteam_store_api-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canonicalwebteam.store-api
-Version: 4.8.0
+Version: 4.9.0
 Summary: 
 License: LGPL-3.0
 Author: Canonical Web Team
 Author-email: webteam@canonical.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
```

