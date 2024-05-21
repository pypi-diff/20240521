# Comparing `tmp/rpa_helpers_btime-1.0.5.tar.gz` & `tmp/rpa_helpers_btime-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpa_helpers_btime-1.0.5.tar", last modified: Tue May 21 13:52:10 2024, max compression
+gzip compressed data, was "rpa_helpers_btime-1.0.6.tar", last modified: Tue May 21 13:55:19 2024, max compression
```

## Comparing `rpa_helpers_btime-1.0.5.tar` & `rpa_helpers_btime-1.0.6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.909069 rpa_helpers_btime-1.0.5/
--rw-rw-rw-   0        0        0      743 2024-05-21 13:52:10.907068 rpa_helpers_btime-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1058 2024-05-21 12:29:56.000000 rpa_helpers_btime-1.0.5/license.txt
-drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.815982 rpa_helpers_btime-1.0.5/rpa_helpers/
--rw-rw-rw-   0        0        0       23 2024-05-21 13:44:36.000000 rpa_helpers_btime-1.0.5/rpa_helpers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.817982 rpa_helpers_btime-1.0.5/rpa_helpers/src/
--rw-rw-rw-   0        0        0       39 2024-05-15 20:17:49.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.823006 rpa_helpers_btime-1.0.5/rpa_helpers/src/configuration/
--rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/configuration/__init__.py
--rw-rw-rw-   0        0        0      126 2024-05-15 18:25:35.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/configuration/configuration.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.824988 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.832969 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/configs/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/configs/__init__.py
--rw-rw-rw-   0        0        0       88 2024-05-15 18:09:08.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/configs/base.py
--rw-rw-rw-   0        0        0      763 2024-05-15 18:09:28.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/configs/connection.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.837361 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/entities/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/entities/__init__.py
--rw-rw-rw-   0        0        0      703 2024-05-15 18:10:41.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/entities/log.py
--rw-rw-rw-   0        0        0      305 2024-05-15 18:10:51.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/entities/rpa.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.858221 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/repository/
--rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/repository/__init__.py
--rw-rw-rw-   0        0        0     1325 2024-05-15 18:24:48.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/repository/repository_log.py
--rw-rw-rw-   0        0        0      853 2024-05-15 18:13:23.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/models/repository/repository_rpa.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.865225 rpa_helpers_btime-1.0.5/rpa_helpers/src/utils/
--rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/utils/__init__.py
--rw-rw-rw-   0        0        0     3032 2024-05-21 12:22:41.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/utils/decorator_log.py
--rw-rw-rw-   0        0        0     1293 2024-05-15 18:18:58.000000 rpa_helpers_btime-1.0.5/rpa_helpers/src/utils/send_email.py
-drwxrwxrwx   0        0        0        0 2024-05-21 13:52:10.905065 rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/
--rw-rw-rw-   0        0        0      743 2024-05-21 13:52:10.000000 rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      908 2024-05-21 13:52:10.000000 rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 13:52:10.000000 rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      213 2024-05-21 13:52:10.000000 rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-05-21 13:52:10.000000 rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 13:52:10.910068 rpa_helpers_btime-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1136 2024-05-21 13:52:08.000000 rpa_helpers_btime-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.210406 rpa_helpers_btime-1.0.6/
+-rw-rw-rw-   0        0        0      710 2024-05-21 13:55:19.208348 rpa_helpers_btime-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1058 2024-05-21 12:29:56.000000 rpa_helpers_btime-1.0.6/license.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.133669 rpa_helpers_btime-1.0.6/rpa_helpers/
+-rw-rw-rw-   0        0        0       35 2024-05-21 13:53:04.000000 rpa_helpers_btime-1.0.6/rpa_helpers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.133669 rpa_helpers_btime-1.0.6/rpa_helpers/src/
+-rw-rw-rw-   0        0        0       51 2024-05-21 13:52:57.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.150669 rpa_helpers_btime-1.0.6/rpa_helpers/src/configuration/
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/configuration/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-15 18:25:35.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/configuration/configuration.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.152666 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.159422 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/configs/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/configs/__init__.py
+-rw-rw-rw-   0        0        0       88 2024-05-15 18:09:08.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/configs/base.py
+-rw-rw-rw-   0        0        0      775 2024-05-21 13:53:43.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/configs/connection.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.166112 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/entities/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/entities/__init__.py
+-rw-rw-rw-   0        0        0      727 2024-05-21 13:53:34.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/entities/log.py
+-rw-rw-rw-   0        0        0      317 2024-05-21 13:53:38.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/entities/rpa.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.172141 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/repository/
+-rw-rw-rw-   0        0        0        0 2024-03-19 19:35:05.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/repository/__init__.py
+-rw-rw-rw-   0        0        0     1349 2024-05-21 13:53:25.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/repository/repository_log.py
+-rw-rw-rw-   0        0        0      877 2024-05-21 13:53:29.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/models/repository/repository_rpa.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.177005 rpa_helpers_btime-1.0.6/rpa_helpers/src/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-15 18:08:47.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/utils/__init__.py
+-rw-rw-rw-   0        0        0     3056 2024-05-21 13:53:17.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/utils/decorator_log.py
+-rw-rw-rw-   0        0        0     1293 2024-05-15 18:18:58.000000 rpa_helpers_btime-1.0.6/rpa_helpers/src/utils/send_email.py
+drwxrwxrwx   0        0        0        0 2024-05-21 13:55:19.207349 rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/
+-rw-rw-rw-   0        0        0      710 2024-05-21 13:55:19.000000 rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      908 2024-05-21 13:55:19.000000 rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 13:55:19.000000 rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      196 2024-05-21 13:55:19.000000 rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-05-21 13:55:19.000000 rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 13:55:19.210406 rpa_helpers_btime-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1099 2024-05-21 13:55:08.000000 rpa_helpers_btime-1.0.6/setup.py
```

### Comparing `rpa_helpers_btime-1.0.5/PKG-INFO` & `rpa_helpers_btime-1.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: rpa-helpers-btime
-Version: 1.0.5
+Version: 1.0.6
 Summary: Esse pacote irá oferecer todas as funcionalidades para auxiliar na programação de rpa.
 Author: Geovanne Zanata
 Author-email: geovanne.zanata@btime.com.br
 Keywords: log,loggers
 License-File: license.txt
 Requires-Dist: colorama==0.4.6
 Requires-Dist: flake8==7.0.0
 Requires-Dist: greenlet==3.0.3
 Requires-Dist: loguru==0.7.2
 Requires-Dist: mccabe==0.7.0
