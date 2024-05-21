# Comparing `tmp/rpa_helpers_btime-1.0.6.tar.gz` & `tmp/rpa_helpers_btime-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_helpers_btime-1.0.6.tar", last modified: Tue May 21 13:55:19 2024, max compression
+gzip compressed data, was "rpa_helpers_btime-1.0.7.tar", last modified: Tue May 21 14:05:11 2024, max compression
```

## Comparing `rpa_helpers_btime-1.0.6.tar` & `rpa_helpers_btime-1.0.7.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.210406 rpa_helpers_btime-1.0.6/
--rw-rw-rw-   0        0        0      710 2024-05-21 13:55:19.208348 rpa_helpers_btime-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2024-05-21 12:29:56.000000 rpa_helpers_btime-1.0.6/license.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.133669 rpa_helpers_btime-1.0.6/rpa_helpers/
--rw-rw-rw-   0        0        0       35 2024-05-21 13:53:04.000000 rpa_helpers_btime-1.0.6/rpa_helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.133669 rpa_helpers_btime-1.0.6/rpa_helpers/src/
--rw-rw-rw-   0        0        0       51 2024-05-21 13:52:57.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.150669 rpa_helpers_btime-1.0.6/rpa_helpers/src/configuration/
--rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/configuration/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-15 18:25:35.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/configuration/configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.152666 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.159422 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/configs/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/configs/__init__.py
--rw-rw-rw-   0        0        0       88 2024-05-15 18:09:08.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/configs/base.py
--rw-rw-rw-   0        0        0      775 2024-05-21 13:53:43.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/configs/connection.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.166112 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/entities/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/entities/__init__.py
--rw-rw-rw-   0        0        0      727 2024-05-21 13:53:34.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/entities/log.py
--rw-rw-rw-   0        0        0      317 2024-05-21 13:53:38.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/entities/rpa.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.172141 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/repository/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/repository/__init__.py
--rw-rw-rw-   0        0        0     1349 2024-05-21 13:53:25.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/repository/repository_log.py
--rw-rw-rw-   0        0        0      877 2024-05-21 13:53:29.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/repository/repository_rpa.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.177005 rpa_helpers_btime-1.0.6/rpa_helpers/src/utils/
--rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/utils/__init__.py
--rw-rw-rw-   0        0        0     3056 2024-05-21 13:53:17.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/utils/decorator_log.py
--rw-rw-rw-   0        0        0     1293 2024-05-15 18:18:58.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/utils/send_email.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.207349 rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/
--rw-rw-rw-   0        0        0      710 2024-05-21 13:55:19.000000 rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      908 2024-05-21 13:55:19.000000 rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 13:55:19.000000 rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      196 2024-05-21 13:55:19.000000 rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 13:55:19.000000 rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 13:55:19.210406 rpa_helpers_btime-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1099 2024-05-21 13:55:08.000000 rpa_helpers_btime-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:11.534659 rpa_helpers_btime-1.0.7/
+-rw-rw-rw-   0        0        0      710 2024-05-21 14:05:11.532661 rpa_helpers_btime-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2024-05-21 12:29:56.000000 rpa_helpers_btime-1.0.7/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:11.411647 rpa_helpers_btime-1.0.7/rpa_helpers/
+-rw-rw-rw-   0        0        0       35 2024-05-21 13:53:04.000000 rpa_helpers_btime-1.0.7/rpa_helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:11.411647 rpa_helpers_btime-1.0.7/rpa_helpers/src/
+-rw-rw-rw-   0        0        0       51 2024-05-21 13:52:57.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:11.411647 rpa_helpers_btime-1.0.7/rpa_helpers/src/configuration/
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/configuration/__init__.py
+-rw-rw-rw-   0        0        0      184 2024-05-21 14:01:28.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/configuration/configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:11.427239 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:11.448583 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/configs/
+-rw-rw-rw-   0        0        0        0 2024-05-14 19:21:02.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/configs/__init__.py
+-rw-rw-rw-   0        0        0       84 2024-05-14 19:23:16.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/configs/base.py
+-rw-rw-rw-   0        0        0      841 2024-05-21 14:03:11.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/configs/connection.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:11.448583 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-05-14 19:21:02.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/entities/__init__.py
+-rw-rw-rw-   0        0        0      760 2024-05-21 14:03:36.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/entities/log.py
+-rw-rw-rw-   0        0        0      297 2024-05-21 14:03:28.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/entities/rpa.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:11.461532 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/repository/
+-rw-rw-rw-   0        0        0        0 2024-05-14 19:21:02.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/repository/__init__.py
+-rw-rw-rw-   0        0        0     1436 2024-05-21 14:03:43.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/repository/repository_log.py
+-rw-rw-rw-   0        0        0      935 2024-05-21 14:03:47.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/models/repository/repository_rpa.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:11.461532 rpa_helpers_btime-1.0.7/rpa_helpers/src/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     3056 2024-05-21 13:53:17.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/utils/decorator_log.py
+-rw-rw-rw-   0        0        0     1293 2024-05-15 18:18:58.000000 rpa_helpers_btime-1.0.7/rpa_helpers/src/utils/send_email.py
+drwxrwxrwx   0        0        0        0 2024-05-21 14:05:11.530655 rpa_helpers_btime-1.0.7/rpa_helpers_btime.egg-info/
+-rw-rw-rw-   0        0        0      710 2024-05-21 14:05:11.000000 rpa_helpers_btime-1.0.7/rpa_helpers_btime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2024-05-21 14:05:11.000000 rpa_helpers_btime-1.0.7/rpa_helpers_btime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 14:05:11.000000 rpa_helpers_btime-1.0.7/rpa_helpers_btime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      196 2024-05-21 14:05:11.000000 rpa_helpers_btime-1.0.7/rpa_helpers_btime.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 14:05:11.000000 rpa_helpers_btime-1.0.7/rpa_helpers_btime.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 14:05:11.535664 rpa_helpers_btime-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1099 2024-05-21 14:05:03.000000 rpa_helpers_btime-1.0.7/setup.py
```

### Comparing `rpa_helpers_btime-1.0.6/PKG-INFO` & `rpa_helpers_btime-1.0.7/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-helpers-btime
-Version: 1.0.6
+Version: 1.0.7
 Summary: Esse pacote irá oferecer todas as funcionalidades para auxiliar na programação de rpa.
 Author: Geovanne Zanata
 Author-email: geovanne.zanata@btime.com.br
 Keywords: log,loggers
 License-File: license.txt
 Requires-Dist: colorama==0.4.6
 Requires-Dist: flake8==7.0.0
