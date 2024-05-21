# Comparing `tmp/moveread_dfy-0.1.3.tar.gz` & `tmp/moveread_dfy-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moveread_dfy-0.1.3.tar", last modified: Fri May 17 09:13:11 2024, max compression
+gzip compressed data, was "moveread_dfy-0.1.5.tar", last modified: Tue May 21 09:31:48 2024, max compression
```

## Comparing `moveread_dfy-0.1.3.tar` & `moveread_dfy-0.1.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-04-29 07:55:04.000000 moveread_dfy-0.1.3/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1056 2024-05-17 09:13:09.000000 moveread_dfy-0.1.3/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.587619 moveread_dfy-0.1.3/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.587619 moveread_dfy-0.1.3/src/moveread/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.587619 moveread_dfy-0.1.3/src/moveread/dfy/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      155 2024-04-29 10:13:40.000000 moveread_dfy-0.1.3/src/moveread/dfy/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-05-09 04:41:09.000000 moveread_dfy-0.1.3/src/moveread/dfy/__init__.pyi
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.587619 moveread_dfy-0.1.3/src/moveread/dfy/doer/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-07 14:51:57.000000 moveread_dfy-0.1.3/src/moveread/dfy/doer/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      140 2024-05-07 15:35:42.000000 moveread_dfy-0.1.3/src/moveread/dfy/doer/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2424 2024-05-14 16:56:40.000000 moveread_dfy-0.1.3/src/moveread/dfy/doer/_puller.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1515 2024-05-14 14:28:20.000000 moveread_dfy-0.1.3/src/moveread/dfy/doer/_pusher.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1119 2024-05-14 12:50:44.000000 moveread_dfy-0.1.3/src/moveread/dfy/doer/_run_connect.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/src/moveread/dfy/integrations/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       28 2024-05-07 17:33:32.000000 moveread_dfy-0.1.3/src/moveread/dfy/integrations/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2009 2024-05-14 17:12:01.000000 moveread_dfy-0.1.3/src/moveread/dfy/integrations/core.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/src/moveread/dfy/scripts/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 12:24:37.000000 moveread_dfy-0.1.3/src/moveread/dfy/scripts/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1535 2024-05-12 10:43:00.000000 moveread_dfy-0.1.3/src/moveread/dfy/scripts/api_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      482 2024-05-12 10:50:26.000000 moveread_dfy-0.1.3/src/moveread/dfy/scripts/clientgen_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1745 2024-05-07 17:15:46.000000 moveread_dfy-0.1.3/src/moveread/dfy/scripts/connect_cli.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3837 2024-05-14 17:18:45.000000 moveread_dfy-0.1.3/src/moveread/dfy/scripts/doer_cli.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/src/moveread/dfy/server/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-08 07:12:36.000000 moveread_dfy-0.1.3/src/moveread/dfy/server/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-07 10:08:12.000000 moveread_dfy-0.1.3/src/moveread/dfy/server/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4224 2024-05-13 16:20:11.000000 moveread_dfy-0.1.3/src/moveread/dfy/server/api.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      573 2024-05-12 09:12:38.000000 moveread_dfy-0.1.3/src/moveread/dfy/server/main.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      751 2024-05-12 10:41:22.000000 moveread_dfy-0.1.3/src/moveread/dfy/server/pgns.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4477 2024-05-13 12:52:26.000000 moveread_dfy-0.1.3/src/moveread/dfy/server/sdk.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2437 2024-05-13 12:47:37.000000 moveread_dfy-0.1.3/src/moveread/dfy/types.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-17 09:13:11.597619 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-17 09:13:11.000000 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      995 2024-05-17 09:13:11.000000 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-17 09:13:11.000000 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      216 2024-05-17 09:13:11.000000 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/entry_points.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      284 2024-05-17 09:13:11.000000 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-17 09:13:11.000000 moveread_dfy-0.1.3/src/moveread_dfy.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 09:31:48.887755 moveread_dfy-0.1.5/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-21 09:31:48.887755 moveread_dfy-0.1.5/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       50 2024-04-29 07:55:04.000000 moveread_dfy-0.1.5/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1056 2024-05-21 09:31:46.000000 moveread_dfy-0.1.5/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-21 09:31:48.887755 moveread_dfy-0.1.5/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 09:31:48.877755 moveread_dfy-0.1.5/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 09:31:48.877755 moveread_dfy-0.1.5/src/moveread/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 09:31:48.877755 moveread_dfy-0.1.5/src/moveread/dfy/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      155 2024-04-29 10:13:40.000000 moveread_dfy-0.1.5/src/moveread/dfy/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      310 2024-05-09 04:41:09.000000 moveread_dfy-0.1.5/src/moveread/dfy/__init__.pyi
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 09:31:48.877755 moveread_dfy-0.1.5/src/moveread/dfy/doer/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-07 14:51:57.000000 moveread_dfy-0.1.5/src/moveread/dfy/doer/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      140 2024-05-07 15:35:42.000000 moveread_dfy-0.1.5/src/moveread/dfy/doer/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2424 2024-05-14 16:56:40.000000 moveread_dfy-0.1.5/src/moveread/dfy/doer/_puller.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1515 2024-05-14 14:28:20.000000 moveread_dfy-0.1.5/src/moveread/dfy/doer/_pusher.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1119 2024-05-14 12:50:44.000000 moveread_dfy-0.1.5/src/moveread/dfy/doer/_run_connect.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 09:31:48.887755 moveread_dfy-0.1.5/src/moveread/dfy/integrations/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       28 2024-05-07 17:33:32.000000 moveread_dfy-0.1.5/src/moveread/dfy/integrations/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2009 2024-05-14 17:12:01.000000 moveread_dfy-0.1.5/src/moveread/dfy/integrations/core.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 09:31:48.887755 moveread_dfy-0.1.5/src/moveread/dfy/scripts/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        0 2024-04-29 12:24:37.000000 moveread_dfy-0.1.5/src/moveread/dfy/scripts/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1813 2024-05-21 09:22:09.000000 moveread_dfy-0.1.5/src/moveread/dfy/scripts/api_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      482 2024-05-12 10:50:26.000000 moveread_dfy-0.1.5/src/moveread/dfy/scripts/clientgen_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1745 2024-05-07 17:15:46.000000 moveread_dfy-0.1.5/src/moveread/dfy/scripts/connect_cli.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3909 2024-05-19 12:14:04.000000 moveread_dfy-0.1.5/src/moveread/dfy/scripts/doer_cli.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 09:31:48.887755 moveread_dfy-0.1.5/src/moveread/dfy/server/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-08 07:12:36.000000 moveread_dfy-0.1.5/src/moveread/dfy/server/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      112 2024-05-07 10:08:12.000000 moveread_dfy-0.1.5/src/moveread/dfy/server/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4622 2024-05-21 09:29:51.000000 moveread_dfy-0.1.5/src/moveread/dfy/server/api.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      573 2024-05-12 09:12:38.000000 moveread_dfy-0.1.5/src/moveread/dfy/server/main.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      768 2024-05-21 09:28:01.000000 moveread_dfy-0.1.5/src/moveread/dfy/server/pgns.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     4958 2024-05-21 09:28:25.000000 moveread_dfy-0.1.5/src/moveread/dfy/server/sdk.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     2152 2024-05-20 06:41:30.000000 moveread_dfy-0.1.5/src/moveread/dfy/types.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-21 09:31:48.887755 moveread_dfy-0.1.5/src/moveread_dfy.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1227 2024-05-21 09:31:48.000000 moveread_dfy-0.1.5/src/moveread_dfy.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      995 2024-05-21 09:31:48.000000 moveread_dfy-0.1.5/src/moveread_dfy.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-21 09:31:48.000000 moveread_dfy-0.1.5/src/moveread_dfy.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      216 2024-05-21 09:31:48.000000 moveread_dfy-0.1.5/src/moveread_dfy.egg-info/entry_points.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      284 2024-05-21 09:31:48.000000 moveread_dfy-0.1.5/src/moveread_dfy.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-21 09:31:48.000000 moveread_dfy-0.1.5/src/moveread_dfy.egg-info/top_level.txt
```

### Comparing `moveread_dfy-0.1.3/PKG-INFO` & `moveread_dfy-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-dfy
-Version: 0.1.3
+Version: 0.1.5
 Summary: Moveread DFY data models and API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-dfy.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Requires-Dist: pydantic
