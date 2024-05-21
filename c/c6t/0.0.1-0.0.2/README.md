# Comparing `tmp/c6t-0.0.1.tar.gz` & `tmp/c6t-0.0.2.tar.gz`

## Comparing `c6t-0.0.1.tar` & `c6t-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 c6t-0.0.1/.python-version
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 c6t-0.0.1/requirements-dev.lock
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 c6t-0.0.1/requirements.lock
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 c6t-0.0.1/.github/workflows/dump-env.yml
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 c6t-0.0.1/src/c6t/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 c6t-0.0.1/src/c6t/__main__.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 c6t-0.0.1/src/c6t/cli.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.1/src/c6t/api/__init__.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 c6t-0.0.1/src/c6t/api/agent_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.1/src/c6t/configure/__init__.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 c6t-0.0.1/src/c6t/configure/credentials.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.1/src/c6t/external/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.1/src/c6t/external/integrations/scw/__init__.py
--rw-r--r--   0        0        0     5970 2020-02-02 00:00:00.000000 c6t-0.0.1/src/c6t/external/integrations/scw/contrast_api.py
--rw-r--r--   0        0        0     8507 2020-02-02 00:00:00.000000 c6t-0.0.1/src/c6t/external/integrations/scw/contrast_scw.py
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 c6t-0.0.1/src/c6t/templates/contrast_security.yaml.j2
--rw-r--r--   0        0        0    14567 2020-02-02 00:00:00.000000 c6t-0.0.1/src/c6t/ui/auth.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 c6t-0.0.1/.gitignore
--rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 c6t-0.0.1/LICENSE
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 c6t-0.0.1/README.md
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 c6t-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 c6t-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 c6t-0.0.2/.python-version
+-rw-r--r--   0        0        0     1666 2020-02-02 00:00:00.000000 c6t-0.0.2/requirements-dev.lock
+-rw-r--r--   0        0        0     1229 2020-02-02 00:00:00.000000 c6t-0.0.2/requirements.lock
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 c6t-0.0.2/.github/workflows/dump-env.yml
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/__main__.py
+-rw-r--r--   0        0        0     5115 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/cli.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/api/__init__.py
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/api/agent_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/configure/__init__.py
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/configure/credentials.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/external/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/external/integrations/scw/__init__.py
+-rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/external/integrations/scw/contrast_api.py
+-rw-r--r--   0        0        0     9008 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/external/integrations/scw/contrast_scw.py
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/templates/contrast_security.yaml.j2
+-rw-r--r--   0        0        0    14981 2020-02-02 00:00:00.000000 c6t-0.0.2/src/c6t/ui/auth.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 c6t-0.0.2/.gitignore
+-rw-r--r--   0        0        0      563 2020-02-02 00:00:00.000000 c6t-0.0.2/LICENSE
+-rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 c6t-0.0.2/README.md
+-rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 c6t-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2444 2020-02-02 00:00:00.000000 c6t-0.0.2/PKG-INFO
```

### Comparing `c6t-0.0.1/requirements-dev.lock` & `c6t-0.0.2/requirements-dev.lock`

 * *Files 8% similar despite different names*

```diff
@@ -14,24 +14,24 @@
 certifi==2024.2.2
     # via requests
 charset-normalizer==3.3.2
     # via requests
 click==8.1.7
     # via black
     # via typer
+exceptiongroup==1.2.1
+    # via pytest
 gitdb==4.0.11
     # via gitpython
 gitpython==3.1.43
     # via c6t
 idna==3.7
     # via requests
 iniconfig==2.0.0
     # via pytest
-inquirerpy==0.3.4
-    # via c6t
 jinja2==3.1.4
     # via c6t
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via jinja2
 mdurl==0.1.2
@@ -41,43 +41,55 @@
     # via black
     # via mypy
 packaging==24.0
     # via black
     # via pytest
 pathspec==0.12.1
     # via black