```

### Comparing `rpa_helpers_btime-1.0.6/license.txt` & `rpa_helpers_btime-1.0.7/license.txt`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.6/rpa_helpers/src/models/configs/connection.py` & `rpa_helpers_btime-1.0.7/rpa_helpers/src/models/configs/connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
+from rpa_helpers.src.models.configs.base import Base
 from rpa_helpers.src.configuration.configuration import CONNECTION_STRING
 
 
 class DBConnectionHandler:
 
     def __init__(self) -> None:
         self.__connection_string = CONNECTION_STRING
         self.__engine = self.__create_database_engine()
         self.session = None
 
     def __create_database_engine(self):
         engine = create_engine(self.__connection_string)
         return engine
-
+    
     def get_engine(self):
         return self.__engine
-
+    
     def __enter__(self):
         session_maker = sessionmaker(bind=self.__engine)
         self.session = session_maker()
-        return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
-        self.session.close()
+        return self
+    
+    def __exit__(self, exc_tupe, exc_val, exc_tb):
+        self.session.close()
```

### Comparing `rpa_helpers_btime-1.0.6/rpa_helpers/src/models/entities/log.py` & `rpa_helpers_btime-1.0.7/rpa_helpers/src/models/entities/log.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,10 +10,11 @@
     id = Column(Integer, primary_key=True, autoincrement=True)
     message = Column(String)
     status = Column(String)
     description = Column(String)
     start_date = Column(DateTime)
     end_date = Column(DateTime)
     rpa_id = Column(Integer, ForeignKey(Rpa.id))
+    execution_id = Column(String)
 
     def __repr__(self):
-        return f"Logs [MESSAGE='(self.message)', STATUS='(self.status)', DESCRIPTION='(self.description)', START_DATE='(self.start_date)', END_DATE='(self.end_date)', RPA_ID='(self.rpa_id)']"
+        return f"Logs [MESSAGE='(self.message)', STATUS='(self.status)', DESCRIPTION='(self.description)', START_DATE='(self.start_date)', END_DATE='(self.end_date)', RPA_ID='(self.rpa_id)']"
```

### Comparing `rpa_helpers_btime-1.0.6/rpa_helpers/src/models/repository/repository_log.py` & `rpa_helpers_btime-1.0.7/rpa_helpers/src/models/repository/repository_log.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,35 +5,38 @@
 
 
 class LogRepository:
     def __init__(self) -> None:
         self.create_table()
         self.date = datetime.now()
 
