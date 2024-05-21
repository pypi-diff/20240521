# Comparing `tmp/encorsa_e_factura-0.2.9.tar.gz` & `tmp/encorsa_e_factura-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encorsa_e_factura-0.2.9.tar", last modified: Tue May 14 21:55:43 2024, max compression
+gzip compressed data, was "encorsa_e_factura-0.3.0.tar", last modified: Tue May 21 13:13:20 2024, max compression
```

## Comparing `encorsa_e_factura-0.2.9.tar` & `encorsa_e_factura-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 21:55:43.577598 encorsa_e_factura-0.2.9/
--rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-14 21:55:43.577598 encorsa_e_factura-0.2.9/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-05-14 21:55:40.000000 encorsa_e_factura-0.2.9/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)      679 2024-05-14 21:55:43.577598 encorsa_e_factura-0.2.9/setup.cfg
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 21:55:43.577598 encorsa_e_factura-0.2.9/src/
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 21:55:43.577598 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/
--rw-r--r--   0 vsts      (1001) docker     (127)     8253 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/WebConRequestUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)    15963 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/XMLUtils.py
--rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      624 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/runLocaly.py
--rw-r--r--   0 vsts      (1001) docker     (127)    25044 2024-05-14 21:55:27.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/sincronizare.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-14 21:55:43.577598 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-14 21:55:43.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-14 21:55:43.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-14 21:55:43.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-05-14 21:55:43.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-05-14 21:55:43.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-05-14 21:55:43.000000 encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 13:13:20.265640 encorsa_e_factura-0.3.0/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1073 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-21 13:13:20.265640 encorsa_e_factura-0.3.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      885 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-05-21 13:13:17.000000 encorsa_e_factura-0.3.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)      679 2024-05-21 13:13:20.265640 encorsa_e_factura-0.3.0/setup.cfg
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 13:13:20.261640 encorsa_e_factura-0.3.0/src/
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 13:13:20.265640 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/
+-rw-r--r--   0 vsts      (1001) docker     (127)     8253 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/WebConRequestUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    15963 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/XMLUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)       27 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      624 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/runLocaly.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    25383 2024-05-21 13:13:05.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/sincronizare.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-21 13:13:20.265640 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1331 2024-05-21 13:13:20.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      499 2024-05-21 13:13:20.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-21 13:13:20.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       88 2024-05-21 13:13:20.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        9 2024-05-21 13:13:20.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       18 2024-05-21 13:13:20.000000 encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/top_level.txt
```

### Comparing `encorsa_e_factura-0.2.9/LICENCE` & `encorsa_e_factura-0.3.0/LICENCE`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.9/PKG-INFO` & `encorsa_e_factura-0.3.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Encorsa_e_Factura
-Version: 0.2.9
+Version: 0.3.0
 Summary: A small example package
 Home-page: https://encorsa.ro
 Author: Dan Popescu, Razvan Ogrezeanu
 Author-email: dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `encorsa_e_factura-0.2.9/README.md` & `encorsa_e_factura-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.9/setup.cfg` & `encorsa_e_factura-0.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = Encorsa_e_Factura
-version = 0.2.9
+version = 0.3.0
 author = Dan Popescu, Razvan Ogrezeanu
 author_email = dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 description = A small example package
 long_description = file: README.md
 url = https://encorsa.ro
 classifiers = 
 	Programming Language :: Python :: 3
```

### Comparing `encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/WebConRequestUtils.py` & `encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/WebConRequestUtils.py`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/XMLUtils.py` & `encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/XMLUtils.py`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/runLocaly.py` & `encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/runLocaly.py`

 * *Files identical despite different names*

### Comparing `encorsa_e_factura-0.2.9/src/Encorsa_e_Factura/sincronizare.py` & `encorsa_e_factura-0.3.0/src/Encorsa_e_Factura/sincronizare.py`

 * *Files 1% similar despite different names*

```diff
@@ -416,14 +416,15 @@
             'xmlns': "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2",
             'xmlns:qdt': "urn:oasis:names:specification:ubl:schema:xsd:QualifiedDataTypes-2",
             'xmlns:ccts': "urn:un:unece:uncefact:documentation:2",
             'xmlns:udt': "urn:oasis:names:specification:ubl:schema:xsd:UnqualifiedDataTypes-2",
             'xmlns:cac': "urn:oasis:names:specification:ubl:schema:xsd:CommonAggregateComponents-2",
             'xmlns:cbc': "urn:oasis:names:specification:ubl:schema:xsd:CommonBasicComponents-2",
             'xsi:schemaLocation': "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2",
+            'xmlns:schemaLocation': "urn:oasis:names:specification:ubl:schema:xsd:Invoice-2",
         },
         'CreditNote': {
             'xmlns': "urn:oasis:names:specification:ubl:schema:xsd:CreditNote-2",
             'xmlns:xsi': "http://www.w3.org/2001/XMLSchema-instance",
             'xmlns:ccts': "urn:un:unece:uncefact:documentation:2",
             'xmlns:qdt': "urn:oasis:names:specification:ubl:schema:xsd:QualifiedDataTypes-2",
             'xmlns:udt': "urn:oasis:names:specification:ubl:schema:xsd:UnqualifiedDataTypes-2",
@@ -487,14 +488,18 @@
     def replace_namespace(match):
         attribute = match.group('attribute')  # Attribute name (e.g., xmlns, xsi:schemaLocation)
         uri = match.group('uri')
         # Check if the attribute is in the replacements dictionary and replace URI if present
         if attribute in namespace_replacements:
             return f' {attribute}="{namespace_replacements[attribute]}"'
         else:
+            # Handle the specific case for URIs containing "../../"
+            if '../../' in uri:
+                # Remove spaces and split the URI, then take the first part before "../../"
+                uri = uri.split("../../")[0].strip()
             return f' {attribute}="{uri}"'
 
     # Replace found namespaces in the node string with potential replacements from the dictionary
     updated_node_string = namespace_pattern.sub(replace_namespace, node_string)
 
     return updated_node_string
```

### Comparing `encorsa_e_factura-0.2.9/src/Encorsa_e_Factura.egg-info/PKG-INFO` & `encorsa_e_factura-0.3.0/src/Encorsa_e_Factura.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Encorsa_e_Factura
-Version: 0.2.9
+Version: 0.3.0
 Summary: A small example package
 Home-page: https://encorsa.ro
 Author: Dan Popescu, Razvan Ogrezeanu
 Author-email: dan.popescu@encorsa.com, razvan.ogrezeanu@encorsa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

