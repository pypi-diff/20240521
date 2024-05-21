# Comparing `tmp/smartcard_identifier-1.8.2.tar.gz` & `tmp/smartcard_identifier-1.8.3.tar.gz`

## Comparing `smartcard_identifier-1.8.2.tar` & `smartcard_identifier-1.8.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/Makefile
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/macOS/com.shortstorybox.SmartcardIdentifier.plist
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/macOS/distribution.xml
--rwxr-xr-x   0        0        0      378 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/macOS/scripts/postinstall
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/macOS/scripts/preinstall
--rwxr-xr-x   0        0        0     6002 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/src/smartcard_identifier.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/LICENSE
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.3/Makefile
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.3/macOS/com.shortstorybox.SmartcardIdentifier.plist
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.3/macOS/distribution.xml
+-rwxr-xr-x   0        0        0      466 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.3/macOS/scripts/postinstall
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.3/macOS/scripts/preinstall
+-rwxr-xr-x   0        0        0     6002 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.3/src/smartcard_identifier.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.3/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.3/LICENSE
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.3/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.3/PKG-INFO
```

### Comparing `smartcard_identifier-1.8.2/Makefile` & `smartcard_identifier-1.8.3/Makefile`

 * *Files identical despite different names*

### Comparing `smartcard_identifier-1.8.2/macOS/distribution.xml` & `smartcard_identifier-1.8.3/macOS/distribution.xml`

 * *Files identical despite different names*

### Comparing `smartcard_identifier-1.8.2/src/smartcard_identifier.py` & `smartcard_identifier-1.8.3/src/smartcard_identifier.py`

 * *Files identical despite different names*

### Comparing `smartcard_identifier-1.8.2/.gitignore` & `smartcard_identifier-1.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `smartcard_identifier-1.8.2/LICENSE` & `smartcard_identifier-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `smartcard_identifier-1.8.2/README.md` & `smartcard_identifier-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `smartcard_identifier-1.8.2/pyproject.toml` & `smartcard_identifier-1.8.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "smartcard-identifier"
-version = "1.8.2"
+version = "1.8.3"
 authors = [
   { name="Samuel Hoffstaetter", email="sam@shortstorybox.com" },
 ]
 description = "Read smart card ID number and emulate a keyboard to paste it as text."
 readme = "README.md"
 requires-python = ">=3.3"
 classifiers = [
```

### Comparing `smartcard_identifier-1.8.2/PKG-INFO` & `smartcard_identifier-1.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: smartcard-identifier
-Version: 1.8.2
+Version: 1.8.3
 Summary: Read smart card ID number and emulate a keyboard to paste it as text.
 Project-URL: Homepage, https://github.com/shortstorybox/smartcard-identifier
 Project-URL: Issues, https://github.com/shortstorybox/smartcard-identifier/issues
 Author-email: Samuel Hoffstaetter <sam@shortstorybox.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
```

