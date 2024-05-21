# Comparing `tmp/c6t-0.0.3.tar.gz` & `tmp/c6t-0.0.4.tar.gz`

## Comparing `c6t-0.0.3.tar` & `c6t-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 c6t-0.0.3/.python-version
--rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 c6t-0.0.3/requirements-dev.lock
--rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 c6t-0.0.3/requirements.lock
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 c6t-0.0.3/.github/workflows/dump-env.yml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/__main__.py
--rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/api/__init__.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/api/agent_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/configure/__init__.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/configure/credentials.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/external/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/external/integrations/scw/__init__.py
--rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/external/integrations/scw/contrast_api.py
--rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/external/integrations/scw/contrast_scw.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/templates/contrast_security.yaml.j2
--rw-r--r--   0        0        0    14607 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/ui/auth.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 c6t-0.0.3/.gitignore
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 c6t-0.0.3/LICENSE
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 c6t-0.0.3/README.md
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 c6t-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 c6t-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 c6t-0.0.4/.python-version
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 c6t-0.0.4/requirements-dev.lock
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 c6t-0.0.4/requirements.lock
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 c6t-0.0.4/.github/workflows/dump-env.yml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 c6t-0.0.4/src/c6t/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 c6t-0.0.4/src/c6t/__main__.py
+-rw-r--r--   0        0        0     4892 2020-02-02 00:00:00.000000 c6t-0.0.4/src/c6t/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.4/src/c6t/api/__init__.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 c6t-0.0.4/src/c6t/api/agent_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.4/src/c6t/configure/__init__.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 c6t-0.0.4/src/c6t/configure/credentials.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.4/src/c6t/external/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.4/src/c6t/external/integrations/scw/__init__.py
+-rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 c6t-0.0.4/src/c6t/external/integrations/scw/contrast_api.py
+-rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 c6t-0.0.4/src/c6t/external/integrations/scw/contrast_scw.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 c6t-0.0.4/src/c6t/templates/contrast_security.yaml.j2
+-rw-r--r--   0        0        0    14560 2020-02-02 00:00:00.000000 c6t-0.0.4/src/c6t/ui/auth.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 c6t-0.0.4/.gitignore
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 c6t-0.0.4/LICENSE
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 c6t-0.0.4/README.md
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 c6t-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 c6t-0.0.4/PKG-INFO
```

### Comparing `c6t-0.0.3/requirements-dev.lock` & `c6t-0.0.4/requirements-dev.lock`

 * *Files identical despite different names*

### Comparing `c6t-0.0.3/requirements.lock` & `c6t-0.0.4/requirements.lock`

 * *Files identical despite different names*

### Comparing `c6t-0.0.3/src/c6t/cli.py` & `c6t-0.0.4/src/c6t/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -38,52 +38,23 @@
                 "name": "Free Trial",
                 "value": "https://cs004.contrastsecurity.com/Contrast",
             },
             {
                 "name": "Evaluation",
                 "value": "https://eval.contrastsecurity.com/Contrast",
             },
-            {
-                "name": "Production - App",
-                "value": "https://app.contrastsecurity.com/Contrast",
-            },
-            {
-                "name": "Production - AppTwo",
-                "value": "https://apptwo.contrastsecurity.com/Contrast",
-            },
-            {
-                "name": "Production - CS001",
-                "value": "https://cs001.contrastsecurity.com/Contrast",
-            },
-            {
-                "name": "Production - CS002",
-                "value": "https://cs002.contrastsecurity.com/Contrast",
-            },
-            {
-                "name": "Production - CS003",
-                "value": "https://cs003.contrastsecurity.com/Contrast",
-            },
-            {
-                "name": "Production - CS004",
-                "value": "https://cs004.contrastsecurity.com/Contrast",
-            },
-            {"name": "Other", "value": "Other"},
-            {"Name": "Exit", "value": None},
+            {"name": "Enterprise", "value": "Enterprise"},
         ],
         default={
             "name": "Free Trial",
             "value": "https://cs004.contrastsecurity.com/Contrast",
         },
     ).ask()
 
-    if contrast_environment is None:
-        print("Exiting...")
-        return
-
-    if contrast_environment == "Other":
+    if contrast_environment == "Enterprise":
         contrast_environment = questionary.text(
             "Enter your Contrast TeamServer URL:"
         ).ask()
 
     if contrast_environment:
         auth = ContrastUIAuthManager(base_url=contrast_environment)
         auth.login(profile=profile)
```

### Comparing `c6t-0.0.3/src/c6t/api/agent_config.py` & `c6t-0.0.4/src/c6t/api/agent_config.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.3/src/c6t/configure/credentials.py` & `c6t-0.0.4/src/c6t/configure/credentials.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.3/src/c6t/external/integrations/scw/contrast_api.py` & `c6t-0.0.4/src/c6t/external/integrations/scw/contrast_api.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.3/src/c6t/external/integrations/scw/contrast_scw.py` & `c6t-0.0.4/src/c6t/external/integrations/scw/contrast_scw.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.3/src/c6t/ui/auth.py` & `c6t-0.0.4/src/c6t/ui/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -303,26 +303,22 @@
             organization_choices.append(
                 {
                     "name": organization.get("name"),
                     "value": organization.get("organization_uuid"),
                 }
             )
 
-        organization_choices.append(
-            {
-                "name": "Exit",
-                "value": None,
-            }
-        )
+        if len(organization_choices) == 1:
+            return organization_choices[0].get("value")
 
         organization_uuid = questionary.select(
             message="Select your organization:",
             choices=organization_choices,
         ).ask()
-        
+
         return organization_uuid
 
     def toggle_superadmin(self) -> None:
         """
         Toggle the SuperAdmin role for the user.
         This is a hack to get the Contrast UI key cookies set.
         Cookies are set as a side-effect of this request.
```

### Comparing `c6t-0.0.3/.gitignore` & `c6t-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `c6t-0.0.3/LICENSE` & `c6t-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `c6t-0.0.3/README.md` & `c6t-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `c6t-0.0.3/pyproject.toml` & `c6t-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "c6t"
-version = "0.0.3"
+version = "0.0.4"
 description = "Unofficial Administrative Command Line Interface for Contrast Security"
 authors = [
     { name = "Jonathan Harper", email = "39912347+jharper-sec@users.noreply.github.com" },
 ]
 dependencies = [
     "requests>=2.32.0",
     "shellingham>=1.5.4",
```

### Comparing `c6t-0.0.3/PKG-INFO` & `c6t-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: c6t
-Version: 0.0.3
+Version: 0.0.4
 Summary: Unofficial Administrative Command Line Interface for Contrast Security
 Project-URL: Homepage, https://github.com/jharper-sec/c6t
 Project-URL: Issues, https://github.com/jharper-sec/c6t/issues
 Project-URL: Documentation, https://github.com/jharper-sec/c6t/blob/main/README.md
 Author-email: Jonathan Harper <39912347+jharper-sec@users.noreply.github.com>
 License: Copyright 2023 Contrast Security, Inc.
```

