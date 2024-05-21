# Comparing `tmp/loopquest-0.2.5.tar.gz` & `tmp/loopquest-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loopquest-0.2.5.tar", last modified: Mon May 13 19:19:58 2024, max compression
+gzip compressed data, was "loopquest-0.2.6.tar", last modified: Tue May 21 05:24:46 2024, max compression
```

## Comparing `loopquest-0.2.5.tar` & `loopquest-0.2.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-13 19:19:58.233238 loopquest-0.2.5/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.5/LICENSE
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-13 19:19:58.233238 loopquest-0.2.5/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5418 2024-04-29 17:12:15.000000 loopquest-0.2.5/README.md
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-13 19:19:58.233238 loopquest-0.2.5/loopquest/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.5/loopquest/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1517 2024-05-08 05:44:07.000000 loopquest-0.2.5/loopquest/api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9495 2024-05-08 05:56:32.000000 loopquest-0.2.5/loopquest/crud.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1933 2024-04-19 04:43:26.000000 loopquest-0.2.5/loopquest/datasets.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-13 19:19:58.233238 loopquest-0.2.5/loopquest/env/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 05:17:29.000000 loopquest-0.2.5/loopquest/env/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4768 2024-05-08 06:15:15.000000 loopquest-0.2.5/loopquest/env/api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6492 2024-05-11 19:42:13.000000 loopquest-0.2.5/loopquest/env/gym_wrappers.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9238 2024-04-19 04:43:26.000000 loopquest-0.2.5/loopquest/env/space_utils.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6293 2024-05-10 17:45:41.000000 loopquest-0.2.5/loopquest/eval.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-13 19:19:58.233238 loopquest-0.2.5/loopquest/policy/
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-04-19 04:43:26.000000 loopquest-0.2.5/loopquest/policy/__init__.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      321 2024-05-08 05:05:33.000000 loopquest-0.2.5/loopquest/policy/base.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1383 2024-04-19 04:43:26.000000 loopquest-0.2.5/loopquest/policy/sb3_policy.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     2001 2024-05-03 04:41:02.000000 loopquest-0.2.5/loopquest/private_api.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5798 2024-05-13 18:34:45.000000 loopquest-0.2.5/loopquest/schema.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.5/loopquest/typing.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.5/loopquest/ui.py
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4740 2024-05-03 05:20:31.000000 loopquest-0.2.5/loopquest/utils.py
-drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-13 19:19:58.233238 loopquest-0.2.5/loopquest.egg-info/
--rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6605 2024-05-13 19:19:58.000000 loopquest-0.2.5/loopquest.egg-info/PKG-INFO
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      578 2024-05-13 19:19:58.000000 loopquest-0.2.5/loopquest.egg-info/SOURCES.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-05-13 19:19:58.000000 loopquest-0.2.5/loopquest.egg-info/dependency_links.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      302 2024-05-13 19:19:58.000000 loopquest-0.2.5/loopquest.egg-info/requires.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-05-13 19:19:58.000000 loopquest-0.2.5/loopquest.egg-info/top_level.txt
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-05-13 19:19:58.233238 loopquest-0.2.5/setup.cfg
--rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1144 2024-05-13 19:18:30.000000 loopquest-0.2.5/setup.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-21 05:24:46.877519 loopquest-0.2.6/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)    11357 2024-04-19 04:42:45.000000 loopquest-0.2.6/LICENSE
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6567 2024-05-21 05:24:46.877519 loopquest-0.2.6/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5380 2024-05-21 03:41:05.000000 loopquest-0.2.6/README.md
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-21 05:24:46.877519 loopquest-0.2.6/loopquest/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       86 2024-04-24 04:38:12.000000 loopquest-0.2.6/loopquest/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1465 2024-05-21 03:27:00.000000 loopquest-0.2.6/loopquest/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9814 2024-05-21 05:03:28.000000 loopquest-0.2.6/loopquest/crud.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1943 2024-05-21 03:39:28.000000 loopquest-0.2.6/loopquest/datasets.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-21 05:24:46.877519 loopquest-0.2.6/loopquest/env/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-05-01 05:17:29.000000 loopquest-0.2.6/loopquest/env/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4768 2024-05-08 06:15:15.000000 loopquest-0.2.6/loopquest/env/api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6568 2024-05-21 05:15:32.000000 loopquest-0.2.6/loopquest/env/gym_wrappers.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     9238 2024-04-19 04:43:26.000000 loopquest-0.2.6/loopquest/env/space_utils.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     6321 2024-05-18 04:12:03.000000 loopquest-0.2.6/loopquest/eval.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-21 05:24:46.877519 loopquest-0.2.6/loopquest/policy/
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        0 2024-04-19 04:43:26.000000 loopquest-0.2.6/loopquest/policy/__init__.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      281 2024-05-17 06:20:02.000000 loopquest-0.2.6/loopquest/policy/base.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1383 2024-04-19 04:43:26.000000 loopquest-0.2.6/loopquest/policy/sb3_policy.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1961 2024-05-20 06:22:52.000000 loopquest-0.2.6/loopquest/private_api.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     5916 2024-05-21 03:48:15.000000 loopquest-0.2.6/loopquest/schema.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      168 2024-04-19 04:43:26.000000 loopquest-0.2.6/loopquest/typing.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      376 2024-04-19 04:42:45.000000 loopquest-0.2.6/loopquest/ui.py
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     4740 2024-05-19 04:55:08.000000 loopquest-0.2.6/loopquest/utils.py
+drwxrwxr-x   0 jinyu     (1000) jinyu     (1000)        0 2024-05-21 05:24:46.877519 loopquest-0.2.6/loopquest.egg-info/
+-rw-r--r--   0 jinyu     (1000) jinyu     (1000)     6567 2024-05-21 05:24:46.000000 loopquest-0.2.6/loopquest.egg-info/PKG-INFO
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      578 2024-05-21 05:24:46.000000 loopquest-0.2.6/loopquest.egg-info/SOURCES.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)        1 2024-05-21 05:24:46.000000 loopquest-0.2.6/loopquest.egg-info/dependency_links.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)      302 2024-05-21 05:24:46.000000 loopquest-0.2.6/loopquest.egg-info/requires.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       10 2024-05-21 05:24:46.000000 loopquest-0.2.6/loopquest.egg-info/top_level.txt
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)       38 2024-05-21 05:24:46.877519 loopquest-0.2.6/setup.cfg
+-rw-rw-r--   0 jinyu     (1000) jinyu     (1000)     1144 2024-05-21 05:23:55.000000 loopquest-0.2.6/setup.py
```

### Comparing `loopquest-0.2.5/LICENSE` & `loopquest-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.5/PKG-INFO` & `loopquest-0.2.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopquest
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Production Tool for Embodied AI.
 Home-page: https://github.com/LoopMind-AI/loopquest
 Author: LoopMind
 Author-email: contactus@loopmind.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
