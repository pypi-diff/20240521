# Comparing `tmp/PyTestLog2DB-0.3.0.tar.gz` & `tmp/PyTestLog2DB-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyTestLog2DB-0.3.0.tar", last modified: Fri May 17 08:56:02 2024, max compression
+gzip compressed data, was "PyTestLog2DB-0.3.1.tar", last modified: Tue May 21 13:42:01 2024, max compression
```

## Comparing `PyTestLog2DB-0.3.0.tar` & `PyTestLog2DB-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:56:02.688442 PyTestLog2DB-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-05-17 08:56:02.688442 PyTestLog2DB-0.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:56:02.688442 PyTestLog2DB-0.3.0/PyTestLog2DB/
--rw-r--r--   0 runner    (1001) docker     (127)   520412 2024-05-17 08:56:02.000000 PyTestLog2DB-0.3.0/PyTestLog2DB/PyTestLog2DB.pdf
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/PyTestLog2DB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/PyTestLog2DB/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43689 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/PyTestLog2DB/pytestlog2db.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/PyTestLog2DB/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:56:02.688442 PyTestLog2DB-0.3.0/PyTestLog2DB/xsd/
--rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/PyTestLog2DB/xsd/junit.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 08:56:02.688442 PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-05-17 08:56:02.000000 PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-17 08:56:02.000000 PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 08:56:02.000000 PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 08:56:02.000000 PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-17 08:56:02.000000 PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 08:56:02.688442 PyTestLog2DB-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-05-17 08:54:29.000000 PyTestLog2DB-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:42:01.388018 PyTestLog2DB-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 13:40:18.000000 PyTestLog2DB-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-05-21 13:42:01.388018 PyTestLog2DB-0.3.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:42:01.388018 PyTestLog2DB-0.3.1/PyTestLog2DB/
+-rw-r--r--   0 runner    (1001) docker     (127)   520598 2024-05-21 13:42:01.000000 PyTestLog2DB-0.3.1/PyTestLog2DB/PyTestLog2DB.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-21 13:40:18.000000 PyTestLog2DB-0.3.1/PyTestLog2DB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      693 2024-05-21 13:40:18.000000 PyTestLog2DB-0.3.1/PyTestLog2DB/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43712 2024-05-21 13:40:18.000000 PyTestLog2DB-0.3.1/PyTestLog2DB/pytestlog2db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-21 13:40:18.000000 PyTestLog2DB-0.3.1/PyTestLog2DB/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:42:01.388018 PyTestLog2DB-0.3.1/PyTestLog2DB/xsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     6847 2024-05-21 13:40:18.000000 PyTestLog2DB-0.3.1/PyTestLog2DB/xsd/junit.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 13:42:01.388018 PyTestLog2DB-0.3.1/PyTestLog2DB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10878 2024-05-21 13:42:01.000000 PyTestLog2DB-0.3.1/PyTestLog2DB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-21 13:42:01.000000 PyTestLog2DB-0.3.1/PyTestLog2DB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 13:42:01.000000 PyTestLog2DB-0.3.1/PyTestLog2DB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-21 13:42:01.000000 PyTestLog2DB-0.3.1/PyTestLog2DB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-21 13:42:01.000000 PyTestLog2DB-0.3.1/PyTestLog2DB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    10041 2024-05-21 13:40:18.000000 PyTestLog2DB-0.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 13:42:01.388018 PyTestLog2DB-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     9117 2024-05-21 13:40:18.000000 PyTestLog2DB-0.3.1/setup.py
```

### Comparing `PyTestLog2DB-0.3.0/LICENSE` & `PyTestLog2DB-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.3.0/PKG-INFO` & `PyTestLog2DB-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTestLog2DB
-Version: 0.3.0
+Version: 0.3.1
 Summary: Imports pytest result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/python-pytestlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyTestLog2DB-0.3.0/PyTestLog2DB/PyTestLog2DB.pdf` & `PyTestLog2DB-0.3.1/PyTestLog2DB/PyTestLog2DB.pdf`

 * *Files 6% similar despite different names*

#### Comparing `PyTestLog2DB-0.3.0/PyTestLog2DB/PyTestLog2DB.pdf` & `PyTestLog2DB-0.3.1/PyTestLog2DB/PyTestLog2DB.pdf`

 * *Document info*

```diff
@@ -1,10 +1,10 @@
 Author: ''