-pfzy==0.3.4
-    # via inquirerpy
 platformdirs==4.2.2
     # via black
 pluggy==1.5.0
     # via pytest
-prompt-toolkit==3.0.43
-    # via inquirerpy
+prompt-toolkit==1.0.14
+    # via pyinquirer
 pygments==2.18.0
+    # via pyinquirer
     # via rich
+pyinquirer==1.0.3
+    # via c6t
 pytest==8.2.1
 pyyaml==6.0.1
     # via c6t
+regex==2024.5.15
+    # via pyinquirer
 requests==2.32.0
     # via c6t
 rich==13.7.1
     # via c6t
     # via typer
 ruff==0.4.4
 shellingham==1.5.4
     # via c6t
     # via typer
+six==1.16.0
+    # via prompt-toolkit
 smmap==5.0.1
     # via gitdb
+tomli==2.0.1
+    # via black
+    # via mypy
+    # via pytest
 typer==0.12.3
     # via c6t
 types-requests==2.31.0.20240406
     # via c6t
 typing-extensions==4.11.0
+    # via annotated-types
+    # via black
     # via mypy
+    # via rich
     # via typer
 urllib3==2.2.1
     # via requests
     # via types-requests
 wcwidth==0.2.13
     # via prompt-toolkit
```

### Comparing `c6t-0.0.1/requirements.lock` & `c6t-0.0.2/requirements.lock`

 * *Files 10% similar despite different names*

```diff
@@ -18,46 +18,51 @@
     # via typer
 gitdb==4.0.11
     # via gitpython
 gitpython==3.1.43
     # via c6t
 idna==3.7
     # via requests
-inquirerpy==0.3.4
-    # via c6t
 jinja2==3.1.4
     # via c6t
 markdown-it-py==3.0.0
     # via rich
 markupsafe==2.1.5
     # via jinja2
 mdurl==0.1.2
     # via markdown-it-py
-pfzy==0.3.4
-    # via inquirerpy
-prompt-toolkit==3.0.43
-    # via inquirerpy
+prompt-toolkit==1.0.14
+    # via pyinquirer
 pygments==2.18.0
+    # via pyinquirer
     # via rich
+pyinquirer==1.0.3
+    # via c6t
 pyyaml==6.0.1
     # via c6t
+regex==2024.5.15
+    # via pyinquirer
 requests==2.32.0
     # via c6t
 rich==13.7.1
     # via c6t
     # via typer
 shellingham==1.5.4
     # via c6t
     # via typer
+six==1.16.0
+    # via prompt-toolkit
 smmap==5.0.1
     # via gitdb
 typer==0.12.3
     # via c6t
 types-requests==2.31.0.20240406
     # via c6t
 typing-extensions==4.11.0
+    # via annotated-types
+    # via rich
     # via typer
 urllib3==2.2.1
     # via requests
     # via types-requests
 wcwidth==0.2.13
     # via prompt-toolkit
```

### Comparing `c6t-0.0.1/src/c6t/cli.py` & `c6t-0.0.2/src/c6t/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 import yaml
 import pathlib
 from git.repo import Repo
 from jinja2 import Environment, FileSystemLoader
 
 from rich import print as rprint
 
-from InquirerPy import inquirer
-from InquirerPy.base.control import Choice
+from PyInquirer import prompt  # type: ignore
+
+# from InquirerPy import inquirer
+# from InquirerPy.base.control import Choice
 
 from c6t.configure.credentials import ContrastAPICredentials
 from c6t.ui.auth import ContrastUIAuthManager
 from c6t.api.agent_config import AgentConfig
 
 from c6t.external.integrations.scw.contrast_scw import scw_create, scw_delete
 
@@ -28,33 +30,42 @@
 def login(profile: str = "default") -> None:
     """
     Login to the Contrast platform using your UI credentials (username/password).
     This will automatically configure your API credentials and save them to the
     credentials file.
     """
 
