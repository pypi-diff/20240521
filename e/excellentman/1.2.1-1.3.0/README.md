# Comparing `tmp/excellentman-1.2.1.tar.gz` & `tmp/excellentman-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "excellentman-1.2.1.tar", last modified: Tue Feb  6 13:57:23 2024, max compression
+gzip compressed data, was "excellentman-1.3.0.tar", last modified: Tue May 21 12:55:54 2024, max compression
```

## Comparing `excellentman-1.2.1.tar` & `excellentman-1.3.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2024-02-06 13:57:23.371155 excellentman-1.2.1/
--rw-r--r--   0 alec       (501) staff       (20)     2869 2024-02-06 13:57:23.371003 excellentman-1.2.1/PKG-INFO
--rw-r--r--   0 alec       (501) staff       (20)     2508 2024-01-16 14:03:13.000000 excellentman-1.2.1/README.md
--rw-r--r--   0 alec       (501) staff       (20)       38 2024-02-06 13:57:23.371202 excellentman-1.2.1/setup.cfg
--rw-r--r--   0 alec       (501) staff       (20)     1322 2024-02-06 13:54:11.000000 excellentman-1.2.1/setup.py
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2024-02-06 13:57:23.369195 excellentman-1.2.1/src/
-drwxr-xr-x   0 alec       (501) staff       (20)        0 2024-02-06 13:57:23.370797 excellentman-1.2.1/src/excellentman.egg-info/
--rw-r--r--   0 alec       (501) staff       (20)     2869 2024-02-06 13:57:23.000000 excellentman-1.2.1/src/excellentman.egg-info/PKG-INFO
--rw-r--r--   0 alec       (501) staff       (20)      280 2024-02-06 13:57:23.000000 excellentman-1.2.1/src/excellentman.egg-info/SOURCES.txt
--rw-r--r--   0 alec       (501) staff       (20)        1 2024-02-06 13:57:23.000000 excellentman-1.2.1/src/excellentman.egg-info/dependency_links.txt
--rw-r--r--   0 alec       (501) staff       (20)       51 2024-02-06 13:57:23.000000 excellentman-1.2.1/src/excellentman.egg-info/entry_points.txt
--rw-r--r--   0 alec       (501) staff       (20)        9 2024-02-06 13:57:23.000000 excellentman-1.2.1/src/excellentman.egg-info/requires.txt
--rw-r--r--   0 alec       (501) staff       (20)       13 2024-02-06 13:57:23.000000 excellentman-1.2.1/src/excellentman.egg-info/top_level.txt
--rw-r--r--   0 alec       (501) staff       (20)     5522 2024-02-06 13:53:39.000000 excellentman-1.2.1/src/excellentman.py
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2024-05-21 12:55:54.330287 excellentman-1.3.0/
+-rw-r--r--   0 alec       (501) staff       (20)     2869 2024-05-21 12:55:54.330104 excellentman-1.3.0/PKG-INFO
+-rw-r--r--   0 alec       (501) staff       (20)     2508 2024-01-16 14:03:13.000000 excellentman-1.3.0/README.md
+-rw-r--r--   0 alec       (501) staff       (20)       38 2024-05-21 12:55:54.330341 excellentman-1.3.0/setup.cfg
+-rw-r--r--   0 alec       (501) staff       (20)     1322 2024-05-21 12:54:31.000000 excellentman-1.3.0/setup.py
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2024-05-21 12:55:54.328302 excellentman-1.3.0/src/
+drwxr-xr-x   0 alec       (501) staff       (20)        0 2024-05-21 12:55:54.329846 excellentman-1.3.0/src/excellentman.egg-info/
+-rw-r--r--   0 alec       (501) staff       (20)     2869 2024-05-21 12:55:54.000000 excellentman-1.3.0/src/excellentman.egg-info/PKG-INFO
+-rw-r--r--   0 alec       (501) staff       (20)      280 2024-05-21 12:55:54.000000 excellentman-1.3.0/src/excellentman.egg-info/SOURCES.txt
+-rw-r--r--   0 alec       (501) staff       (20)        1 2024-05-21 12:55:54.000000 excellentman-1.3.0/src/excellentman.egg-info/dependency_links.txt
+-rw-r--r--   0 alec       (501) staff       (20)       51 2024-05-21 12:55:54.000000 excellentman-1.3.0/src/excellentman.egg-info/entry_points.txt
+-rw-r--r--   0 alec       (501) staff       (20)        9 2024-05-21 12:55:54.000000 excellentman-1.3.0/src/excellentman.egg-info/requires.txt
+-rw-r--r--   0 alec       (501) staff       (20)       13 2024-05-21 12:55:54.000000 excellentman-1.3.0/src/excellentman.egg-info/top_level.txt
+-rw-r--r--   0 alec       (501) staff       (20)     6099 2024-05-21 12:54:31.000000 excellentman-1.3.0/src/excellentman.py
```

### Comparing `excellentman-1.2.1/PKG-INFO` & `excellentman-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excellentman
-Version: 1.2.1
+Version: 1.3.0
 Summary: A tool for running Newman with parameters from an Excel file
 Author: Alec and Lindsay
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `excellentman-1.2.1/README.md` & `excellentman-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `excellentman-1.2.1/setup.py` & `excellentman-1.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="excellentman",                     # This is the name of the package
-    version="1.2.1",                        
+    version="1.3.0",                        
     author="Alec and Lindsay",                     # Full name of the author
     description="A tool for running Newman with parameters from an Excel file",
     long_description=long_description,      # Long description read from the the readme file
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),    # List of all python modules to be installed
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `excellentman-1.2.1/src/excellentman.egg-info/PKG-INFO` & `excellentman-1.3.0/src/excellentman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: excellentman
-Version: 1.2.1
+Version: 1.3.0
 Summary: A tool for running Newman with parameters from an Excel file
 Author: Alec and Lindsay
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `excellentman-1.2.1/src/excellentman.py` & `excellentman-1.3.0/src/excellentman.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,32 +27,36 @@
     subprocess.run(" ".join(command), shell = True)
     if xunit_file is not None:
         insert_name_into_xunit_results(xunit_file, worksheet_csv)
 
 def insert_name_into_xunit_results(xunit_file, name):
     with open(xunit_file) as original:
         contents= original.read()
