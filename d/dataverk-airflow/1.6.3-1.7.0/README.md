# Comparing `tmp/dataverk_airflow-1.6.3.tar.gz` & `tmp/dataverk_airflow-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataverk_airflow-1.6.3.tar", max compression
+gzip compressed data, was "dataverk_airflow-1.7.0.tar", max compression
```

## Comparing `dataverk_airflow-1.6.3.tar` & `dataverk_airflow-1.7.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1061 2024-04-17 08:40:28.300348 dataverk_airflow-1.6.3/LICENSE
--rw-r--r--   0        0        0     8319 2024-04-17 08:40:28.304348 dataverk_airflow-1.6.3/README.md
--rw-r--r--   0        0        0      381 2024-04-17 08:40:28.304348 dataverk_airflow-1.6.3/dataverk_airflow/__init__.py
--rw-r--r--   0        0        0      752 2024-04-17 08:40:28.304348 dataverk_airflow-1.6.3/dataverk_airflow/bucket_read.py
--rw-r--r--   0        0        0     1264 2024-04-17 08:40:28.304348 dataverk_airflow-1.6.3/dataverk_airflow/git_clone.py
--rw-r--r--   0        0        0     9712 2024-04-17 08:40:28.304348 dataverk_airflow-1.6.3/dataverk_airflow/kubernetes_operator.py
--rw-r--r--   0        0        0     4222 2024-04-17 08:40:28.304348 dataverk_airflow-1.6.3/dataverk_airflow/notebook_operator.py
--rw-r--r--   0        0        0     1058 2024-04-17 08:40:28.304348 dataverk_airflow-1.6.3/dataverk_airflow/notifications.py
--rw-r--r--   0        0        0     4051 2024-04-17 08:40:28.304348 dataverk_airflow-1.6.3/dataverk_airflow/python_operator.py
--rw-r--r--   0        0        0     5716 2024-04-17 08:40:28.304348 dataverk_airflow-1.6.3/dataverk_airflow/quarto_operator.py
--rw-r--r--   0        0        0      877 2024-04-17 08:40:28.560351 dataverk_airflow-1.6.3/pyproject.toml
--rw-r--r--   0        0        0     9295 1970-01-01 00:00:00.000000 dataverk_airflow-1.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/LICENSE
+-rw-r--r--   0        0        0     8443 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/README.md
+-rw-r--r--   0        0        0      381 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/__init__.py
+-rw-r--r--   0        0        0      752 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/bucket_read.py
+-rw-r--r--   0        0        0     1264 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/git_clone.py
+-rw-r--r--   0        0        0    10042 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/kubernetes_operator.py
+-rw-r--r--   0        0        0     4377 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/notebook_operator.py
+-rw-r--r--   0        0        0     1058 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/notifications.py
+-rw-r--r--   0        0        0     4206 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/python_operator.py
+-rw-r--r--   0        0        0     5871 2024-05-21 10:54:34.847525 dataverk_airflow-1.7.0/dataverk_airflow/quarto_operator.py
+-rw-r--r--   0        0        0      877 2024-05-21 10:54:35.111521 dataverk_airflow-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0     9419 1970-01-01 00:00:00.000000 dataverk_airflow-1.7.0/PKG-INFO
```

### Comparing `dataverk_airflow-1.6.3/LICENSE` & `dataverk_airflow-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.6.3/README.md` & `dataverk_airflow-1.7.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 ## Våre operators
 
 Alle våre operators lar deg klone et annet repo enn der DAGene er definert, bare legg det til med `repo="navikt/<repo>`.
 
 Vi har også støtte for å installere Python pakker ved oppstart av Airflow task, spesifiser `requirements.txt`-filen din med `requirements_path="/path/to/requirements.txt"`.
 Merk at hvis du kombinerer `repo` og `requirements_path`, må `requirements.txt` ligge i repoet nevnt i `repo`.
 