-    contrast_environment = inquirer.select(  # type: ignore
-        message="Select your Contrast TeamServer Environment:",
-        choices=[
-            Choice(
-                value="https://cs004.contrastsecurity.com/Contrast", name="Free Trial"
-            ),
-            Choice(
-                value="https://eval.contrastsecurity.com/Contrast", name="Evaluation"
-            ),
-            Choice(
-                value="https://app.contrastsecurity.com/Contrast", name="Enterprise"
-            ),
-            Choice(value=None, name="Exit"),
-        ],
-        default="Free Trial",
-    ).execute()
+    environment_questions = [
+        {
+            "type": "list",
+            "name": "environment",
+            "message": "Select your Contrast TeamServer Environment:",
+            "choices": [
+                {
+                    "name": "Free Trial",
+                    "value": "https://cs004.contrastsecurity.com/Contrast",
+                },
+                {
+                    "name": "Evaluation",
+                    "value": "https://eval.contrastsecurity.com/Contrast",
+                },
+                {
+                    "name": "Enterprise",
+                    "value": "https://app.contrastsecurity.com/Contrast",
+                },
+                {"name": "Exit", "value": None},
+            ],
+        }
+    ]
+
+    answers = prompt(environment_questions)  # type: ignore
+    contrast_environment = answers.get("environment")  # type: ignore
 
     if contrast_environment:
-        auth = ContrastUIAuthManager(base_url=contrast_environment)
+        auth = ContrastUIAuthManager(base_url=contrast_environment)  # type: ignore
         auth.login(profile=profile)
 
 
 @app.command("configure")
 def configure(profile: str = "default") -> None:
     """
     Configure the c6t CLI credentials.
```

### Comparing `c6t-0.0.1/src/c6t/api/agent_config.py` & `c6t-0.0.2/src/c6t/api/agent_config.py`

 * *Files identical despite different names*

### Comparing `c6t-0.0.1/src/c6t/configure/credentials.py` & `c6t-0.0.2/src/c6t/configure/credentials.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 
 from pathlib import Path
 
 import typer
 
+
 class ContrastUICredentials:
     base_url: str
     username: str
     superadmin: bool
     password: str
     code: str
```

### Comparing `c6t-0.0.1/src/c6t/external/integrations/scw/contrast_api.py` & `c6t-0.0.2/src/c6t/external/integrations/scw/contrast_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Author: josh.anderson@contrastsecurity.com / jonathan.harper@contrastsecurity.com
 
 import json
 import re
 import base64
 from urllib.request import Request, urlopen
 
-from typing import Any, Dict
+from typing import Any, Dict, List
 
 from c6t.configure.credentials import ContrastAPICredentials
 
 
 def load_config():
     with open("config.json", "r") as config:
         config = json.load(config)
@@ -138,21 +138,23 @@
                 self._title_cwe_cache[policy["title"]] = (
                     policy["cwe"].split("/")[-1].replace(".html", "")
                 )
 
         return self._title_cwe_cache[title]
 
     def update_rule_references(
-        self, org_id: str, rule_name: str, references: str, api_key: str
-    ):
+        self, org_id: str, rule_name: str, references: List[str], api_key: str
+    ) -> Dict[str, Any]:
         values = {"references": references}
 
         data = json.dumps(values).encode("utf-8")
 
-        response = self.post_api_request(org_id + "/rules/" + rule_name, data, api_key)
+        response = json.loads(
+            self.post_api_request(org_id + "/rules/" + rule_name, data, api_key)
+        ).decode("utf-8")
 
         return response
 
     def send_usage_event(self, org_id: str, is_reset: bool, api_key: str):
         usage_mode_endpoint = "undo" if is_reset else "setup"
 
         values = {"type": usage_mode_endpoint}
```

### Comparing `c6t-0.0.1/src/c6t/external/integrations/scw/contrast_scw.py` & `c6t-0.0.2/src/c6t/external/integrations/scw/contrast_scw.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,185 +1,222 @@
 # Script to query Contrast TeamServer to populate the vulnerability references with Secure Code Warrior video links
 # Author(s): josh.anderson@contrastsecurity.com / david.archer@contrastsecurity.com / jonathan.harper@contrastsecurity.com
 
 from urllib.request import Request, urlopen
-from c6t.external.integrations.scw.contrast_api import load_config, contrast_instance_from_json
-from c6t.external.integrations.scw.contrast_api import ContrastTeamServer
+from c6t.external.integrations.scw.contrast_api import contrast_instance_from_json
 import traceback
 import json
 import urllib.parse
-import sys
+import urllib.error
+
+from typing import List
 
 from c6t.configure.credentials import ContrastAPICredentials
 
-def get_scw_base_url(cwe):
-    return 'https://integration-api.securecodewarrior.com/api/v1/trial?Id=contrast&MappingList=cwe&MappingKey=' + cwe
+
+def get_scw_base_url(cwe: str):
+    return (
+        "https://integration-api.securecodewarrior.com/api/v1/trial?Id=contrast&MappingList=cwe&MappingKey="
+        + cwe
+    )
 
 
-def get_scw_data(url):
+def get_scw_data(url: str):
     try:
         req = Request(url)
 
         res = urlopen(req).read()
-        data = json.loads(res.decode('utf-8'))
+        data = json.loads(res.decode("utf-8"))
 
         return data
     except urllib.error.HTTPError as err:
         print(err)
 
 
-def map_contrast_lang_to_scw_lang(contrast_lang):
-    langs = {'.NET': 'c#', '.NET Core': 'c#(.net):mvc', 'Java': 'java',
-             'Node': 'nodejs', 'Python': 'python:django', 'Ruby': 'ruby'}  # 'Go': 'go'
-    return langs.get(contrast_lang, '')
+def map_contrast_lang_to_scw_lang(contrast_lang: str):
+    langs = {
+        ".NET": "c#",
+        ".NET Core": "c#(.net):mvc",
+        "Java": "java",
+        "Node": "nodejs",
+        "Python": "python:django",
+        "Ruby": "ruby",
+    }  # 'Go': 'go'
+    return langs.get(contrast_lang, "")
 
 
 def scw_create(profile: str) -> None:
     credentials = ContrastAPICredentials()
     credentials.get_credentials_from_file(profile=profile)
 
     org_id = credentials.organization_uuid
     contrast = contrast_instance_from_json(credentials)
 
-    allow_product_usage_analytics =  False
-    enable_verbose_error_logging =  False
+    allow_product_usage_analytics = False
+    enable_verbose_error_logging = False
     org_key = credentials.api_key
 
     # Loop through all the Assess rules
     for rule in contrast.list_org_policy(org_id, org_key):
-        print('Processing rule: ' + rule['name'] + '/' + rule['title'])
+        print("Processing rule: " + rule["name"] + "/" + rule["title"])
 
-        refs = []
-        video = ''
+        refs: List[str] = []
+        video = ""
 
         # Extract the CWE number for this rule
         reserves = {
-            'escape-templates-off': 'https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4',
-            'clickjacking-control-missing': 'https://media.securecodewarrior.com/v2/Module_25_CLICKJACKING_v2.mp4',
-            'event-validation-disabled': 'https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4',
-            'forms-auth-protection': 'https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4',
-            'forms-auth-redirect': 'https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4',
-            'http-only-disabled': 'https://media.securecodewarrior.com/v2/Module_74_WEAK_SESSION_TOKEN_GENERATION_v2.mp4',
-            'httponly': 'https://media.securecodewarrior.com/v2/Module_74_WEAK_SESSION_TOKEN_GENERATION_v2.mp4',
-            'max-request-length': 'https://media.securecodewarrior.com/v2/Module_54_DoS_Generic_v2.mp4',
-            'rails-http-only-disabled': 'https://media.securecodewarrior.com/v2/Module_74_WEAK_SESSION_TOKEN_GENERATION_v2.mp4',
-            'reflected-xss': 'https://media.securecodewarrior.com/v2/Module_73_Reflected_Cross+Site+Scripting_v2.mp4',
-            'request-validation-disabled': 'https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4',
-            'request-validation-control-disabled': 'https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4',
-            'role-manager-protection': 'https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4',
-            'session-rewriting': 'https://media.securecodewarrior.com/v2/module_136_exposed_session_tokens.mp4',
-            'session-regenerate': 'https://media.securecodewarrior.com/v2/Module_74_WEAK_SESSION_TOKEN_GENERATION_v2.mp4',
-            'stored-xss': 'https://media.securecodewarrior.com/v2/Module_72_Stored_Cross+Site+Scripting_v2.mp4',
-            'version-header-enabled': 'https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4',
-            'verb-tampering': 'https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4',
-            'viewstate-mac-disabled': 'https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4',
-            'wcf-detect-replays': 'https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4',
-            'wcf-exception-details': 'https://media.securecodewarrior.com/v2/module_184_error_details.mp4',
-            'wcf-metadata-enabled': 'https://media.securecodewarrior.com/v2/module_184_error_details.mp4',
-            'x-powered-by-header': 'https://media.securecodewarrior.com/v2/module_184_error_details.mp4',
-            'xxssprotection-header-disabled': 'https://media.securecodewarrior.com/v2/Module_73_Reflected_Cross+Site+Scripting_v2.mp4'
+            "escape-templates-off": "https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4",
+            "clickjacking-control-missing": "https://media.securecodewarrior.com/v2/Module_25_CLICKJACKING_v2.mp4",
+            "event-validation-disabled": "https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4",
+            "forms-auth-protection": "https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4",
+            "forms-auth-redirect": "https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4",
+            "http-only-disabled": "https://media.securecodewarrior.com/v2/Module_74_WEAK_SESSION_TOKEN_GENERATION_v2.mp4",
+            "httponly": "https://media.securecodewarrior.com/v2/Module_74_WEAK_SESSION_TOKEN_GENERATION_v2.mp4",
+            "max-request-length": "https://media.securecodewarrior.com/v2/Module_54_DoS_Generic_v2.mp4",
+            "rails-http-only-disabled": "https://media.securecodewarrior.com/v2/Module_74_WEAK_SESSION_TOKEN_GENERATION_v2.mp4",
+            "reflected-xss": "https://media.securecodewarrior.com/v2/Module_73_Reflected_Cross+Site+Scripting_v2.mp4",
+            "request-validation-disabled": "https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4",
+            "request-validation-control-disabled": "https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4",
+            "role-manager-protection": "https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4",
+            "session-rewriting": "https://media.securecodewarrior.com/v2/module_136_exposed_session_tokens.mp4",
+            "session-regenerate": "https://media.securecodewarrior.com/v2/Module_74_WEAK_SESSION_TOKEN_GENERATION_v2.mp4",
+            "stored-xss": "https://media.securecodewarrior.com/v2/Module_72_Stored_Cross+Site+Scripting_v2.mp4",
+            "version-header-enabled": "https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4",
+            "verb-tampering": "https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4",
+            "viewstate-mac-disabled": "https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4",
+            "wcf-detect-replays": "https://media.securecodewarrior.com/v2/Security_Misconfiguration_v2.mp4",
+            "wcf-exception-details": "https://media.securecodewarrior.com/v2/module_184_error_details.mp4",
+            "wcf-metadata-enabled": "https://media.securecodewarrior.com/v2/module_184_error_details.mp4",
+            "x-powered-by-header": "https://media.securecodewarrior.com/v2/module_184_error_details.mp4",
+            "xxssprotection-header-disabled": "https://media.securecodewarrior.com/v2/Module_73_Reflected_Cross+Site+Scripting_v2.mp4",
         }
 
-        cwe = contrast.trace_cwe(org_id, rule['title'], org_key)
+        cwe = contrast.trace_cwe(org_id, rule["title"], org_key)
 
         # Compose a url for this training exercise
         scw_url = get_scw_base_url(cwe)
 
         # Get the data for this exercise from scw
         response = get_scw_data(scw_url)
 
         # We got a hit
         if response:
             # Do we have a video, if so add it?
-            if 'videos' in response and len(response['videos']) > 0:
-                file = response['videos'][0].replace(' ', '+')
-                print('Video found: ' + file)
+            if "videos" in response and len(response["videos"]) > 0:
+                file = response["videos"][0].replace(" ", "+")
+                print("Video found: " + file)
             else:
-                file = reserves.get(rule['name'], '')
+                file = reserves.get(rule["name"], "")
         else:
-            print('No CWE videos received from secure code warrior: ' +
-                rule['name'] + '/' + rule['title'] + ', cwe ' + cwe + ', SCW url: ' + scw_url)
-            file = reserves.get(rule['name'], '')
-        
-        if file != '':
-            video = '<br>Watch a video on this topic with Secure Code Warrior (beta):<br>' + file
+            print(
+                "No CWE videos received from secure code warrior: "
+                + rule["name"]
+                + "/"
+                + rule["title"]
+                + ", cwe "
+                + cwe
+                + ", SCW url: "
+                + scw_url
+            )
+            file = reserves.get(rule["name"], "")
+
+        if file != "":
+            video = (
+                "<br>Watch a video on this topic with Secure Code Warrior (beta):<br>"
+                + file
+            )
         else:
-            print('Missing video cwe ' + cwe + ', SCW url: ' + scw_url)
+            print("Missing video cwe " + cwe + ", SCW url: " + scw_url)
 
         # Loop through all the languages for this rule
-        for lang in rule['languages']:
+        for lang in rule["languages"]:
 
             # Map the contrast language to a SCW language
             scw_lang = map_contrast_lang_to_scw_lang(lang)
 
-            if scw_lang != '':
+            if scw_lang != "":
                 # Compose the URL for training exercise
-                training_url = scw_url + '&LanguageKey=' + \
-                    urllib.parse.quote(lang) + '&redirect=true'
+                training_url = (
+                    scw_url
+                    + "&LanguageKey="
+                    + urllib.parse.quote(lang)
+                    + "&redirect=true"
+                )
 
                 # If this is the first language, add some chrome:
                 if len(refs) == 0:
-                    ref = '<br>Complete a training exercise on this topic for your language using Secure Code Warrior (beta):<br><b>' + \
-                        lang + '</b>: ' + training_url
+                    ref = (
+                        "<br>Complete a training exercise on this topic for your language using Secure Code Warrior (beta):<br><b>"
+                        + lang
+                        + "</b>: "
+                        + training_url
+                    )
                 else:
-                    ref = '<b>' + lang + '</b>: ' + training_url
+                    ref = "<b>" + lang + "</b>: " + training_url
 
                 refs.append(ref)
 
-        if video != '':
+        if video != "":
             refs.insert(0, video)
 
         if len(refs) > 0:
-            print('Updating rule references: ', len(refs))
-            print(*refs,sep='\n')
+            print("Updating rule references: ", len(refs))
+            print(*refs, sep="\n")
             # Update the rule references in Contrast
-            res = contrast.update_rule_references(
-                org_id, rule['name'], refs, org_key)
+            res = contrast.update_rule_references(org_id, rule["name"], refs, org_key)
 
-            if res['success'] == True:
-                print(rule['name'] + '/' + rule['title'] + ' updated successfully')
+            if res["success"] == True:
+                print(rule["name"] + "/" + rule["title"] + " updated successfully")
         else:
-            print('\n[WARNING] ' + rule['name'] + '/' + rule['title'] + ' no references added')
+            print(
+                "\n[WARNING] "
+                + rule["name"]
+                + "/"
+                + rule["title"]
+                + " no references added"
+            )
 
         print("---")
 
         if allow_product_usage_analytics:
             try:
                 contrast.send_usage_event(org_id, False, org_key)
 
             except urllib.error.HTTPError as err:
                 if enable_verbose_error_logging:
+                    print(err)
                     print(traceback.format_exc())
                 else:
                     print("Unable to send usage data")
 
+
 def scw_delete(profile: str) -> None:
 
     credentials = ContrastAPICredentials()
     credentials.get_credentials_from_file(profile=profile)
 
     org_id = credentials.organization_uuid
     contrast = contrast_instance_from_json(credentials)
 
-    allow_product_usage_analytics =  False
-    enable_verbose_error_logging =  False
+    allow_product_usage_analytics = False
+    enable_verbose_error_logging = False
     org_key = credentials.api_key
 
     for rule in contrast.list_org_policy(org_id, org_key):
-        print('Processing rule: ' + rule['name'] + '/' + rule['title'])
+        print("Processing rule: " + rule["name"] + "/" + rule["title"])
 
-        #The reset argument has been passed, erase all rule references.
-        res = contrast.update_rule_references(
-            org_id, rule['name'], [], org_key)
+        # The reset argument has been passed, erase all rule references.
+        res = contrast.update_rule_references(org_id, rule["name"], [], org_key)
 
-        if res['success'] == True:
-            print(rule['title'] + ' reset successfully')
+        if res["success"] == True:
+            print(rule["title"] + " reset successfully")
 
     if allow_product_usage_analytics:
         try:
             contrast.send_usage_event(org_id, True, org_key)
 
         except urllib.error.HTTPError as err:
             if enable_verbose_error_logging:
+                print(err)
                 print(traceback.format_exc())
             else:
-                print("Unable to send usage data")
+                print("Unable to send usage data")
```

### Comparing `c6t-0.0.1/src/c6t/ui/auth.py` & `c6t-0.0.2/src/c6t/ui/auth.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import sys
 
 import requests
 
-from typing import Any, List
+from typing import Any, List, Dict, Optional
 
 import typer
-from InquirerPy import inquirer
-from InquirerPy.base.control import Choice
+
+from PyInquirer import prompt  # type: ignore
+
+# from InquirerPy import inquirer
+# from InquirerPy.base.control import Choice
 
 from c6t.configure.credentials import ContrastAPICredentials, ContrastUICredentials
 
 
 class ContrastUIAuthManager:
     def __init__(self, base_url: str):
         self.ui_credentials = ContrastUICredentials()
@@ -266,15 +269,15 @@
             else:
                 response.raise_for_status()
             return ""
         except requests.exceptions.HTTPError as e:
             print(e)
             sys.exit(1)
 
-    def get_organizations(self) -> list[str]:
+    def get_organizations(self) -> List[str]:
         """
         Get the organizations from TeamServer
         """
         url = f"{self.base_url}/api/ng/profile/organizations"
 
         try:
             response = self.session.get(url)
@@ -293,31 +296,44 @@
             sys.exit(1)
 
     def select_organization(self, organizations: Any) -> Any:
         """
         Ask the user to select an organization by index number
         """
 
-        organization_choices: List[Choice] = []
+        organization_choices: List[Dict[str, Optional[str]]] = []
 
         for organization in organizations:
             organization_choices.append(
-                Choice(
-                    value=organization.get("organization_uuid"),
-                    name=organization.get("name"),
-                )
+                {
+                    "name": organization.get("name"),
+                    "value": organization.get("organization_uuid"),
+                }
             )
-        organization_choices.append(Choice(value=None, name="Exit"))
 
-        organization_uuid = inquirer.select(  # type: ignore
-            message="Select your organization:",
-            choices=organization_choices,
-        ).execute()
+        organization_choices.append(
+            {
+                "name": "Exit",
+                "value": None,
+            }
+        )
+
+        organization_questions = [
+            {
+                "type": "list",
+                "name": "organization",
+                "message": "Select your organization:",
+                "choices": organization_choices,
+            }
+        ]
+
+        organization_answers = prompt(organization_questions)  # type: ignore
+        organization_uuid = organization_answers.get("organization")  # type: ignore
 
-        return organization_uuid
+        return organization_uuid  # type: ignore
 
     def toggle_superadmin(self) -> None:
         """
         Toggle the SuperAdmin role for the user.
         This is a hack to get the Contrast UI key cookies set.
         Cookies are set as a side-effect of this request.
         """
@@ -326,15 +342,15 @@
             response = self.session.get(url)
             if response.status_code != 200:
                 response.raise_for_status()
         except requests.exceptions.HTTPError as e:
             print(e)
             sys.exit(1)
 
-    def get_superadmin_users_roles(self) -> list[str]:
+    def get_superadmin_users_roles(self) -> List[str]:
         # TODO: This may not be needed.
         # TODO: Determine the meaning of the returned roles.
         """
         Get the SuperAdmin roles for the user
         """
         url = f"{self.base_url}/api/ng/superadmin/users/roles"
         try:
```

### Comparing `c6t-0.0.1/.gitignore` & `c6t-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `c6t-0.0.1/LICENSE` & `c6t-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `c6t-0.0.1/README.md` & `c6t-0.0.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 ### Features
 - Login to your Contrast account and save your API credentials to your local machine.
 - Configure your API credentials manually.
 - Download the agent configuration file to your local machine.
 
 ### Pre-requisites
-- Python 3.11+
+- Python 3.8 or higher
 
 ### Installation
 ```shell
 $ pip install c6t
 ```
 
 ### Usage
```

### Comparing `c6t-0.0.1/pyproject.toml` & `c6t-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [project]
 name = "c6t"
-version = "0.0.1"
+version = "0.0.2"
 description = "Unofficial Administrative Command Line Interface for Contrast Security"
 authors = [
-    { name = "Jonathan Harper", email = "39912347+jharper-sec@users.noreply.github.com" }
+    { name = "Jonathan Harper", email = "39912347+jharper-sec@users.noreply.github.com" },
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
-    "inquirerpy>=0.3.4",
+    "pyinquirer>=1.0.3",
 ]
-license = {file = "LICENSE"}
+license = { file = "LICENSE" }
 readme = "README.md"
-requires-python = ">= 3.11"
+requires-python = ">= 3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
 ]
 
 [project.urls]
```

### Comparing `c6t-0.0.1/PKG-INFO` & `c6t-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: c6t
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial Administrative Command Line Interface for Contrast Security
 Project-URL: Homepage, https://github.com/jharper-sec/c6t
 Project-URL: Issues, https://github.com/jharper-sec/c6t/issues
 Project-URL: Documentation, https://github.com/jharper-sec/c6t/blob/main/README.md
 Author-email: Jonathan Harper <39912347+jharper-sec@users.noreply.github.com>
 License: Copyright 2023 Contrast Security, Inc.
         
@@ -19,19 +19,19 @@
         WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
         See the License for the specific language governing permissions and
         limitations under the License.
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.11
+Requires-Python: >=3.8
 Requires-Dist: annotated-types>=0.6.0
 Requires-Dist: gitpython>=3.1.43
-Requires-Dist: inquirerpy>=0.3.4
 Requires-Dist: jinja2>=3.1.4
+Requires-Dist: pyinquirer>=1.0.3
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: requests>=2.32.0
 Requires-Dist: rich>=13.7.1
 Requires-Dist: shellingham>=1.5.4
 Requires-Dist: typer[all]>=0.12.3
 Requires-Dist: types-requests>=2.31.0.20240406
 Description-Content-Type: text/markdown
@@ -41,15 +41,15 @@
 
 ### Features
 - Login to your Contrast account and save your API credentials to your local machine.
 - Configure your API credentials manually.
 - Download the agent configuration file to your local machine.
 
 ### Pre-requisites
-- Python 3.11+
+- Python 3.8 or higher
 
 ### Installation
 ```shell
 $ pip install c6t
 ```
 
 ### Usage
```

