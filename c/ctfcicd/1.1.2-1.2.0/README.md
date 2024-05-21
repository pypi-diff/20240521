# Comparing `tmp/ctfcicd-1.1.2.tar.gz` & `tmp/ctfcicd-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctfcicd-1.1.2.tar", last modified: Fri Oct 20 14:57:21 2023, max compression
+gzip compressed data, was "ctfcicd-1.2.0.tar", last modified: Tue May 21 08:04:22 2024, max compression
```

## Comparing `ctfcicd-1.1.2.tar` & `ctfcicd-1.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 14:57:21.595664 ctfcicd-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2023-10-20 14:57:07.000000 ctfcicd-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-10-20 14:57:21.595664 ctfcicd-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2023-10-20 14:57:07.000000 ctfcicd-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 14:57:21.595664 ctfcicd-1.1.2/ctfcicd/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-10-20 14:57:07.000000 ctfcicd-1.1.2/ctfcicd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-10-20 14:57:07.000000 ctfcicd-1.1.2/ctfcicd/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2023-10-20 14:57:07.000000 ctfcicd-1.1.2/ctfcicd/cicd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 14:57:21.595664 ctfcicd-1.1.2/ctfcicd/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-20 14:57:07.000000 ctfcicd-1.1.2/ctfcicd/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      805 2023-10-20 14:57:07.000000 ctfcicd-1.1.2/ctfcicd/utils/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13768 2023-10-20 14:57:07.000000 ctfcicd-1.1.2/ctfcicd/utils/challenge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2023-10-20 14:57:07.000000 ctfcicd-1.1.2/ctfcicd/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2553 2023-10-20 14:57:07.000000 ctfcicd-1.1.2/ctfcicd/utils/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)       99 2023-10-20 14:57:07.000000 ctfcicd-1.1.2/ctfcicd/utils/images.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-20 14:57:21.595664 ctfcicd-1.1.2/ctfcicd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2023-10-20 14:57:21.000000 ctfcicd-1.1.2/ctfcicd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      422 2023-10-20 14:57:21.000000 ctfcicd-1.1.2/ctfcicd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-20 14:57:21.000000 ctfcicd-1.1.2/ctfcicd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2023-10-20 14:57:21.000000 ctfcicd-1.1.2/ctfcicd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2023-10-20 14:57:21.000000 ctfcicd-1.1.2/ctfcicd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-10-20 14:57:21.000000 ctfcicd-1.1.2/ctfcicd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-10-20 14:57:07.000000 ctfcicd-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-20 14:57:21.595664 ctfcicd-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:22.036954 ctfcicd-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-21 08:04:18.000000 ctfcicd-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-21 08:04:22.036954 ctfcicd-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-21 08:04:18.000000 ctfcicd-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:22.032954 ctfcicd-1.2.0/ctfcicd/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 08:04:18.000000 ctfcicd-1.2.0/ctfcicd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-21 08:04:18.000000 ctfcicd-1.2.0/ctfcicd/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5916 2024-05-21 08:04:18.000000 ctfcicd-1.2.0/ctfcicd/cicd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:22.036954 ctfcicd-1.2.0/ctfcicd/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:18.000000 ctfcicd-1.2.0/ctfcicd/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-21 08:04:18.000000 ctfcicd-1.2.0/ctfcicd/utils/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14081 2024-05-21 08:04:18.000000 ctfcicd-1.2.0/ctfcicd/utils/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-21 08:04:18.000000 ctfcicd-1.2.0/ctfcicd/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-21 08:04:18.000000 ctfcicd-1.2.0/ctfcicd/utils/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-21 08:04:18.000000 ctfcicd-1.2.0/ctfcicd/utils/images.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:22.036954 ctfcicd-1.2.0/ctfcicd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-05-21 08:04:22.000000 ctfcicd-1.2.0/ctfcicd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-21 08:04:22.000000 ctfcicd-1.2.0/ctfcicd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:04:22.000000 ctfcicd-1.2.0/ctfcicd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 08:04:22.000000 ctfcicd-1.2.0/ctfcicd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 08:04:22.000000 ctfcicd-1.2.0/ctfcicd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 08:04:22.000000 ctfcicd-1.2.0/ctfcicd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-21 08:04:18.000000 ctfcicd-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:04:22.036954 ctfcicd-1.2.0/setup.cfg
```

### Comparing `ctfcicd-1.1.2/LICENSE` & `ctfcicd-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ctfcicd-1.1.2/ctfcicd/cicd.py` & `ctfcicd-1.2.0/ctfcicd/cicd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,22 @@
-import imp
 import os
 from pathlib import PurePath
 import re
 import logging as log
 import subprocess