@@ -139,15 +139,15 @@
     'reward': -0.00,
     'prev_observation': [-0.55, 0.00],
     'termnated': False,
     'truncated': False,
     'done': False,
     'info': '{}',
     'sub_goal': None,
-    'image_urls': ['http://localhost:5667/api/step/34yixvic-0-1/image/0'],
+    'image_ids': ['34yixvic-0-1-0'],
     'images': [<PIL.JpegImagePlugin.JpegImageFile image mode=RGB size=600x400 at 0x7F8D33094450>]
 }
 ```
 
 - All the regular MLOps features are included, e.g. data visualization, simulation rendering, experiment management.
 
 # Installation
```

### Comparing `loopquest-0.2.5/README.md` & `loopquest-0.2.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     'reward': -0.00,
     'prev_observation': [-0.55, 0.00],
     'termnated': False,
     'truncated': False,
     'done': False,
     'info': '{}',
     'sub_goal': None,
-    'image_urls': ['http://localhost:5667/api/step/34yixvic-0-1/image/0'],
+    'image_ids': ['34yixvic-0-1-0'],
     'images': [<PIL.JpegImagePlugin.JpegImageFile image mode=RGB size=600x400 at 0x7F8D33094450>]
 }
 ```
 
 - All the regular MLOps features are included, e.g. data visualization, simulation rendering, experiment management.
 
 # Installation
```

### Comparing `loopquest-0.2.5/loopquest/api.py` & `loopquest-0.2.6/loopquest/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,15 @@
         return
     sign_in_url = f"{CLOUD_FRONTEND_URL}/token"
     print(
         f"Opening LoopQuest Sign-In page ... \nIf the browser does not open automatically, visit {sign_in_url} manually."
     )
     webbrowser.open_new(sign_in_url)
     while True:
-        token = getpass.getpass(
-            "Enter your LoopQuest user token (the token expires in 1 hour): "
-        ).strip()
+        token = getpass.getpass("Enter your LoopQuest user token: ").strip()
         if verify_token(token):
             print("Token is verified.")
             break
         else:
             print("Token is invalid. Please try again.")
 
     print(
```

### Comparing `loopquest-0.2.5/loopquest/crud.py` & `loopquest-0.2.6/loopquest/crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 def make_request(method: str, url: str, skip_auth_check=False, **kwargs):
     if not skip_auth_check:
         if TOKEN_ENV_VAR_NAME not in os.environ:
             raise Exception(
                 f"Please run loopquest.init() before calling other loopquest functions."
             )
         headers = kwargs.get("headers", {})
-        headers["Authorization"] = f"Bearer {os.getenv(TOKEN_ENV_VAR_NAME)}"
+        headers["Authorization"] = f"{os.getenv(TOKEN_ENV_VAR_NAME)}"
         kwargs["headers"] = headers
 
     try:
         response = requests.request(method, url, **kwargs)
         response.raise_for_status()
     except HTTPError as e:
         if e.response.status_code == 500:
@@ -58,15 +58,18 @@
     )
     res.raise_for_status()
 
 
 def create_environment(backend_url: str, env: gymnasium.Env, user_id: str) -> str:
     environment = EnvironmentCreate(
         id=replace_special_chars_with_dash(env.spec.id),
-        name=env.spec.id,
+        name=env.spec.name,
+        namespace=env.spec.namespace,
+        version=env.spec.version,
+        metadata=env.metadata,
         gym_id=env.spec.id,
         user_id=user_id,
         env_spec=str(env.spec),
         observation_metadata=create_var_tree(env.observation_space, name="Obs"),
         action_metadata=create_var_tree(env.action_space, name="Act"),
         is_legacy_gym=False,
     )
@@ -300,17 +303,23 @@
 
 def get_steps_by_experiment(backend_url: str, experiment_id: str):
     response = make_request("GET", f"{backend_url}/step/exp/{experiment_id}")
     steps = response.json()
     return [Step(**s) for s in steps]
 
 
-def get_image_by_url(image_url: str):
-    response = make_request("GET", image_url)
+def get_image_by_id(backend_url: str, id: str):
+    response = make_request("GET", f"{backend_url}/step/image/{id}")
     image = Image.open(BytesIO(response.content))
     return image
 
 
+def get_image_ids_by_step(backend_url: str, step_id: str):
+    response = make_request("GET", f"{backend_url}/step/{step_id}/image")
+    image_ids = response.json()
+    return image_ids
+
+
 def get_cloud_user_id(backend_url: str):
     response = make_request("GET", f"{backend_url}/user_id")
     user_id = response.json()
     return user_id["userId"]
```

### Comparing `loopquest-0.2.5/loopquest/datasets.py` & `loopquest-0.2.6/loopquest/datasets.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datasets import Dataset
-from .crud import get_steps_by_experiment, get_image_by_url
+from .crud import get_steps_by_experiment, get_image_by_id
 from .api import get_backend_url
 from .env.space_utils import recover_from_space_val
 from PIL import Image
 
 
 def dataset_gen(experiment_ids: list[str]):
     for experiment_id in experiment_ids:
@@ -15,18 +15,18 @@
             step_dict["observation"] = recover_from_space_val(step.observation)
             if step.action is not None:
                 step_dict["action"] = recover_from_space_val(step.action)
             yield step_dict
 
 
 def to_pilow(examples):
-    image_urls_across_examples = examples["image_urls"]
+    image_ids_across_examples = examples["image_ids"]
     images = [
-        [get_image_by_url(url) for url in image_urls]
-        for image_urls in image_urls_across_examples
+        [get_image_by_id(get_backend_url(), id) for id in image_ids]
+        for image_ids in image_ids_across_examples
     ]
     examples["images"] = images
     return examples
 
 
 # TODO: add environment info to the dataset so the foundation model training can
 # be conditioned on each of the environment.
```

### Comparing `loopquest-0.2.5/loopquest/env/api.py` & `loopquest-0.2.6/loopquest/env/api.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.5/loopquest/env/gym_wrappers.py` & `loopquest-0.2.6/loopquest/env/gym_wrappers.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import gymnasium
 from ..crud import (
     create_step,
     get_environment,
     update_environment,
     update_experiment,
     upload_rgb_as_image,
-    get_image_by_url,
+    get_image_ids_by_step,
 )
 from ..schema import StepCreate, ExperimentUpdate, ExperimentStatus, EnvironmentUpdate
 from ..utils import safe_jsonize
 from .space_utils import construct_space_val
 from ..api import get_backend_url
 from concurrent.futures import ThreadPoolExecutor
 
