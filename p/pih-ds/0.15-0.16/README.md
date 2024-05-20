# Comparing `tmp/pih-ds-0.15.tar.gz` & `tmp/pih-ds-0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-ds-0.15.tar", last modified: Wed Apr 24 06:44:23 2024, max compression
+gzip compressed data, was "pih-ds-0.16.tar", last modified: Mon May 20 22:50:09 2024, max compression
```

## Comparing `pih-ds-0.15.tar` & `pih-ds-0.16.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 06:44:23.667592 pih-ds-0.15/
-drwxrwxrwx   0        0        0        0 2024-04-24 06:44:23.162232 pih-ds-0.15/DataSourceService/
--rw-rw-rw-   0        0        0        0 2024-02-15 06:26:50.000000 pih-ds-0.15/DataSourceService/__init__.py
--rw-rw-rw-   0        0        0      144 2024-02-15 23:04:12.000000 pih-ds-0.15/DataSourceService/__main__.py
--rw-rw-rw-   0        0        0    15082 2024-02-15 07:48:06.000000 pih-ds-0.15/DataSourceService/anecdotica.py
--rw-rw-rw-   0        0        0    39146 2024-04-23 05:34:57.000000 pih-ds-0.15/DataSourceService/api.py
--rw-rw-rw-   0        0        0     3309 2024-04-24 06:44:01.000000 pih-ds-0.15/DataSourceService/const.py
--rw-rw-rw-   0        0        0     9780 2024-04-24 06:43:48.000000 pih-ds-0.15/DataSourceService/service.py
--rw-rw-rw-   0        0        0      380 2024-02-15 08:29:16.000000 pih-ds-0.15/DataSourceService/tools.py
--rw-rw-rw-   0        0        0      394 2024-04-24 06:44:23.620716 pih-ds-0.15/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-24 06:44:23.572790 pih-ds-0.15/pih_ds.egg-info/
--rw-rw-rw-   0        0        0      394 2024-04-24 06:44:21.000000 pih-ds-0.15/pih_ds.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-04-24 06:44:22.000000 pih-ds-0.15/pih_ds.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 06:44:21.000000 pih-ds-0.15/pih_ds.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2024-04-24 06:44:22.000000 pih-ds-0.15/pih_ds.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       53 2024-04-24 06:44:22.000000 pih-ds-0.15/pih_ds.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-04-24 06:44:22.000000 pih-ds-0.15/pih_ds.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 06:44:23.667592 pih-ds-0.15/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-20 22:50:09.354992 pih-ds-0.16/
+drwxrwxrwx   0        0        0        0 2024-05-20 22:50:08.906070 pih-ds-0.16/DataSourceService/
+-rw-rw-rw-   0        0        0        0 2024-02-15 06:26:50.000000 pih-ds-0.16/DataSourceService/__init__.py
+-rw-rw-rw-   0        0        0      144 2024-02-15 23:04:12.000000 pih-ds-0.16/DataSourceService/__main__.py
+-rw-rw-rw-   0        0        0    15082 2024-02-15 07:48:06.000000 pih-ds-0.16/DataSourceService/anecdotica.py
+-rw-rw-rw-   0        0        0    39153 2024-05-15 07:14:24.000000 pih-ds-0.16/DataSourceService/api.py
+-rw-rw-rw-   0        0        0     3309 2024-05-20 22:38:30.000000 pih-ds-0.16/DataSourceService/const.py
+-rw-rw-rw-   0        0        0     9780 2024-04-24 06:43:48.000000 pih-ds-0.16/DataSourceService/service.py
+-rw-rw-rw-   0        0        0      380 2024-02-15 08:29:16.000000 pih-ds-0.16/DataSourceService/tools.py
+-rw-rw-rw-   0        0        0      394 2024-05-20 22:50:09.323736 pih-ds-0.16/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-20 22:50:09.292487 pih-ds-0.16/pih_ds.egg-info/
+-rw-rw-rw-   0        0        0      394 2024-05-20 22:50:08.000000 pih-ds-0.16/pih_ds.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      381 2024-05-20 22:50:08.000000 pih-ds-0.16/pih_ds.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 22:50:08.000000 pih-ds-0.16/pih_ds.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2024-05-20 22:50:08.000000 pih-ds-0.16/pih_ds.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       53 2024-05-20 22:50:08.000000 pih-ds-0.16/pih_ds.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-20 22:50:08.000000 pih-ds-0.16/pih_ds.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 22:50:09.370610 pih-ds-0.16/setup.cfg
```

### Comparing `pih-ds-0.15/DataSourceService/anecdotica.py` & `pih-ds-0.16/DataSourceService/anecdotica.py`

 * *Files identical despite different names*

### Comparing `pih-ds-0.15/DataSourceService/api.py` & `pih-ds-0.16/DataSourceService/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             if catch_exception:
                 raise Error(error._full_msg, None)
         finally:
             if ne(connection):
                 connection.close()
         return result
 
-    def get_settings_value(self, key: str, default_value: Any | None = None) -> Any:
+    def get_settings_value(self, key: str | None, default_value: Any | None = None) -> Any:
         result: dict | None = self.get_storage_value(key, SETTINGS_SECTION)
         if n(result):
             self.set_settings_value(key, default_value)
         return result
 
     def set_settings_value(self, key: str, value: Any) -> bool:
         self.set_storage_value(key, value, SETTINGS_SECTION)
```

### Comparing `pih-ds-0.15/DataSourceService/const.py` & `pih-ds-0.16/DataSourceService/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 DATABASE_NAME: str = "pih_db"
 DATABASE_PORT: int = 3306
 DATABASE_POOL_SIZE: int = 5
 
 HOST = Hosts.BACKUP_WORKER
 
-VERSION: str = "0.15"
+VERSION: str = "0.16"
 
 MODULES: tuple[str, ...] = ("mysql-connector-python", "lmdb==1.4.0", "lmdbm", "dadata")
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Data storage and source service",
     host=HOST.NAME,
```

### Comparing `pih-ds-0.15/DataSourceService/service.py` & `pih-ds-0.16/DataSourceService/service.py`

 * *Files identical despite different names*