+from urllib.parse import urlparse
+from typing import List
 
 from ctfcicd.utils.deploy import DEPLOY_HANDLERS
 from ctfcicd.utils.config import Config
 from ctfcicd.utils.challenge import load_installed_challenges, load_challenge, Yaml, sync_challenge, create_challenge
-from urllib.parse import urlparse
 
 log.basicConfig(level=log.INFO)
 
+
 class CiCd:
     def __init__(self, prod=True, tls_verify=True):
         self.deploy_uri = os.getenv("DEPLOY_HOST", default=None)
         self.deploy_network = os.getenv("DEPLOY_NETWORK", default="bridge")
         self.prod = prod
         Config.generate_config(tls_verify)
         log.info("CTFcli initialized")
@@ -24,86 +25,117 @@
         installed_challenges = load_installed_challenges()
         for c in installed_challenges:
             if c["name"] == challenge["name"]:
                 return True
 
         return False
 
-    def deploy_challenge(self, challenge: str):
+    def deploy_challenge(self, challenge: str) -> None:
         if os.path.exists(f"{challenge}/challenge.yml"):
-                log.info(f"Checking challenge: {challenge}")
+            log.info("Checking challenge: %s", challenge)
 
-                if self.prod:
-                    if os.path.exists(f"{challenge}/disabled"):
-                        log.info(f"{challenge} is disabled.")
-                        log.info(f"{challenge} won't be deployed.")
-                        return
+            if self.prod:
+                if os.path.exists(f"{challenge}/disabled"):
+                    log.info("%s is disabled.", challenge)
+                    log.info("%s won't be deployed.", challenge)
+                    return
 
-                try:
-                    chall_class = load_challenge(f"{challenge}/challenge.yml")
-                except Exception as e:
-                    log.warning(f"Error loading challenge {challenge}/challenge.yml - ", e)
+            try:
+                chall_class = load_challenge(f"{challenge}/challenge.yml")
+            except Exception as e:
+                log.warning(
+                    "Error loading challenge %s/challenge.yml - %s", challenge, e)
+                return
+
+            if self.check_if_challenge_exists(chall_class):
+                log.info("Synchronising %s/challenge.yml", challenge)
+                sync_challenge(chall_class, ignore=["state"])
+            else:
+                log.info("Installing %s/challenge.yml", challenge)
+                create_challenge(chall_class, [])
+
+            if chall_class.get("image") is not None or os.path.exists(f"{challenge}/docker-compose.yml"):
+                target_host = chall_class.get("host") or self.deploy_uri
+                if bool(target_host) is False:
+                    log.warning(
+                        "This challenge can't be deployed because there is no target host to deploy to.")
                     return
 
-                if self.check_if_challenge_exists(chall_class):
-                    log.info(f"Synchronising {challenge}/challenge.yml")
-                    sync_challenge(chall_class,ignore=["state"])
-                else:
-                    log.info(f"Installing {challenge}/challenge.yml")
-                    create_challenge(chall_class)
-
-                if chall_class.get("image") is not None or os.path.exists(f"{challenge}/docker-compose.yml"):
-                    target_host = chall_class.get("host") or self.deploy_uri
-                    if bool(target_host) is False:
-                        log.warning("This challenge can't be deployed because there is no target host to deploy to.")
-                        return
-
-                    url = urlparse(target_host)
-                    if bool(url.netloc) is False:
-                        log.warning("Provided host has no URI scheme. Provide a URI scheme like ssh:// or registry://")
-
-                    try:
-                        port = DEPLOY_HANDLERS[url.scheme](
-                            challenge=chall_class, host=target_host, network=self.deploy_network
-                        )
-                    except Exception as e:
-                        log.warning("Error while deploying challenge - " + str(e))
-                        exit(1)
+                url = urlparse(target_host)
+                if bool(url.netloc) is False:
+                    log.warning(
+                        "Provided host has no URI scheme. Provide a URI scheme like ssh:// or registry://")
 
