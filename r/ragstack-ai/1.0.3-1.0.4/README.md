# Comparing `tmp/ragstack_ai-1.0.3.tar.gz` & `tmp/ragstack_ai-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ragstack_ai-1.0.3.tar", max compression
+gzip compressed data, was "ragstack_ai-1.0.4.tar", max compression
```

## Comparing `ragstack_ai-1.0.3.tar` & `ragstack_ai-1.0.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     3781 2024-05-13 16:48:14.666685 ragstack_ai-1.0.3/LICENSE.md
--rw-r--r--   0        0        0     2395 2024-05-13 16:48:14.666685 ragstack_ai-1.0.3/PACKAGE_README.md
--rw-r--r--   0        0        0     1794 2024-05-13 16:48:14.694685 ragstack_ai-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      271 2024-05-13 16:48:14.694685 ragstack_ai-1.0.3/ragstack/__init__.py
--rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 ragstack_ai-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     3781 2024-05-21 20:21:58.965071 ragstack_ai-1.0.4/LICENSE.md
+-rw-r--r--   0        0        0     2395 2024-05-21 20:21:58.965071 ragstack_ai-1.0.4/PACKAGE_README.md
+-rw-r--r--   0        0        0     1796 2024-05-21 20:21:58.993070 ragstack_ai-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0      271 2024-05-21 20:21:58.993070 ragstack_ai-1.0.4/ragstack/__init__.py
+-rw-r--r--   0        0        0     3207 1970-01-01 00:00:00.000000 ragstack_ai-1.0.4/PKG-INFO
```

### Comparing `ragstack_ai-1.0.3/LICENSE.md` & `ragstack_ai-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ragstack_ai-1.0.3/PACKAGE_README.md` & `ragstack_ai-1.0.4/PACKAGE_README.md`

 * *Files identical despite different names*

### Comparing `ragstack_ai-1.0.3/pyproject.toml` & `ragstack_ai-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "ragstack-ai"
-version = "1.0.3"
+version = "1.0.4"
 description = "DataStax RAGStack"
 license = "BUSL-1.1"
 authors = ["DataStax"]
 readme = "PACKAGE_README.md"
 repository = "https://github.com/datastax/ragstack-ai"
 documentation = "https://docs.datastax.com/en/ragstack"
 packages = [{ include = "ragstack" }]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
-ragstack-ai-langchain = { version = "1.0.3", extras = ["colbert", "google", "nvidia"] }
-ragstack-ai-llamaindex = { version = "1.0.2", extras = ["colbert", "google", "azure", "bedrock"] }
-ragstack-ai-colbert = "1.0.2"
+ragstack-ai-langchain = { version = "1.0.4", extras = ["colbert", "google", "nvidia"] }
+ragstack-ai-llamaindex = { version = "1.0.3", extras = ["colbert", "google", "azure", "bedrock"] }
+ragstack-ai-colbert = "1.0.3"
 
 [tool.poetry.group.test.dependencies]
 ragstack-ai-langchain = { path = "libs/langchain", develop = true, extras = ["colbert", "google", "nvidia"] }
 ragstack-ai-llamaindex = { path = "libs/llamaindex", develop = true, extras = ["colbert", "google", "azure", "bedrock"] }
 ragstack-ai-colbert = { path = "libs/colbert", develop = true }
 
 pytest = "^7.3.0"
@@ -50,16 +50,18 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 
 
+
 [tool.poetry.group.dev.dependencies]
 yamllint = "^1.34.0"
 
 
 
 
+
 [tool.poetry.group.notebooks.dependencies]
 nbmake = "*"
 astrapy = "*"
```

### Comparing `ragstack_ai-1.0.3/PKG-INFO` & `ragstack_ai-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ragstack-ai
-Version: 1.0.3
+Version: 1.0.4
 Summary: DataStax RAGStack
 Home-page: https://github.com/datastax/ragstack-ai
 License: BUSL-1.1
 Author: DataStax
 Requires-Python: >=3.9,<3.12
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ragstack-ai-colbert (==1.0.2)
-Requires-Dist: ragstack-ai-langchain[colbert,google,nvidia] (==1.0.3)
-Requires-Dist: ragstack-ai-llamaindex[azure,bedrock,colbert,google] (==1.0.2)
+Requires-Dist: ragstack-ai-colbert (==1.0.3)
+Requires-Dist: ragstack-ai-langchain[colbert,google,nvidia] (==1.0.4)
+Requires-Dist: ragstack-ai-llamaindex[azure,bedrock,colbert,google] (==1.0.3)
 Project-URL: Documentation, https://docs.datastax.com/en/ragstack
 Project-URL: Repository, https://github.com/datastax/ragstack-ai
 Description-Content-Type: text/markdown
 
 # RAGStack
 [![Release Notes](https://img.shields.io/github/v/release/datastax/ragstack-ai.svg)](https://github.com/datastax/ragstack-ai/releases)
 [![Downloads](https://static.pepy.tech/badge/ragstack-ai/month)](https://www.pepy.tech/projects/ragstack-ai)
```