-Requires-Dist: rpa_helpers==1.0
 Requires-Dist: setuptools==69.5.1
 Requires-Dist: pycodestyle==2.11.1
 Requires-Dist: pyflakes==3.2.0
 Requires-Dist: SQLAlchemy==2.0.30
 Requires-Dist: typing_extensions==4.11.0
 Requires-Dist: win32-setctime==1.1.0
```

### Comparing `rpa_helpers_btime-1.0.5/license.txt` & `rpa_helpers_btime-1.0.6/license.txt`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.5/rpa_helpers/src/models/configs/connection.py` & `rpa_helpers_btime-1.0.6/rpa_helpers/src/models/configs/connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
-from src.configuration.configuration import CONNECTION_STRING
+from rpa_helpers.src.configuration.configuration import CONNECTION_STRING
 
 
 class DBConnectionHandler:
 
     def __init__(self) -> None:
         self.__connection_string = CONNECTION_STRING
         self.__engine = self.__create_database_engine()
```

### Comparing `rpa_helpers_btime-1.0.5/rpa_helpers/src/models/entities/log.py` & `rpa_helpers_btime-1.0.6/rpa_helpers/src/models/entities/log.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from sqlalchemy import Column, String, Integer, DateTime, ForeignKey
-from src.models.configs.base import Base
-from src.models.entities.rpa import Rpa
+from rpa_helpers.src.models.configs.base import Base
+from rpa_helpers.src.models.entities.rpa import Rpa
 
 
 class Logs(Base):
 
     __tablename__ = "logs"
 
     id = Column(Integer, primary_key=True, autoincrement=True)
```

### Comparing `rpa_helpers_btime-1.0.5/rpa_helpers/src/models/repository/repository_log.py` & `rpa_helpers_btime-1.0.6/rpa_helpers/src/models/repository/repository_log.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
-from src.models.configs.connection import DBConnectionHandler
-from src.models.entities.log import Logs
+from rpa_helpers.src.models.configs.connection import DBConnectionHandler
+from rpa_helpers.src.models.entities.log import Logs
 from sqlalchemy import text
 
 
 class LogRepository:
     def __init__(self) -> None:
         self.create_table()
         self.date = datetime.now()
