# Comparing `tmp/answerrocket_client-0.2.5.tar.gz` & `tmp/answerrocket_client-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "answerrocket_client-0.2.5.tar", last modified: Mon May 20 20:25:44 2024, max compression
+gzip compressed data, was "answerrocket_client-0.2.6.tar", last modified: Tue May 21 20:57:26 2024, max compression
```

## Comparing `answerrocket_client-0.2.5.tar` & `answerrocket_client-0.2.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:25:44.967934 answerrocket_client-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-20 20:25:44.967934 answerrocket_client-0.2.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:25:44.963934 answerrocket_client-0.2.5/answer_rocket/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/data.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:25:44.963934 answerrocket_client-0.2.5/answer_rocket/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/graphql/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    51671 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/graphql/sdk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/skill.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/answer_rocket/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:25:44.967934 answerrocket_client-0.2.5/answerrocket_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-20 20:25:44.000000 answerrocket_client-0.2.5/answerrocket_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-20 20:25:44.000000 answerrocket_client-0.2.5/answerrocket_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 20:25:44.000000 answerrocket_client-0.2.5/answerrocket_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 20:25:44.000000 answerrocket_client-0.2.5/answerrocket_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 20:25:44.000000 answerrocket_client-0.2.5/answerrocket_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 20:25:44.967934 answerrocket_client-0.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 20:25:44.967934 answerrocket_client-0.2.5/test/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-20 20:25:38.000000 answerrocket_client-0.2.5/test/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:57:26.564246 answerrocket_client-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-21 20:57:26.564246 answerrocket_client-0.2.6/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:57:26.560246 answerrocket_client-0.2.6/answer_rocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13583 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:57:26.560246 answerrocket_client-0.2.6/answer_rocket/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/graphql/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51799 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/graphql/sdk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/answer_rocket/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:57:26.564246 answerrocket_client-0.2.6/answerrocket_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-21 20:57:26.000000 answerrocket_client-0.2.6/answerrocket_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-21 20:57:26.000000 answerrocket_client-0.2.6/answerrocket_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:57:26.000000 answerrocket_client-0.2.6/answerrocket_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-21 20:57:26.000000 answerrocket_client-0.2.6/answerrocket_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 20:57:26.000000 answerrocket_client-0.2.6/answerrocket_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:57:26.564246 answerrocket_client-0.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:57:26.564246 answerrocket_client-0.2.6/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-21 20:57:22.000000 answerrocket_client-0.2.6/test/test_client.py
```

### Comparing `answerrocket_client-0.2.5/PKG-INFO` & `answerrocket_client-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket_client-0.2.5/answer_rocket/auth.py` & `answerrocket_client-0.2.6/answer_rocket/auth.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.5/answer_rocket/chat.py` & `answerrocket_client-0.2.6/answer_rocket/chat.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.5/answer_rocket/client.py` & `answerrocket_client-0.2.6/answer_rocket/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.5/answer_rocket/config.py` & `answerrocket_client-0.2.6/answer_rocket/config.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.5/answer_rocket/data.py` & `answerrocket_client-0.2.6/answer_rocket/data.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.5/answer_rocket/graphql/client.py` & `answerrocket_client-0.2.6/answer_rocket/graphql/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.5/answer_rocket/graphql/schema.py` & `answerrocket_client-0.2.6/answer_rocket/graphql/schema.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,17 +325,18 @@
     last_modified_utc = sgqlc.types.Field(sgqlc.types.non_null(DateTime), graphql_name='lastModifiedUtc')
     version = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='version')
     is_deleted = sgqlc.types.Field(sgqlc.types.non_null(Boolean), graphql_name='isDeleted')
 
 
 class MaxCopilotSkill(sgqlc.types.Type):
     __schema__ = schema
-    __field_names__ = ('copilot_skill_id', 'name', 'detailed_name', 'description', 'detailed_description', 'dataset_id', 'skill_chat_questions', 'yaml_code', 'skill_code', 'misc_info', 'scheduling_only', 'copilot_skill_nodes')
+    __field_names__ = ('copilot_skill_id', 'name', 'copilot_skill_type', 'detailed_name', 'description', 'detailed_description', 'dataset_id', 'skill_chat_questions', 'yaml_code', 'skill_code', 'misc_info', 'scheduling_only', 'copilot_skill_nodes')
     copilot_skill_id = sgqlc.types.Field(sgqlc.types.non_null(UUID), graphql_name='copilotSkillId')
     name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='name')
+    copilot_skill_type = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='copilotSkillType')
     detailed_name = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='detailedName')
     description = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='description')
     detailed_description = sgqlc.types.Field(String, graphql_name='detailedDescription')
     dataset_id = sgqlc.types.Field(UUID, graphql_name='datasetId')
     skill_chat_questions = sgqlc.types.Field(sgqlc.types.non_null(sgqlc.types.list_of('MaxCopilotSkillChatQuestion')), graphql_name='skillChatQuestions')
     yaml_code = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='yamlCode')
     skill_code = sgqlc.types.Field(sgqlc.types.non_null(String), graphql_name='skillCode')
```

### Comparing `answerrocket_client-0.2.5/answer_rocket/graphql/sdk_operations.py` & `answerrocket_client-0.2.6/answer_rocket/graphql/sdk_operations.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.5/answer_rocket/output.py` & `answerrocket_client-0.2.6/answer_rocket/output.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.5/answer_rocket/skill.py` & `answerrocket_client-0.2.6/answer_rocket/skill.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.5/answerrocket_client.egg-info/PKG-INFO` & `answerrocket_client-0.2.6/answerrocket_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket_client-0.2.5/answerrocket_client.egg-info/SOURCES.txt` & `answerrocket_client-0.2.6/answerrocket_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.5/readme.md` & `answerrocket_client-0.2.6/readme.md`

 * *Files identical despite different names*

