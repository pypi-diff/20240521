# Comparing `tmp/inni-0.5.1.tar.gz` & `tmp/inni-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inni-0.5.1.tar", max compression
+gzip compressed data, was "inni-0.5.2.tar", max compression
```

## Comparing `inni-0.5.1.tar` & `inni-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    34580 2024-03-31 17:04:25.743804 inni-0.5.1/LICENSE
--rw-r--r--   0        0        0       72 2024-03-31 17:04:25.743804 inni-0.5.1/README.md
--rw-r--r--   0        0        0        0 2024-03-31 17:05:35.833524 inni-0.5.1/inni/__init__.py
--rw-r--r--   0        0        0     4900 2024-05-07 09:05:03.056356 inni-0.5.1/inni/cli.py
--rw-r--r--   0        0        0      846 2024-04-01 18:30:02.973972 inni-0.5.1/inni/config.py
--rw-r--r--   0        0        0      302 2024-04-01 16:40:38.551065 inni-0.5.1/inni/loader.py
--rw-r--r--   0        0        0        0 2024-03-31 19:25:36.344130 inni-0.5.1/inni/modules/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-07 14:41:37.839809 inni-0.5.1/inni/modules/base.py
--rw-r--r--   0        0        0     3498 2024-05-07 09:32:52.521490 inni-0.5.1/inni/modules/bitrix.py
--rw-r--r--   0        0        0      495 2024-04-09 08:17:52.592982 inni-0.5.1/inni/modules/dummy.py
--rw-r--r--   0        0        0     1558 2024-04-08 19:28:25.219466 inni-0.5.1/inni/modules/email.py
--rw-r--r--   0        0        0     3631 2024-04-10 21:18:35.144206 inni-0.5.1/inni/modules/jira.py
--rw-r--r--   0        0        0     3204 2024-04-24 06:28:15.343430 inni-0.5.1/inni/modules/runner.py
--rw-r--r--   0        0        0     1027 2024-04-07 14:25:00.952306 inni-0.5.1/inni/modules/skype.py
--rw-r--r--   0        0        0      407 2024-04-01 18:29:29.514140 inni-0.5.1/inni/template.py
--rw-r--r--   0        0        0      742 2024-05-07 09:33:19.731707 inni-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 inni-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    34580 2024-03-31 17:04:25.743804 inni-0.5.2/LICENSE
+-rw-r--r--   0        0        0       72 2024-03-31 17:04:25.743804 inni-0.5.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-31 17:05:35.833524 inni-0.5.2/inni/__init__.py
+-rw-r--r--   0        0        0     4900 2024-05-07 09:05:03.056356 inni-0.5.2/inni/cli.py
+-rw-r--r--   0        0        0      846 2024-04-01 18:30:02.973972 inni-0.5.2/inni/config.py
+-rw-r--r--   0        0        0      302 2024-04-01 16:40:38.551065 inni-0.5.2/inni/loader.py
+-rw-r--r--   0        0        0        0 2024-03-31 19:25:36.344130 inni-0.5.2/inni/modules/__init__.py
+-rw-r--r--   0        0        0     1003 2024-04-07 14:41:37.839809 inni-0.5.2/inni/modules/base.py
+-rw-r--r--   0        0        0     3498 2024-05-21 06:38:16.901014 inni-0.5.2/inni/modules/bitrix.py
+-rw-r--r--   0        0        0      495 2024-04-09 08:17:52.592982 inni-0.5.2/inni/modules/dummy.py
+-rw-r--r--   0        0        0     1558 2024-04-08 19:28:25.219466 inni-0.5.2/inni/modules/email.py
+-rw-r--r--   0        0        0     3631 2024-04-10 21:18:35.144206 inni-0.5.2/inni/modules/jira.py
+-rw-r--r--   0        0        0     3255 2024-05-21 06:39:36.434759 inni-0.5.2/inni/modules/runner.py
+-rw-r--r--   0        0        0     1027 2024-04-07 14:25:00.952306 inni-0.5.2/inni/modules/skype.py
+-rw-r--r--   0        0        0      407 2024-04-01 18:29:29.514140 inni-0.5.2/inni/template.py
+-rw-r--r--   0        0        0      742 2024-05-21 06:40:07.144923 inni-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 inni-0.5.2/PKG-INFO
```

### Comparing `inni-0.5.1/LICENSE` & `inni-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `inni-0.5.1/inni/cli.py` & `inni-0.5.2/inni/cli.py`

 * *Files identical despite different names*

### Comparing `inni-0.5.1/inni/config.py` & `inni-0.5.2/inni/config.py`

 * *Files identical despite different names*

### Comparing `inni-0.5.1/inni/modules/base.py` & `inni-0.5.2/inni/modules/base.py`

 * *Files identical despite different names*

### Comparing `inni-0.5.1/inni/modules/bitrix.py` & `inni-0.5.2/inni/modules/bitrix.py`

 * *Files identical despite different names*

### Comparing `inni-0.5.1/inni/modules/email.py` & `inni-0.5.2/inni/modules/email.py`

 * *Files identical despite different names*

### Comparing `inni-0.5.1/inni/modules/jira.py` & `inni-0.5.2/inni/modules/jira.py`

 * *Files identical despite different names*

### Comparing `inni-0.5.1/inni/modules/runner.py` & `inni-0.5.2/inni/modules/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,16 +78,19 @@
             stderr=subprocess.DEVNULL,
             shell=shell,
         )
 
     def run_all(self, login: bool):
         entries = self.config.get("login" if login else "logout", [])
         self.processes = [
-            " ".join(i.cmdline()) or i.name() for i in psutil.process_iter()
+            " ".join(i.cmdline()) or i.name()
+            for i in psutil.process_iter()
+            if i.status() != "zombie"
         ]
+
         for entry in entries:
             self.handle_entry(entry)
             self.out.print()
 
     def login(self, responses):
         self.run_all(True)
```

### Comparing `inni-0.5.1/inni/modules/skype.py` & `inni-0.5.2/inni/modules/skype.py`

 * *Files identical despite different names*

### Comparing `inni-0.5.1/pyproject.toml` & `inni-0.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "inni"
-version = "0.5.1"
+version = "0.5.2"
 description = "Modular system to perform tasks surrounding log-in and log-out."
 authors = ["Ceda EI <ceda_ei@webionite.com>"]
 license = "GPL-3.0"
 readme = "README.md"
 homepage = "https://gitlab.com/ceda_ei/inni"
 repository = "https://gitlab.com/ceda_ei/inni"
```

### Comparing `inni-0.5.1/PKG-INFO` & `inni-0.5.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: inni
-Version: 0.5.1
+Version: 0.5.2
 Summary: Modular system to perform tasks surrounding log-in and log-out.
 Home-page: https://gitlab.com/ceda_ei/inni
 License: GPL-3.0
 Author: Ceda EI
 Author-email: ceda_ei@webionite.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

