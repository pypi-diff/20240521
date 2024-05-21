# Comparing `tmp/c6t-0.0.2.tar.gz` & `tmp/c6t-0.0.3.tar.gz`

## Comparing `c6t-0.0.2.tar` & `c6t-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 c6t-0.0.2/.python-version
--rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 c6t-0.0.2/requirements-dev.lock
--rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 c6t-0.0.2/requirements.lock
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 c6t-0.0.2/.github/workflows/dump-env.yml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/__main__.py
--rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/api/__init__.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/api/agent_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/configure/__init__.py
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/configure/credentials.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/external/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/external/integrations/scw/__init__.py
--rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/external/integrations/scw/contrast_api.py
--rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/external/integrations/scw/contrast_scw.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/templates/contrast_security.yaml.j2
--rw-r--r--   0        0        0    14981 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/ui/auth.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 c6t-0.0.2/.gitignore
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 c6t-0.0.2/LICENSE
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 c6t-0.0.2/README.md
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 c6t-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 c6t-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 c6t-0.0.3/.python-version
+-rw-r--r--   0        0        0     1572 2020-02-02 00:00:00.000000 c6t-0.0.3/requirements-dev.lock
+-rw-r--r--   0        0        0     1135 2020-02-02 00:00:00.000000 c6t-0.0.3/requirements.lock
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 c6t-0.0.3/.github/workflows/dump-env.yml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/__main__.py
+-rw-r--r--   0        0        0     5883 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/api/__init__.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/api/agent_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/configure/__init__.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/configure/credentials.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/external/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/external/integrations/scw/__init__.py
+-rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/external/integrations/scw/contrast_api.py
+-rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/external/integrations/scw/contrast_scw.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/templates/contrast_security.yaml.j2
+-rw-r--r--   0        0        0    14607 2020-02-02 00:00:00.000000 c6t-0.0.3/src/c6t/ui/auth.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 c6t-0.0.3/.gitignore
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 c6t-0.0.3/LICENSE
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 c6t-0.0.3/README.md
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 c6t-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 c6t-0.0.3/PKG-INFO
```

### Comparing `c6t-0.0.2/requirements-dev.lock` & `c6t-0.0.3/requirements-dev.lock`

 * *Files 8% similar despite different names*

```diff
@@ -45,37 +45,32 @@
     # via pytest
 pathspec==0.12.1
     # via black
 platformdirs==4.2.2
     # via black
 pluggy==1.5.0
     # via pytest
-prompt-toolkit==1.0.14
-    # via pyinquirer
+prompt-toolkit==3.0.36
+    # via questionary
 pygments==2.18.0
-    # via pyinquirer
     # via rich
-pyinquirer==1.0.3
-    # via c6t
 pytest==8.2.1
 pyyaml==6.0.1
     # via c6t
-regex==2024.5.15
-    # via pyinquirer
+questionary==2.0.1
+    # via c6t
 requests==2.32.0
     # via c6t
 rich==13.7.1
     # via c6t
     # via typer
 ruff==0.4.4
 shellingham==1.5.4
     # via c6t
     # via typer
-six==1.16.0
-    # via prompt-toolkit
 smmap==5.0.1
     # via gitdb
 tomli==2.0.1
     # via black
     # via mypy
     # via pytest
 typer==0.12.3
```

### Comparing `c6t-0.0.2/requirements.lock` & `c6t-0.0.3/requirements.lock`

 * *Files 8% similar despite different names*

```diff
@@ -26,35 +26,30 @@
     # via c6t
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
-prompt-toolkit==1.0.14
-    # via pyinquirer
+prompt-toolkit==3.0.36
+    # via questionary
 pygments==2.18.0
-    # via pyinquirer
     # via rich
-pyinquirer==1.0.3
-    # via c6t
 pyyaml==6.0.1
     # via c6t
-regex==2024.5.15
-    # via pyinquirer
+questionary==2.0.1
+    # via c6t
 requests==2.32.0
     # via c6t
 rich==13.7.1
     # via c6t
     # via typer
 shellingham==1.5.4
     # via c6t
     # via typer
