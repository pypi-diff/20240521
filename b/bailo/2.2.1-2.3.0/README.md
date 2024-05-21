# Comparing `tmp/bailo-2.2.1.tar.gz` & `tmp/bailo-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bailo-2.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bailo-2.3.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bailo-2.2.1.tar` & `bailo-2.3.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0     2241 2024-05-17 10:50:21.393252 bailo-2.2.1/README.md
--rw-r--r--   0        0        0     4889 2024-05-17 10:50:21.393252 bailo-2.2.1/pyproject.toml
--rw-r--r--   0        0        0      636 2024-05-17 10:50:21.393252 bailo-2.2.1/src/bailo/__init__.py
--rw-r--r--   0        0        0      153 2024-05-17 10:50:21.393252 bailo-2.2.1/src/bailo/core/__init__.py
--rw-r--r--   0        0        0     3594 2024-05-17 10:50:21.393252 bailo-2.2.1/src/bailo/core/agent.py
--rw-r--r--   0        0        0    19238 2024-05-17 10:50:21.397251 bailo-2.2.1/src/bailo/core/client.py
--rw-r--r--   0        0        0      672 2024-05-17 10:50:21.397251 bailo-2.2.1/src/bailo/core/enums.py
--rw-r--r--   0        0        0      221 2024-05-17 10:50:21.397251 bailo-2.2.1/src/bailo/core/exceptions.py
--rw-r--r--   0        0        0     1072 2024-05-17 10:50:21.397251 bailo-2.2.1/src/bailo/core/utils.py
--rw-r--r--   0        0        0      521 2024-05-17 10:50:21.397251 bailo-2.2.1/src/bailo/helper/__init__.py
--rw-r--r--   0        0        0     3923 2024-05-17 10:50:21.397251 bailo-2.2.1/src/bailo/helper/access_request.py
--rw-r--r--   0        0        0    15468 2024-05-17 10:50:21.397251 bailo-2.2.1/src/bailo/helper/model.py
--rw-r--r--   0        0        0     9816 2024-05-17 10:50:21.397251 bailo-2.2.1/src/bailo/helper/release.py
--rw-r--r--   0        0        0     2976 2024-05-17 10:50:21.397251 bailo-2.2.1/src/bailo/helper/schema.py
--rw-r--r--   0        0        0     3674 1970-01-01 00:00:00.000000 bailo-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     2241 2024-05-21 16:08:28.781113 bailo-2.3.0/README.md
+-rw-r--r--   0        0        0     4889 2024-05-21 16:08:28.785113 bailo-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0      685 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/__init__.py
+-rw-r--r--   0        0        0      153 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/core/__init__.py
+-rw-r--r--   0        0        0     3594 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/core/agent.py
+-rw-r--r--   0        0        0    19238 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/core/client.py
+-rw-r--r--   0        0        0      672 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/core/enums.py
+-rw-r--r--   0        0        0      221 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/core/exceptions.py
+-rw-r--r--   0        0        0     1072 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/core/utils.py
+-rw-r--r--   0        0        0      521 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/__init__.py
+-rw-r--r--   0        0        0     3923 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/access_request.py
+-rw-r--r--   0        0        0     3833 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/datacard.py
+-rw-r--r--   0        0        0     3367 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/entry.py
+-rw-r--r--   0        0        0    13134 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/model.py
+-rw-r--r--   0        0        0     9816 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/release.py
+-rw-r--r--   0        0        0     2976 2024-05-21 16:08:28.785113 bailo-2.3.0/src/bailo/helper/schema.py
+-rw-r--r--   0        0        0     3674 1970-01-01 00:00:00.000000 bailo-2.3.0/PKG-INFO
```

### Comparing `bailo-2.2.1/README.md` & `bailo-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bailo-2.2.1/pyproject.toml` & `bailo-2.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bailo-2.2.1/src/bailo/__init__.py` & `bailo-2.3.0/src/bailo/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 ===================
 
 Bailo is a ecosystem for managing the lifecycle of managing machine learning models. This package provides support for interacting with models within Bailo.
 """
 from __future__ import annotations
 
 
-# Package Version
-__version__ = "2.2.1"
+# Package Version 2.3.0
+__version__ = "2.3.0"
 
 
 from bailo.core.agent import Agent, PkiAgent, TokenAgent
 from bailo.core.client import Client
 from bailo.core.enums import EntryKind, ModelVisibility, Role, SchemaKind
 from bailo.helper.access_request import AccessRequest
+from bailo.helper.datacard import Datacard
 from bailo.helper.model import Experiment, Model
 from bailo.helper.release import Release
 from bailo.helper.schema import Schema
```

### Comparing `bailo-2.2.1/src/bailo/core/agent.py` & `bailo-2.3.0/src/bailo/core/agent.py`

 * *Files identical despite different names*

### Comparing `bailo-2.2.1/src/bailo/core/client.py` & `bailo-2.3.0/src/bailo/core/client.py`

 * *Files identical despite different names*

### Comparing `bailo-2.2.1/src/bailo/core/enums.py` & `bailo-2.3.0/src/bailo/core/enums.py`

 * *Files identical despite different names*

### Comparing `bailo-2.2.1/src/bailo/core/utils.py` & `bailo-2.3.0/src/bailo/core/utils.py`

 * *Files identical despite different names*

### Comparing `bailo-2.2.1/src/bailo/helper/__init__.py` & `bailo-2.3.0/src/bailo/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `bailo-2.2.1/src/bailo/helper/access_request.py` & `bailo-2.3.0/src/bailo/helper/access_request.py`

 * *Files identical despite different names*

### Comparing `bailo-2.2.1/src/bailo/helper/model.py` & `bailo-2.3.0/src/bailo/helper/model.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,177 +5,123 @@
 import tempfile
 from typing import Any
 
 from bailo.core.client import Client
 from bailo.core.enums import EntryKind, ModelVisibility
 from bailo.core.exceptions import BailoException
 from bailo.core.utils import NestedDict
+from bailo.helper.entry import Entry
 from bailo.helper.release import Release
 from semantic_version import Version
 
 try:
     import mlflow
 
     ml_flow = True
 except ImportError:
     ml_flow = False
 
 
-class Model:
+class Model(Entry):
     """Represent a model within Bailo.
 
     :param client: A client object used to interact with Bailo
     :param model_id: A unique ID for the model
     :param name: Name of model