+    
     def create_table(self):
         with DBConnectionHandler() as db:
             query = text(
                 """
                 CREATE TABLE IF NOT EXISTS logs
-                (id INTEGER PRIMARY KEY, message TEXT, status TEXT, description TEXT, start_date DATETIME, end_date DATETIME, rpa_id INTEGER)
+                (id SERIAL PRIMARY KEY, message TEXT, status TEXT, description TEXT, start_date TEXT, end_date TEXT, rpa_id INTEGER, execution_id TEXT)
                 """
             )
 
             db.session.execute(query)
             db.session.commit()
 
-    def insert(self, message, status, description, start_date, end_date, rpa_id):
+
+    def insert(self, message, status, description, start_date, end_date, rpa_id, execution_id):
         start_date = datetime.strptime(start_date, "%d/%m/%Y %H:%M:%S")
         end_date = datetime.strptime(end_date, "%d/%m/%Y %H:%M:%S")
 
         with DBConnectionHandler() as db:
             data_insert = Logs(
-                message=message,
-                status=status,
-                description=description,
-                start_date=start_date,
-                end_date=end_date,
-                rpa_id=rpa_id,
+                message = message,
+                status = status,
+                description = description,
+                start_date = start_date,
+                end_date = end_date,
+                rpa_id = rpa_id,
+                execution_id = execution_id
             )
 
             db.session.add(data_insert)
-            db.session.commit()
+            db.session.commit()
```

### Comparing `rpa_helpers_btime-1.0.6/rpa_helpers/src/models/repository/repository_rpa.py` & `rpa_helpers_btime-1.0.7/rpa_helpers/src/models/repository/repository_rpa.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,27 +5,32 @@
 
 
 class RpaRepository:
     def __init__(self) -> None:
         self.create_table()
         self.date = datetime.now()
 
+    
     def create_table(self):
         with DBConnectionHandler() as db:
             query = text(
                 """
                     CREATE TABLE IF NOT EXISTS rpa
                     (id INTEGER PRIMARY KEY, name TEXT)
                 """
             )
 
             db.session.execute(query)
             db.session.commit()
 
+
     def insert(self, name):
         with DBConnectionHandler() as db:
             data_insert = Rpa(
-                name=name
+                name = name
             )
-
+            
             db.session.add(data_insert)
             db.session.commit()
+
+    def update(self):
+        ...
```

### Comparing `rpa_helpers_btime-1.0.6/rpa_helpers/src/utils/decorator_log.py` & `rpa_helpers_btime-1.0.7/rpa_helpers/src/utils/decorator_log.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.6/rpa_helpers/src/utils/send_email.py` & `rpa_helpers_btime-1.0.7/rpa_helpers/src/utils/send_email.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/PKG-INFO` & `rpa_helpers_btime-1.0.7/rpa_helpers_btime.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rpa-helpers-btime
-Version: 1.0.6
+Version: 1.0.7
 Summary: Esse pacote irá oferecer todas as funcionalidades para auxiliar na programação de rpa.
 Author: Geovanne Zanata
 Author-email: geovanne.zanata@btime.com.br
 Keywords: log,loggers
 License-File: license.txt
 Requires-Dist: colorama==0.4.6
 Requires-Dist: flake8==7.0.0
```

### Comparing `rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/SOURCES.txt` & `rpa_helpers_btime-1.0.7/rpa_helpers_btime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.6/setup.py` & `rpa_helpers_btime-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # try:
 #     long_description = Path("README.md").read_text()
 # except FileNotFoundError:
 #     long_description = "Default long description if README.md is not found."
 
 setup(
     name="rpa-helpers-btime",
-    version="1.0.6",
+    version="1.0.7",
     description="Esse pacote irá oferecer todas as funcionalidades para auxiliar na programação de rpa.",
     long_description="Default long description if README.md is not found.",
     author="Geovanne Zanata",
     author_email="geovanne.zanata@btime.com.br",
     keywords=['log', 'loggers'],
     packages=find_packages(),
     install_requires=[
```

