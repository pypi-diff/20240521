# Comparing `tmp/mpspenv-0.1.0.tar.gz` & `tmp/mpspenv-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpspenv-0.1.0.tar", last modified: Mon May 20 17:36:35 2024, max compression
+gzip compressed data, was "mpspenv-0.1.1.tar", last modified: Tue May 21 08:50:14 2024, max compression
```

## Comparing `mpspenv-0.1.0.tar` & `mpspenv-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-20 17:36:35.404058 mpspenv-0.1.0/
--rw-r--r--   0 axelhojmark   (501) staff       (20)       19 2024-05-07 12:14:46.000000 mpspenv-0.1.0/MANIFEST.in
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-20 17:36:35.399380 mpspenv-0.1.0/MPSPEnv/
--rw-r--r--   0 axelhojmark   (501) staff       (20)       46 2024-05-17 13:25:45.000000 mpspenv-0.1.0/MPSPEnv/__init__.py
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-20 17:36:35.397675 mpspenv-0.1.0/MPSPEnv/c/
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-20 17:36:35.402848 mpspenv-0.1.0/MPSPEnv/c/src/
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3686 2024-05-20 17:10:52.000000 mpspenv-0.1.0/MPSPEnv/c/src/array.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      738 2024-05-20 17:18:13.000000 mpspenv-0.1.0/MPSPEnv/c/src/array.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     7721 2024-05-20 16:39:13.000000 mpspenv-0.1.0/MPSPEnv/c/src/bay.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      861 2024-05-20 12:41:08.000000 mpspenv-0.1.0/MPSPEnv/c/src/bay.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     9914 2024-05-20 17:22:44.000000 mpspenv-0.1.0/MPSPEnv/c/src/env.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      620 2024-05-20 17:04:20.000000 mpspenv-0.1.0/MPSPEnv/c/src/env.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1694 2024-05-20 16:47:49.000000 mpspenv-0.1.0/MPSPEnv/c/src/random.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      204 2024-05-20 16:48:38.000000 mpspenv-0.1.0/MPSPEnv/c/src/random.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1472 2024-05-20 16:30:09.000000 mpspenv-0.1.0/MPSPEnv/c/src/sort.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)      132 2024-01-16 19:28:34.000000 mpspenv-0.1.0/MPSPEnv/c/src/sort.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     6456 2024-05-20 17:06:41.000000 mpspenv-0.1.0/MPSPEnv/c/src/transportation_matrix.c
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1027 2024-05-20 17:05:53.000000 mpspenv-0.1.0/MPSPEnv/c/src/transportation_matrix.h
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1911 2024-05-20 17:05:13.000000 mpspenv-0.1.0/MPSPEnv/c_interface.py
--rw-r--r--   0 axelhojmark   (501) staff       (20)     7910 2024-05-20 17:21:01.000000 mpspenv-0.1.0/MPSPEnv/env.py
--rw-r--r--   0 axelhojmark   (501) staff       (20)     4927 2024-05-20 17:19:49.000000 mpspenv-0.1.0/MPSPEnv/visualizer.py
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-20 17:36:35.403661 mpspenv-0.1.0/MPSPEnv.egg-info/
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-20 17:36:35.000000 mpspenv-0.1.0/MPSPEnv.egg-info/PKG-INFO
--rw-r--r--   0 axelhojmark   (501) staff       (20)      570 2024-05-20 17:36:35.000000 mpspenv-0.1.0/MPSPEnv.egg-info/SOURCES.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)        1 2024-05-20 17:36:35.000000 mpspenv-0.1.0/MPSPEnv.egg-info/dependency_links.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)       31 2024-05-20 17:36:35.000000 mpspenv-0.1.0/MPSPEnv.egg-info/requires.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)        8 2024-05-20 17:36:35.000000 mpspenv-0.1.0/MPSPEnv.egg-info/top_level.txt
--rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-20 17:36:35.403861 mpspenv-0.1.0/PKG-INFO
--rw-r--r--   0 axelhojmark   (501) staff       (20)     2848 2024-05-20 11:08:18.000000 mpspenv-0.1.0/README.md
--rw-r--r--   0 axelhojmark   (501) staff       (20)       38 2024-05-20 17:36:35.404110 mpspenv-0.1.0/setup.cfg
--rw-r--r--   0 axelhojmark   (501) staff       (20)      890 2024-05-20 17:36:15.000000 mpspenv-0.1.0/setup.py
-drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-20 17:36:35.403134 mpspenv-0.1.0/tests/
--rw-r--r--   0 axelhojmark   (501) staff       (20)     1237 2024-05-20 11:15:35.000000 mpspenv-0.1.0/tests/test_env.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-21 08:50:14.407277 mpspenv-0.1.1/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       19 2024-05-07 12:14:46.000000 mpspenv-0.1.1/MANIFEST.in
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-21 08:50:14.402137 mpspenv-0.1.1/MPSPEnv/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       46 2024-05-17 13:25:45.000000 mpspenv-0.1.1/MPSPEnv/__init__.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-21 08:50:14.400768 mpspenv-0.1.1/MPSPEnv/c/
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-21 08:50:14.406239 mpspenv-0.1.1/MPSPEnv/c/src/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3686 2024-05-20 17:10:52.000000 mpspenv-0.1.1/MPSPEnv/c/src/array.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      738 2024-05-20 17:18:13.000000 mpspenv-0.1.1/MPSPEnv/c/src/array.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     7721 2024-05-20 16:39:13.000000 mpspenv-0.1.1/MPSPEnv/c/src/bay.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      861 2024-05-20 12:41:08.000000 mpspenv-0.1.1/MPSPEnv/c/src/bay.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)    10621 2024-05-21 08:48:12.000000 mpspenv-0.1.1/MPSPEnv/c/src/env.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      620 2024-05-20 17:04:20.000000 mpspenv-0.1.1/MPSPEnv/c/src/env.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1694 2024-05-20 16:47:49.000000 mpspenv-0.1.1/MPSPEnv/c/src/random.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      204 2024-05-20 16:48:38.000000 mpspenv-0.1.1/MPSPEnv/c/src/random.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1472 2024-05-20 16:30:09.000000 mpspenv-0.1.1/MPSPEnv/c/src/sort.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      132 2024-01-16 19:28:34.000000 mpspenv-0.1.1/MPSPEnv/c/src/sort.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     6456 2024-05-20 17:06:41.000000 mpspenv-0.1.1/MPSPEnv/c/src/transportation_matrix.c
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1027 2024-05-20 17:05:53.000000 mpspenv-0.1.1/MPSPEnv/c/src/transportation_matrix.h
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1911 2024-05-20 17:05:13.000000 mpspenv-0.1.1/MPSPEnv/c_interface.py
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     7910 2024-05-21 06:32:25.000000 mpspenv-0.1.1/MPSPEnv/env.py
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     4927 2024-05-20 17:19:49.000000 mpspenv-0.1.1/MPSPEnv/visualizer.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-21 08:50:14.406788 mpspenv-0.1.1/MPSPEnv.egg-info/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-21 08:50:14.000000 mpspenv-0.1.1/MPSPEnv.egg-info/PKG-INFO
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      570 2024-05-21 08:50:14.000000 mpspenv-0.1.1/MPSPEnv.egg-info/SOURCES.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)        1 2024-05-21 08:50:14.000000 mpspenv-0.1.1/MPSPEnv.egg-info/dependency_links.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       31 2024-05-21 08:50:14.000000 mpspenv-0.1.1/MPSPEnv.egg-info/requires.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)        8 2024-05-21 08:50:14.000000 mpspenv-0.1.1/MPSPEnv.egg-info/top_level.txt
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     3238 2024-05-21 08:50:14.407015 mpspenv-0.1.1/PKG-INFO
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     2848 2024-05-20 11:08:18.000000 mpspenv-0.1.1/README.md
+-rw-r--r--   0 axelhojmark   (501) staff       (20)       38 2024-05-21 08:50:14.407323 mpspenv-0.1.1/setup.cfg
+-rw-r--r--   0 axelhojmark   (501) staff       (20)      890 2024-05-21 08:49:38.000000 mpspenv-0.1.1/setup.py
+drwxr-xr-x   0 axelhojmark   (501) staff       (20)        0 2024-05-21 08:50:14.406492 mpspenv-0.1.1/tests/
+-rw-r--r--   0 axelhojmark   (501) staff       (20)     1826 2024-05-21 08:48:42.000000 mpspenv-0.1.1/tests/test_env.py
```

### Comparing `mpspenv-0.1.0/MPSPEnv/c/src/array.c` & `mpspenv-0.1.1/MPSPEnv/c/src/array.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/MPSPEnv/c/src/array.h` & `mpspenv-0.1.1/MPSPEnv/c/src/array.h`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/MPSPEnv/c/src/bay.c` & `mpspenv-0.1.1/MPSPEnv/c/src/bay.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/MPSPEnv/c/src/bay.h` & `mpspenv-0.1.1/MPSPEnv/c/src/bay.h`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/MPSPEnv/c/src/env.c` & `mpspenv-0.1.1/MPSPEnv/c/src/env.c`

 * *Files 6% similar despite different names*

```diff
@@ -76,21 +76,23 @@
     // [c0r1, c0r2, c0r3, …, c0rR, c1r1, c1r2, …, c2*C-1rR]
     int is_add = i < env.bay.C * env.bay.R;
     int column = (i / env.bay.R) % env.bay.C;
     int n_to_place = i % env.bay.R + 1;
     int n_of_type = env.T->matrix.values[env.T->last_non_zero_column];
     if (is_add)
     {
+        int non_zero = env.T->last_non_zero_column != -1;
         int no_column_overflow = n_to_place + containers_in_column(env.bay, column) <= env.bay.R;
         int not_more_than_type = n_of_type >= n_to_place;
         int add_to_the_left = column < *(env.bay.right_most_added_column);
         int not_traped = empty_spots_to_left + n_to_place >= n_of_type;
         int no_right_identical = !identical_columns.values[env.bay.C + column];
 
-        return (no_column_overflow &&
+        return (non_zero &&
+                no_column_overflow &&
                 not_more_than_type &&
                 add_to_the_left &&
                 not_traped &&
                 no_right_identical);
     }
     else
     {
@@ -217,17 +219,36 @@
 {
     if (is_container_blocking(env.bay, column, next_container))
         return -n_containers;
     else
         return 0;
 }
 
-int get_remove_reward(Env env, Array reshuffled)
+int get_remove_reward(Env env, int column, int n_containers)
 {
-    return -get_sum(reshuffled);
+    int reward = 0;
+    for (int n = 0; n < n_containers; n++)
+    {
+        int row = env.bay.R - env.bay.column_counts.values[column] + n;
+        int index = row * env.bay.C + column;
+        int container = env.bay.matrix.values[index];
+        int is_blocking = 0;
+        for (int offset = row + 1; offset < env.bay.R; offset++)
+        {
+            int next_container = env.bay.matrix.values[offset * env.bay.C + column];
+            if (next_container < container)
+            {
+                is_blocking = 1;
+                break;
+            }
+        }
+        if (!is_blocking)
+            reward -= 1;
+    }
+    return reward;
 }
 
 void handle_sailing(Env env)
 {
     while (no_containers_at_port(env.T) && !is_last_port(env.T))
     {
         transportation_sail_along(env.T);
@@ -260,17 +281,17 @@
 }
 
 int remove_container(Env env, int action)
 {
     int column = (action / env.bay.R) % env.bay.C;
     int n_containers = action % env.bay.R + 1;
     *env.containers_left += n_containers;
+    int reward = get_remove_reward(env, column, n_containers);
     Array reshuffled = bay_pop_containers(env.bay, column, n_containers);
     transportation_insert_reshuffled(env.T, reshuffled);
-    int reward = get_remove_reward(env, reshuffled);
 
     free_array(reshuffled);
     return reward;
 }
 
 int decide_is_terminated(Env env)
 {
@@ -296,13 +317,11 @@
     step_info.reward = step_action(env, action);
     step_info.is_terminal = decide_is_terminated(env);
     *env.total_reward += step_info.reward;
 
     insert_flat_T_matrix(env);
     int only_legal_action = insert_mask(env);
     if (env.auto_move && !step_info.is_terminal && only_legal_action != -1)
-    {
         return step(env, only_legal_action);
-    }
 
     return step_info;
 }
```

### Comparing `mpspenv-0.1.0/MPSPEnv/c/src/env.h` & `mpspenv-0.1.1/MPSPEnv/c/src/env.h`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/MPSPEnv/c/src/random.c` & `mpspenv-0.1.1/MPSPEnv/c/src/random.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/MPSPEnv/c/src/sort.c` & `mpspenv-0.1.1/MPSPEnv/c/src/sort.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/MPSPEnv/c/src/transportation_matrix.c` & `mpspenv-0.1.1/MPSPEnv/c/src/transportation_matrix.c`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/MPSPEnv/c/src/transportation_matrix.h` & `mpspenv-0.1.1/MPSPEnv/c/src/transportation_matrix.h`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/MPSPEnv/c_interface.py` & `mpspenv-0.1.1/MPSPEnv/c_interface.py`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/MPSPEnv/env.py` & `mpspenv-0.1.1/MPSPEnv/env.py`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/MPSPEnv/visualizer.py` & `mpspenv-0.1.1/MPSPEnv/visualizer.py`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/MPSPEnv.egg-info/PKG-INFO` & `mpspenv-0.1.1/MPSPEnv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MPSPEnv
-Version: 0.1.0
+Version: 0.1.1
 Summary: A reinforcement learning environment for the Multi Port Stowage Planning problem
 Author: Axel Højmark
 Author-email: axelhojmark@gmail.com
 Project-URL: Repository, https://github.com/hojmax/MPSPEnv
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 Requires-Dist: gymnasium
```

### Comparing `mpspenv-0.1.0/MPSPEnv.egg-info/SOURCES.txt` & `mpspenv-0.1.1/MPSPEnv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/PKG-INFO` & `mpspenv-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MPSPEnv
-Version: 0.1.0
+Version: 0.1.1
 Summary: A reinforcement learning environment for the Multi Port Stowage Planning problem
 Author: Axel Højmark
 Author-email: axelhojmark@gmail.com
 Project-URL: Repository, https://github.com/hojmax/MPSPEnv
 Description-Content-Type: text/markdown
 Requires-Dist: pygame
 Requires-Dist: gymnasium
```

### Comparing `mpspenv-0.1.0/README.md` & `mpspenv-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mpspenv-0.1.0/setup.py` & `mpspenv-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 )
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="MPSPEnv",
-    version="0.1.0",
+    version="0.1.1",
     author="Axel Højmark",
     author_email="axelhojmark@gmail.com",
     description="A reinforcement learning environment for the Multi Port Stowage Planning problem",
     long_description=long_description,
     long_description_content_type="text/markdown",
     ext_modules=[ext_modules],
     packages=["MPSPEnv"],
```

### Comparing `mpspenv-0.1.0/tests/test_env.py` & `mpspenv-0.1.1/tests/test_env.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pytest
 import subprocess
-from helpers import run_env_against_rollout, get_rollouts, recreate_env
+from helpers import *
 
 
 @pytest.fixture(scope="session", autouse=True)
 def build_env():
     subprocess.run("make build", shell=True)  # Setup
     yield
     subprocess.run("make clean", shell=True)  # Teardown
@@ -43,7 +43,27 @@
 def test_rollouts():
     rollouts = get_rollouts()
 
     for rollout in rollouts:
         env = recreate_env(rollout["settings"], rollout["seed"])
         run_env_against_rollout(env, rollout["states"])
         env.close()
+
+
+def test_quicktest():
+    episodes = 1000
+
+    for _ in range(episodes):
+        settings = get_random_settings()
+        seed = np.random.randint(0, 1000000)
+        initial_containers = get_initial_containers(settings, seed)
+        env = recreate_env(settings, seed)
+        additional_info = get_additional_env_info(env)
+
+        while not env.terminal:
+            sanity_check_env(env, **additional_info)
+            action = get_random_action(env.mask)
+            env.step(action)
+
+        sanity_check_env(env, **additional_info)
+        assert initial_containers - env.total_reward == env.containers_placed
+        env.close()
```

