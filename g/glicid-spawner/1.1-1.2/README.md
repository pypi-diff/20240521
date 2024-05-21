# Comparing `tmp/glicid_spawner-1.1.tar.gz` & `tmp/glicid_spawner-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glicid_spawner-1.1.tar", max compression
+gzip compressed data, was "glicid_spawner-1.2.tar", max compression
```

## Comparing `glicid_spawner-1.1.tar` & `glicid_spawner-1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1542 2024-03-22 19:01:18.304484 glicid_spawner-1.1/LICENSE.md
--rw-r--r--   0        0        0     1677 2024-03-22 19:01:18.304484 glicid_spawner-1.1/README.md
--rw-r--r--   0        0        0     2574 2024-03-22 19:01:18.304484 glicid_spawner-1.1/pyproject.toml
--rw-r--r--   0        0        0      175 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/__init__.py
--rw-r--r--   0        0        0     2036 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/form.py
--rw-r--r--   0        0        0     1851 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/micromamba.py
--rw-r--r--   0        0        0     1568 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/progress.py
--rw-r--r--   0        0        0     1113 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/resources.py
--rw-r--r--   0        0        0      837 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/singleuser.py
--rw-r--r--   0        0        0     4978 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/slurm.py
--rw-r--r--   0        0        0     3780 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/spawner.py
--rw-r--r--   0        0        0     1804 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/templates/slurm_script.jinja
--rw-r--r--   0        0        0      302 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/templates/spawner_form.jinja
--rw-r--r--   0        0        0      676 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/templates/static/style.css
--rw-r--r--   0        0        0      511 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/templates/views/chdir.jinja
--rw-r--r--   0        0        0      550 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/templates/views/envs.jinja
--rw-r--r--   0        0        0     2577 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/templates/views/resources.jinja
--rw-r--r--   0        0        0     6499 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/templates/views/slurm.jinja
--rw-r--r--   0        0        0      192 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/templates/views/username.jinja
--rw-r--r--   0        0        0      653 2024-03-22 19:01:18.308484 glicid_spawner-1.1/src/glicid_spawner/templates.py
--rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 glicid_spawner-1.1/PKG-INFO
+-rw-r--r--   0        0        0     1542 2024-05-21 15:52:53.292245 glicid_spawner-1.2/LICENSE.md
+-rw-r--r--   0        0        0     1677 2024-05-21 15:52:53.292245 glicid_spawner-1.2/README.md
+-rw-r--r--   0        0        0     2574 2024-05-21 15:55:38.140321 glicid_spawner-1.2/pyproject.toml
+-rw-r--r--   0        0        0      175 2024-05-21 15:52:53.296245 glicid_spawner-1.2/src/glicid_spawner/__init__.py
+-rw-r--r--   0        0        0     2036 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/form.py
+-rw-r--r--   0        0        0     1896 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/micromamba.py
+-rw-r--r--   0        0        0     1568 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/progress.py
+-rw-r--r--   0        0        0     1113 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/resources.py
+-rw-r--r--   0        0        0      837 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/singleuser.py
+-rw-r--r--   0        0        0     4982 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/slurm.py
+-rw-r--r--   0        0        0     3925 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/spawner.py
+-rw-r--r--   0        0        0     1853 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/templates/slurm_script.jinja
+-rw-r--r--   0        0        0      302 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/templates/spawner_form.jinja
+-rw-r--r--   0        0        0      676 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/templates/static/style.css
+-rw-r--r--   0        0        0      511 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/templates/views/chdir.jinja
+-rw-r--r--   0        0        0      550 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/templates/views/envs.jinja
+-rw-r--r--   0        0        0     2636 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/templates/views/resources.jinja
+-rw-r--r--   0        0        0     6499 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/templates/views/slurm.jinja
+-rw-r--r--   0        0        0      192 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/templates/views/username.jinja
+-rw-r--r--   0        0        0      653 2024-05-21 15:52:53.300245 glicid_spawner-1.2/src/glicid_spawner/templates.py
+-rw-r--r--   0        0        0     2467 1970-01-01 00:00:00.000000 glicid_spawner-1.2/PKG-INFO
```

### Comparing `glicid_spawner-1.1/LICENSE.md` & `glicid_spawner-1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `glicid_spawner-1.1/README.md` & `glicid_spawner-1.2/README.md`

 * *Files identical despite different names*