@@ -137,23 +137,25 @@
         self.env.close()
         self.executor.shutdown()
         # TODO: add a callback to compute custom metrics.
 
     def _try_update_env_profile_image(self):
         env_info = get_environment(self.backend_url, self.cloud_env_id)
         env_update = EnvironmentUpdate()
-        if env_info.profile_image is None:
-            step_id = f"{self.exp_id}-{self.cloud_env_id}-0-1"
-            image_url = self.backend_url + f"/step/{step_id}/image/0"
-            try:
-                img = get_image_by_url(image_url)
-                env_update.profile_image = f"{BLOB_URL_PREFIX}/{step_id}-0.jpg"
-            except Exception as e:
-                return
-        update_environment(self.backend_url, self.cloud_env_id, env_update)
+        if env_info.profile_image_id is None:
+            image_ids = get_image_ids_by_step(
+                self.backend_url, f"{self.exp_id}-{self.cloud_env_id}-0-1"
+            )
+            print(image_ids)
+            if len(image_ids) > 0:
+                print("Setting profile image for environment.")
+                env_update.profile_image_id = image_ids[0]
+                update_environment(self.backend_url, self.cloud_env_id, env_update)
+            else:
+                print("No image found for environment.")
 
     def render(self):
         if self.render_mode == "human":
             raise ValueError(
                 "'human' mode is not supported for cloud rendering. Please use other render mode."
             )
         elif self.render_mode in ["ansi", "ansi_list"]:
```

### Comparing `loopquest-0.2.5/loopquest/env/space_utils.py` & `loopquest-0.2.6/loopquest/env/space_utils.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.5/loopquest/eval.py` & `loopquest-0.2.6/loopquest/eval.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,17 +44,19 @@
     if all(["rgb_array" in env.metadata.get("render_modes", []) for env in gym_envs]):
         render_mode = "rgb_array"
     elif all(
         ["rgb_array_list" in env.metadata.get("render_modes", []) for env in gym_envs]
     ):
         render_mode = "rgb_array_list"
     else:
-        raise ValueError(
-            "All the environments must support rgb_array or rgb_array_list."
-        )
+        # raise ValueError(
+        #     "All the environments must support rgb_array or rgb_array_list."
+        # )
+        render_mode = None
+
     gym_envs = [gym.make(env_id, render_mode=render_mode) for env_id in env_ids]
 
     if project_name is None:
         project_name = generate_project_name()
 
     if experiment_name is None:
         experiment_name = generate_experiment_name()
@@ -101,15 +103,15 @@
                     backend_env_id,
                     experiment.id,
                     episode=eps,
                     use_thread_pool=use_thread_pool,
                     max_workers=max_workers,
                     backend_url=backend_url,
                 )
-                policy.set_action_space(env.action_space)
+                policy.set_env(env)
                 obs, info = env.reset()
                 for _ in tqdm(
                     range(num_steps_per_episode),
                     desc="Steps",
                     leave=False,
                     disable=disable_progress_bar,
                 ):
@@ -125,14 +127,15 @@
             backend_url,
             experiment.id,
             ExperimentUpdate(
                 status=ExperimentStatus.FAILED,
                 error_message=str(e),
             ),
         )
