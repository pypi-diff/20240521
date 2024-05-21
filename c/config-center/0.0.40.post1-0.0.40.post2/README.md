# Comparing `tmp/config_center-0.0.40.post1.tar.gz` & `tmp/config_center-0.0.40.post2.tar.gz`

## Comparing `config_center-0.0.40.post1.tar` & `config_center-0.0.40.post2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/MAINFEST.in
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/readme.md
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/test.py
--rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/.idea/.gitignore
--rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/.idea/config-center.iml
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/.idea/misc.xml
--rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/.idea/modules.xml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/.idea/vcs.xml
--rw-r--r--   0        0        0     8018 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/cfgc/__init__.py
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/cfgc/center.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/cfgc/envs/__init__.py
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/LICENSE.txt
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/README.md
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/pyproject.toml
--rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 config_center-0.0.40.post1/PKG-INFO
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/MAINFEST.in
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/readme.md
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/test.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/.idea/.gitignore
+-rw-r--r--   0        0        0      330 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/.idea/config-center.iml
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/.idea/misc.xml
+-rw-r--r--   0        0        0      285 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/.idea/modules.xml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/.idea/vcs.xml
+-rw-r--r--   0        0        0     8554 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/cfgc/__init__.py
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/cfgc/center.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/cfgc/envs/__init__.py
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/LICENSE.txt
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/README.md
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/pyproject.toml
+-rw-r--r--   0        0        0     2652 2020-02-02 00:00:00.000000 config_center-0.0.40.post2/PKG-INFO
```

### Comparing `config_center-0.0.40.post1/readme.md` & `config_center-0.0.40.post2/readme.md`

 * *Files identical despite different names*

### Comparing `config_center-0.0.40.post1/test.py` & `config_center-0.0.40.post2/test.py`

 * *Files identical despite different names*

### Comparing `config_center-0.0.40.post1/.idea/workspace.xml` & `config_center-0.0.40.post2/.idea/workspace.xml`

 * *Files 5% similar despite different names*

#### Comparing `config_center-0.0.40.post1/.idea/workspace.xml` & `config_center-0.0.40.post2/.idea/workspace.xml`

```diff
@@ -1,11 +1,15 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="ChangeListManager">
     <list default="true" id="3aef8cc2-14b5-468e-8927-eb128873056f" name="默认变更列表" comment="building... 🏗️">
+      <change beforePath="$PROJECT_DIR$/cfgc/__init__.py" beforeDir="false" afterPath="$PROJECT_DIR$/cfgc/__init__.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/cfgc/center.py" beforeDir="false" afterPath="$PROJECT_DIR$/cfgc/center.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/dist/config_center-0.0.40-py3-none-any.whl" beforeDir="false"/>
+      <change beforePath="$PROJECT_DIR$/dist/config_center-0.0.40.tar.gz" beforeDir="false"/>
       <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
@@ -75,14 +79,15 @@
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1716036017945</updated>
       <workItem from="1716036020520" duration="187000"/>
       <workItem from="1716036371070" duration="1933000"/>
       <workItem from="1716102721317" duration="114000"/>
       <workItem from="1716104323900" duration="804000"/>
+      <workItem from="1716258326544" duration="42000"/>
     </task>
     <task id="LOCAL-00001" summary="building... 🏗️">
       <created>1716036119683</created>
       <option name="number" value="00001"/>
       <option name="presentableId" value="LOCAL-00001"/>
       <option name="project" value="LOCAL"/>
       <updated>1716036119683</updated>
```

### Comparing `config_center-0.0.40.post1/cfgc/__init__.py` & `config_center-0.0.40.post2/cfgc/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,8 +8,9 @@
  │ Description:
     Default import conts
 """  # [By: HuYw]
 
 # region |- Import -|
 from . import center
 from . import envs
+from .center import *
 # endregion
```

### Comparing `config_center-0.0.40.post1/cfgc/center.py` & `config_center-0.0.40.post2/cfgc/center.py`

 * *Files identical despite different names*

### Comparing `config_center-0.0.40.post1/cfgc/envs/__init__.py` & `config_center-0.0.40.post2/cfgc/envs/__init__.py`

 * *Files identical despite different names*

### Comparing `config_center-0.0.40.post1/LICENSE.txt` & `config_center-0.0.40.post2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `config_center-0.0.40.post1/README.md` & `config_center-0.0.40.post2/README.md`

 * *Files identical despite different names*

### Comparing `config_center-0.0.40.post1/pyproject.toml` & `config_center-0.0.40.post2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "hatchling.build"
 
 [tool.hatch.build.targets.wheel]
 packages = ["cfgc"]
 
 [project] 
 name = "config-center"
-version = "0.0.40-1"
+version = "0.0.40-2"
 keywords = ["config", "pipeline", "local", "tool"]
 description = "A site-package to create your local pypi-sitepackage, manage your own scripts pack as an env!"
 readme = "README.md"
 license = {text = "MIT License"}
 requires-python = ">= 3.4"
 dependencies = [
   "importlib",
```

### Comparing `config_center-0.0.40.post1/PKG-INFO` & `config_center-0.0.40.post2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: config-center
-Version: 0.0.40.post1
+Version: 0.0.40.post2
 Summary: A site-package to create your local pypi-sitepackage, manage your own scripts pack as an env!
 Project-URL: Repository, https://github.com/WhatMelonGua/config-center
 Author-email: VaterFus <1107818699@qq.com>
 License: MIT License
 License-File: LICENSE.txt
 Keywords: config,local,pipeline,tool
 Requires-Python: >=3.4
```

