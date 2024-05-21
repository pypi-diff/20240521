# Comparing `tmp/pycutroh-0.1.1.tar.gz` & `tmp/pycutroh-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycutroh-0.1.1.tar", last modified: Mon Mar 11 17:34:29 2024, max compression
+gzip compressed data, was "pycutroh-0.1.2.tar", last modified: Tue May 21 16:33:14 2024, max compression
```

## Comparing `pycutroh-0.1.1.tar` & `pycutroh-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:34:29.967326 pycutroh-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-03-11 17:34:17.000000 pycutroh-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-11 17:34:29.967326 pycutroh-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-03-11 17:34:17.000000 pycutroh-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-11 17:34:17.000000 pycutroh-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 17:34:29.967326 pycutroh-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:34:29.967326 pycutroh-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:34:29.967326 pycutroh-0.1.1/src/pycutroh/
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-03-11 17:34:17.000000 pycutroh-0.1.1/src/pycutroh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-03-11 17:34:17.000000 pycutroh-0.1.1/src/pycutroh/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 17:34:29.967326 pycutroh-0.1.1/src/pycutroh.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-11 17:34:29.000000 pycutroh-0.1.1/src/pycutroh.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-11 17:34:29.000000 pycutroh-0.1.1/src/pycutroh.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 17:34:29.000000 pycutroh-0.1.1/src/pycutroh.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-11 17:34:29.000000 pycutroh-0.1.1/src/pycutroh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:33:14.179305 pycutroh-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-21 16:33:02.000000 pycutroh-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-21 16:33:14.179305 pycutroh-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-21 16:33:02.000000 pycutroh-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-21 16:33:02.000000 pycutroh-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 16:33:14.179305 pycutroh-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:33:14.175305 pycutroh-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:33:14.179305 pycutroh-0.1.2/src/pycutroh/
+-rw-r--r--   0 runner    (1001) docker     (127)     7672 2024-05-21 16:33:02.000000 pycutroh-0.1.2/src/pycutroh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3433 2024-05-21 16:33:02.000000 pycutroh-0.1.2/src/pycutroh/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:33:14.179305 pycutroh-0.1.2/src/pycutroh.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-21 16:33:14.000000 pycutroh-0.1.2/src/pycutroh.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-21 16:33:14.000000 pycutroh-0.1.2/src/pycutroh.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 16:33:14.000000 pycutroh-0.1.2/src/pycutroh.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 16:33:14.000000 pycutroh-0.1.2/src/pycutroh.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:33:14.179305 pycutroh-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7013 2024-05-21 16:33:02.000000 pycutroh-0.1.2/tests/test_pycutroh.py
```

### Comparing `pycutroh-0.1.1/LICENSE` & `pycutroh-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycutroh-0.1.1/pyproject.toml` & `pycutroh-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pycutroh"
-version = "0.1.1"
+version = "0.1.2"
 description = "A python module for cutting strings."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
   {name = "IT-Administrators" },
 ]
```

### Comparing `pycutroh-0.1.1/src/pycutroh/__main__.py` & `pycutroh-0.1.2/src/pycutroh/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,17 @@
     # Declaring parameters.
     parser = argparse.ArgumentParser()
     parser.add_argument('-s', '--string', type=str, default='This is a demonstration string.')
     group1 = parser.add_mutually_exclusive_group()
     # If using default = 0, the mutally exclusive group is not working.
     group1.add_argument('-glop', '--getLetterOnPos', type=int, help=("Letter on position to return."))
     group1.add_argument('-glbp', '--getLettersFromPosToPos', type=tuple, help=("Get letter between positions."), nargs=2)
+    group1.add_argument('-glbfs', '--getLettersBeforeSign', type=str, help=("Get letters Before specified sign."))
+    group1.add_argument('-glas', '--getLettersAfterSign', type=str, help=("Get letters after specified sign."))
+    group1.add_argument('-glbs', '--getLettersBetweenSigns', type=tuple, help=("Get letters between specified signs.") , nargs=2)
     
     # Create subparser.
     fieldparser = parser.add_subparsers(dest='fields', help=("Get fields separated by specified delimiter."))
     # Subparsers can not be optional (-f not working).
     fieldparserold = fieldparser.add_parser('f', help=("Get fields by delimiter and join using same delimiter."))
     fieldparserold.add_argument('--getFields', type=tuple, help=("Fields as tuple."), nargs="*")
     fieldparserold.add_argument('--delimiter', type=str, help=("Delimiter to use for field calculation."), nargs=1)
@@ -31,14 +34,20 @@
     elif args.getLettersFromPosToPos:
         # Create tuple from list of tuples.
         # python -m pycutroh -glbp (0,25)
         # [('0',), ('2', '5')]
         # res = (0,25)
         res = [int(' '.join(tups).replace(' ','')) for tups in args.getLettersFromPosToPos]
         print(get_letters_from_pos_to_pos(args.string, res))
+    elif args.getLettersBeforeSign:
+        print(get_letters_before_sign(args.string, args.getLettersBeforeSign))
+    elif args.getLettersAfterSign:
+        print(get_letters_after_sign(args.string, args.getLettersAfterSign))
+    elif args.getLettersBetweenSigns:
+        print(get_letters_between_signs(args.string, args.getLettersBetweenSigns[0][0], args.getLettersBetweenSigns[1][0]))
     elif args.fields:
         # # Create tuple from list of tuples.
         fieldtup = [int(' '.join(tups).replace(' ','')) for tups in args.getFields]
         # Catch if newDelimiter is used otherwise run normal get_fields function. 
         if args.newDelimiter == None:
             print(get_fields(args.string, tuple(fieldtup), args.delimiter[0]))
         elif args.getFields == 0 and args.newDelimiter != None:
```