-                    if port is not None:
-                        log.info(f"Challenge {challenge} deployed at {url.netloc[url.netloc.find('@') + 1 :]}:{port}")
+                try:
+                    port = DEPLOY_HANDLERS[url.scheme](  # type: ignore
+                        challenge=chall_class, host=target_host, network=self.deploy_network  # type: ignore
+                    )
+                except Exception as e:
+                    log.warning("Error while deploying challenge - %s", str(e))
+                    exit(1)
+
+                if port is not None:
+                    log.info("Challenge %s deployed at %s:%s", challenge,
+                             url.netloc[url.netloc.find('@') + 1:], port)  # type: ignore
 
     # Synchronize all challenges in the given category, where each challenge is in it's own folder.
-    def sync_folder(self, category):
-        local_challenges = [f"{category}/{name}" for name in os.listdir(f"./{category}") if
-                            os.path.isdir(f"{category}/{name}")]
+    def sync_folder(self, category: str, challenges: List[str]) -> None:
+        local_challenges, deployed_challs = [], []
+
+        for name in os.listdir(f"./{category}"):
+            if os.path.isdir(f"{category}/{name}"):
+                local_challenges += [f"{category}/{name}"]
+                if name in challenges:
+                    challenges.remove(name)
+                    self.deploy_challenge(f"{category}/{name}")
+                    deployed_challs += [name]
+
+        if len(deployed_challs) == 0 and len(challenges) == 0:
+            self.deploy_all_challenges(local_challenges)
+        else:
+            not_deployed_challs = set(
+                challenges).difference(set(deployed_challs))
+            for c in not_deployed_challs:
+                log.warning("Challenge %s does not exist", c)
 
+    def deploy_all_challenges(self, local_challenges) -> None:
         for challenge in local_challenges:
             self.deploy_challenge(challenge)
 
-
-    def sync_folder_with_git(self, github_event, github_sha):
+    def sync_folder_with_git(self, github_event, github_sha) -> None:
         log.info("Differential syncronise")
         try:
-            files = subprocess.check_output(['git', 'diff', '--name-only', github_event, github_sha]).split()
-            folders_with_change = list(set([ PurePath(i.decode()).parents[-3] for i in files if len(PurePath(i.decode()).parents) >= 3 ]))
+            files = subprocess.check_output(
+                ['git', 'diff', '--name-only', github_event, github_sha]).split()
+            folders_with_change = list(set([PurePath(
+                i.decode()).parents[-3] for i in files if len(PurePath(i.decode()).parents) >= 3]))
             for i in folders_with_change:
-                self.deploy_challenge(i)
+                self.deploy_challenge(i.as_posix())
         except subprocess.CalledProcessError as e:
-            log.warning(f"Error running - {e}")
+            log.warning("Error running - %s", e)
             self.deploy_current_folder()
 
+    def deploy_current_folder(self, *challenges) -> None:
+        challs: List[str] = list(challenges)
+        initial_challs_len = len(challenges)
+
+        for category in self.get_categories():
+            log.info("Synchronizing %s challenges", category)
+            # challenges variable is pass-by-reference
+            # https://www.geeksforgeeks.org/pass-by-reference-vs-value-in-python/
+            if initial_challs_len != 0 and len(challs) == 0:
+                continue
+            else:
+                self.sync_folder(category, challs)
 
-    def deploy_current_folder(self):
-        for i in self.get_categories():
-            log.info("Synchronizing " + i + " challenges")
-            self.sync_folder(i)
-
-    # Each category is in it's own directory, get the names of all directories that do not begin with '.'.
+    # Each category is in it's own directory,
+    # get the names of all directories that do not begin with '.'.
     @staticmethod
-    def get_categories():
-        denylist_regex = r'\..*'
+    def get_categories() -> List[str]:
+        denylist_regex = r"\..*"
 
         categories = [name for name in os.listdir(".") if
                       os.path.isdir(name) and not re.match(denylist_regex, name)]
-        log.info("Categories: " + ", ".join(categories))
+        # Fix: Use lazy % formatting in logging function
+        log.info("Categories: %s", ", ".join(categories))
+
         return categories
```

### Comparing `ctfcicd-1.1.2/ctfcicd/utils/api.py` & `ctfcicd-1.2.0/ctfcicd/utils/api.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 from urllib.parse import urljoin
 
 from requests import Session
 
 
 class APISession(Session):