-    :param kind: Either a Model or a Datacard
     :param description: Description of model
     :param visibility: Visibility of model, using ModelVisibility enum (e.g Public or Private), defaults to None
     """
 
     def __init__(
         self,
         client: Client,
         model_id: str,
         name: str,
-        kind: EntryKind,
         description: str,
         visibility: ModelVisibility | None = None,
     ) -> None:
-        self.client = client
+        super().__init__(
+            client=client, id=model_id, name=name, description=description, kind=EntryKind.MODEL, visibility=visibility
+        )
 
         self.model_id = model_id
-        self.name = name
-        self.kind = kind
-        self.description = description
-        self.visibility = visibility
-
-        self.model_card = None
-        self.model_card_version = None
-        self.model_card_schema = None
 
     @classmethod
     def create(
         cls,
         client: Client,
         name: str,
-        kind: EntryKind,
         description: str,
         team_id: str,
         visibility: ModelVisibility | None = None,
     ) -> Model:
-        """Build a model from Bailo and uploads it.
+        """Build a model from Bailo and upload it.
 
         :param client: A client object used to interact with Bailo
         :param name: Name of model
-        :param kind: Either a Model or a Datacard
         :param description: Description of model
         :param team_id: A unique team ID
         :param visibility: Visibility of model, using ModelVisibility enum (e.g Public or Private), defaults to None
         :return: Model object
         """
-        res = client.post_model(name=name, kind=kind, description=description, team_id=team_id, visibility=visibility)
+        res = client.post_model(
+            name=name, kind=EntryKind.MODEL, description=description, team_id=team_id, visibility=visibility
+        )
         model = cls(
             client=client,
             model_id=res["model"]["id"],
             name=name,
-            kind=kind,
             description=description,
             visibility=visibility,
         )
 
-        model.__unpack(res["model"])
+        model._unpack(res["model"])
 
         return model
 
     @classmethod
     def from_id(cls, client: Client, model_id: str) -> Model:
         """Return an existing model from Bailo.
 
         :param client: A client object used to interact with Bailo
         :param model_id: A unique model ID
         :return: A model object
         """
         res = client.get_model(model_id=model_id)["model"]
+        if res["kind"] != "model":
+            raise BailoException(f"ID {model_id} does not belong to a model. Did you mean to use Datacard.from_id()?")
+
         model = cls(
             client=client,
             model_id=model_id,
-            kind=res["kind"],
             name=res["name"],
             description=res["description"],
         )
-        model.__unpack(res)
 
+        model._unpack(res)
         model.get_card_latest()
 
         return model
 
-    def update(self) -> None:
-        """Upload and retrieves any changes to the model summary on Bailo."""
-        res = self.client.patch_model(
-            model_id=self.model_id,
-            name=self.name,
-            kind=self.kind,
-            description=self.description,
-            visibility=self.visibility,
-        )
-        self.__unpack(res["model"])
-
     def update_model_card(self, model_card: dict[str, Any] | None = None) -> None:
-        """Upload and retrieves any changes to the model card on Bailo.
+        """Upload and retrieve any changes to the model card on Bailo.
 
         :param model_card: Model card dictionary, defaults to None
 
         ..note:: If a model card is not provided, the current model card attribute value is used
         """
-        if model_card is None:
-            model_card = self.model_card
-        res = self.client.put_model_card(model_id=self.model_id, metadata=model_card)
-        self.__unpack_mc(res["card"])
-
-    def card_from_schema(self, schema_id: str) -> None:
-        """Create a model card using a schema on Bailo.
-
-        :param schema_id: A unique schema ID
-        """
-        res = self.client.model_card_from_schema(model_id=self.model_id, schema_id=schema_id)
-        self.__unpack_mc(res["card"])
-
-    def card_from_model(self):
-        """Copy a model card from a different model (not yet implemented).
-
-        :raises NotImplementedError: Not implemented error
-        """
-        raise NotImplementedError
-
-    def card_from_template(self):
-        """Create a model card using a template (not yet implemented).
-
-        :raises NotImplementedError: Not implemented error
-        """
-        raise NotImplementedError
-
-    def get_card_latest(self) -> None:
-        """Get the latest model card from Bailo."""
-        res = self.client.get_model(model_id=self.model_id)
-        if "card" in res["model"]:
-            self.__unpack_mc(res["model"]["card"])
-        else:
-            raise BailoException(f"A model card doesn't exist for model {self.model_id}")
-
-    def get_card_revision(self, version: str) -> None:
-        """Get a specific model card revision from Bailo.
-
-        :param version: Model card version
-        """
-        res = self.client.get_model_card(model_id=self.model_id, version=version)
-        self.__unpack_mc(res["modelCard"])
+        self._update_card(card=model_card)
 
     def create_experiment(
         self,
     ) -> Experiment:
+        """Create an experiment locally
+
+        :return: An experiment object
+        """
         return Experiment.create(model=self)
 
     def create_release(
         self,
         version: Version | str,
         notes: str,
         files: list[str] | None = None,
@@ -250,50 +196,37 @@
     def get_image(self):
         """Get a model image reference.
 
         :raises NotImplementedError: Not implemented error.
         """
         raise NotImplementedError
 
-    def get_roles(self):
-        """Get all roles for the model.
-
-        :return: List of roles
-        """
-        res = self.client.get_model_roles(model_id=self.model_id)
-
-        return res["roles"]
-
-    def get_user_roles(self):
-        """Get all user roles for the model.
-
-        :return: List of user roles
-        """
-        res = self.client.get_model_user_roles(model_id=self.model_id)
-
-        return res["roles"]
-
-    def __unpack(self, res):
-        self.model_id = res["id"]
-        self.name = res["name"]
-        self.description = res["description"]
-
-        if res["visibility"] == "private":
-            self.visibility = ModelVisibility.PRIVATE
-        else:
-            self.visibility = ModelVisibility.PUBLIC
-
-    def __unpack_mc(self, res):
-        self.model_card_version = res["version"]
-        self.model_card_schema = res["schemaId"]
-
-        try:
-            self.model_card = res["metadata"]
-        except KeyError:
-            self.model_card = None
+    @property
+    def model_card(self):
+        return self._card
+
+    @model_card.setter
+    def model_card(self, value):
+        self._card = value
+
+    @property
+    def model_card_version(self):
+        return self._card_version
+
+    @model_card_version.setter
+    def model_card_version(self, value):
+        self._card_version = value
+
+    @property
+    def model_card_schema(self):
+        return self._card_schema
+
+    @model_card_schema.setter
+    def model_card_schema(self, value):
+        self._card_schema = value
 
 
 class Experiment:
     """Represent an experiment locally.
 
     :param model: A Bailo model object which the experiment is being run on
     :param raw: Raw information about the experiment runs
```

### Comparing `bailo-2.2.1/src/bailo/helper/release.py` & `bailo-2.3.0/src/bailo/helper/release.py`

 * *Files identical despite different names*

### Comparing `bailo-2.2.1/src/bailo/helper/schema.py` & `bailo-2.3.0/src/bailo/helper/schema.py`

 * *Files identical despite different names*

### Comparing `bailo-2.2.1/PKG-INFO` & `bailo-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bailo
-Version: 2.2.1
+Version: 2.3.0
 Summary: Simplifies interacting with Bailo
 Requires-Python: >=3.8.1
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bailo Version: 2.2.1 Summary: Simplifies
+Metadata-Version: 2.1 Name: bailo Version: 2.3.0 Summary: Simplifies
 interacting with Bailo Requires-Python: >=3.8.1 Description-Content-Type: text/
 markdown Classifier: Development Status :: 3 - Alpha Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: semantic-version==2.10.0 Requires-Dist: requests>=2.22 Requires-
 Dist: tqdm>=4.66.2 Requires-Dist: black==23.3.0 ; extra == "test" Requires-
```

