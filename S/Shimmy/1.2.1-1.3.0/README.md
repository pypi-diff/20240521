# Comparing `tmp/Shimmy-1.2.1.tar.gz` & `tmp/Shimmy-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shimmy-1.2.1.tar", last modified: Fri Jul 21 06:25:07 2023, max compression
+gzip compressed data, was "Shimmy-1.3.0.tar", last modified: Tue Oct 17 19:21:27 2023, max compression
```

## Comparing `Shimmy-1.2.1.tar` & `Shimmy-1.3.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:25:07.895684 Shimmy-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 06:25:07.895684 Shimmy-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-07-21 06:24:58.000000 Shimmy-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:25:07.891684 Shimmy-1.2.1/Shimmy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-07-21 06:25:07.000000 Shimmy-1.2.1/Shimmy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-21 06:25:07.000000 Shimmy-1.2.1/Shimmy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 06:25:07.000000 Shimmy-1.2.1/Shimmy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-21 06:25:07.000000 Shimmy-1.2.1/Shimmy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-21 06:25:07.000000 Shimmy-1.2.1/Shimmy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-21 06:25:07.000000 Shimmy-1.2.1/Shimmy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-21 06:24:58.000000 Shimmy-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 06:25:07.895684 Shimmy-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-07-21 06:24:58.000000 Shimmy-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:25:07.891684 Shimmy-1.2.1/shimmy/
--rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16080 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/atari_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/bsuite_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     8962 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/dm_control_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/dm_control_multiagent_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/dm_lab_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)     8687 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/meltingpot_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    11159 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/openai_gym_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    17283 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/openspiel_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10209 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/registration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:25:07.895684 Shimmy-1.2.1/shimmy/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/utils/dm_control_multiagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/utils/dm_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     4735 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/utils/dm_lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     5752 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/utils/envs_configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-07-21 06:24:58.000000 Shimmy-1.2.1/shimmy/utils/meltingpot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 06:25:07.895684 Shimmy-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_atari.py
--rw-r--r--   0 runner    (1001) docker     (123)     8175 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_bsuite.py
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_dm_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     6408 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_dm_control_multi_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3502 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_dm_lab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     5241 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_meltingpot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7420 2023-07-21 06:24:58.000000 Shimmy-1.2.1/tests/test_openspiel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 19:21:27.839989 Shimmy-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2023-10-17 19:21:27.839989 Shimmy-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6538 2023-10-17 19:21:16.000000 Shimmy-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 19:21:27.831989 Shimmy-1.3.0/Shimmy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2023-10-17 19:21:27.000000 Shimmy-1.3.0/Shimmy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2023-10-17 19:21:27.000000 Shimmy-1.3.0/Shimmy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-17 19:21:27.000000 Shimmy-1.3.0/Shimmy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2023-10-17 19:21:27.000000 Shimmy-1.3.0/Shimmy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2023-10-17 19:21:27.000000 Shimmy-1.3.0/Shimmy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2023-10-17 19:21:27.000000 Shimmy-1.3.0/Shimmy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2023-10-17 19:21:16.000000 Shimmy-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-17 19:21:27.839989 Shimmy-1.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2023-10-17 19:21:16.000000 Shimmy-1.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 19:21:27.831989 Shimmy-1.3.0/shimmy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2763 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16080 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/atari_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3368 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/bsuite_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9163 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/dm_control_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/dm_control_multiagent_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6942 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/dm_lab_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8858 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/meltingpot_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/openai_gym_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17283 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/openspiel_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/registration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 19:21:27.835989 Shimmy-1.3.0/shimmy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/utils/dm_control_multiagent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/utils/dm_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4735 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/utils/dm_lab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5752 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/utils/envs_configs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2023-10-17 19:21:16.000000 Shimmy-1.3.0/shimmy/utils/meltingpot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-17 19:21:27.835989 Shimmy-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3729 2023-10-17 19:21:16.000000 Shimmy-1.3.0/tests/test_atari.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8175 2023-10-17 19:21:16.000000 Shimmy-1.3.0/tests/test_bsuite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2023-10-17 19:21:16.000000 Shimmy-1.3.0/tests/test_dm_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6408 2023-10-17 19:21:16.000000 Shimmy-1.3.0/tests/test_dm_control_multi_agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3502 2023-10-17 19:21:16.000000 Shimmy-1.3.0/tests/test_dm_lab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3926 2023-10-17 19:21:16.000000 Shimmy-1.3.0/tests/test_gym.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2023-10-17 19:21:16.000000 Shimmy-1.3.0/tests/test_meltingpot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2023-10-17 19:21:16.000000 Shimmy-1.3.0/tests/test_openspiel.py
```

### Comparing `Shimmy-1.2.1/README.md` & `Shimmy-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/Shimmy.egg-info/SOURCES.txt` & `Shimmy-1.3.0/Shimmy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/pyproject.toml` & `Shimmy-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/setup.py` & `Shimmy-1.3.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         "dm-control>=1.0.10",
         "imageio",
         "h5py>=3.7.0",
         "pettingzoo>=1.23",
     ],
     "dm-lab": ["dm-env>=1.6"],
     "openspiel": ["open_spiel>=1.2", "pettingzoo>=1.23"],
