# Comparing `tmp/sde-1.1.8.tar.gz` & `tmp/sde-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sde-1.1.8.tar", last modified: Wed Mar 30 15:54:09 2022, max compression
+gzip compressed data, was "sde-1.1.9.tar", last modified: Mon Nov 14 07:50:50 2022, max compression
```

## Comparing `sde-1.1.8.tar` & `sde-1.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 15:54:09.556947 sde-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-03-30 15:53:58.000000 sde-1.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-03-30 15:54:09.556947 sde-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2257 2022-03-30 15:53:58.000000 sde-1.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 15:54:09.556947 sde-1.1.8/sde/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-03-30 15:53:58.000000 sde-1.1.8/sde/__about__.py
--rw-r--r--   0 runner    (1001) docker     (121)      954 2022-03-30 15:53:58.000000 sde-1.1.8/sde/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       30 2022-03-30 15:53:58.000000 sde-1.1.8/sde/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12300 2022-03-30 15:53:58.000000 sde-1.1.8/sde/collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3459 2022-03-30 15:53:58.000000 sde-1.1.8/sde/sde.py
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-03-30 15:53:58.000000 sde-1.1.8/sde/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 15:54:09.556947 sde-1.1.8/sde.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2850 2022-03-30 15:54:09.000000 sde-1.1.8/sde.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      307 2022-03-30 15:54:09.000000 sde-1.1.8/sde.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-30 15:54:09.000000 sde-1.1.8/sde.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-03-30 15:54:09.000000 sde-1.1.8/sde.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-30 15:54:09.000000 sde-1.1.8/sde.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-03-30 15:54:09.000000 sde-1.1.8/sde.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        4 2022-03-30 15:54:09.000000 sde-1.1.8/sde.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-30 15:54:09.556947 sde-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-03-30 15:53:58.000000 sde-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:50:50.400618 sde-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1326 2022-11-14 07:50:41.000000 sde-1.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-11-14 07:50:50.400618 sde-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2723 2022-11-14 07:50:41.000000 sde-1.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:50:50.400618 sde-1.1.9/sde/
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2022-11-14 07:50:41.000000 sde-1.1.9/sde/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      954 2022-11-14 07:50:41.000000 sde-1.1.9/sde/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       30 2022-11-14 07:50:41.000000 sde-1.1.9/sde/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12300 2022-11-14 07:50:41.000000 sde-1.1.9/sde/collection.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3905 2022-11-14 07:50:41.000000 sde-1.1.9/sde/sde.py
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-11-14 07:50:41.000000 sde-1.1.9/sde/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-14 07:50:50.400618 sde-1.1.9/sde.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3296 2022-11-14 07:50:50.000000 sde-1.1.9/sde.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      307 2022-11-14 07:50:50.000000 sde-1.1.9/sde.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 07:50:50.000000 sde-1.1.9/sde.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-11-14 07:50:50.000000 sde-1.1.9/sde.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-14 07:50:50.000000 sde-1.1.9/sde.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-11-14 07:50:50.000000 sde-1.1.9/sde.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        4 2022-11-14 07:50:50.000000 sde-1.1.9/sde.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-14 07:50:50.400618 sde-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1850 2022-11-14 07:50:41.000000 sde-1.1.9/setup.py
```

### Comparing `sde-1.1.8/LICENSE` & `sde-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sde-1.1.8/PKG-INFO` & `sde-1.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sde
-Version: 1.1.8
+Version: 1.1.9
 Summary: A CLI tool to edit simple JSON and YAML data files
 Home-page: https://github.com/dvershinin/sde
 Author: Danila Vershinin
 Author-email: info@getpagespeed.com
 License: BSD
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Provides-Extra: tests
@@ -33,17 +32,23 @@
 
 ```bash
 jq '.address = "abcde"' test.json|sponge test.json
 ```
     
 Does this seem readable or elegant to you?
 
+How about this instead:
+
+```bash
+sde address abcde test.json
+```
+
 `sde` is not a substitute for `jq` or `sed`.
 
