# Comparing `tmp/alfrd-0.0.2.tar.gz` & `tmp/alfrd-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alfrd-0.0.2.tar", last modified: Thu May  9 13:25:41 2024, max compression
+gzip compressed data, was "alfrd-0.0.3.tar", last modified: Tue May 21 20:52:07 2024, max compression
```

## Comparing `alfrd-0.0.2.tar` & `alfrd-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:25:41.818977 alfrd-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-09 13:25:34.000000 alfrd-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-09 13:25:41.818977 alfrd-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-05-09 13:25:34.000000 alfrd-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-09 13:25:41.818977 alfrd-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-09 13:25:34.000000 alfrd-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:25:41.814977 alfrd-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:25:41.818977 alfrd-0.0.2/src/alfrd/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-09 13:25:34.000000 alfrd-0.0.2/src/alfrd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-05-09 13:25:34.000000 alfrd-0.0.2/src/alfrd/lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5848 2024-05-09 13:25:34.000000 alfrd-0.0.2/src/alfrd/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 13:25:41.818977 alfrd-0.0.2/src/alfrd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7213 2024-05-09 13:25:41.000000 alfrd-0.0.2/src/alfrd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-09 13:25:41.000000 alfrd-0.0.2/src/alfrd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 13:25:41.000000 alfrd-0.0.2/src/alfrd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-09 13:25:41.000000 alfrd-0.0.2/src/alfrd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-09 13:25:41.000000 alfrd-0.0.2/src/alfrd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-09 13:25:41.000000 alfrd-0.0.2/src/alfrd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:52:07.419275 alfrd-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-21 20:52:03.000000 alfrd-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-21 20:52:07.419275 alfrd-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6296 2024-05-21 20:52:03.000000 alfrd-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-21 20:52:07.419275 alfrd-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-21 20:52:03.000000 alfrd-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:52:07.415275 alfrd-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:52:07.415275 alfrd-0.0.3/src/alfrd/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-21 20:52:03.000000 alfrd-0.0.3/src/alfrd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9972 2024-05-21 20:52:03.000000 alfrd-0.0.3/src/alfrd/lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-05-21 20:52:03.000000 alfrd-0.0.3/src/alfrd/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:52:07.419275 alfrd-0.0.3/src/alfrd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7282 2024-05-21 20:52:07.000000 alfrd-0.0.3/src/alfrd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-21 20:52:07.000000 alfrd-0.0.3/src/alfrd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:52:07.000000 alfrd-0.0.3/src/alfrd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 20:52:07.000000 alfrd-0.0.3/src/alfrd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-21 20:52:07.000000 alfrd-0.0.3/src/alfrd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 20:52:07.000000 alfrd-0.0.3/src/alfrd.egg-info/top_level.txt
```

### Comparing `alfrd-0.0.2/LICENSE` & `alfrd-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alfrd-0.0.2/PKG-INFO` & `alfrd-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfrd
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automated Logical FRamework for script execution Dynamically(ALFRD)
 Home-page: https://github.com/avialxee/alfrd/
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/alfrd/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -83,23 +83,25 @@
   Select keys tab > Add keys > Create New Keys > JSON > save
   
 - step 13
   Go to the Google spreadsheet and "share" the sheet to the email address that was copied, as Editor.
 
 ### 2. Installing
 