-    "meltingpot": ["pettingzoo>=1.23"],
+    "meltingpot": ["pettingzoo>=1.23", "dm-meltingpot>=2.2.0; python_version > '3.9'"],
     "bsuite": ["bsuite>=0.3.5"],
 }
 extras["all"] = [
     lib for key, libs in extras.items() if key != "gym-v21" for lib in libs
 ]
 extras["testing"] = [
     "pytest==7.1.3",
```

### Comparing `Shimmy-1.2.1/shimmy/__init__.py` & `Shimmy-1.3.0/shimmy/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
     "DmLabCompatibilityV0",
     "GymV21CompatibilityV0",
     "GymV26CompatibilityV0",
     "MeltingPotCompatibilityV0",
 ]
 
 
-__version__ = "1.2.1"
+__version__ = "1.3.0"
 
 
 try:
     import sys
 
     from farama_notifications import notifications
```

### Comparing `Shimmy-1.2.1/shimmy/atari_env.py` & `Shimmy-1.3.0/shimmy/atari_env.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/shimmy/bsuite_compatibility.py` & `Shimmy-1.3.0/shimmy/bsuite_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/shimmy/dm_control_compatibility.py` & `Shimmy-1.3.0/shimmy/dm_control_compatibility.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,20 @@
         super().reset(seed=seed)
         if seed is not None:
             self.np_random = np.random.RandomState(seed=seed)
 
         timestep = self._env.reset()
         obs, reward, terminated, truncated, info = dm_env_step2gym_step(timestep)
 
+        if self.render_mode == "human":
+            self.viewer.close()
+            self.viewer = MujocoRenderer(
+                self._env.physics.model.ptr, self._env.physics.data.ptr
+            )
+
         return obs, info
 
     def step(
         self, action: np.ndarray
     ) -> tuple[ObsType, float, bool, bool, dict[str, Any]]:
         """Steps through the dm-control environment."""
         timestep = self._env.step(action)
```

### Comparing `Shimmy-1.2.1/shimmy/dm_control_multiagent_compatibility.py` & `Shimmy-1.3.0/shimmy/dm_control_multiagent_compatibility.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Wrapper to convert a dm_env multiagent environment into a pettingzoo compatible environment."""
 from __future__ import annotations
 
 import functools
-from itertools import repeat
 from typing import TYPE_CHECKING, Any
 
 import dm_control.composer
 import dm_env
 import gymnasium
 import numpy as np
 from gymnasium.envs.mujoco.mujoco_rendering import MujocoRenderer
@@ -39,35 +38,38 @@
             term = True
 
     # expand the observations
     list_observations = [dm_obs2gym_obs(obs) for obs in timestep.observation]
     observations: dict[AgentID, Any] = dict(zip(agents, list_observations))
 
     # sometimes deepmind decides not to reward people
-    rewards: dict[AgentID, float] = dict(zip(agents, repeat(0.0)))
+    rewards: dict[AgentID, float] = {agent: 0.0 for agent in agents}
+
     if timestep.reward:
         rewards = dict(zip(agents, timestep.reward))
 
     # expand everything else
-    terminations: dict[AgentID, bool] = dict(zip(agents, repeat(term)))
-    truncations: dict[AgentID, bool] = dict(zip(agents, repeat(trunc)))
+    terminations: dict[AgentID, bool] = {agent: term for agent in agents}
+    truncations: dict[AgentID, bool] = {agent: trunc for agent in agents}
 
-    # duplicate infos
-    info = {
-        "timestep.discount": timestep.discount,
-        "timestep.step_type": timestep.step_type,
+    # duplicate infos across agents
+    infos = {
+        agent: {
+            "timestep.discount": timestep.discount,
+            "timestep.step_type": timestep.step_type,
+        }
+        for agent in agents
     }
-    info: dict[AgentID, Any] = dict(zip(agents, repeat(info)))
 
     return (
         observations,
         rewards,
         terminations,
         truncations,
-        info,
+        infos,
     )
 
 
 class DmControlMultiAgentCompatibilityV0(ParallelEnv, EzPickle):
     """This compatibility wrapper converts multi-agent dm-control environments, primarily soccer, into a PettingZoo environment.
 
     Dm-control is DeepMind's software stack for physics-based simulation and Reinforcement Learning environments,