+Ønsker du å benytte [UV](https://github.com/astral-sh/uv) for `pip install`, så kan du sette `use_uv_pip_install=True`.
+
 ### Quarto operator (datafortelling)
 
 Denne kjører `quarto render` for deg, som lager en HTML-fil som kan lastes opp til Datamarkedsplassen.
 
 Vi har støtte for enkeltfiler, og kataloger, dette kan du spesifisere med `path` for enkeltfiler, og `folder` hvis du har et Quarto prosjekt i en katalog.
 Quarto prosjekter brukes hovedsakelig for [book](https://quarto.org/docs/books/), [website](https://quarto.org/docs/websites/), eller [dashboard](https://quarto.org/docs/dashboards/).
 Enkeltfiler bygges `self-contained`, som betyr at HTML-filen blir bygd med alle sine eksterne avhengighter (Javascript, CSS, og bilder).
```

### Comparing `dataverk_airflow-1.6.3/dataverk_airflow/bucket_read.py` & `dataverk_airflow-1.7.0/dataverk_airflow/bucket_read.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.6.3/dataverk_airflow/git_clone.py` & `dataverk_airflow-1.7.0/dataverk_airflow/git_clone.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.6.3/dataverk_airflow/kubernetes_operator.py` & `dataverk_airflow-1.7.0/dataverk_airflow/kubernetes_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
         retries: int = 3,
         delete_on_finish: bool = True,
         retry_delay: timedelta = timedelta(seconds=5),
         do_xcom_push: bool = False,
         container_uid: int = 50000,
         on_success_callback: Callable = None,
         working_dir: str = None,
+        use_uv_pip_install: bool = False,
 ):
     """Simplified operator for creating KubernetesPodOperator.
 
     If you use the slack_channel argument, the following host will also be added:
     - hooks.slack.com
 
     If you use the email argument, the following host will also be added:
@@ -88,14 +89,15 @@
     :param container_uid: int: User ID for the container image. Root (id = 0) is not allowed, defaults to 50000 (standard uid for airflow).
     :param on_success_callback: a function or list of functions to be called when a task instance
         of this task fails. a context dictionary is passed as a single
         parameter to this function. Context contains references to related
         objects to the task instance and is documented under the macros
         section of the API.
     :param working_dir: str: Path to working directory
+    :param use_uv_pip_install: bool: Use uv pip install, default False
 
     :return: KubernetesPodOperator
     """
     is_composer = True if os.getenv("GCS_BUCKET") else False
 
     if not is_composer:
         if repo in [None, ""]:
@@ -129,16 +131,20 @@
 
     if working_dir:
         working_dir = POD_WORKSPACE_DIR + "/" + working_dir
     else:
         working_dir = POD_WORKSPACE_DIR
 
     if requirements_path:
-        cmds = [
-            f"pip install -r {POD_WORKSPACE_DIR}/{requirements_path} --user --no-cache-dir"] + cmds
+        if use_uv_pip_install:
+            cmds = [
+                f"uv venv .local && . .local/bin/activate && uv pip install -r {POD_WORKSPACE_DIR}/{requirements_path} --no-cache-dir"] + cmds
+        else:
+            cmds = [
+                f"pip install -r {POD_WORKSPACE_DIR}/{requirements_path} --user --no-cache-dir"] + cmds
 
         allowlist.append("pypi.org")
         allowlist.append("files.pythonhosted.org")
         allowlist.append("pypi.python.org")
 
     if resources is None:
         resources = client.V1ResourceRequirements(
```

### Comparing `dataverk_airflow-1.6.3/dataverk_airflow/notebook_operator.py` & `dataverk_airflow-1.7.0/dataverk_airflow/notebook_operator.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         startup_timeout_seconds: int = None,
         retries: int = None,
         delete_on_finish: bool = True,
         retry_delay: timedelta = None,
         do_xcom_push: bool = False,
         on_success_callback: Callable = None,
         container_uid: int = 50000,
+        use_uv_pip_install: bool = False,
 ):
     """Operator for executing Jupyter notebooks.
 
     :param dag: DAG: owner DAG
     :param name: str: Name of task
     :param repo: str: Github repo
     :param nb_path: str: Path to notebook in repo
@@ -51,14 +52,15 @@
     :param startup_timeout_seconds: int: pod startup timeout
     :param retries: int: Number of retries for task before DAG fails, default 3
     :param delete_on_finish: bool: Whether to delete pod on completion
     :param retry_delay: timedelta: Time inbetween retries, default 5 seconds
     :param do_xcom_push: bool: Enable xcom push of content in file '/airflow/xcom/return.json', default False
     :param container_uid: int: User ID for the container image. Root (id = 0) is not allowed, defaults to 50000 (standard uid for airflow).
     :param on_success_callback: Callable
+    :param use_uv_pip_install: bool: Use uv pip install, default False
 
     :return: KubernetesPodOperator
     """
     if not image:
         if python_version not in VALID_PYTHON_VERSIONS:
             raise ValueError(
                 f"When using the default image the python_version argument must be set to "
@@ -74,12 +76,12 @@
         cmds[-1] += " --log-output"
 
     kwargs = {
         "dag": dag, "name": name, "repo": repo, "image": image, "cmds": cmds, "branch": branch, "email": email,
         "slack_channel": slack_channel, "extra_envs": extra_envs, "allowlist": allowlist, "requirements_path": requirements_path,
         "resources": resources, "startup_timeout_seconds": startup_timeout_seconds, 
         "retries": retries, "delete_on_finish": delete_on_finish, "retry_delay": retry_delay, "do_xcom_push": do_xcom_push,
-        "on_success_callback": on_success_callback, "working_dir": str(Path(nb_path).parent), "container_uid": container_uid,
+        "on_success_callback": on_success_callback, "working_dir": str(Path(nb_path).parent), "container_uid": container_uid, "use_uv_pip_install": use_uv_pip_install,
     }
     kwargs = {k: v for k, v in kwargs.items() if v is not None}
 
     return kubernetes_operator(**kwargs)
```

### Comparing `dataverk_airflow-1.6.3/dataverk_airflow/notifications.py` & `dataverk_airflow-1.7.0/dataverk_airflow/notifications.py`

 * *Files identical despite different names*

### Comparing `dataverk_airflow-1.6.3/dataverk_airflow/python_operator.py` & `dataverk_airflow-1.7.0/dataverk_airflow/python_operator.py`

 * *Files 17% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         startup_timeout_seconds: int = None,
         retries: int = None,
         delete_on_finish: bool = True,
         retry_delay: timedelta = None,
         do_xcom_push: bool = False,
         container_uid: int = 50000,
         on_success_callback: Callable = None,
+        use_uv_pip_install: bool = False,
 ):
     """Operator for executing Python scripts.
 
     :param dag: DAG: owner DAG
     :param name: str: Name of task
     :param repo: str: Github repo
     :param script_path: str: Path to script in repo
@@ -49,14 +50,15 @@
     :param startup_timeout_seconds: int: pod startup timeout
     :param retries: int: Number of retries for task before DAG fails, default 3
     :param delete_on_finish: bool: Whether to delete pod on completion
     :param retry_delay: timedelta: Time inbetween retries, default 5 seconds
     :param do_xcom_push: bool: Enable xcom push of content in file '/airflow/xcom/return.json', default False
     :param container_uid: int: User ID for the container image. Root (id = 0) is not allowed, defaults to 50000 (standard uid for airflow).
     :param on_success_callback: Callable
+    :param use_uv_pip_install: bool: Use uv pip install, default False
 
     :return: KubernetesPodOperator
     """
     if not image:
         if python_version not in VALID_PYTHON_VERSIONS:
             raise ValueError(
                 f"When using the default image the python_version argument must be set to " \
@@ -70,12 +72,12 @@
     cmds = [f"python {Path(script_path).name}"]
 
     kwargs = {
         "dag": dag, "name": name, "repo": repo, "image": image, "cmds": cmds, "branch": branch, "email": email,
         "slack_channel": slack_channel, "extra_envs": extra_envs, "allowlist": allowlist, "requirements_path": requirements_path,
         "resources": resources, "startup_timeout_seconds": startup_timeout_seconds, 
         "retries": retries, "delete_on_finish": delete_on_finish, "retry_delay": retry_delay, "do_xcom_push": do_xcom_push,
-        "on_success_callback": on_success_callback, "working_dir": str(Path(script_path).parent), "container_uid": container_uid,
+        "on_success_callback": on_success_callback, "working_dir": str(Path(script_path).parent), "container_uid": container_uid, "use_uv_pip_install": use_uv_pip_install,
     }
     kwargs = {k: v for k, v in kwargs.items() if v is not None}
 
     return kubernetes_operator(**kwargs)
```

### Comparing `dataverk_airflow-1.6.3/dataverk_airflow/quarto_operator.py` & `dataverk_airflow-1.7.0/dataverk_airflow/quarto_operator.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
         startup_timeout_seconds: int = None,
         retries: int = None,
         delete_on_finish: bool = True,
         retry_delay: timedelta = None,
         do_xcom_push: bool = False,
         container_uid: int = 50000,
         on_success_callback: Callable = None,
+        use_uv_pip_install: bool = False,
 ):
     """Operator for rendering Quarto.
 
     This operator will automatically add Datamarkedsplassen, and cdnjs.cloudflare.com to the allow list, as these are required to render and publish a Quarto story.
 
     :param dag: DAG: owner DAG
     :param name: str: Name of task
@@ -51,14 +52,15 @@
     :param startup_timeout_seconds: int: Pod startup timeout
     :param retries: int: Number of retries for task before DAG fails, default 3
     :param delete_on_finish: bool: Whether to delete pod on completion
     :param retry_delay: timedelta: Time inbetween retries, default 5 seconds
     :param do_xcom_push: bool: Enable xcom push of content in file '/airflow/xcom/return.json', default False
     :param container_uid: int: User ID for the container image. Root (id = 0) is not allowed, defaults to 50000 (standard uid for airflow).
     :param on_success_callback: Callable
+    :param use_uv_pip_install: bool: Use uv pip install, default False
 
     :return: KubernetesPodOperator
     """
     if not image:
         if python_version not in VALID_PYTHON_VERSIONS:
             raise ValueError(
                 f"When using the default image the python_version argument must be set to " \
@@ -93,15 +95,15 @@
     allowlist.append("cdnjs.cloudflare.com")
 
     kwargs = {
         "dag": dag, "name": name, "repo": repo, "image": image, "cmds": cmds, "branch": branch, "email": email,
         "slack_channel": slack_channel, "extra_envs": extra_envs, "allowlist": allowlist, "requirements_path": requirements_path,
         "resources": resources, "startup_timeout_seconds": startup_timeout_seconds, 
         "retries": retries, "delete_on_finish": delete_on_finish, "retry_delay": retry_delay, "do_xcom_push": do_xcom_push,
-        "on_success_callback": on_success_callback, "working_dir": str(working_dir), "container_uid": container_uid,
+        "on_success_callback": on_success_callback, "working_dir": str(working_dir), "container_uid": container_uid, "use_uv_pip_install": use_uv_pip_install,
     }
 
     kwargs = {k: v for k, v in kwargs.items() if v is not None}
     return kubernetes_operator(**kwargs)
 
 
 def create_quarto_cmds(quarto: dict, host: str) -> list:
```

### Comparing `dataverk_airflow-1.6.3/pyproject.toml` & `dataverk_airflow-1.7.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataverk-airflow"
-version = "1.6.3"
+version = "1.7.0"
 description = ""
 authors = ["NAV", "NADA"]
 readme = "README.md"
 packages = [{include = "dataverk_airflow"}]
 repository = "https://github.com/navikt/dataverk-airflow"
 classifiers = [
   'Development Status :: 5 - Production/Stable',
```

### Comparing `dataverk_airflow-1.6.3/PKG-INFO` & `dataverk_airflow-1.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataverk-airflow
-Version: 1.6.3
+Version: 1.7.0
 Summary: 
 Home-page: https://github.com/navikt/dataverk-airflow
 Author: NAV
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Apache Airflow
 Classifier: Framework :: Apache Airflow :: Provider
@@ -29,14 +29,16 @@
 ## Våre operators
 
 Alle våre operators lar deg klone et annet repo enn der DAGene er definert, bare legg det til med `repo="navikt/<repo>`.
 
 Vi har også støtte for å installere Python pakker ved oppstart av Airflow task, spesifiser `requirements.txt`-filen din med `requirements_path="/path/to/requirements.txt"`.
 Merk at hvis du kombinerer `repo` og `requirements_path`, må `requirements.txt` ligge i repoet nevnt i `repo`.
 
+Ønsker du å benytte [UV](https://github.com/astral-sh/uv) for `pip install`, så kan du sette `use_uv_pip_install=True`.
+
 ### Quarto operator (datafortelling)
 
 Denne kjører `quarto render` for deg, som lager en HTML-fil som kan lastes opp til Datamarkedsplassen.
 
 Vi har støtte for enkeltfiler, og kataloger, dette kan du spesifisere med `path` for enkeltfiler, og `folder` hvis du har et Quarto prosjekt i en katalog.
 Quarto prosjekter brukes hovedsakelig for [book](https://quarto.org/docs/books/), [website](https://quarto.org/docs/websites/), eller [dashboard](https://quarto.org/docs/dashboards/).
 Enkeltfiler bygges `self-contained`, som betyr at HTML-filen blir bygd med alle sine eksterne avhengighter (Javascript, CSS, og bilder).
```