### Comparing `glicid_spawner-1.1/pyproject.toml` & `glicid_spawner-1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "glicid-spawner"
-version = "1.1"
+version = "1.2"
 description = "JupyterHub Batch Spawner for GLiCID"
 authors = ["Benoit Seignovert <benoit.seignovert@univ-nantes.fr>"]
 license = "BSD 3-Clause License"
 readme = "README.md"
 repository = "https://gitlab.univ-nantes.fr/glicid/jupyter/spawner"
 packages = [{ include = "glicid_spawner", from = "src"}]
 
@@ -86,15 +86,15 @@
 exclude_lines = [
     'def __repr__',
     'pragma: no cover',
     'raise NotImplementedError',
 ]
 
 [tool.tbump.version]
-current = "1.1"
+current = "1.2"
 regex = '(?P<major>\d+)\.(?P<patch>\d+)'
 
 [tool.tbump.git]
 message_template = "Bump to version {new_version}"
 tag_template = "v{new_version}"
 
 [[tool.tbump.file]]
```

### Comparing `glicid_spawner-1.1/src/glicid_spawner/form.py` & `glicid_spawner-1.2/src/glicid_spawner/form.py`

 * *Files identical despite different names*

### Comparing `glicid_spawner-1.1/src/glicid_spawner/micromamba.py` & `glicid_spawner-1.2/src/glicid_spawner/micromamba.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from pathlib import Path
 
 MICROMAMBA_ROOT = Path('/micromamba')  # default micromamba root location
 GLOBAL_USER = 'operator'
 
 MAMBA_ROOT_PREFIX = f'{MICROMAMBA_ROOT}/{GLOBAL_USER}'
 MAMBA_EXE = f'{MAMBA_ROOT_PREFIX}/bin/micromamba'
+MAMBA_USER_BASE = f'{MICROMAMBA_ROOT}/$USER'
 
 
 @dataclass
 class MicromambaEnv:
     """Generic micromamba environment."""
 
     scope: str
```

### Comparing `glicid_spawner-1.1/src/glicid_spawner/progress.py` & `glicid_spawner-1.2/src/glicid_spawner/progress.py`

 * *Files identical despite different names*

### Comparing `glicid_spawner-1.1/src/glicid_spawner/resources.py` & `glicid_spawner-1.2/src/glicid_spawner/resources.py`

 * *Files identical despite different names*

### Comparing `glicid_spawner-1.1/src/glicid_spawner/singleuser.py` & `glicid_spawner-1.2/src/glicid_spawner/singleuser.py`

 * *Files identical despite different names*

### Comparing `glicid_spawner-1.1/src/glicid_spawner/slurm.py` & `glicid_spawner-1.2/src/glicid_spawner/slurm.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def __init__(self, cluster, partition, hostname, state, cpus_state, memory_mb, gres):  # noqa: PLR0913
         self.cluster = cluster.strip()
         self.partition = partition.strip()
         self.hostname = hostname.strip()
         self.state = state.strip().lower()
         self.cpu = SlurmCpu(*re.findall(r'(\d+)/(\d+)/\d+/(\d+)', cpus_state)[0])
         self.mem = int(memory_mb) // 1000  # in GB
-        self.gpu = SlurmGpu(*re.findall(r'gpu:(\w+):(\d+)', gres)[0] if 'gpu:' in gres else [])
+        self.gpu = SlurmGpu(*re.findall(r'gpu:([\w\.]+):(\d+)', gres)[0] if 'gpu:' in gres else [])
 
     def __str__(self):
         return self.hostname
 
     def __eq__(self, other):
         return str(self) == str(other)
```

### Comparing `glicid_spawner-1.1/src/glicid_spawner/spawner.py` & `glicid_spawner-1.2/src/glicid_spawner/spawner.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,37 +5,42 @@
 import sys
 from pathlib import Path
 
 from batchspawner import JobStatus, SlurmSpawner
 from traitlets import Bool, Integer, Unicode, default
 
 from .form import options_form, options_from_form