-    contents=contents.replace('classname="','classname="'+ name + " - ")
+    contents=contents.replace('package="','package="'+ name + " - ")
     with open(xunit_file,'w') as new:
         new.write(contents)
-
+        
+def match_all(worksheet_name):
+    return True
 
 def read_worksheets_from_excel(file_name):
     excel = openpyxl.load_workbook(file_name)
     return excel.worksheets
 
-def process_excel(file_name, collection, environment, custom_formats={}, custom_template=None, xunit_file=None):
+def process_excel(file_name, collection, environment, custom_formats={}, custom_template=None, xunit_file=None, worksheet_filter=match_all):
     worksheets = read_worksheets_from_excel(file_name)
     if xunit_file is not None:
         xunit_base, xunit_ext = os.path.splitext(xunit_file)
         xunit_files = []
         xunit_count = 0
     else:
         xunit_passthrough = None
     for worksheet in worksheets:
+        if not worksheet_filter(worksheet.title):
+            continue 
         if xunit_file is not None:
             xunit_count += 1
             xunit_passthrough = f"{xunit_base}_{xunit_count}{xunit_ext}"
             xunit_files.append(xunit_passthrough)
         csv_title = f'{worksheet.title}.csv'
         column_names = []
         with open(csv_title,'w', newline="") as csv_file: # for python 3
@@ -90,42 +94,49 @@
         combined_output.write(XUNIT_ENDING)
 
 def parse_xunit(xunit_file):
     with open(xunit_file) as the_file:
         lines = the_file.readlines()[2:-1]
     return "".join(lines)
 
-
+def match_string(pattern):
+    def matcher(worksheet_name):
+        return pattern in worksheet_name
+    return matcher
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("excel_file", help="The excel file containing worksheets with parameter data for postman requests")
     parser.add_argument("collection", help="The path (or a URL) to a postman JSON collection")
     parser.add_argument("environment", help="The path to a postman environment JSON", default=None)
     parser.add_argument("--custom_formats", help="The Python file containing functions to format specific fields", default={})
     parser.add_argument("--custom_template", help="The HBS file for Newman to use when formatting output.", default=None)
     parser.add_argument("--xunit_file", help="File to write xunit results to. If omitted it will not produce a file.", default=None)
+    parser.add_argument("--worksheet_filter", help="Only process worksheets that include this string in the worksheet name.", default=None)
     args = parser.parse_args()
     excel_file = args.excel_file
     collection = args.collection
     environment = args.environment
+    matcher = match_all
+    if args.worksheet_filter != None:
+        matcher = match_string(args.worksheet_filter)
     if args.custom_formats:
         import importlib
         import os.path
         import sys
 
         custom_dir, custom_formats = os.path.split(args.custom_formats)
         if custom_dir:
             sys.path.insert(0, custom_dir)
         else:
             sys.path.insert(0, os.getcwd())
         
         formats = importlib.import_module(custom_formats.strip(".py"))
         if not hasattr(formats, 'custom_formats'):
             raise Exception(f'The custom format file {args.custom_formats} was passed in but did not have a custom_formats mapped.')
-        process_excel(excel_file, collection, environment, custom_formats= formats.custom_formats,custom_template=args.custom_template,xunit_file=args.xunit_file)
+        process_excel(excel_file, collection, environment, custom_formats= formats.custom_formats,custom_template=args.custom_template,xunit_file=args.xunit_file, worksheet_filter=matcher)
     else:
-        process_excel(excel_file, collection, environment,custom_template=args.custom_template, xunit_file=args.xunit_file)
+        process_excel(excel_file, collection, environment,custom_template=args.custom_template, xunit_file=args.xunit_file, worksheet_filter=matcher)
 
 if __name__ == "__main__":
     main()
- 
+
```

