# Comparing `tmp/ms_general_utils-2.1.1.tar.gz` & `tmp/ms_general_utils-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_general_utils-2.1.1.tar", last modified: Tue May 21 14:12:58 2024, max compression
+gzip compressed data, was "ms_general_utils-2.1.2.tar", last modified: Tue May 21 14:21:29 2024, max compression
```

## Comparing `ms_general_utils-2.1.1.tar` & `ms_general_utils-2.1.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 14:12:58.247511 ms_general_utils-2.1.1/
--rw-rw-rw-   0        0        0     1091 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/LICENSE.txt
--rw-rw-rw-   0        0        0      354 2024-05-21 14:12:58.246511 ms_general_utils-2.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      591 2024-05-09 14:38:49.000000 ms_general_utils-2.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 14:12:58.245510 ms_general_utils-2.1.1/ms_general_utils.egg-info/
--rw-rw-rw-   0        0        0      354 2024-05-21 14:12:58.000000 ms_general_utils-2.1.1/ms_general_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      784 2024-05-21 14:12:58.000000 ms_general_utils-2.1.1/ms_general_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 14:12:58.000000 ms_general_utils-2.1.1/ms_general_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-05-21 14:12:58.000000 ms_general_utils-2.1.1/ms_general_utils.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-05-21 14:12:58.000000 ms_general_utils-2.1.1/ms_general_utils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 14:12:58.242512 ms_general_utils-2.1.1/ms_utils/
--rw-rw-rw-   0        0        0      829 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/__init__.py
--rw-rw-rw-   0        0        0     1053 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/abort.py
--rw-rw-rw-   0        0        0      406 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/abstract_model.py
--rw-rw-rw-   0        0        0     6714 2024-03-07 11:35:41.000000 ms_general_utils-2.1.1/ms_utils/authentication.py
--rw-rw-rw-   0        0        0     1073 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/binary_uuid.py
--rw-rw-rw-   0        0        0      629 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/deploy.py
-drwxrwxrwx   0        0        0        0 2024-05-21 14:12:58.244510 ms_general_utils-2.1.1/ms_utils/devops/
--rw-rw-rw-   0        0        0      987 2023-12-28 13:02:56.000000 ms_general_utils-2.1.1/ms_utils/devops/Dockerfile
--rw-rw-rw-   0        0        0     2051 2023-12-28 13:02:56.000000 ms_general_utils-2.1.1/ms_utils/devops/Jenkinsfile
-drwxrwxrwx   0        0        0        0 2024-05-21 14:12:58.244510 ms_general_utils-2.1.1/ms_utils/devops/deploy/
--rw-rw-rw-   0        0        0      218 2023-12-28 13:02:56.000000 ms_general_utils-2.1.1/ms_utils/devops/deploy/script.sh
--rw-rw-rw-   0        0        0      390 2023-12-28 13:02:56.000000 ms_general_utils-2.1.1/ms_utils/devops/docker-compose.yml
--rw-rw-rw-   0        0        0      727 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/func_date.py
--rw-rw-rw-   0        0        0      799 2024-02-09 13:56:55.000000 ms_general_utils-2.1.1/ms_utils/function_utils.py
--rw-rw-rw-   0        0        0     2679 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/generic_crud_class.py
--rw-rw-rw-   0        0        0      659 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/generic_pagination.py
--rw-rw-rw-   0        0        0     1288 2024-02-09 13:56:52.000000 ms_general_utils-2.1.1/ms_utils/logger.py
--rw-rw-rw-   0        0        0     1527 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/model_utils.py
--rw-rw-rw-   0        0        0      357 2023-11-30 14:21:36.000000 ms_general_utils-2.1.1/ms_utils/prepare_json_response.py
--rw-rw-rw-   0        0        0     2152 2023-12-28 13:02:56.000000 ms_general_utils-2.1.1/ms_utils/requests_utils.py
--rw-rw-rw-   0        0        0      639 2024-01-12 12:24:21.000000 ms_general_utils-2.1.1/ms_utils/schema_utils.py
--rw-rw-rw-   0        0        0      656 2023-12-04 12:35:36.000000 ms_general_utils-2.1.1/ms_utils/validation_utils.py
--rw-rw-rw-   0        0        0     8910 2024-05-21 14:12:28.000000 ms_general_utils-2.1.1/ms_utils/view_utils.py
--rw-rw-rw-   0        0        0       42 2024-05-21 14:12:58.247511 ms_general_utils-2.1.1/setup.cfg
--rw-rw-rw-   0        0        0      888 2024-05-21 14:12:48.000000 ms_general_utils-2.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:21:29.106269 ms_general_utils-2.1.2/
+-rw-rw-rw-   0        0        0     1091 2023-11-30 14:21:36.000000 ms_general_utils-2.1.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      354 2024-05-21 14:21:29.105269 ms_general_utils-2.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      591 2024-05-09 14:38:49.000000 ms_general_utils-2.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 14:21:29.105269 ms_general_utils-2.1.2/ms_general_utils.egg-info/
+-rw-rw-rw-   0        0        0      354 2024-05-21 14:21:29.000000 ms_general_utils-2.1.2/ms_general_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      784 2024-05-21 14:21:29.000000 ms_general_utils-2.1.2/ms_general_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:21:29.000000 ms_general_utils-2.1.2/ms_general_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-21 14:21:29.000000 ms_general_utils-2.1.2/ms_general_utils.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-21 14:21:29.000000 ms_general_utils-2.1.2/ms_general_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 14:21:29.101267 ms_general_utils-2.1.2/ms_utils/
+-rw-rw-rw-   0        0        0      829 2023-11-30 14:21:36.000000 ms_general_utils-2.1.2/ms_utils/__init__.py
+-rw-rw-rw-   0        0        0     1053 2023-11-30 14:21:36.000000 ms_general_utils-2.1.2/ms_utils/abort.py
+-rw-rw-rw-   0        0        0      406 2023-11-30 14:21:36.000000 ms_general_utils-2.1.2/ms_utils/abstract_model.py
+-rw-rw-rw-   0        0        0     6714 2024-03-07 11:35:41.000000 ms_general_utils-2.1.2/ms_utils/authentication.py
+-rw-rw-rw-   0        0        0     1073 2023-11-30 14:21:36.000000 ms_general_utils-2.1.2/ms_utils/binary_uuid.py
+-rw-rw-rw-   0        0        0      629 2023-11-30 14:21:36.000000 ms_general_utils-2.1.2/ms_utils/deploy.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:21:29.103267 ms_general_utils-2.1.2/ms_utils/devops/
+-rw-rw-rw-   0        0        0      987 2023-12-28 13:02:56.000000 ms_general_utils-2.1.2/ms_utils/devops/Dockerfile
+-rw-rw-rw-   0        0        0     2051 2023-12-28 13:02:56.000000 ms_general_utils-2.1.2/ms_utils/devops/Jenkinsfile
+drwxrwxrwx   0        0        0        0 2024-05-21 14:21:29.104267 ms_general_utils-2.1.2/ms_utils/devops/deploy/
+-rw-rw-rw-   0        0        0      218 2023-12-28 13:02:56.000000 ms_general_utils-2.1.2/ms_utils/devops/deploy/script.sh
+-rw-rw-rw-   0        0        0      390 2023-12-28 13:02:56.000000 ms_general_utils-2.1.2/ms_utils/devops/docker-compose.yml
+-rw-rw-rw-   0        0        0      727 2023-11-30 14:21:36.000000 ms_general_utils-2.1.2/ms_utils/func_date.py
+-rw-rw-rw-   0        0        0      799 2024-02-09 13:56:55.000000 ms_general_utils-2.1.2/ms_utils/function_utils.py
+-rw-rw-rw-   0        0        0     2679 2023-11-30 14:21:36.000000 ms_general_utils-2.1.2/ms_utils/generic_crud_class.py
+-rw-rw-rw-   0        0        0      659 2023-11-30 14:21:36.000000 ms_general_utils-2.1.2/ms_utils/generic_pagination.py
+-rw-rw-rw-   0        0        0     1288 2024-02-09 13:56:52.000000 ms_general_utils-2.1.2/ms_utils/logger.py
+-rw-rw-rw-   0        0        0     1527 2023-11-30 14:21:36.000000 ms_general_utils-2.1.2/ms_utils/model_utils.py
+-rw-rw-rw-   0        0        0      357 2023-11-30 14:21:36.000000 ms_general_utils-2.1.2/ms_utils/prepare_json_response.py
+-rw-rw-rw-   0        0        0     2152 2023-12-28 13:02:56.000000 ms_general_utils-2.1.2/ms_utils/requests_utils.py
+-rw-rw-rw-   0        0        0      639 2024-01-12 12:24:21.000000 ms_general_utils-2.1.2/ms_utils/schema_utils.py
+-rw-rw-rw-   0        0        0      656 2023-12-04 12:35:36.000000 ms_general_utils-2.1.2/ms_utils/validation_utils.py
+-rw-rw-rw-   0        0        0     8945 2024-05-21 14:21:17.000000 ms_general_utils-2.1.2/ms_utils/view_utils.py
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:21:29.106269 ms_general_utils-2.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      888 2024-05-21 14:21:17.000000 ms_general_utils-2.1.2/setup.py
```

### Comparing `ms_general_utils-2.1.1/LICENSE.txt` & `ms_general_utils-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/README.md` & `ms_general_utils-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_general_utils.egg-info/SOURCES.txt` & `ms_general_utils-2.1.2/ms_general_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/__init__.py` & `ms_general_utils-2.1.2/ms_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/abort.py` & `ms_general_utils-2.1.2/ms_utils/abort.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/authentication.py` & `ms_general_utils-2.1.2/ms_utils/authentication.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/binary_uuid.py` & `ms_general_utils-2.1.2/ms_utils/binary_uuid.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/deploy.py` & `ms_general_utils-2.1.2/ms_utils/deploy.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/devops/Dockerfile` & `ms_general_utils-2.1.2/ms_utils/devops/Dockerfile`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/devops/Jenkinsfile` & `ms_general_utils-2.1.2/ms_utils/devops/Jenkinsfile`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/func_date.py` & `ms_general_utils-2.1.2/ms_utils/func_date.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/function_utils.py` & `ms_general_utils-2.1.2/ms_utils/function_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/generic_crud_class.py` & `ms_general_utils-2.1.2/ms_utils/generic_crud_class.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/generic_pagination.py` & `ms_general_utils-2.1.2/ms_utils/generic_pagination.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/logger.py` & `ms_general_utils-2.1.2/ms_utils/logger.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/model_utils.py` & `ms_general_utils-2.1.2/ms_utils/model_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/requests_utils.py` & `ms_general_utils-2.1.2/ms_utils/requests_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/schema_utils.py` & `ms_general_utils-2.1.2/ms_utils/schema_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/validation_utils.py` & `ms_general_utils-2.1.2/ms_utils/validation_utils.py`

 * *Files identical despite different names*

### Comparing `ms_general_utils-2.1.1/ms_utils/view_utils.py` & `ms_general_utils-2.1.2/ms_utils/view_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,52 +173,53 @@
         :return: jsonify
         """
         data = self.prepare_data_form()
         action_text = 'created'
         self.validate(validation_class, data)
 
         try:
-            with self.session_scope() as session:
-                if object_id is None:
-                    self.create(data, session)
-                else:
-                    action_text = 'updated'
-                    self.update(data, session)
+            if object_id is None:
+                self.create(data)
+            else:
+                action_text = 'updated'
+                self.update(data)
         except ValueError:
             abort_bad_request(f'{self.model.__name__} can not be {action_text} successfully')
         return prepare_json_response(f'{self.model.__name__} {action_text} successfully')
 
-    def create(self, data, session):
+    def create(self, data):
         """
         Generic Create method
         :param data:
         :return:
         """
         if self.model is None:
             raise ValueError("'Model' is not defined.")
-        self.instance = self.model(**data)
-        session.add(self.instance)
-        return self.instance
+        with self.session_scope() as session:
+            self.instance = self.model(**data)
+            session.add(self.instance)
+            return self.instance
 
-    def update(self, data, session):
+    def update(self, data):
         """
         Generic Update method
         :param data:
         :return:
         """
-        for key, value in data.items():
-            if hasattr(self.instance, key):
-                attribute = getattr(self.instance, key)
-                if not hasattr(attribute, '__tablename__'):
-                    # If the attribute is not a relationship
-                    setattr(self.instance, key, value)
+        with self.session_scope() as session:
+            for key, value in data.items():
+                if hasattr(self.instance, key):
+                    attribute = getattr(self.instance, key)
+                    if not hasattr(attribute, '__tablename__'):
+                        # If the attribute is not a relationship
+                        setattr(self.instance, key, value)
 
-        if hasattr(self.instance, 'updated_at') and 'updated_at' not in data.keys():
-            setattr(self.instance, 'updated_at', datetime.now())
-        session.commit()
+            if hasattr(self.instance, 'updated_at') and 'updated_at' not in data.keys():
+                setattr(self.instance, 'updated_at', datetime.now())
+            session.commit()
 
     def details(self, object_id):
         """
         Generic details method
         :param object_id:
         :return:
         """
```

### Comparing `ms_general_utils-2.1.1/setup.py` & `ms_general_utils-2.1.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ms_general_utils',
     packages=find_packages(),
     package_data={'ms_utils': ['devops/*', 'devops/deploy/*']},
     include_package_data=True,
-    version='2.1.1',
+    version='2.1.2',
     description='General functions for the implementation of microservices.',
     authors=[
         {"name": "Alejandro A. Serrano Correa", "email": "alejandroasc93@gmail.com"},
         {"name": "Rene Gonzalez Ramos", "email": "rgramos9310@gmail.com"}
     ],
     license="GPLv3",
     url="https://github.com/rgramos/ms-utils.git",
```