-six==1.16.0
-    # via prompt-toolkit
 smmap==5.0.1
     # via gitdb
 typer==0.12.3
     # via c6t
 types-requests==2.31.0.20240406
     # via c6t
 typing-extensions==4.11.0
```

### Comparing `c6t-0.0.2/src/c6t/cli.py` & `c6t-0.0.3/src/c6t/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 import yaml
 import pathlib
 from git.repo import Repo
 from jinja2 import Environment, FileSystemLoader
 
 from rich import print as rprint
 
-from PyInquirer import prompt  # type: ignore
-
-# from InquirerPy import inquirer
-# from InquirerPy.base.control import Choice
+import questionary
 
 from c6t.configure.credentials import ContrastAPICredentials
 from c6t.ui.auth import ContrastUIAuthManager
 from c6t.api.agent_config import AgentConfig
 
 from c6t.external.integrations.scw.contrast_scw import scw_create, scw_delete
 
@@ -30,42 +27,69 @@
 def login(profile: str = "default") -> None:
     """
     Login to the Contrast platform using your UI credentials (username/password).
     This will automatically configure your API credentials and save them to the
     credentials file.
     """
 
-    environment_questions = [
-        {
-            "type": "list",
-            "name": "environment",
-            "message": "Select your Contrast TeamServer Environment:",
-            "choices": [
-                {
-                    "name": "Free Trial",
-                    "value": "https://cs004.contrastsecurity.com/Contrast",
-                },
-                {
-                    "name": "Evaluation",
-                    "value": "https://eval.contrastsecurity.com/Contrast",
-                },
-                {
-                    "name": "Enterprise",
-                    "value": "https://app.contrastsecurity.com/Contrast",
-                },
-                {"name": "Exit", "value": None},
-            ],
-        }
-    ]
-
-    answers = prompt(environment_questions)  # type: ignore
-    contrast_environment = answers.get("environment")  # type: ignore
+    contrast_environment = questionary.select(
+        "Select your Contrast TeamServer Environment:",
+        choices=[
+            {
+                "name": "Free Trial",
+                "value": "https://cs004.contrastsecurity.com/Contrast",
+            },
+            {
+                "name": "Evaluation",
+                "value": "https://eval.contrastsecurity.com/Contrast",
+            },
+            {
+                "name": "Production - App",
+                "value": "https://app.contrastsecurity.com/Contrast",
+            },
+            {
+                "name": "Production - AppTwo",
+                "value": "https://apptwo.contrastsecurity.com/Contrast",
+            },
+            {
+                "name": "Production - CS001",
+                "value": "https://cs001.contrastsecurity.com/Contrast",
+            },
+            {
+                "name": "Production - CS002",
+                "value": "https://cs002.contrastsecurity.com/Contrast",
+            },
+            {
+                "name": "Production - CS003",
+                "value": "https://cs003.contrastsecurity.com/Contrast",
+            },
+            {
+                "name": "Production - CS004",
+                "value": "https://cs004.contrastsecurity.com/Contrast",
+            },
+            {"name": "Other", "value": "Other"},
+            {"Name": "Exit", "value": None},
+        ],
+        default={
+            "name": "Free Trial",
+            "value": "https://cs004.contrastsecurity.com/Contrast",
+        },
+    ).ask()
+
+    if contrast_environment is None:
+        print("Exiting...")
+        return
+
+    if contrast_environment == "Other":
+        contrast_environment = questionary.text(
+            "Enter your Contrast TeamServer URL:"
+        ).ask()
 
     if contrast_environment:
