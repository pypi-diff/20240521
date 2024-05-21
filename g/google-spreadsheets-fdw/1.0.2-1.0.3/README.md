# Comparing `tmp/google_spreadsheets_fdw-1.0.2.tar.gz` & `tmp/google_spreadsheets_fdw-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google_spreadsheets_fdw-1.0.2.tar", last modified: Thu May  6 07:20:14 2021, max compression
+gzip compressed data, was "google_spreadsheets_fdw-1.0.3.tar", last modified: Tue May 21 07:32:37 2024, max compression
```

## Comparing `google_spreadsheets_fdw-1.0.2.tar` & `google_spreadsheets_fdw-1.0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 07:20:14.423286 google_spreadsheets_fdw-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2021-05-06 07:20:14.423286 google_spreadsheets_fdw-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2169 2021-05-06 07:20:01.000000 google_spreadsheets_fdw-1.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 07:20:14.423286 google_spreadsheets_fdw-1.0.2/google_spreadsheets_fdw/
--rw-r--r--   0 runner    (1001) docker     (121)     6722 2021-05-06 07:20:01.000000 google_spreadsheets_fdw-1.0.2/google_spreadsheets_fdw/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-06 07:20:14.423286 google_spreadsheets_fdw-1.0.2/google_spreadsheets_fdw.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3342 2021-05-06 07:20:14.000000 google_spreadsheets_fdw-1.0.2/google_spreadsheets_fdw.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      288 2021-05-06 07:20:14.000000 google_spreadsheets_fdw-1.0.2/google_spreadsheets_fdw.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-06 07:20:14.000000 google_spreadsheets_fdw-1.0.2/google_spreadsheets_fdw.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-05-06 07:20:14.000000 google_spreadsheets_fdw-1.0.2/google_spreadsheets_fdw.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2021-05-06 07:20:14.000000 google_spreadsheets_fdw-1.0.2/google_spreadsheets_fdw.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-06 07:20:14.423286 google_spreadsheets_fdw-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      762 2021-05-06 07:20:01.000000 google_spreadsheets_fdw-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:32:37.896675 google_spreadsheets_fdw-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-21 07:32:29.000000 google_spreadsheets_fdw-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-21 07:32:37.896675 google_spreadsheets_fdw-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-21 07:32:29.000000 google_spreadsheets_fdw-1.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:32:37.896675 google_spreadsheets_fdw-1.0.3/google_spreadsheets_fdw/
+-rw-r--r--   0 runner    (1001) docker     (127)     6722 2024-05-21 07:32:29.000000 google_spreadsheets_fdw-1.0.3/google_spreadsheets_fdw/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:32:37.896675 google_spreadsheets_fdw-1.0.3/google_spreadsheets_fdw.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-05-21 07:32:37.000000 google_spreadsheets_fdw-1.0.3/google_spreadsheets_fdw.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-21 07:32:37.000000 google_spreadsheets_fdw-1.0.3/google_spreadsheets_fdw.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:32:37.000000 google_spreadsheets_fdw-1.0.3/google_spreadsheets_fdw.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 07:32:37.000000 google_spreadsheets_fdw-1.0.3/google_spreadsheets_fdw.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 07:32:37.000000 google_spreadsheets_fdw-1.0.3/google_spreadsheets_fdw.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 07:32:37.896675 google_spreadsheets_fdw-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-21 07:32:29.000000 google_spreadsheets_fdw-1.0.3/setup.py
```

### Comparing `google_spreadsheets_fdw-1.0.2/PKG-INFO` & `google_spreadsheets_fdw-1.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,103 @@
 Metadata-Version: 2.1
 Name: google_spreadsheets_fdw
-Version: 1.0.2
+Version: 1.0.3
 Summary: Multicorn-based PostgreSQL foreign data wrapper for Google Spreadsheets
 Home-page: https://github.com/TheDeadJoe/google_spreadsheets_fdw
 Author: TheDeadJoe
