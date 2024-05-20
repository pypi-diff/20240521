# Comparing `tmp/smartcard_identifier-1.8.1.tar.gz` & `tmp/smartcard_identifier-1.8.2.tar.gz`

## Comparing `smartcard_identifier-1.8.1.tar` & `smartcard_identifier-1.8.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/Makefile
--rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/macOS/com.shortstorybox.SmartcardIdentifier.plist
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/macOS/distribution.xml
--rwxr-xr-x   0        0        0      378 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/macOS/scripts/postinstall
--rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/macOS/scripts/preinstall
--rwxr-xr-x   0        0        0     5980 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/src/smartcard_identifier.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/LICENSE
--rw-r--r--   0        0        0     2128 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/README.md
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/pyproject.toml
--rw-r--r--   0        0        0     2871 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.1/PKG-INFO
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/Makefile
+-rw-r--r--   0        0        0      432 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/macOS/com.shortstorybox.SmartcardIdentifier.plist
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/macOS/distribution.xml
+-rwxr-xr-x   0        0        0      378 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/macOS/scripts/postinstall
+-rwxr-xr-x   0        0        0      251 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/macOS/scripts/preinstall
+-rwxr-xr-x   0        0        0     6002 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/src/smartcard_identifier.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/LICENSE
+-rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/README.md
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/pyproject.toml
+-rw-r--r--   0        0        0     2801 2020-02-02 00:00:00.000000 smartcard_identifier-1.8.2/PKG-INFO
```

### Comparing `smartcard_identifier-1.8.1/Makefile` & `smartcard_identifier-1.8.2/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -16,41 +16,41 @@
 	# installed in your keychain. You can download it from
 	# https://developer.apple.com/account/resources/certificates/list
 	productbuild --distribution macOS/distribution.xml --package-path build/ --sign 'Developer ID Installer: Short Story, Inc. (PD7WK7PS94)' SmartcardIdentifier.pkg
 
 .PHONY: dist
 dist: lint
 	rm -rf dist/
-	python3 -m pip install build
+	python3 -m pip install build --break-system-packages
 	python3 -m build
 
 .PHONY: lint
 lint:
-	python3 -m pip install ruff black isort
+	python3 -m pip install ruff black isort --break-system-packages
 	python3 -m ruff check src/
 	@python3 -m black --check src/ || (echo "Please run 'make format' to fix formatting issues."; exit 1)
 	@python3 -m isort src/ || (echo "Please run 'make format' to fix formatting issues."; exit 1)
 
 .PHONY: format
 format:
-	python3 -m pip install black isort
+	python3 -m pip install black isort --break-system-packages
 	python3 -m black src/
 	python3 -m isort src/
 
 .PHONY: release
 release: dist SmartcardIdentifier.pkg
 	@git diff --exit-code || (echo "Please commit your git changes before releasing."; exit 1)
 	@git diff --cached --exit-code || (echo "Please commit your git changes before releasing."; exit 1)
 	@which gh >/dev/null || (echo "The 'gh' command is missing. Please install the GitHub CLI: https://cli.github.com/"; exit 1)
 	@echo 'Uploading release to Github...'
 	@GH_PROMPT_DISABLED= gh release create --target="$$(git rev-parse HEAD)" \
 		--title=v"$$(grep '^version *= *' pyproject.toml|sed 's/^version *= *//;s/\"//g')" \
 		--generate-notes v"$$(grep '^version *= *' pyproject.toml|sed 's/^version *= *//;s/\"//g')" \
 		SmartcardIdentifier.pkg
-	python3 -m pip install --upgrade twine
+	python3 -m pip install --upgrade twine --break-system-packages
 	@echo
 	@if [ ! -e ~/.pypirc ]; \
 	 then echo "Please create a PyPI API token: https://pypi.org/manage/account/token/"; \
 	      echo "Then save it to your ~/.pypirc file, or enter it as your PyPI password below."; \
 	      echo "Press Enter to continue..."; \
 	      read waiting; \
 	 fi
```

### Comparing `smartcard_identifier-1.8.1/macOS/distribution.xml` & `smartcard_identifier-1.8.2/macOS/distribution.xml`

 * *Files identical despite different names*

### Comparing `smartcard_identifier-1.8.1/src/smartcard_identifier.py` & `smartcard_identifier-1.8.2/src/smartcard_identifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 
 def simulate_keypress(text, use_linux_uinput, osx_control_modifier=False):
     """
     Paste the given text into the current application.
     """
     without_special_characters = (
-        text.replace("\n", "").replace(" ", "").replace(":", "")
+        text.replace("\n", "").replace(" ", "").replace(":", "").replace("\u00A7", "")
     )
     if without_special_characters and not without_special_characters.isalnum():
         raise Exception(
             "Keystroke text must be alphanumeric (spaces/newlines/colon allowed)"
         )
 
     if platform_system() == "Darwin":
```

### Comparing `smartcard_identifier-1.8.1/.gitignore` & `smartcard_identifier-1.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `smartcard_identifier-1.8.1/LICENSE` & `smartcard_identifier-1.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smartcard_identifier-1.8.1/README.md` & `smartcard_identifier-1.8.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Smartcard Identifier
 
 This is an extremely simple smartcard system that reads only the smart card's
 ID number, and pastes it as text into the currently open application. This can
-be used for applications that rely on nothing more than the identity of the
-scanned card, such as an authentication system in a low-security environment.
+be used for applications that rely on nothing more than the ID of the
+scanned card.
 
 
 # Installation: macOS
 
 [Download for macOS](https://github.com/shortstorybox/smartcard-identifier/releases/latest)
 
  * Install the package above. This will also add python3 to the security settings
```

### Comparing `smartcard_identifier-1.8.1/pyproject.toml` & `smartcard_identifier-1.8.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "smartcard-identifier"
-version = "1.8.1"
+version = "1.8.2"
 authors = [
   { name="Samuel Hoffstaetter", email="sam@shortstorybox.com" },
 ]
 description = "Read smart card ID number and emulate a keyboard to paste it as text."
 readme = "README.md"
 requires-python = ">=3.3"
 classifiers = [
```

### Comparing `smartcard_identifier-1.8.1/PKG-INFO` & `smartcard_identifier-1.8.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: smartcard-identifier
-Version: 1.8.1
+Version: 1.8.2
 Summary: Read smart card ID number and emulate a keyboard to paste it as text.
 Project-URL: Homepage, https://github.com/shortstorybox/smartcard-identifier
 Project-URL: Issues, https://github.com/shortstorybox/smartcard-identifier/issues
 Author-email: Samuel Hoffstaetter <sam@shortstorybox.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: MacOS :: MacOS X
@@ -15,16 +15,16 @@
 Requires-Dist: pyscard
 Description-Content-Type: text/markdown
 
 # Smartcard Identifier
 
 This is an extremely simple smartcard system that reads only the smart card's
 ID number, and pastes it as text into the currently open application. This can
-be used for applications that rely on nothing more than the identity of the
-scanned card, such as an authentication system in a low-security environment.
+be used for applications that rely on nothing more than the ID of the
+scanned card.
 
 
 # Installation: macOS
 
 [Download for macOS](https://github.com/shortstorybox/smartcard-identifier/releases/latest)
 
  * Install the package above. This will also add python3 to the security settings
```