-    def __init__(self, prefix_url=None, verify_tls=True, *args, **kwargs):
+    def __init__(self, *args, prefix_url: str = "", verify_tls: bool = True, **kwargs):
         super(APISession, self).__init__(*args, **kwargs)
         # Strip out ending slashes and append a singular one so we generate
         # clean base URLs for both main deployments and subdir deployments
-        self.prefix_url = prefix_url.rstrip("/") + "/"
-        self.verify = verify_tls
+        self.prefix_url: str = prefix_url.rstrip("/") + "/"
+        self.verify: bool = verify_tls
 
-    def request(self, method, url, *args, **kwargs):
+    def request(self, method: str, url: str, *args, **kwargs):
         # Strip out the preceding / so that urljoin creates the right url
         # considering the appended / on the prefix_url
         url = urljoin(self.prefix_url, url.lstrip("/"))
-        return super(APISession, self).request(method, url, *args, **kwargs)
+        return super(APISession, self).request(method, url, *args, **kwargs)
```

### Comparing `ctfcicd-1.1.2/ctfcicd/utils/challenge.py` & `ctfcicd-1.2.0/ctfcicd/utils/challenge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,44 @@
 """
 Copy from ctfcli with some adaptations
 """
 
 import logging
 import subprocess
 from pathlib import Path
+from typing import Any, Dict, List
 
 import yaml
 
 from .config import Config
 
 
 class Yaml(dict):
-    def __init__(self, data, file_path=None):
+    def __init__(self, data: Dict[str, Any], file_path: str = ""):
         super().__init__(data)
         self.file_path = Path(file_path)
         self.directory = self.file_path.parent
 
 
-def load_challenge(path):
+def load_challenge(path: str) -> Yaml:
     try:
-        with open(path) as f:
+        with open(path, "r", encoding="utf-8") as f:
             return Yaml(data=yaml.safe_load(f.read()), file_path=path)
-    except FileNotFoundError:
-        raise Exception(f"No challenge.yml was found in {path}")
-        return
+    except FileNotFoundError as exc:
+        raise FileNotFoundError(
+            f"No challenge.yml was found in {path}") from exc
 
 
 def load_installed_challenges():
     s = Config.generate_session()
     return s.get("/api/v1/challenges?view=admin", json=True).json()["data"]
 
 
