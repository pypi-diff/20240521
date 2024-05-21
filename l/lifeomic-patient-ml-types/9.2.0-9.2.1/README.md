# Comparing `tmp/lifeomic_patient_ml_types-9.2.0.tar.gz` & `tmp/lifeomic_patient_ml_types-9.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeomic_patient_ml_types-9.2.0.tar", max compression
+gzip compressed data, was "lifeomic_patient_ml_types-9.2.1.tar", max compression
```

## Comparing `lifeomic_patient_ml_types-9.2.0.tar` & `lifeomic_patient_ml_types-9.2.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    18210 2024-05-01 13:22:37.945237 lifeomic_patient_ml_types-9.2.0/lifeomic_patient_ml_types/schemas.py
--rw-r--r--   0        0        0      970 2024-05-01 13:23:48.877090 lifeomic_patient_ml_types-9.2.0/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-9.2.0/setup.py
--rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-9.2.0/PKG-INFO
+-rw-r--r--   0        0        0    18210 2024-05-01 19:54:01.253192 lifeomic_patient_ml_types-9.2.1/lifeomic_patient_ml_types/schemas.py
+-rw-r--r--   0        0        0      970 2024-05-01 19:55:12.857000 lifeomic_patient_ml_types-9.2.1/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-9.2.1/setup.py
+-rw-r--r--   0        0        0      478 1970-01-01 00:00:00.000000 lifeomic_patient_ml_types-9.2.1/PKG-INFO
```

### Comparing `lifeomic_patient_ml_types-9.2.0/lifeomic_patient_ml_types/schemas.py` & `lifeomic_patient_ml_types-9.2.1/lifeomic_patient_ml_types/schemas.py`

 * *Files identical despite different names*

### Comparing `lifeomic_patient_ml_types-9.2.0/pyproject.toml` & `lifeomic_patient_ml_types-9.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lifeomic-patient-ml-types"
-version = "9.2.0"
+version = "9.2.1"
 description = "Shared types for the patient-ml-service repos."
 authors = ["LifeOmic <development@lifeomic.com>"]
 license = "UNLICENSED"
 
 [tool.poe.tasks]
 format = "black lifeomic_patient_ml_types"
 lint = "pyright lifeomic_patient_ml_types"
```

### Comparing `lifeomic_patient_ml_types-9.2.0/setup.py` & `lifeomic_patient_ml_types-9.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['lifeomic_patient_ml_types']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'lifeomic-patient-ml-types',
-    'version': '9.2.0',
+    'version': '9.2.1',
     'description': 'Shared types for the patient-ml-service repos.',
     'long_description': 'None',
     'author': 'LifeOmic',
     'author_email': 'development@lifeomic.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