@@ -232,14 +234,20 @@
         self.agents = self.possible_agents[:]
         self.num_moves = 0
 
         self._env._random_state = np.random.RandomState(seed)
         timestep = self._env.reset()
         observations, _, _, _, info = _unravel_ma_timestep(timestep, self.agents)
 
+        if self.render_mode == "human":
+            self.viewer.close()
+            self.viewer = MujocoRenderer(
+                self._env.physics.model.ptr, self._env.physics.data.ptr
+            )
+
         return observations, info
 
     def step(
         self, actions: ActionDict
     ) -> tuple[
         ObsDict,
         dict[AgentID, float],
```

### Comparing `Shimmy-1.2.1/shimmy/dm_lab_compatibility.py` & `Shimmy-1.3.0/shimmy/dm_lab_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/shimmy/meltingpot_compatibility.py` & `Shimmy-1.3.0/shimmy/meltingpot_compatibility.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,27 +4,29 @@
 https://github.com/deepmind/meltingpot/blob/main/examples/pettingzoo/utils.py
 and modified to modern PettingZoo API
 """
 # pyright: reportOptionalSubscript=false
 from __future__ import annotations
 
 import functools
+from itertools import repeat
 from typing import TYPE_CHECKING, Any, Optional
 
 import dm_env
 import gymnasium
 import numpy as np
 import pygame
 from gymnasium.utils.ezpickle import EzPickle
 from pettingzoo.utils.env import ActionDict, AgentID, ObsDict, ParallelEnv
 
 import shimmy.utils.meltingpot as utils
 
 if TYPE_CHECKING:
-    import meltingpot.python
+    import meltingpot
+    from meltingpot.utils.substrates import substrate
 
 
 class MeltingPotCompatibilityV0(ParallelEnv, EzPickle):
     """This compatibility wrapper converts a Melting Pot substrate into a PettingZoo environment.
 
     Due to how the underlying environment is set up, this environment is nondeterministic, so seeding doesn't work.
 
@@ -42,23 +44,23 @@
     }
 
     PLAYER_STR_FORMAT = "player_{index}"
     MAX_CYCLES = 1000
 
     def __init__(
         self,
-        env: meltingpot.python.utils.substrates.substrate.Substrate | None = None,
+        env: substrate.Substrate | None = None,
         substrate_name: str | None = None,
         max_cycles: int = MAX_CYCLES,
         render_mode: str | None = None,
     ):
         """Wrapper that converts a Melting Pot environment into a PettingZoo environment.
 
         Args:
-            env (Optional[meltingpot.python.utils.substrates.substrate.Substrate]): existing Melting Pot environment to wrap
+            env (Optional[substrate.Substrate]): existing Melting Pot environment to wrap
             substrate_name (Optional[str]): name of Melting Pot substrate to load (instead of existing environment)
             max_cycles (Optional[int]): maximum number of cycles before truncation
             render_mode (Optional[str]): rendering mode
         """
         EzPickle.__init__(
             self,
             env,
@@ -154,15 +156,15 @@
         """
         return self._env.observation()
 
     def reset(
         self,
         seed: int | None = None,
         options: dict | None = None,
-    ) -> tuple[ObsDict, dict[str, Any]]:
+    ) -> tuple[ObsDict, dict[AgentID, Any]]:
         """reset.
 
         Resets the environment.
 
         Args:
             seed: the seed to reset the environment with (not used, due to nondeterministic underlying environment)
             options: the options to reset the environment with
@@ -172,19 +174,25 @@
         """
         timestep: dm_env.TimeStep = self._env.reset()
         self.agents = self.possible_agents[:]
         self.num_cycles = 0
 
         observations = utils.timestep_to_observations(timestep)
 
-        return observations, {
-            "step-type": timestep.step_type,
-            "discount": timestep.discount,
+        # duplicate infos across agents
+        infos = {
+            agent: {
+                "timestep.discount": timestep.discount,
+                "timestep.step_type": timestep.step_type,
+            }
+            for agent in self.agents
         }
 
+        return observations, infos
+
     def step(
         self, actions: ActionDict
     ) -> tuple[
         ObsDict, dict[str, float], dict[str, bool], dict[str, bool], dict[str, dict]
     ]:
         """step.
```

### Comparing `Shimmy-1.2.1/shimmy/openai_gym_compatibility.py` & `Shimmy-1.3.0/shimmy/openai_gym_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/shimmy/openspiel_compatibility.py` & `Shimmy-1.3.0/shimmy/openspiel_compatibility.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/shimmy/registration.py` & `Shimmy-1.3.0/shimmy/registration.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/shimmy/utils/dm_control_multiagent.py` & `Shimmy-1.3.0/shimmy/utils/dm_control_multiagent.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/shimmy/utils/dm_env.py` & `Shimmy-1.3.0/shimmy/utils/dm_env.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/shimmy/utils/dm_lab.py` & `Shimmy-1.3.0/shimmy/utils/dm_lab.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/shimmy/utils/envs_configs.py` & `Shimmy-1.3.0/shimmy/utils/envs_configs.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/shimmy/utils/meltingpot.py` & `Shimmy-1.3.0/shimmy/utils/meltingpot.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,34 +14,30 @@
 def load_meltingpot(substrate_name: str):
     """Helper function to load Melting Pot substrates.
 
     Args:
         substrate_name: str
 
     Returns:
-        env: meltingpot.python.utils.substrates.substrate.Substrate
+        env: meltingpot.utils.substrates.substrate.Substrate
     """
-    import meltingpot.python
+    import meltingpot
     from ml_collections import config_dict
 
     # Create env config
     substrate_name = substrate_name
-    player_roles = meltingpot.python.substrate.get_config(
-        substrate_name
-    ).default_player_roles
+    player_roles = meltingpot.substrate.get_config(substrate_name).default_player_roles
     env_config = {
         "substrate": substrate_name,
         "roles": player_roles,
     }
 
     # Build substrate from pickle
     env_config = config_dict.ConfigDict(env_config)
-    env = meltingpot.python.substrate.build(
-        env_config["substrate"], roles=env_config["roles"]
-    )
+    env = meltingpot.substrate.build(env_config["substrate"], roles=env_config["roles"])
     return env
 
 
 def timestep_to_observations(timestep: dm_env.TimeStep) -> ObsDict:
     """Extracts Gymnasium-compatible observations from a Melting Pot timestep.
 
     Args:
```

### Comparing `Shimmy-1.2.1/tests/test_atari.py` & `Shimmy-1.3.0/tests/test_atari.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/tests/test_bsuite.py` & `Shimmy-1.3.0/tests/test_bsuite.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/tests/test_dm_control.py` & `Shimmy-1.3.0/tests/test_dm_control.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/tests/test_dm_control_multi_agent.py` & `Shimmy-1.3.0/tests/test_dm_control_multi_agent.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/tests/test_dm_lab.py` & `Shimmy-1.3.0/tests/test_dm_lab.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/tests/test_gym.py` & `Shimmy-1.3.0/tests/test_gym.py`

 * *Files identical despite different names*

### Comparing `Shimmy-1.2.1/tests/test_meltingpot.py` & `Shimmy-1.3.0/tests/test_meltingpot.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 
 import pytest
 from gymnasium.utils.env_checker import data_equivalence
 from pettingzoo.test import parallel_api_test
 
 pytest.importorskip("meltingpot")
 
-import meltingpot.python
-from meltingpot.python.configs.substrates import SUBSTRATES
+import meltingpot
+from meltingpot.substrate import SUBSTRATES
 
 from shimmy.meltingpot_compatibility import MeltingPotCompatibilityV0
 from shimmy.utils.meltingpot import load_meltingpot
 
 
 @pytest.mark.parametrize("substrate_name", SUBSTRATES)
 def test_loading_env(substrate_name):
```

### Comparing `Shimmy-1.2.1/tests/test_openspiel.py` & `Shimmy-1.3.0/tests/test_openspiel.py`

 * *Files identical despite different names*