-It allows *simple* in-place JSON/YAML value changes, for *simple* data.
+It allows *simple* in-place JSON/YAML value changes, for *structured* data.
 
 ### Sample JSON
 
 ```json
 {
    "name":"John",
    "age":31,
@@ -66,15 +71,15 @@
 
 ```bash
 sde name Jack data.json
 sde extra.gender male data.json
 sde database.user john data.yml
 ```
 
-It is possible to modify data in arrays, e.g.:
+It is possible to modify data in arrays using a dotted notation. Let's take another sample:
 
 ```json
 {
     "users": [
         {
             "username": "foo", 
             "enabled": true
@@ -83,21 +88,21 @@
             "username": "bar", 
             "enabled": true
         }      
     ],
 }
 ```
 
-Set the first user's `enabled` property to `false`:
+We can set the first user's `enabled` property to `false`:
 
 ```bash
 sde users.0.enabled false data.json
 ```
 
-## Installation for CentOS/RHEL 7, 8 or Amazon Linux 2
+## Installation for CentOS/RHEL 7, 8 or Amazon Linux 2, or Fedora Linux
 
 ```bash
 sudo yum -y install https://extras.getpagespeed.com/release-latest.rpm
 sudo yum -y install sde
 ```
    
 ## Installation for other systems
@@ -106,35 +111,50 @@
 
 ```bash
 pip install sde
 ```
 
 ## Notes
 
+### Quoting in JSON
+
 Quoting is avoided for `null`, `true`, `false`, and numeric values.
 To ensure that a given value is quoted, use `-s` (or `--string`) option:
 
 ```bash
 sde -s key null file.json
 ```
 
+### Force-fail on missing keys
+
 If you must *edit* the file, by ensuring to update only the existing key, use `-e` (`--must-exist`)
 option. The program will exit without adding the key which doesn't exist.
 
 ```bash
 sde -e key val file.json
 ```
 
+### Force-fail on unchanged file
+
+If the data is unchanged after running `sde` (values already match), you can force
+a failure exit code `2` by passing the `-m` option:
+
+```bash
+sde -m key sameval file.json
+# > exit code 0
+sde -m key sameval file.json
+# > exit code 2
+```
+
 ## TODO
 
 ### Work with stdin
 
 ```bash
 echo $json | sde name Jack
 ```
 
 ### Query simple data
 
 ```bash
 sdg name data.json
 ```
-
```

### Comparing `sde-1.1.8/README.md` & `sde-1.1.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -13,17 +13,23 @@
 
 ```bash
 jq '.address = "abcde"' test.json|sponge test.json
 ```
     
 Does this seem readable or elegant to you?
 
+How about this instead:
+
+```bash
+sde address abcde test.json
+```
+
 `sde` is not a substitute for `jq` or `sed`.
 
-It allows *simple* in-place JSON/YAML value changes, for *simple* data.
+It allows *simple* in-place JSON/YAML value changes, for *structured* data.
 
 ### Sample JSON
 
 ```json
 {
    "name":"John",
    "age":31,
@@ -46,15 +52,15 @@
 
 ```bash
 sde name Jack data.json
 sde extra.gender male data.json
 sde database.user john data.yml
 ```
 
-It is possible to modify data in arrays, e.g.:
+It is possible to modify data in arrays using a dotted notation. Let's take another sample:
 
 ```json
 {
     "users": [
         {
             "username": "foo", 
             "enabled": true
@@ -63,21 +69,21 @@
             "username": "bar", 
             "enabled": true
         }      
     ],
 }
 ```
 
-Set the first user's `enabled` property to `false`:
+We can set the first user's `enabled` property to `false`:
 
 ```bash
 sde users.0.enabled false data.json
 ```
 
-## Installation for CentOS/RHEL 7, 8 or Amazon Linux 2
+## Installation for CentOS/RHEL 7, 8 or Amazon Linux 2, or Fedora Linux
 
 ```bash
 sudo yum -y install https://extras.getpagespeed.com/release-latest.rpm
 sudo yum -y install sde
 ```
    
 ## Installation for other systems
@@ -86,34 +92,50 @@
 
 ```bash
 pip install sde
 ```
 
 ## Notes
 
+### Quoting in JSON
+
 Quoting is avoided for `null`, `true`, `false`, and numeric values.
 To ensure that a given value is quoted, use `-s` (or `--string`) option:
 
 ```bash
 sde -s key null file.json
 ```
 
+### Force-fail on missing keys
+
 If you must *edit* the file, by ensuring to update only the existing key, use `-e` (`--must-exist`)
 option. The program will exit without adding the key which doesn't exist.
 
 ```bash
 sde -e key val file.json
 ```
 
+### Force-fail on unchanged file
+
+If the data is unchanged after running `sde` (values already match), you can force
+a failure exit code `2` by passing the `-m` option:
+
+```bash
+sde -m key sameval file.json
+# > exit code 0
+sde -m key sameval file.json
+# > exit code 2
+```
+
 ## TODO
 
 ### Work with stdin
 
 ```bash
 echo $json | sde name Jack
 ```
 
 ### Query simple data
 
 ```bash
 sdg name data.json