-from .micromamba import MAMBA_EXE, MAMBA_ROOT_PREFIX
+from .micromamba import MAMBA_EXE, MAMBA_ROOT_PREFIX, MAMBA_USER_BASE
 from .progress import ElapseTime, get_progress
 from .templates import get_template_src
 
 SPAWNER_BIN = Path(sys.exec_prefix) / 'bin'
 
 
 class GlicidSpawner(SlurmSpawner):
     """Glicid SLURM Spawner."""
 
     batchspawner_singleuser_cmd = Unicode(
         'glicid-spawner-singleuser',
         help='Spawner singleuser command.',
     ).tag(config=True)
 
+    req_mamba_exe = Unicode(
+        MAMBA_EXE,
+        help='Micromamba global exe',
+    ).tag(config=True)
+
     req_mamba_root_prefix = Unicode(
         MAMBA_ROOT_PREFIX,
         help='Micromamba global root prefix',
     ).tag(config=True)
 
-    req_mamba_exe = Unicode(
-        MAMBA_EXE,
-        help='Micromamba global exe',
+    req_mamba_user_base = Unicode(
+        MAMBA_USER_BASE,
+        help='Micromamba user base prefix',
     ).tag(config=True)
 
     req_job_name = Unicode(
         'jupyterhub_glicid',
         help='SLURM job name',
     ).tag(config=True)
```

### Comparing `glicid_spawner-1.1/src/glicid_spawner/templates/slurm_script.jinja` & `glicid_spawner-1.2/src/glicid_spawner/templates/slurm_script.jinja`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 
     {# SLURM config -#}
     scontrol write batch_script ${SLURM_JOB_ID}{% if cluster %} --cluster={{cluster}}{% endif %} -;
 
     {# Micromamba config -#}
     export MAMBA_EXE={{mamba_exe}};
     export MAMBA_ROOT_PREFIX={{mamba_root_prefix}};
+    export PYTHONUSERBASE={{ mamba_user_base }};
     source $MAMBA_ROOT_PREFIX/etc/profile.d/micromamba.sh;
 
     {# Activate micromamba env requested by the user -#}
     micromamba activate {{ pyenv }};
     export JUPYTER_PATH={{ pyenv }}/share/jupyter;
 
     {# Prologue -#}
```

### Comparing `glicid_spawner-1.1/src/glicid_spawner/templates/static/style.css` & `glicid_spawner-1.2/src/glicid_spawner/templates/static/style.css`

 * *Files identical despite different names*

### Comparing `glicid_spawner-1.1/src/glicid_spawner/templates/views/envs.jinja` & `glicid_spawner-1.2/src/glicid_spawner/templates/views/envs.jinja`

 * *Files identical despite different names*

### Comparing `glicid_spawner-1.1/src/glicid_spawner/templates/views/resources.jinja` & `glicid_spawner-1.2/src/glicid_spawner/templates/views/resources.jinja`

 * *Files 13% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         <div class="col-sm-9">
             {%- for gpu, max_duration in gpus.items() -%}
             <div class="col-sm-2">
                 <input type="radio" name="gpu" id="gpu_{{gpu}}" value="{{gpu}}"
                     data-max-duration="{{max_duration}}"
                     {%- if loop.first %} checked{% endif %}>
                 <label for="gpu_{{gpu}}" class="btn btn-default btn-block">
-                    {{ gpu }}
+                    {{ gpu | replace("_"," ") | replace("."," ") | replace("gb","GB") }}
                 </label>
             </div>
             {% endfor -%}
         </div>
     </div>
 
 </div>
```

### Comparing `glicid_spawner-1.1/src/glicid_spawner/templates/views/slurm.jinja` & `glicid_spawner-1.2/src/glicid_spawner/templates/views/slurm.jinja`

 * *Files identical despite different names*

### Comparing `glicid_spawner-1.1/src/glicid_spawner/templates.py` & `glicid_spawner-1.2/src/glicid_spawner/templates.py`

 * *Files identical despite different names*

### Comparing `glicid_spawner-1.1/PKG-INFO` & `glicid_spawner-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glicid-spawner
-Version: 1.1
+Version: 1.2
 Summary: JupyterHub Batch Spawner for GLiCID
 Home-page: https://gitlab.univ-nantes.fr/glicid/jupyter/spawner
 License: BSD 3-Clause License
 Author: Benoit Seignovert
 Author-email: benoit.seignovert@univ-nantes.fr
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
```