-def sync_challenge(challenge, ignore=[]):
-    data = {
+def sync_challenge(challenge: Yaml, ignore: List[str]) -> None:
+    data: Dict[str, Any] = {
         "name": challenge["name"],
         "category": challenge["category"],
         "description": challenge["description"],
         "type": challenge.get("type", "standard"),
         "value": int(challenge["value"]) if challenge["value"] else challenge["value"],
         **challenge.get("extra", {}),
     }
@@ -69,28 +70,29 @@
 
     r = s.patch(f"/api/v1/challenges/{challenge_id}", json=data)
     r.raise_for_status()
 
     # Create new flags
     if challenge.get("flags") and "flags" not in ignore:
         # Delete existing flags
-        current_flags = s.get(f"/api/v1/flags", json=data).json()["data"]
+        current_flags = s.get("/api/v1/flags", json=data).json()["data"]
         for flag in current_flags:
             if flag["challenge_id"] == challenge_id:
                 flag_id = flag["id"]
                 r = s.delete(f"/api/v1/flags/{flag_id}", json=True)
                 r.raise_for_status()
         for flag in challenge["flags"]:
-            if type(flag) == str:
-                data = {"content": flag, "type": "static", "challenge_id": challenge_id}
-                r = s.post(f"/api/v1/flags", json=data)
+            if isinstance(flag, str):
+                data = {"content": flag, "type": "static",
+                        "challenge_id": challenge_id}
+                r = s.post("/api/v1/flags", json=data)
                 r.raise_for_status()
-            elif type(flag) == dict:
+            elif isinstance(flag, dict):
                 flag["challenge_id"] = challenge_id
-                r = s.post(f"/api/v1/flags", json=flag)
+                r = s.post("/api/v1/flags", json=flag)
                 r.raise_for_status()
 
     # Update topics
     if challenge.get("topics") and "topics" not in ignore:
         # Delete existing challenge topics
         current_topics = s.get(
             f"/api/v1/challenges/{challenge_id}/topics", json=""
@@ -100,42 +102,42 @@
             r = s.delete(
                 f"/api/v1/topics?type=challenge&target_id={topic_id}", json=True
             )
             r.raise_for_status()
         # Add new challenge topics
         for topic in challenge["topics"]:
             r = s.post(
-                f"/api/v1/topics",
+                "/api/v1/topics",
                 json={
                     "value": topic,
                     "type": "challenge",
                     "challenge_id": challenge_id,
                 },
             )
             r.raise_for_status()
 
     # Update tags
     if challenge.get("tags") and "tags" not in ignore:
         # Delete existing tags
-        current_tags = s.get(f"/api/v1/tags", json=data).json()["data"]
+        current_tags = s.get("/api/v1/tags", json=data).json()["data"]
         for tag in current_tags:
             if tag["challenge_id"] == challenge_id:
                 tag_id = tag["id"]
                 r = s.delete(f"/api/v1/tags/{tag_id}", json=True)
                 r.raise_for_status()
         for tag in challenge["tags"]:
             r = s.post(
-                f"/api/v1/tags", json={"challenge_id": challenge_id, "value": tag}
+                "/api/v1/tags", json={"challenge_id": challenge_id, "value": tag}
             )
             r.raise_for_status()
 
     # Upload files
     if challenge.get("files") and "files" not in ignore:
         # Delete existing files
-        all_current_files = s.get(f"/api/v1/files?type=challenge", json=data).json()[
+        all_current_files = s.get("/api/v1/files?type=challenge", json=data).json()[
             "data"
         ]
         for f in all_current_files:
             for used_file in original_challenge["files"]:
                 if f["location"] in used_file:
                     file_id = f["id"]
                     r = s.delete(f"/api/v1/files/{file_id}", json=True)
@@ -143,55 +145,56 @@
         files = []
         for f in challenge["files"]:
             file_path = Path(challenge.directory, f)
             if file_path.exists():
                 file_object = ("file", file_path.open(mode="rb"))
                 files.append(file_object)
             else:
-                logging.warning(f"File {file_path} was not found")
+                logging.warning("File %s was not found", file_path)
                 raise Exception(f"File {file_path} was not found")
 
         data = {"challenge_id": challenge_id, "type": "challenge"}
         # Specifically use data= here instead of json= to send multipart/form-data
-        r = s.post(f"/api/v1/files", files=files, data=data)
+        r = s.post("/api/v1/files", files=files, data=data)
         r.raise_for_status()
 
     # Create hints
     if challenge.get("hints") and "hints" not in ignore:
         # Delete existing hints
-        current_hints = s.get(f"/api/v1/hints", json=data).json()["data"]
+        current_hints = s.get("/api/v1/hints", json=data).json()["data"]
         for hint in current_hints:
             if hint["challenge_id"] == challenge_id:
                 hint_id = hint["id"]
                 r = s.delete(f"/api/v1/hints/{hint_id}", json=True)
                 r.raise_for_status()
 
         for hint in challenge["hints"]:
-            if type(hint) == str:
-                data = {"content": hint, "cost": 0, "challenge_id": challenge_id}
+            if isinstance(hint, str):
+                data = {"content": hint, "cost": 0,
+                        "challenge_id": challenge_id}
             else:
                 data = {
                     "content": hint["content"],
                     "cost": hint["cost"],
                     "challenge_id": challenge_id,
                 }
 
-            r = s.post(f"/api/v1/hints", json=data)
+            r = s.post("/api/v1/hints", json=data)
             r.raise_for_status()
 
     # Update requirements
     if challenge.get("requirements") and "requirements" not in ignore:
         installed_challenges = load_installed_challenges()
         required_challenges = []
         for r in challenge["requirements"]:
-            if type(r) == str:
+            if isinstance(r, str):
                 for c in installed_challenges:
                     if c["name"] == r:
                         required_challenges.append(c["id"])
-            elif type(r) == int:
+            elif isinstance(r, int):
                 required_challenges.append(r)
 
         required_challenges = list(set(required_challenges))
         data = {"requirements": {"prerequisites": required_challenges}}
         r = s.patch(f"/api/v1/challenges/{challenge_id}", json=data)
         r.raise_for_status()
 
@@ -202,15 +205,15 @@
             if challenge["state"] in ["hidden", "visible"]:
                 data["state"] = challenge["state"]
 
         r = s.patch(f"/api/v1/challenges/{challenge_id}", json=data)
         r.raise_for_status()
 
 
-def create_challenge(challenge, ignore=[]):
+def create_challenge(challenge: Yaml, ignore: List[str]):
     data = {
         "name": challenge["name"],
         "category": challenge["category"],
         "description": challenge["description"],
         "type": challenge.get("type", "standard"),
         "value": int(challenge["value"]) if challenge["value"] else challenge["value"],
         **challenge.get("extra", {}),
@@ -234,86 +237,88 @@
 
     challenge_data = r.json()
     challenge_id = challenge_data["data"]["id"]
 
     # Create flags
     if challenge.get("flags") and "flags" not in ignore:
         for flag in challenge["flags"]:
-            if type(flag) == str:
-                data = {"content": flag, "type": "static", "challenge_id": challenge_id}
-                r = s.post(f"/api/v1/flags", json=data)
+            if isinstance(flag, str):
+                data = {"content": flag, "type": "static",
+                        "challenge_id": challenge_id}
+                r = s.post("/api/v1/flags", json=data)
                 r.raise_for_status()
-            elif type(flag) == dict:
+            elif isinstance(flag, dict):
                 flag["challenge"] = challenge_id
-                r = s.post(f"/api/v1/flags", json=flag)
+                r = s.post("/api/v1/flags", json=flag)
                 r.raise_for_status()
 
     # Create topics
     if challenge.get("topics") and "topics" not in ignore:
         for topic in challenge["topics"]:
             r = s.post(
-                f"/api/v1/topics",
+                "/api/v1/topics",
                 json={
                     "value": topic,
                     "type": "challenge",
                     "challenge_id": challenge_id,
                 },
             )
             r.raise_for_status()
 
     # Create tags
     if challenge.get("tags") and "tags" not in ignore:
         for tag in challenge["tags"]:
             r = s.post(
-                f"/api/v1/tags", json={"challenge_id": challenge_id, "value": tag}
+                "/api/v1/tags", json={"challenge_id": challenge_id, "value": tag}
             )
             r.raise_for_status()
 
     # Upload files
     if challenge.get("files") and "files" not in ignore:
         files = []
         for f in challenge["files"]:
             file_path = Path(challenge.directory, f)
             if file_path.exists():
                 file_object = ("file", file_path.open(mode="rb"))
                 files.append(file_object)
             else:
-                logging.warning(f"File {file_path} was not found")
+                logging.warning("File %s was not found", file_path)
                 raise Exception(f"File {file_path} was not found")
 
         data = {"challenge_id": challenge_id, "type": "challenge"}
         # Specifically use data= here instead of json= to send multipart/form-data
-        r = s.post(f"/api/v1/files", files=files, data=data)
+        r = s.post("/api/v1/files", files=files, data=data)
         r.raise_for_status()
 
     # Add hints
     if challenge.get("hints") and "hints" not in ignore:
         for hint in challenge["hints"]:
-            if type(hint) == str:
-                data = {"content": hint, "cost": 0, "challenge_id": challenge_id}
+            if isinstance(hint, str):
+                data = {"content": hint, "cost": 0,
+                        "challenge_id": challenge_id}
             else:
                 data = {
                     "content": hint["content"],
                     "cost": hint["cost"],
                     "challenge_id": challenge_id,
                 }
 
-            r = s.post(f"/api/v1/hints", json=data)
+            r = s.post("/api/v1/hints", json=data)
             r.raise_for_status()
 
     # Add requirements
     if challenge.get("requirements") and "requirements" not in ignore:
         installed_challenges = load_installed_challenges()
         required_challenges = []
         for r in challenge["requirements"]:
-            if type(r) == str:
+            if isinstance(r, str):
                 for c in installed_challenges:
                     if c["name"] == r:
                         required_challenges.append(c["id"])
-            elif type(r) == int:
+            elif isinstance(r, int):
                 required_challenges.append(r)
 
         required_challenges = list(set(required_challenges))
         data = {"requirements": {"prerequisites": required_challenges}}
         r = s.patch(f"/api/v1/challenges/{challenge_id}", json=data)
         r.raise_for_status()
 
@@ -327,15 +332,15 @@
         r.raise_for_status()
 
 
 def lint_challenge(path):
     try:
         challenge = load_challenge(path)
     except yaml.YAMLError as e:
-        logging.warning(f"Error parsing challenge.yml: {e}")
+        logging.warning("Error parsing challenge.yml: %s", e)
         exit(1)
 
     required_fields = ["name", "author", "category", "description", "value"]
     errors = []
     for field in required_fields:
         if field == "value" and challenge.get("type") == "dynamic":
             pass
@@ -364,14 +369,15 @@
             print("Dockerfile missing EXPOSE")
             exit(1)
 
         # Check Dockerfile with hadolint
         proc = subprocess.run(
             ["docker", "run", "--rm", "-i", "hadolint/hadolint"],
             input=dockerfile.encode(),
+            check=False
         )
         if proc.returncode != 0:
             print("Hadolint found Dockerfile lint issues, please resolve")
             exit(1)
 
     # Check that all files exists
     files = challenge.get("files", [])
```

### Comparing `ctfcicd-1.1.2/ctfcicd/utils/deploy.py` & `ctfcicd-1.2.0/ctfcicd/utils/deploy.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,70 +1,76 @@
 import logging as log
 import os
 import subprocess
 from pathlib import Path
+from typing import Optional, Dict
 
 from docker import from_env
 
 from .images import sanitize_name
 from .config import Config
 
-def ssh(challenge, host, network="bridge"):
+
+def ssh(challenge, host: str, network: str = "bridge") -> Optional[str]:
     os.environ["DOCKER_HOST"] = host
 
     path = str(Path(challenge.file_path).parent.absolute())
     if os.path.exists(f"{path}/docker-compose.yml"):
         log.info("Deploying docker-compose")
-        subprocess.run( Config.get_docker_compose_command() + ["-f", f"{path}/docker-compose.yml", "build", "--no-cache"], check=False)
+        subprocess.run(Config.get_docker_compose_command(
+        ) + ["-f", f"{path}/docker-compose.yml", "build", "--no-cache"], check=False)
         try:
-            subprocess.run( Config.get_docker_compose_command() + [ "-f", f"{path}/docker-compose.yml", "down"], check=False)
-            subprocess.run( Config.get_docker_compose_command() + ["-f", f"{path}/docker-compose.yml", "up", "-d"], check=True)
+            subprocess.run(Config.get_docker_compose_command(
+            ) + ["-f", f"{path}/docker-compose.yml", "down"], check=False)
+            subprocess.run(Config.get_docker_compose_command(
+            ) + ["-f", f"{path}/docker-compose.yml", "up", "-d"], check=True)
         except Exception as e:
             log.warning(e)
             log.critical("Docker-compose deployed with problem.")
             exit(1)
-        
+
         log.info("Docker-compose deployed correctly.")
         return None
 
     else:
         client = from_env(use_ssh_client=True)
 
         image_name = sanitize_name(challenge.get("image"))
         if image_name == "":
             image_name = sanitize_name(challenge.get("name"))
             if image_name == "":
-                log.critical("Unable to build docker image for " + challenge.get("name"))
+                log.critical("Unable to build docker image for %s",
+                             challenge.get("name"))
                 return None
 
-
         container_name = image_name + "_cont"
 
         image, _ = client.images.build(path=path, tag=image_name)
 
-        cont = client.containers.list(filters={'name': container_name}, sparse=True)
+        cont = client.containers.list(
+            filters={'name': container_name}, sparse=True)
 
         assert len(cont) <= 1
 
         if len(cont) == 1:
             if cont[0].image.id != image.id:
-                """ Remove container """
+                # Remove container
                 cont[0].stop()
                 cont[0].remove(v=True, force=True)
             else:
                 log.info("It's not necessary to update the container")
                 return
 
         try:
             ports = image.attrs['Config']['ExposedPorts'].keys()
         except KeyError:
             log.warning("Docker image doesn't have exposed ports.")
             return
 
-        exposed_ports = {}
+        exposed_ports: Dict[str, str] = {}
         for i in ports:
             exposed_ports[i] = i.split("/")[0]
 
         client.containers.run(image=image_name, name=container_name, restart_policy={"Name": "unless-stopped"},
                               ports=exposed_ports, network=network, detach=True)
         log.info("Container update with success")
```

### Comparing `ctfcicd-1.1.2/pyproject.toml` & `ctfcicd-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ctfcicd"
-version = "1.1.2"
+version = "1.2.0"
 description = "Tool for CI/CD pipelines to deploy CTFs"
 readme = "README.md"
 requires-python = ">=3.9"
 authors = [
   {name = "André Cirne"},
 ]
```