-        auth = ContrastUIAuthManager(base_url=contrast_environment)  # type: ignore
+        auth = ContrastUIAuthManager(base_url=contrast_environment)
         auth.login(profile=profile)
 
 
 @app.command("configure")
 def configure(profile: str = "default") -> None:
     """
     Configure the c6t CLI credentials.
```

### Comparing `c6t-0.0.2/src/c6t/api/agent_config.py` & `c6t-0.0.3/src/c6t/api/agent_config.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.2/src/c6t/configure/credentials.py` & `c6t-0.0.3/src/c6t/configure/credentials.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.2/src/c6t/external/integrations/scw/contrast_api.py` & `c6t-0.0.3/src/c6t/external/integrations/scw/contrast_api.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.2/src/c6t/external/integrations/scw/contrast_scw.py` & `c6t-0.0.3/src/c6t/external/integrations/scw/contrast_scw.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.2/src/c6t/ui/auth.py` & `c6t-0.0.3/src/c6t/ui/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 
 import requests
 
 from typing import Any, List, Dict, Optional
 
 import typer
 
-from PyInquirer import prompt  # type: ignore
-
-# from InquirerPy import inquirer
-# from InquirerPy.base.control import Choice
+import questionary
 
 from c6t.configure.credentials import ContrastAPICredentials, ContrastUICredentials
 
 
 class ContrastUIAuthManager:
     def __init__(self, base_url: str):
         self.ui_credentials = ContrastUICredentials()
@@ -313,27 +310,20 @@
         organization_choices.append(
             {
                 "name": "Exit",
                 "value": None,
             }
         )
 
-        organization_questions = [
-            {
-                "type": "list",
-                "name": "organization",
-                "message": "Select your organization:",
-                "choices": organization_choices,
-            }
-        ]
-
-        organization_answers = prompt(organization_questions)  # type: ignore
-        organization_uuid = organization_answers.get("organization")  # type: ignore
-
-        return organization_uuid  # type: ignore
+        organization_uuid = questionary.select(
+            message="Select your organization:",
+            choices=organization_choices,
+        ).ask()
+        
+        return organization_uuid
 
     def toggle_superadmin(self) -> None:
         """
         Toggle the SuperAdmin role for the user.
         This is a hack to get the Contrast UI key cookies set.
         Cookies are set as a side-effect of this request.
         """
```

### Comparing `c6t-0.0.2/.gitignore` & `c6t-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `c6t-0.0.2/LICENSE` & `c6t-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `c6t-0.0.2/README.md` & `c6t-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `c6t-0.0.2/pyproject.toml` & `c6t-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "c6t"
-version = "0.0.2"
+version = "0.0.3"
 description = "Unofficial Administrative Command Line Interface for Contrast Security"
 authors = [
     { name = "Jonathan Harper", email = "39912347+jharper-sec@users.noreply.github.com" },
 ]
 dependencies = [
     "requests>=2.32.0",
     "shellingham>=1.5.4",
     "rich>=13.7.1",
     "typer[all]>=0.12.3",
     "annotated-types>=0.6.0",
     "types-requests>=2.31.0.20240406",
     "jinja2>=3.1.4",
     "pyyaml>=6.0.1",
     "gitpython>=3.1.43",
-    "pyinquirer>=1.0.3",
+    "questionary>=2.0.1",
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">= 3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
```

### Comparing `c6t-0.0.2/PKG-INFO` & `c6t-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: c6t
-Version: 0.0.2
+Version: 0.0.3
 Summary: Unofficial Administrative Command Line Interface for Contrast Security
 Project-URL: Homepage, https://github.com/jharper-sec/c6t
 Project-URL: Issues, https://github.com/jharper-sec/c6t/issues
 Project-URL: Documentation, https://github.com/jharper-sec/c6t/blob/main/README.md
 Author-email: Jonathan Harper <39912347+jharper-sec@users.noreply.github.com>
 License: Copyright 2023 Contrast Security, Inc.
         
@@ -23,16 +23,16 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: annotated-types>=0.6.0
 Requires-Dist: gitpython>=3.1.43
 Requires-Dist: jinja2>=3.1.4
-Requires-Dist: pyinquirer>=1.0.3
 Requires-Dist: pyyaml>=6.0.1
+Requires-Dist: questionary>=2.0.1
 Requires-Dist: requests>=2.32.0
 Requires-Dist: rich>=13.7.1
 Requires-Dist: shellingham>=1.5.4
 Requires-Dist: typer[all]>=0.12.3
 Requires-Dist: types-requests>=2.31.0.20240406
 Description-Content-Type: text/markdown
```