```

### Comparing `rpa_helpers_btime-1.0.5/rpa_helpers/src/models/repository/repository_rpa.py` & `rpa_helpers_btime-1.0.6/rpa_helpers/src/models/repository/repository_rpa.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
-from src.models.configs.connection import DBConnectionHandler
-from src.models.entities.rpa import Rpa
+from rpa_helpers.src.models.configs.connection import DBConnectionHandler
+from rpa_helpers.src.models.entities.rpa import Rpa
 from sqlalchemy import text
 
 
 class RpaRepository:
     def __init__(self) -> None:
         self.create_table()
         self.date = datetime.now()
```

### Comparing `rpa_helpers_btime-1.0.5/rpa_helpers/src/utils/decorator_log.py` & `rpa_helpers_btime-1.0.6/rpa_helpers/src/utils/decorator_log.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from loguru import logger
 from functools import wraps
 import datetime
 import sys
 import uuid
-from src.models.repository.repository_log import LogRepository
-from src.models.repository.repository_rpa import RpaRepository
+from rpa_helpers.src.models.repository.repository_log import LogRepository
+from rpa_helpers.src.models.repository.repository_rpa import RpaRepository
 
 logger.add(sys.stdout, format="{time} | {message} | {level}", level="INFO")
 
 log_db = LogRepository()
 rpa_db = RpaRepository()
 uuid_execution = uuid.uuid1()
```

### Comparing `rpa_helpers_btime-1.0.5/rpa_helpers/src/utils/send_email.py` & `rpa_helpers_btime-1.0.6/rpa_helpers/src/utils/send_email.py`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/PKG-INFO` & `rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: rpa-helpers-btime
-Version: 1.0.5
+Version: 1.0.6
 Summary: Esse pacote irá oferecer todas as funcionalidades para auxiliar na programação de rpa.
 Author: Geovanne Zanata
 Author-email: geovanne.zanata@btime.com.br
 Keywords: log,loggers
 License-File: license.txt
 Requires-Dist: colorama==0.4.6
 Requires-Dist: flake8==7.0.0
 Requires-Dist: greenlet==3.0.3
 Requires-Dist: loguru==0.7.2
 Requires-Dist: mccabe==0.7.0
-Requires-Dist: rpa_helpers==1.0
 Requires-Dist: setuptools==69.5.1
 Requires-Dist: pycodestyle==2.11.1
 Requires-Dist: pyflakes==3.2.0
 Requires-Dist: SQLAlchemy==2.0.30
 Requires-Dist: typing_extensions==4.11.0
 Requires-Dist: win32-setctime==1.1.0
```

### Comparing `rpa_helpers_btime-1.0.5/rpa_helpers_btime.egg-info/SOURCES.txt` & `rpa_helpers_btime-1.0.6/rpa_helpers_btime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rpa_helpers_btime-1.0.5/setup.py` & `rpa_helpers_btime-1.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,28 +4,27 @@
 # try:
 #     long_description = Path("README.md").read_text()
 # except FileNotFoundError:
 #     long_description = "Default long description if README.md is not found."
 
 setup(
     name="rpa-helpers-btime",
-    version="1.0.5",
+    version="1.0.6",
     description="Esse pacote irá oferecer todas as funcionalidades para auxiliar na programação de rpa.",
     long_description="Default long description if README.md is not found.",
     author="Geovanne Zanata",
     author_email="geovanne.zanata@btime.com.br",
     keywords=['log', 'loggers'],
     packages=find_packages(),
     install_requires=[
                 'colorama==0.4.6',
                 'flake8==7.0.0',
                 'greenlet==3.0.3',
                 'loguru==0.7.2',
                 'mccabe==0.7.0',
-                'rpa_helpers==1.0',
                 'setuptools==69.5.1',
                 'pycodestyle==2.11.1',
                 'pyflakes==3.2.0',
                 'SQLAlchemy==2.0.30',
                 'typing_extensions==4.11.0',
                 'win32-setctime==1.1.0',
             ],
```