-License: UNKNOWN
-Description: # Google Spreadsheets FDW
-        
-        Multicorn based PostgreSQL foreign data wrapper for Google Spreadsheets
-        
-        ## Installation
-        
-        ### Requirements
-        
-        PostgreSQL 9.1+ with [Multicorn](http://multicorn.org/) extension installed.
-        
-        If you haven't used Multicorn yet, enable it with:
-        
-        ```postgresql
-        create extension multicorn;
-        ```
-        
-        From source:
-        
-        ```bash
-        git clone https://github.com/TheDeadJoe/google_spreadsheets_fdw
-        cd google_spreadsheets_fdw
-        python setup.py install
-        ```
-        
-        ## Usage
-        
-        ```postgresql
-        create server multicorn_srv foreign data wrapper multicorn options (
-            wrapper 'google_spreadsheets_fdw.GoogleSpreadsheetFDW'
-        );
-        
-        create foreign table my_table (
-            id int default nextval('my_seq'),
-            foo varchar,
-            bar int,
-            baz float
-        ) server multicorn_srv options (
-            gskey 'zVshdGDuaQKKaQoXqNOwjeTWcxcUtOlSJDZoLeIMUsYx',
-            keyfile '/path/to/credentials.json',
-            sheet '0',
-            row_id 'id'
-        );
-        ```
-        
-        ### Options
-        
-        - `gskey` - "ID" of a spreadsheet (the 44 char length part between `/spreadsheets/d/` and `/edit/` from spreadsheet URL)
-        - `keyfile` - path to Google Cloud Services credentials json file
-        - `sheet` - index of a sheet
-        - `row_id` - name of the column which value will be treated as an ID of the whole row
-        
-        ## Example
-        
-        We start with an empty spreadsheet:
-        
-        ![1](https://user-images.githubusercontent.com/8329442/87254938-d9629600-c486-11ea-8ed2-b5ccb342868b.png)
-        
-        Let's insert some data into it:
-        
-        ```postgresql
-        insert into my_table(foo, bar, baz) values ('a', 1, 0.1);
-        insert into my_table(foo, bar, baz) values ('b', 2, 0.2);
-        insert into my_table(foo, bar, baz) values ('c', 3, 0.3);
-        insert into my_table(baz, bar, foo) values (0.4, 4, 'd') returning *;
-        ```
-        
-        Spreadsheet contains our data.
-        
-        ![2](https://user-images.githubusercontent.com/8329442/87254971-2a728a00-c487-11ea-88ac-9916b84af62f.png)
-        
-        Now let's try retrieve the data:
-        
-        ```postgresql
-        select * from my_table;
-        ```
-        
-        The result:
-        
-        ![3](https://user-images.githubusercontent.com/8329442/87254972-2ba3b700-c487-11ea-8a44-4d993aeeeccd.png)
-        
-        
-        Of course, we can also perform other SQL operations e.g.: 
-        
-        ```postgresql
-        update my_table set bar = 9, baz = 0.9 where bar = 2;
-        
-        delete from my_table where bar > 5;
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: gspread<4.0.0,>=3.6.0
+Requires-Dist: multicorn<3.0.0,>=1.4.0
+Requires-Dist: oauth2client<5.0.0,==4.1.3
+
+# Google Spreadsheets FDW
+
+Multicorn based PostgreSQL foreign data wrapper for Google Spreadsheets
+
+## Installation
+
+### Requirements
+
+PostgreSQL 9.1+ with [Multicorn](http://multicorn.org/) extension installed.
+
+If you haven't used Multicorn yet, enable it with:
+
+```postgresql
+create extension multicorn;
+```
+
+From source:
+
+```bash
+git clone https://github.com/TheDeadJoe/google_spreadsheets_fdw
+cd google_spreadsheets_fdw
+python setup.py install
+```
+
+## Usage
+
+```postgresql
+create server multicorn_srv foreign data wrapper multicorn options (
+    wrapper 'google_spreadsheets_fdw.GoogleSpreadsheetFDW'
+);
+
+create foreign table my_table (
+    id int default nextval('my_seq'),
+    foo varchar,
+    bar int,
+    baz float
+) server multicorn_srv options (
+    gskey 'zVshdGDuaQKKaQoXqNOwjeTWcxcUtOlSJDZoLeIMUsYx',
+    keyfile '/path/to/credentials.json',
+    sheet '0',
+    row_id 'id'
+);
+```
+
+### Options
+
+- `gskey` - "ID" of a spreadsheet (the 44 char length part between `/spreadsheets/d/` and `/edit/` from spreadsheet URL)
+- `keyfile` - path to Google Cloud Services credentials json file
+- `sheet` - index of a sheet
+- `row_id` - name of the column which value will be treated as an ID of the whole row
+
+## Example
+
+We start with an empty spreadsheet:
+
+![1](https://user-images.githubusercontent.com/8329442/87254938-d9629600-c486-11ea-8ed2-b5ccb342868b.png)
+
+Let's insert some data into it:
+
+```postgresql
+insert into my_table(foo, bar, baz) values ('a', 1, 0.1);
+insert into my_table(foo, bar, baz) values ('b', 2, 0.2);
+insert into my_table(foo, bar, baz) values ('c', 3, 0.3);
+insert into my_table(baz, bar, foo) values (0.4, 4, 'd') returning *;
+```
+
+Spreadsheet contains our data.
+
+![2](https://user-images.githubusercontent.com/8329442/87254971-2a728a00-c487-11ea-88ac-9916b84af62f.png)
+
+Now let's try retrieve the data:
+
+```postgresql
+select * from my_table;
+```
+
+The result:
+
+![3](https://user-images.githubusercontent.com/8329442/87254972-2ba3b700-c487-11ea-8a44-4d993aeeeccd.png)
+
+
+Of course, we can also perform other SQL operations e.g.: 
+
+```postgresql
+update my_table set bar = 9, baz = 0.9 where bar = 2;
+
+delete from my_table where bar > 5;
+```
```

### Comparing `google_spreadsheets_fdw-1.0.2/README.md` & `google_spreadsheets_fdw-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `google_spreadsheets_fdw-1.0.2/google_spreadsheets_fdw/__init__.py` & `google_spreadsheets_fdw-1.0.3/google_spreadsheets_fdw/__init__.py`

 * *Files identical despite different names*

### Comparing `google_spreadsheets_fdw-1.0.2/google_spreadsheets_fdw.egg-info/PKG-INFO` & `google_spreadsheets_fdw-1.0.3/google_spreadsheets_fdw.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,101 +1,103 @@
 Metadata-Version: 2.1
-Name: google-spreadsheets-fdw
-Version: 1.0.2
+Name: google_spreadsheets_fdw
+Version: 1.0.3
 Summary: Multicorn-based PostgreSQL foreign data wrapper for Google Spreadsheets
 Home-page: https://github.com/TheDeadJoe/google_spreadsheets_fdw
 Author: TheDeadJoe
-License: UNKNOWN
-Description: # Google Spreadsheets FDW
-        
-        Multicorn based PostgreSQL foreign data wrapper for Google Spreadsheets
-        
-        ## Installation
-        
-        ### Requirements
-        
-        PostgreSQL 9.1+ with [Multicorn](http://multicorn.org/) extension installed.
-        
-        If you haven't used Multicorn yet, enable it with:
-        
-        ```postgresql
-        create extension multicorn;
-        ```
-        
-        From source:
-        
-        ```bash
-        git clone https://github.com/TheDeadJoe/google_spreadsheets_fdw
-        cd google_spreadsheets_fdw
-        python setup.py install
-        ```
-        
-        ## Usage
-        
-        ```postgresql
-        create server multicorn_srv foreign data wrapper multicorn options (
-            wrapper 'google_spreadsheets_fdw.GoogleSpreadsheetFDW'
-        );
-        
-        create foreign table my_table (
-            id int default nextval('my_seq'),
-            foo varchar,
-            bar int,
-            baz float
-        ) server multicorn_srv options (
-            gskey 'zVshdGDuaQKKaQoXqNOwjeTWcxcUtOlSJDZoLeIMUsYx',
-            keyfile '/path/to/credentials.json',
-            sheet '0',
-            row_id 'id'
-        );
-        ```
-        
-        ### Options
-        
-        - `gskey` - "ID" of a spreadsheet (the 44 char length part between `/spreadsheets/d/` and `/edit/` from spreadsheet URL)
-        - `keyfile` - path to Google Cloud Services credentials json file
-        - `sheet` - index of a sheet
-        - `row_id` - name of the column which value will be treated as an ID of the whole row
-        
-        ## Example
-        
-        We start with an empty spreadsheet:
-        
-        ![1](https://user-images.githubusercontent.com/8329442/87254938-d9629600-c486-11ea-8ed2-b5ccb342868b.png)
-        
-        Let's insert some data into it:
-        
-        ```postgresql
-        insert into my_table(foo, bar, baz) values ('a', 1, 0.1);
-        insert into my_table(foo, bar, baz) values ('b', 2, 0.2);
-        insert into my_table(foo, bar, baz) values ('c', 3, 0.3);
-        insert into my_table(baz, bar, foo) values (0.4, 4, 'd') returning *;
-        ```
-        
-        Spreadsheet contains our data.
-        
-        ![2](https://user-images.githubusercontent.com/8329442/87254971-2a728a00-c487-11ea-88ac-9916b84af62f.png)
-        
-        Now let's try retrieve the data:
-        
-        ```postgresql
-        select * from my_table;
-        ```
-        
-        The result:
-        
-        ![3](https://user-images.githubusercontent.com/8329442/87254972-2ba3b700-c487-11ea-8a44-4d993aeeeccd.png)
-        
-        
-        Of course, we can also perform other SQL operations e.g.: 
-        
-        ```postgresql
-        update my_table set bar = 9, baz = 0.9 where bar = 2;
-        
-        delete from my_table where bar > 5;
-        ```
-        
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.5
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: gspread<4.0.0,>=3.6.0
+Requires-Dist: multicorn<3.0.0,>=1.4.0
+Requires-Dist: oauth2client<5.0.0,==4.1.3
+
+# Google Spreadsheets FDW
+
+Multicorn based PostgreSQL foreign data wrapper for Google Spreadsheets
+
+## Installation
+
+### Requirements
+
+PostgreSQL 9.1+ with [Multicorn](http://multicorn.org/) extension installed.
+
+If you haven't used Multicorn yet, enable it with:
+
+```postgresql
+create extension multicorn;
+```
+
+From source:
+
+```bash
+git clone https://github.com/TheDeadJoe/google_spreadsheets_fdw
+cd google_spreadsheets_fdw
+python setup.py install
+```
+
+## Usage
+
+```postgresql
+create server multicorn_srv foreign data wrapper multicorn options (
+    wrapper 'google_spreadsheets_fdw.GoogleSpreadsheetFDW'
+);
+
+create foreign table my_table (
+    id int default nextval('my_seq'),
+    foo varchar,
+    bar int,
+    baz float
+) server multicorn_srv options (
+    gskey 'zVshdGDuaQKKaQoXqNOwjeTWcxcUtOlSJDZoLeIMUsYx',
+    keyfile '/path/to/credentials.json',
+    sheet '0',
+    row_id 'id'
+);
+```
+
+### Options
+
+- `gskey` - "ID" of a spreadsheet (the 44 char length part between `/spreadsheets/d/` and `/edit/` from spreadsheet URL)
+- `keyfile` - path to Google Cloud Services credentials json file
+- `sheet` - index of a sheet
+- `row_id` - name of the column which value will be treated as an ID of the whole row
+
+## Example
+
+We start with an empty spreadsheet:
+
+![1](https://user-images.githubusercontent.com/8329442/87254938-d9629600-c486-11ea-8ed2-b5ccb342868b.png)
+
+Let's insert some data into it:
+
+```postgresql
+insert into my_table(foo, bar, baz) values ('a', 1, 0.1);
+insert into my_table(foo, bar, baz) values ('b', 2, 0.2);
+insert into my_table(foo, bar, baz) values ('c', 3, 0.3);
+insert into my_table(baz, bar, foo) values (0.4, 4, 'd') returning *;
+```
+
+Spreadsheet contains our data.
+
+![2](https://user-images.githubusercontent.com/8329442/87254971-2a728a00-c487-11ea-88ac-9916b84af62f.png)
+
+Now let's try retrieve the data:
+
+```postgresql
+select * from my_table;
+```
+
+The result:
+
+![3](https://user-images.githubusercontent.com/8329442/87254972-2ba3b700-c487-11ea-8a44-4d993aeeeccd.png)
+
+
+Of course, we can also perform other SQL operations e.g.: 
+
+```postgresql
+update my_table set bar = 9, baz = 0.9 where bar = 2;
+
+delete from my_table where bar > 5;
+```
```

### Comparing `google_spreadsheets_fdw-1.0.2/setup.py` & `google_spreadsheets_fdw-1.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="google_spreadsheets_fdw",
-    version="1.0.2",
+    version="1.0.3",
     author="TheDeadJoe",
     description="Multicorn-based PostgreSQL foreign data wrapper for Google Spreadsheets",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TheDeadJoe/google_spreadsheets_fdw",
     packages=setuptools.find_packages(),
     install_requires=[
-        'gspread==3.6.0',
-        'multicorn==1.4.0',
-        'oauth2client==4.1.3',
+        'gspread>=3.6.0,<4.0.0',
+        'multicorn>=1.4.0,<3.0.0',
+        'oauth2client==4.1.3,<5.0.0',
     ],
     classifiers=[
         "Programming Language :: Python :: 3.5",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
 )
```