+        raise e
     return experiment.id, experiment.project_id
 
 
 # Only supports stable baseline3 policies in huggingface for now.
 def evaluate_remote_policy(
     huggingface_repo_id: str,
     huggingface_filename: str,
```

### Comparing `loopquest-0.2.5/loopquest/policy/sb3_policy.py` & `loopquest-0.2.6/loopquest/policy/sb3_policy.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.5/loopquest/private_api.py` & `loopquest-0.2.6/loopquest/private_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-import time
 import requests
 import os
-from .utils import update_or_append_env_var, is_docker_installed
+from .utils import update_or_append_env_var
 
 
 # For Dev
-# CLOUD_FRONTEND_URL = "http://localhost:5667"
-# CLOUD_BACKEND_URL = "http://localhost:5667/api"
+CLOUD_FRONTEND_URL = "http://localhost:3000"
+CLOUD_BACKEND_URL = "http://localhost:3000/api"
 
-CLOUD_FRONTEND_URL = "https://www.loopquest.ai"
-CLOUD_BACKEND_URL = "https://www.loopquest.ai/api"
+# CLOUD_FRONTEND_URL = "https://www.loopquest.ai"
+# CLOUD_BACKEND_URL = "https://www.loopquest.ai/api"
 TOKEN_ENV_VAR_NAME = "LOOPQUEST_USER_TOKEN"
 
 
 def is_cloud_instance_initialized():
     from .crud import get_cloud_user_id
 
     try:
@@ -22,15 +21,15 @@
     except Exception as e:
         return False
 
 
 def verify_token(token):
     try:
         response = requests.get(
-            f"{CLOUD_BACKEND_URL}/user_id", headers={"Authorization": f"Bearer {token}"}
+            f"{CLOUD_BACKEND_URL}/user_id", headers={"Authorization": f"{token}"}
         )
         response.raise_for_status()
         return True
     except:
         return False
```

### Comparing `loopquest-0.2.5/loopquest/schema.py` & `loopquest-0.2.6/loopquest/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,20 +37,23 @@
 
 class EnvironmentCreate(BaseModel):
     # This could be gym id, [namespace/](env-name)[-v(version)].
     id: str
     name: Optional[str] = ""
     # Created by this user.
     user_id: str
-    profile_image: Optional[str] = None
+    profile_image_id: Optional[str] = None
     gym_id: Optional[str] = None
     description: Optional[str] = None
     # JSON string of gym env spec
     # https://gymnasium.farama.org/api/registry/#gymnasium.envs.registration.EnvSpec
     env_spec: Optional[str] = None
+    namespace: Optional[str] = None
+    version: Optional[int] = None
+    metadata: Optional[Dict[str, Any]] = None
     # Multiple VectorSpecs are used to represent composite spaces, e.g. Dict,
     # Tuple, Sequence etc.
     action_metadata: Optional[VarNode] = None
     observation_metadata: Optional[VarNode] = None
     git_repo: Optional[str] = None
     support_remote_eval: Optional[bool] = False
 
@@ -143,15 +146,15 @@
     step: int
     # NOTE: observation and action are flattened into 1D arrays.
     observation: Optional[SpaceVal] = None
     action: Optional[SpaceVal] = None
     reward: Optional[float] = 0.0
     # This is potentially useful to train a policy conditioned on sub goals.
     sub_goal: Optional[Goal] = None
-    image_urls: Optional[List[str]] = []
+    image_ids: Optional[List[str]] = []
     termnated: Optional[bool] = False
     truncated: Optional[bool] = False
     # This is deprecated by Gymnasium, but we still keep it for backward
     # compatibility.
     done: Optional[bool] = False
     info: Optional[Dict[str, Any]] = None  # JSON string of step info
     human_score: Optional[int] = None
```

### Comparing `loopquest-0.2.5/loopquest/utils.py` & `loopquest-0.2.6/loopquest/utils.py`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.5/loopquest.egg-info/PKG-INFO` & `loopquest-0.2.6/loopquest.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loopquest
-Version: 0.2.5
+Version: 0.2.6
 Summary: A Production Tool for Embodied AI.
 Home-page: https://github.com/LoopMind-AI/loopquest
 Author: LoopMind
 Author-email: contactus@loopmind.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.11
@@ -139,15 +139,15 @@
     'reward': -0.00,
     'prev_observation': [-0.55, 0.00],
     'termnated': False,
     'truncated': False,
     'done': False,
     'info': '{}',
     'sub_goal': None,
-    'image_urls': ['http://localhost:5667/api/step/34yixvic-0-1/image/0'],
+    'image_ids': ['34yixvic-0-1-0'],
     'images': [<PIL.JpegImagePlugin.JpegImageFile image mode=RGB size=600x400 at 0x7F8D33094450>]
 }
 ```
 
 - All the regular MLOps features are included, e.g. data visualization, simulation rendering, experiment management.
 
 # Installation
```

### Comparing `loopquest-0.2.5/loopquest.egg-info/SOURCES.txt` & `loopquest-0.2.6/loopquest.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loopquest-0.2.5/setup.py` & `loopquest-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="loopquest",
-    version="0.2.5",
+    version="0.2.6",
     description="A Production Tool for Embodied AI.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="LoopMind",
     author_email="contactus@loopmind.ai",
     url="https://github.com/LoopMind-AI/loopquest",
     packages=find_packages(),
```