-```
+```
```

### Comparing `sde-1.1.8/sde/__init__.py` & `sde-1.1.9/sde/__init__.py`

 * *Files identical despite different names*

### Comparing `sde-1.1.8/sde/collection.py` & `sde-1.1.9/sde/collection.py`

 * *Files identical despite different names*

### Comparing `sde-1.1.8/sde/sde.py` & `sde-1.1.9/sde/sde.py`

 * *Files 25% similar despite different names*

```diff
@@ -20,23 +20,25 @@
 if sys.version_info[0] >= 3:
     # Python 3
     unicode = str
 
 
 def edit_file(key, value, file, fmt, must_exist=False):
     data = DottedDict(read_file(file, fmt))
-    if must_exist:
-        try:
-            # this is the way I found it works for array vals too
-            # e.g. fruits.0.name
-            data[key]
-        except KeyError:
+    try:
+        # this is the way I found it works for array vals too
+        # e.g. fruits.0.name
+        if data[key] == value and type(data[key]) == type(value):
+            # prevents writing to the file is value is matching already
+            return False
+    except KeyError:
+        if must_exist:
             raise ValueError('{} is not present in {}'.format(key, file))
     data[key] = value
-    write_file(file, fmt, data)
+    return write_file(file, fmt, data)
 
 
 def read_file(file, fmt):
     load = {
         _JSON: json.load,
         _YAML: yaml.safe_load,
     }[fmt]
@@ -56,14 +58,15 @@
     }[fmt]
     tmp = file + ".tmp"
     with os.fdopen(os.open(tmp, os.O_WRONLY | os.O_CREAT | os.O_EXCL), "w") as fd:
         try:
             fd.write(to())
             fd.close()
             os.rename(tmp, file)
+            return True
         except Exception:
             # We can assume we can remove it, because we successfully created
             # it with O_EXCL above.
             os.unlink(tmp)
             raise
 
 
@@ -99,19 +102,21 @@
                                      epilog=epilog,
                                      prog='sde')
     parser.add_argument('key', metavar='<key>', help='Key to edit')
     parser.add_argument('val', metavar='<val>', help='New value')
     parser.add_argument('file', metavar='<filename>', help='Filename to edit')
     parser.add_argument('-e', '--must-exist', dest='must_exist', action='store_true',
                         help='Throw error and exit if the key does not already exist')
+    parser.add_argument('-m', '--must-change', dest='must_change', action='store_true',
+                        help='Exit with status code 2 if the values already match and file unchanged')
     parser.add_argument('-s', '--string', dest='is_string', action='store_true',
                         help='Always treat value as a string by quoting it')
     parser.add_argument('--version', action='version',
                         version='%(prog)s {version}'.format(version=__version__))
-    parser.set_defaults(is_string=False, must_exist=False)
+    parser.set_defaults(is_string=False, must_exist=False, must_change=False)
     args = parser.parse_args()
 
     if args.is_string:
         val = args.val
     else:
         val = normalize_val(args.val)
 