-- Download [ALFRD](https://github.com/avialxee/alfrd) and unzip / Or 
-   `git clone https://github.com/avialxee/alfrd`
-   
-- install alfrd
-    ```
+- Install using the pip package manager:
+  ```bash
+  pip install alfrd
+  ```
+- Alternatively Download [ALFRD](https://github.com/avialxee/alfrd) and unzip / Or 
+    ```bash
+   git clone https://github.com/avialxee/alfrd
    cd alfrd/
    pip install .
     ```
-    this should install alfrd and all the dependencies automatically.
+this should install alfrd and all the dependencies automatically.
     
 
 ### 3. Using ALFRD
 
 ##### Example 1 : Initializing and creating instance
 
 ```python
```

### Comparing `alfrd-0.0.2/README.md` & `alfrd-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -55,23 +55,25 @@
   Select keys tab > Add keys > Create New Keys > JSON > save
   
 - step 13
   Go to the Google spreadsheet and "share" the sheet to the email address that was copied, as Editor.
 
 ### 2. Installing
 
-- Download [ALFRD](https://github.com/avialxee/alfrd) and unzip / Or 
-   `git clone https://github.com/avialxee/alfrd`
-   
-- install alfrd
-    ```
+- Install using the pip package manager:
+  ```bash
+  pip install alfrd
+  ```
+- Alternatively Download [ALFRD](https://github.com/avialxee/alfrd) and unzip / Or 
+    ```bash
+   git clone https://github.com/avialxee/alfrd
    cd alfrd/
    pip install .
     ```
-    this should install alfrd and all the dependencies automatically.
+this should install alfrd and all the dependencies automatically.
     
 
 ### 3. Using ALFRD
 
 ##### Example 1 : Initializing and creating instance
 
 ```python
```

### Comparing `alfrd-0.0.2/setup.py` & `alfrd-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as rdme:
     desc = rdme.read()
 
 setup(
     name = 'alfrd',
-    version = '0.0.2',
+    version = '0.0.3',
     url='https://github.com/avialxee/alfrd/',
     author='Avinash Kumar',
     author_email='avialxee@gmail.com',
     description='Automated Logical FRamework for script execution Dynamically(ALFRD)',
     py_modules = ["alfrd"],
     package_dir={'':'src'},
     classifiers=["Programming Language :: Python :: 3",
```

### Comparing `alfrd-0.0.2/src/alfrd/lib.py` & `alfrd-0.0.3/src/alfrd/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,18 +135,24 @@
         r = str(colv).strip()
         return r
     
     def isvalue(self, value, colname=''):
         """
         Returns boolean by matching value in cell
         """
+        colname = self.working_col if not colname else colname
         v = self.get_value(colname)
         return str(value) == str(v)
     
     def put_value(self, value, colname='', count=0):
+        """
+        puts value to the colname if specified else uses working_col for the colname
+        returns +1 for the counter value
+        Note: This only modifies data in the DataFrame
+        """
         colname = self.working_col if not colname else colname
         count = self.col_data(colname=colname, data=value, count=count)
         return count
     
     def update_sheet(self, count, failed, comment_col='Comment4', csvfile = 'df_sheet.csv'):
         """
         updates the google sheet if there is atleast one new count/failed count for the update
```

### Comparing `alfrd-0.0.2/src/alfrd/util.py` & `alfrd-0.0.3/src/alfrd/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,14 @@
     ---
 
     (params, files, input_folder)
 
     """
     params = defaultdict(list)
     input_folder= None
-    # params['array_type']='generic'
-    
     files=glob.glob(f'{folder}/*{inputfile}',recursive=True)
     if not files: files=glob.glob(f'{folder}/*/*{inputfile}',recursive=False)
     if not files: files=glob.glob(f'{folder}/*/*/*{inputfile}',recursive=False)
     if files:
         input_folder = str(Path(files[-1]).parent) + '/'
         for filepath in files:
             if '.inp' in filepath:
```

### Comparing `alfrd-0.0.2/src/alfrd.egg-info/PKG-INFO` & `alfrd-0.0.3/src/alfrd.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alfrd
-Version: 0.0.2
+Version: 0.0.3
 Summary: Automated Logical FRamework for script execution Dynamically(ALFRD)
 Home-page: https://github.com/avialxee/alfrd/
 Author: Avinash Kumar
 Author-email: avialxee@gmail.com
 Project-URL: Bug Tracker, https://github.com/avialxee/alfrd/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -83,23 +83,25 @@
   Select keys tab > Add keys > Create New Keys > JSON > save
   
 - step 13
   Go to the Google spreadsheet and "share" the sheet to the email address that was copied, as Editor.
 
 ### 2. Installing
 
-- Download [ALFRD](https://github.com/avialxee/alfrd) and unzip / Or 
-   `git clone https://github.com/avialxee/alfrd`
-   
-- install alfrd
-    ```
+- Install using the pip package manager:
+  ```bash
+  pip install alfrd
+  ```
+- Alternatively Download [ALFRD](https://github.com/avialxee/alfrd) and unzip / Or 
+    ```bash
+   git clone https://github.com/avialxee/alfrd
    cd alfrd/
    pip install .
     ```
-    this should install alfrd and all the dependencies automatically.
+this should install alfrd and all the dependencies automatically.
     
 
 ### 3. Using ALFRD
 
 ##### Example 1 : Initializing and creating instance
 
 ```python
```