```

### Comparing `moveread_dfy-0.1.3/pyproject.toml` & `moveread_dfy-0.1.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "moveread-dfy"
-version = "0.1.3"
+version = "0.1.5"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Moveread DFY data models and API"
 dependencies = [
   "lazy-loader", "pydantic",
   "chess-pairings", "dslog",
```

### Comparing `moveread_dfy-0.1.3/src/moveread/dfy/doer/_puller.py` & `moveread_dfy-0.1.5/src/moveread/dfy/doer/_puller.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.3/src/moveread/dfy/doer/_pusher.py` & `moveread_dfy-0.1.5/src/moveread/dfy/doer/_pusher.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.3/src/moveread/dfy/doer/_run_connect.py` & `moveread_dfy-0.1.5/src/moveread/dfy/doer/_run_connect.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.3/src/moveread/dfy/integrations/core.py` & `moveread_dfy-0.1.5/src/moveread/dfy/integrations/core.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.3/src/moveread/dfy/scripts/api_cli.py` & `moveread_dfy-0.1.5/src/moveread/dfy/scripts/api_cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,11 +38,19 @@
   engine = create_engine(db)
   run_api(images, engine, images_path=images_path, port=args.port, host=args.host, logger=logger)
 
 if __name__ == '__main__':
   import sys
   from dotenv import load_dotenv
   load_dotenv()
-  SQL_CONN_STR = os.environ['SQL_CONN_STR']
-  BLOB_CONN_STR = os.environ['BLOB_CONN_STR']
-  sys.argv.extend(f'--blobs {BLOB_CONN_STR} --db {SQL_CONN_STR}'.split(' '))
+
+  MOCK = False
+  if MOCK:
+    SQL_CONN_STR = 'sqlite:////home/m4rs/mr-github/modes/moveread-dfy/local-db/db.sqlite'
+    IMAGES = '/home/m4rs/mr-github/modes/moveread-dfy/local-db/images'
+    sys.argv.extend(f'--images {IMAGES} --db {SQL_CONN_STR}'.split(' '))
+  else:
+    SQL_CONN_STR = os.environ['SQL_CONN_STR']
+    BLOB_CONN_STR = os.environ['BLOB_CONN_STR']
+    sys.argv.extend(f'--blobs {BLOB_CONN_STR} --db {SQL_CONN_STR}'.split(' '))
+  
   main()
```

### Comparing `moveread_dfy-0.1.3/src/moveread/dfy/scripts/connect_cli.py` & `moveread_dfy-0.1.5/src/moveread/dfy/scripts/connect_cli.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.3/src/moveread/dfy/scripts/doer_cli.py` & `moveread_dfy-0.1.5/src/moveread/dfy/scripts/doer_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
   parser.add_argument('-i', '--input', required=True)
   parser.add_argument('-o', '--output', required=True)
   parser.add_argument('-b', '--base-path', required=True)
   parser.add_argument('-d', '--db', required=True, help='Database URL')
   parser.add_argument('-t', '--tournament', required=True, help='Tournament ID')
   parser.add_argument('-m', '--model', required=True, choices=MODEL_IDS, help='Model ID')
   parser.add_argument('--protocol', default='sqlite', required=False, choices=['sqlite', 'fs'], help='Protocol used in queues')
-  parser.add_argument('--images', type=str, help='Local path to images')
-  parser.add_argument('--blobs', type=str, help='Azure Blob connection string')
-  parser.add_argument('--core', type=str, help='Path to output core')
+  parser.add_argument('--images', type=str, help='Local path to images', required=True)
+  parser.add_argument('--blobs', type=str, help='Azure Blob connection string', required=True)
+  parser.add_argument('--core', type=str, help='Path to output core', required=True)
 
   args = parser.parse_args()
 
 
   import os
   from dslog import Logger
   input_path = os.path.join(os.getcwd(), args.input)
@@ -30,14 +30,15 @@
   
   logger = Logger.click().prefix('[DFY]')
   logger(f'Running...')
   logger(f'- Tournament ID: "{tournId}"')
   logger(f'- Database URL: "{db_url}"')
   logger(f'- Images path: "{images_path}"')
   logger(f'- Output core path: "{core_path}"')
+  logger(f'- Model: "{args.model}"')
 
   
   logger(f'- Queues protocol: "{proto}"')
   logger(f'- Input path: "{input_path}"')
   logger(f'- Internal path: "{base_path}"')
   logger(f'- Output path: "{output_path}"')
   
@@ -93,15 +94,15 @@
   os.chdir(path)
   load_dotenv()
 
   SQL_CONN_STR = os.environ['SQL_CONN_STR']
   # SQL_CONN_STR = 'sqlite:////home/m4rs/mr-github/modes/moveread-dfy/local-db/db.sqlite'
   BLOB_CONN_STR = os.environ['BLOB_CONN_STR']
   # BLOB_CONN_STR = '../../../local-db/images'
-  blobs = ''
+  
   args = f'-i queues/in -o queues/out -b queues/internal \
       -t llobregat23 -m llobregat23 \
       --db {SQL_CONN_STR} \
       --blobs {BLOB_CONN_STR} \
       --core core \
       --images images'.replace('\n', '').split(' ')
   args = [arg for arg in args if arg]
```

### Comparing `moveread_dfy-0.1.3/src/moveread/dfy/server/api.py` & `moveread_dfy-0.1.5/src/moveread/dfy/server/api.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Sequence, Literal, Annotated
 import os
 from fastapi import FastAPI, Response, File, Request, status
+from fastapi.responses import StreamingResponse
 from fastapi.staticfiles import StaticFiles
 from fastapi.middleware.cors import CORSMiddleware
 from dslog import Logger
 from dslog.uvicorn import setup_loggers_lifespan, DEFAULT_FORMATTER, ACCESS_FORMATTER
 from kv.api import LocatableKV
-from ..types import FrontendGame, gameId, roundId, Tournament, Group, FrontendPGN
+from chess_pairings import roundId, gameId, groupId
+from ..types import FrontendGame, Tournament, Group, FrontendPGN
 from .sdk import DFY
 
 def fastapi(
   sdk: DFY, *, images_path: str | None = None,
   blobs: LocatableKV[bytes],
   logger = Logger.click().prefix('[DFY API]')
 ):
@@ -46,25 +48,32 @@
   @app.get('/{tournId}', responses={ 404: {}, 200: { 'model': Tournament }})
   def tournament(tournId: str, r: Response) -> Tournament | None:
     tnmt = sdk.tournament(tournId)
     if tnmt is None:
       r.status_code = status.HTTP_404_NOT_FOUND
     return tnmt
   
+  @app.get('/{tournId}/{group}.pgn', response_model=str)
+  def group_pgn(tournId: str, group: str):
+    pgn = sdk.group_pgn(**groupId(tournId, group))
+    return StreamingResponse(content=pgn, media_type='application/x-chess-pgn', headers={
+      'Content-Disposition': f'attachment; filename={tournId}_{group}.pgn'
+    })
+  
   @app.get('/{tournId}/{group}', responses={ 404: {}, 200: { 'model': Group }})
   def group(tournId: str, group: str, r: Response) -> Group | None:
     grp = sdk.group(tournId, group)
     if grp is None:
       r.status_code = status.HTTP_404_NOT_FOUND
     return grp
 
-  @app.get('/{tournId}/{group}/{round}.pgn', response_model=str)
+  @app.get('/{tournId}/{group}/{round}.pgn')
   def round_pgn(tournId: str, group: str, round: str):
     pgn = sdk.round_pgn(**roundId(tournId, group, round))
-    return Response(content=pgn, media_type='application/x-chess-pgn', headers={
+    return StreamingResponse(content=pgn, media_type='application/x-chess-pgn', headers={
       'Content-Disposition': f'attachment; filename={tournId}_{group}_{round}.pgn'
     })
   
   @app.get('/{tournId}/{group}/{round}')
   def round(tournId: str, group: str, round: str) -> Sequence[FrontendGame]:
     return sdk.round(**roundId(tournId, group, round))
```

### Comparing `moveread_dfy-0.1.3/src/moveread/dfy/server/main.py` & `moveread_dfy-0.1.5/src/moveread/dfy/server/main.py`

 * *Files identical despite different names*

### Comparing `moveread_dfy-0.1.3/src/moveread/dfy/server/pgns.py` & `moveread_dfy-0.1.5/src/moveread/dfy/server/pgns.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,9 +11,11 @@
   headers = PGNHeaders(
     Event=event, Site=site, White=pair.white, Black=pair.black,
     Round=f'{game.round}.{game.board}', Result=pair.result,
   )
   comment = '[...]' if game.pgn.early else None
   return export_pgn(game.pgn.moves, headers, comment)
 
-def export_all(games: Iterable[Game], tnmt: Tournament | None = None) -> str:
-  return '\n\n'.join(pgn for game in games if (pgn := export(game, tnmt)) is not None)
+def export_all(games: Iterable[Game], tnmt: Tournament | None = None) -> Iterable[str]:
+  for game in games:
+    if (pgn := export(game, tnmt)) is not None:
+      yield pgn + '\n\n'
```

### Comparing `moveread_dfy-0.1.3/src/moveread/dfy/server/sdk.py` & `moveread_dfy-0.1.5/src/moveread/dfy/server/sdk.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-from typing import Sequence, Literal, TypeAlias, Unpack, Any
-from functools import partial
+from typing import Sequence, Literal, TypeAlias, Unpack, Any, Iterable
 import asyncio
 from sqlalchemy import Engine
 from sqlmodel import Session, select
 from uuid import uuid4
 from haskellian import either as E, Left
 import pure_cv as vc
 from kv.api import KV, InexistentItem, ReadError
+from chess_pairings import GameId, GroupId, RoundId
 from .pgns import export_all
-from ..types import Game, Token, GameId, RoundId, Group, Image, Tournament, FrontendPGN
+from ..types import Game, Token, Group, Image, Tournament, FrontendPGN
 
 ImgExtension: TypeAlias = Literal['.jpg', '.png', '.webp']
 MimeType: TypeAlias = str
 
 def stringify(tournId: str, group: str, round: str, board: str) -> str:
   return f'{tournId}/{group}/{round}/{board}'
 
-def exact_game(tournId: str, group: str, round: str, board: str):
-  return Game.tournId == tournId, Game.group == group, Game.round == round, Game.board == board
-
 def select_game(**gameId: Unpack[GameId]):
   return select(Game).where(*exact_game(**gameId))
 
+def group_games(tournId: str, group: str):
+  return Game.tournId == tournId, Game.group == group
+
 def round_games(tournId: str, group: str, round: str):
   return Game.tournId == tournId, Game.group == group, Game.round == round
 
+def exact_game(tournId: str, group: str, round: str, board: str):
+  return Game.tournId == tournId, Game.group == group, Game.round == round, Game.board == board
+
 def select_tnmt(tournId: str):
   return select(Tournament).where(Tournament.tournId == tournId)
 
 class DFY:
 
   def __init__(self, images: KV[bytes], engine: Engine):
     self._images = images
@@ -53,21 +56,29 @@
   
   def round(self, **roundId: Unpack[RoundId]) -> Sequence[Game]:
     with Session(self._engine) as ses:
       order: Any = Game.index # order_by's typing is messed up
       stmt = select(Game).where(*round_games(**roundId)).order_by(order)
       return ses.exec(stmt).all()
     
-  def round_pgn(self, **roundId: Unpack[RoundId]) -> str:
+  def group_pgn(self, **groupId: Unpack[GroupId]) -> Iterable[str]:
+    with Session(self._engine) as ses:
+      order: Any = Game.index
+      stmt = select(Game).where(*group_games(**groupId)).order_by(order)
+      games = ses.exec(stmt).all()
+      tnmt = ses.exec(select_tnmt(groupId['tournId'])).first()
+      yield from export_all(games, tnmt)
+    
+  def round_pgn(self, **roundId: Unpack[RoundId]) -> Iterable[str]:
     with Session(self._engine) as ses:
       order: Any = Game.index
       stmt = select(Game).where(*round_games(**roundId)).order_by(order)
       games = ses.exec(stmt).all()
       tnmt = ses.exec(select_tnmt(roundId['tournId'])).first()
-      return export_all(games, tnmt)
+      yield from export_all(games, tnmt)
 
   def game_pgn(self, **gameId: Unpack[GameId]) -> FrontendPGN | None:
     with Session(self._engine) as ses:
       game = ses.exec(select_game(**gameId)).first()
       if game and game.pgn:
         return game.pgn
```

### Comparing `moveread_dfy-0.1.3/src/moveread/dfy/types.py` & `moveread_dfy-0.1.5/src/moveread/dfy/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Sequence, TypedDict
 from enum import StrEnum
 from datetime import date
 from pydantic import RootModel, Field as PydanticField
 from sqlmodel import Field, SQLModel, Relationship
 from sqltypes import SpaceDelimitedList, PydanticModel
-from chess_pairings import Paired, Unpaired
+from chess_pairings import Paired, Unpaired, GameId, gameId
 
 class Pairing(RootModel):
   root: Paired | Unpaired = PydanticField(discriminator='tag')
 
 class Tournament(SQLModel, table=True):
   tournId: str = Field(primary_key=True)
   name: str
@@ -50,30 +50,17 @@
   tournId: str
   group: str
   round: str
   index: int
   """Boards may have out of whack names (e.g. in team tournaments "1.3"). This is the order you'd see in chess-results"""
   imgs: list[Image] = Relationship()
   pgn: PGN | None = Relationship()
-  
-class GroupId(TypedDict):
-  tournId: str
-  group: str
-
-class RoundId(GroupId):
-  round: str
-
-class GameId(RoundId):
-  board: str
-
-def gameId(tournId: str, group: str, round: str, board: str) -> GameId:
-  return GameId(tournId=tournId, group=group, round=round, board=board)
 
-def roundId(tournId: str, group: str, round: str) -> RoundId:
-  return RoundId(tournId=tournId, group=group, round=round)
+  def gameId(self) -> GameId:
+    return gameId(self.tournId, self.group, self.round, self.board)
   
 class Token(SQLModel, table=True):
   id: int | None = Field(default=None, primary_key=True)
   token: str
   tournId: str
   
 __all__ = [
```

### Comparing `moveread_dfy-0.1.3/src/moveread_dfy.egg-info/PKG-INFO` & `moveread_dfy-0.1.5/src/moveread_dfy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moveread-dfy
-Version: 0.1.3
+Version: 0.1.5
 Summary: Moveread DFY data models and API
 Author-email: Marcel Claramunt <marcel@moveread.com>
 Project-URL: repo, https://github.com/moveread/moveread-dfy.git
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: lazy-loader
 Requires-Dist: pydantic
```

### Comparing `moveread_dfy-0.1.3/src/moveread_dfy.egg-info/SOURCES.txt` & `moveread_dfy-0.1.5/src/moveread_dfy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