@@ -119,11 +124,13 @@
 
     fmt = _FORMATS.get(extension, None)
     if fmt is None:
         print("\033[91mError: \033[0mUnknown extension: " + extension, file=sys.stderr)
         sys.exit(1)
 
     try:
-        edit_file(args.key, val, args.file, fmt, must_exist=args.must_exist)
+        res = edit_file(args.key, val, args.file, fmt, must_exist=args.must_exist)
+        if args.must_change and res is False:
+            sys.exit(2)
     except ValueError as e:
         print("\033[91mError: \033[0m" + str(e), file=sys.stderr)
         sys.exit(1)
```

### Comparing `sde-1.1.8/sde.egg-info/PKG-INFO` & `sde-1.1.9/sde.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: sde
-Version: 1.1.8
+Version: 1.1.9
 Summary: A CLI tool to edit simple JSON and YAML data files
 Home-page: https://github.com/dvershinin/sde
 Author: Danila Vershinin
 Author-email: info@getpagespeed.com
 License: BSD
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Provides-Extra: tests
@@ -33,17 +32,23 @@
 
 ```bash
 jq '.address = "abcde"' test.json|sponge test.json
 ```
     
 Does this seem readable or elegant to you?
 
+How about this instead:
+
+```bash
+sde address abcde test.json
+```
+
 `sde` is not a substitute for `jq` or `sed`.
 
-It allows *simple* in-place JSON/YAML value changes, for *simple* data.
+It allows *simple* in-place JSON/YAML value changes, for *structured* data.
 
 ### Sample JSON
 
 ```json
 {
    "name":"John",
    "age":31,
@@ -66,15 +71,15 @@
 
 ```bash
 sde name Jack data.json
 sde extra.gender male data.json
 sde database.user john data.yml
 ```
 
-It is possible to modify data in arrays, e.g.:
+It is possible to modify data in arrays using a dotted notation. Let's take another sample:
 
 ```json
 {
     "users": [
         {
             "username": "foo", 
             "enabled": true
@@ -83,21 +88,21 @@
             "username": "bar", 
             "enabled": true
         }      
     ],
 }
 ```
 
-Set the first user's `enabled` property to `false`:
+We can set the first user's `enabled` property to `false`:
 
 ```bash
 sde users.0.enabled false data.json
 ```
 
-## Installation for CentOS/RHEL 7, 8 or Amazon Linux 2
+## Installation for CentOS/RHEL 7, 8 or Amazon Linux 2, or Fedora Linux
 
 ```bash
 sudo yum -y install https://extras.getpagespeed.com/release-latest.rpm
 sudo yum -y install sde
 ```
    
 ## Installation for other systems
@@ -106,35 +111,50 @@
 
 ```bash
 pip install sde
 ```
 
 ## Notes
 
+### Quoting in JSON
+
 Quoting is avoided for `null`, `true`, `false`, and numeric values.
 To ensure that a given value is quoted, use `-s` (or `--string`) option:
 
 ```bash
 sde -s key null file.json
 ```
 
+### Force-fail on missing keys
+
 If you must *edit* the file, by ensuring to update only the existing key, use `-e` (`--must-exist`)
 option. The program will exit without adding the key which doesn't exist.
 
 ```bash
 sde -e key val file.json
 ```
 
+### Force-fail on unchanged file
+
+If the data is unchanged after running `sde` (values already match), you can force
+a failure exit code `2` by passing the `-m` option:
+
+```bash
+sde -m key sameval file.json
+# > exit code 0
+sde -m key sameval file.json
+# > exit code 2
+```
+
 ## TODO
 
 ### Work with stdin
 
 ```bash
 echo $json | sde name Jack
 ```
 
 ### Query simple data
 
 ```bash
 sdg name data.json
 ```
-
```

### Comparing `sde-1.1.8/setup.py` & `sde-1.1.9/setup.py`

 * *Files identical despite different names*