-CreationDate: 'D:20240517085601Z'
+CreationDate: 'D:20240521134159Z'
 Creator: 'LaTeX with hyperref'
 Keywords: ''
-ModDate: 'D:20240517085601Z'
+ModDate: 'D:20240521134159Z'
 PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.22 (TeX Live 2022/dev/Debian) kpathsea version 6.3.4/dev'
 Producer: 'pdfTeX-1.40.22'
 Subject: ''
 Title: ''
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,11 +1,11 @@
 PyTestLog2DB
-v. 0.3.0
+v. 0.3.1
 Tran Duy Ngoan
-07.05.2024
+20.05.2024
 
 CONTENTS
 
 CONTENTS
 
 Contents
 1 Introduction
@@ -1016,19 +1016,19 @@
 
 Name
 
 PyTestLog2DB
 
 Version
 
-0.3.0
+0.3.1
 
 Date
 
-07.05.2024
+20.05.2024
 
 Description
 
 Imports pytest result(s) to TestResultWebApp database
 
 Package URL
 
@@ -1140,21 +1140,30 @@
 Fix missing return of test duration when failed to import testcase
 0.3.0
 
 07.05.2024
 
 Add optional argument
 and rest interfaces
+0.3.1
 
 --interface
 
 which allow to switch between
 
-PyTestLog2DB.pdf
-Created at 17.05.2024 - 08:55:59
-by GenPackageDoc v. 0.41.1
+20.05.2024
+
+Fix type error of lastlog when import with rest interface
 
 18
 
 db
 
+CHAPTER 5. HISTORY
+
+PyTestLog2DB.pdf
+Created at 21.05.2024 - 13:41:57
+by GenPackageDoc v. 0.41.1
+
+19
+
```

### Comparing `PyTestLog2DB-0.3.0/PyTestLog2DB/__init__.py` & `PyTestLog2DB-0.3.1/PyTestLog2DB/__init__.py`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.3.0/PyTestLog2DB/__main__.py` & `PyTestLog2DB-0.3.1/PyTestLog2DB/__main__.py`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.3.0/PyTestLog2DB/pytestlog2db.py` & `PyTestLog2DB-0.3.1/PyTestLog2DB/pytestlog2db.py`

 * *Files 0% similar despite different names*

```diff
@@ -674,15 +674,15 @@
       traceback_log = f"{error[0].get('message')}\n{error[0].text}"
       return_code = 5
    elif list(oTest.iterchildren("skipped")):
       main_result = "unknown"
       traceback_log = f"This test is skipped."
       return_code = 20
 
-   return (main_result, base64.b64encode(traceback_log.encode()), return_code)
+   return (main_result, str(base64.b64encode(traceback_log.encode()), encoding='utf-8'), return_code)
 
 def process_component_info(dConfig, sTestClassname):
    """
 Return the component name bases on provided testcase's classname and component
 mapping.
 
 **Arguments:**
```

### Comparing `PyTestLog2DB-0.3.0/PyTestLog2DB/version.py` & `PyTestLog2DB-0.3.1/PyTestLog2DB/version.py`

 * *Files 17% similar despite different names*

```diff
@@ -14,10 +14,10 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 #
 # **************************************************************************************************************
 #
 # Version and date of PyTestLog2DB
 #
-VERSION      = "0.3.0"
-VERSION_DATE = "07.05.2024"
+VERSION      = "0.3.1"
+VERSION_DATE = "20.05.2024"
```

### Comparing `PyTestLog2DB-0.3.0/PyTestLog2DB/xsd/junit.xsd` & `PyTestLog2DB-0.3.1/PyTestLog2DB/xsd/junit.xsd`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.3.0/PyTestLog2DB.egg-info/PKG-INFO` & `PyTestLog2DB-0.3.1/PyTestLog2DB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyTestLog2DB
-Version: 0.3.0
+Version: 0.3.1
 Summary: Imports pytest result(s) to TestResultWebApp database
 Home-page: https://github.com/test-fullautomation/python-pytestlog2db
 Author: Tran Duy Ngoan
 Author-email: Ngoan.TranDuy@vn.bosch.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `PyTestLog2DB-0.3.0/README.rst` & `PyTestLog2DB-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `PyTestLog2DB-0.3.0/setup.py` & `PyTestLog2DB-0.3.1/setup.py`

 * *Files identical despite different names*

