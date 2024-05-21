# Comparing `tmp/injector_collections-0.0.2.tar.gz` & `tmp/injector_collections-0.0.3.tar.gz`

## Comparing `injector_collections-0.0.2.tar` & `injector_collections-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 injector_collections-0.0.2/src/injector_collections/Collection.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 injector_collections-0.0.2/src/injector_collections/CollectionItem.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 injector_collections-0.0.2/src/injector_collections/Generator.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 injector_collections-0.0.2/src/injector_collections/__init__.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 injector_collections-0.0.2/src/injector_collections/collections.jinja
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 injector_collections-0.0.2/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 injector_collections-0.0.2/LICENSE
--rw-r--r--   0        0        0     4889 2020-02-02 00:00:00.000000 injector_collections-0.0.2/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 injector_collections-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     5466 2020-02-02 00:00:00.000000 injector_collections-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 injector_collections-0.0.3/src/injector_collections/Collection.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 injector_collections-0.0.3/src/injector_collections/CollectionItem.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 injector_collections-0.0.3/src/injector_collections/Generator.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 injector_collections-0.0.3/src/injector_collections/__init__.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 injector_collections-0.0.3/src/injector_collections/collections.jinja
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 injector_collections-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 injector_collections-0.0.3/LICENSE
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 injector_collections-0.0.3/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 injector_collections-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 injector_collections-0.0.3/PKG-INFO
```

### Comparing `injector_collections-0.0.2/src/injector_collections/CollectionItem.py` & `injector_collections-0.0.3/src/injector_collections/CollectionItem.py`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.2/src/injector_collections/Generator.py` & `injector_collections-0.0.3/src/injector_collections/Generator.py`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.2/src/injector_collections/collections.jinja` & `injector_collections-0.0.3/src/injector_collections/collections.jinja`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from {{ inject.__module__ }} import {{ inject.__name__ }}
-from ic.Collection import Collection
+from injector_collections import Collection
 {%- for collection, citems in collectionItems|items %}
 {%- for (key, className) in citems %}
 from {{ className.__module__ }} import {{ className.__name__ }}
 {%- endfor %}
 {%- endfor %}
 
 {%- for collection, citems in collectionItems|items %}
```

### Comparing `injector_collections-0.0.2/LICENSE` & `injector_collections-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.2/README.md` & `injector_collections-0.0.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,49 @@
+Metadata-Version: 2.3
+Name: injector_collections
+Version: 0.0.3
+Summary: Collections for the Injector Package
+Project-URL: Homepage, https://github.com/bschnitz/injector_collections
+Project-URL: Issues, https://github.com/bschnitz/injector_collections/issues
+Author-email: Benjamin Schnitzler <regenbogenbauer@web.de>
+License-File: LICENSE
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.8
+Requires-Dist: jinja2>=3.1
+Description-Content-Type: text/markdown
+
 # Injector Collections
 
 This package adds collections to the
 [Injector](https://github.com/python-injector/injector) python package. A
 collection is an injectable class containing several other classes, which were
 tagged using the `@CollectionItem` keyword and a designated `Collection`-class.
 
 ## Setup
 
 To be able to use this package, You must create a new module-directory inside
 your python project. The name of this module-directory does not matter, let's
-name it `collections` here. Inside this module-directory the two submodules
+name it `my_collections` here. Inside this module-directory the two submodules
 (python-files) `generated.py` and `stubs.py` must be created. The following
 file-tree will be the result:
 ```
-collections
+my_collections
 ├── generated.py
 ├── __init__.py
 └── stubs.py
 ```
 Then include into `__init__.py` everything from `stubs` and `generated`:
 ```python
-from collections.stubs import *
-from collections.generated import *
+from my_collections.stubs import *
+from my_collections.generated import *
 ```
-Make sure, that `collections.generated` is imported last, since it shall
-overwrite the collections from `collections.stubs`.
+Make sure, that `my_collections.generated` is imported last, since it shall
+overwrite the collections from `my_collections.stubs`.
 
 ## Usage / Example
 
 Be sure to have done everything described in [Setup](#setup).
 
 Let's say You have an application and want to add several plugins which are all
 used in the app afterwards, but of course this list of plugins must be easily
@@ -52,19 +67,19 @@
 
 injector = Injector()
 outer = injector.get(App)
 ```
 
 Now the first step is to create a stub collection for your plugins:
 ``` python
-# collections/stub.py
+# my_collections/stub.py
 
 from injector_collections import Collection
 
-class PluginCollection(Collection)
+class PluginCollection(Collection):
     pass
 ```
 **Note:** The collection class (here `PluginCollection`) should not have any
 implementation. Currently any implementation will just be ignored and cannot be
 used after the actual class was generated from the stub. The stubs sole purpose
 is actually just to provied the LSP with some definitions, before the real
 collection is generated.
@@ -73,15 +88,15 @@
 your previously defined `PluginCollection` as argument:
 ```python
 # plugins.py
 
 from injector_collections import CollectionItem
 # the following line will import PluginCollection from stubs, if not yet
 # existing or from the generated collections, if they were already generated.
-from collections import PluginCollection
+from my_collections import PluginCollection
 
 @CollectionItem(PluginCollection)
 class HelloPlugin:
     def run(self):
         print("Hello Friends!")
 
 @CollectionItem(PluginCollection)
@@ -98,53 +113,54 @@
 **before** the application runs. Let's create first another module for this:
 ``` python
 # generate_collections.py
 
 import os
 from injector import inject
 from injector_collections import generateCollections
-import collections
+import my_collections
 
 scandir = os.path.dirname(__file__)
 # This auto-generates the real collections from the stubs. You need to provide
-# the collections-module You created during setup and a list of directories to
+# the my_collections-module You created during setup and a list of directories to
 # scan (recursively) for your collection items.
-generateCollections(inject, collections, [scandir])
+generateCollections(inject, my_collections, [scandir])
 ```
 
 Now you only need to import `generate_collections` and of course the collection
 itself to your `App` and use it:
 
 ```python
 # app.py
 
 import generate_collections
-from collections import PluginCollection
+from my_collections import PluginCollection
 
 from plugins import HelloPlugin
 
 from injector import inject
 
 class App:
     @inject
      def __init__(self, plugins: PluginCollection, '''some other injected classes'''):
          # here comes some code
          self.plugins = plugins
 
          def run(self):
              # plugins.items contains a dict containing the plugins:
-             for plugin in plugins.items.values():
+             for plugin in self.plugins.items.values():
                  plugin.run() # prints "Hello Friends!" and "Goodby Friends!"
              # Or just call a single plugin from the collection:
-             plugins[HelloPlugin].run()
+             self.plugins[HelloPlugin].run()
              # runs the app
 ...
 ```
 **Important:** `PluginCollection` and other collections must be imported only
 after they were generated (by `generate_collections`). Otherwise You will just
 have the stubs imported (if not generated previously).
 
 ### In Production
 
-For a production system, just remove the generation of collections and just
-make sure to check in the generated collections module. Because it suffices to
-generate the collections once.
+For a production system, just remove the generation of collections (in the
+example remove the `import generate_collections` line) and just make sure to
+check in the `my_collections` module. Because it suffices to generate the
+collections once.
```

### Comparing `injector_collections-0.0.2/pyproject.toml` & `injector_collections-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "injector_collections"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Benjamin Schnitzler", email="regenbogenbauer@web.de" },
 ]
 description = "Collections for the Injector Package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `injector_collections-0.0.2/PKG-INFO` & `injector_collections-0.0.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,34 @@
-Metadata-Version: 2.3
-Name: injector_collections
-Version: 0.0.2
-Summary: Collections for the Injector Package
-Project-URL: Homepage, https://github.com/bschnitz/injector_collections
-Project-URL: Issues, https://github.com/bschnitz/injector_collections/issues
-Author-email: Benjamin Schnitzler <regenbogenbauer@web.de>
-License-File: LICENSE
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.8
-Requires-Dist: jinja2>=3.1
-Description-Content-Type: text/markdown
-
 # Injector Collections
 
 This package adds collections to the
 [Injector](https://github.com/python-injector/injector) python package. A
 collection is an injectable class containing several other classes, which were
 tagged using the `@CollectionItem` keyword and a designated `Collection`-class.
 
 ## Setup
 
 To be able to use this package, You must create a new module-directory inside
 your python project. The name of this module-directory does not matter, let's
-name it `collections` here. Inside this module-directory the two submodules
+name it `my_collections` here. Inside this module-directory the two submodules
 (python-files) `generated.py` and `stubs.py` must be created. The following
 file-tree will be the result:
 ```
-collections
+my_collections
 ├── generated.py
 ├── __init__.py
 └── stubs.py
 ```
 Then include into `__init__.py` everything from `stubs` and `generated`:
 ```python
-from collections.stubs import *
-from collections.generated import *
+from my_collections.stubs import *
+from my_collections.generated import *
 ```
-Make sure, that `collections.generated` is imported last, since it shall
-overwrite the collections from `collections.stubs`.
+Make sure, that `my_collections.generated` is imported last, since it shall
+overwrite the collections from `my_collections.stubs`.
 
 ## Usage / Example
 
 Be sure to have done everything described in [Setup](#setup).
 
 Let's say You have an application and want to add several plugins which are all
 used in the app afterwards, but of course this list of plugins must be easily
@@ -67,19 +52,19 @@
 
 injector = Injector()
 outer = injector.get(App)
 ```
 
 Now the first step is to create a stub collection for your plugins:
 ``` python
-# collections/stub.py
+# my_collections/stub.py
 
 from injector_collections import Collection
 
-class PluginCollection(Collection)
+class PluginCollection(Collection):
     pass
 ```
 **Note:** The collection class (here `PluginCollection`) should not have any
 implementation. Currently any implementation will just be ignored and cannot be
 used after the actual class was generated from the stub. The stubs sole purpose
 is actually just to provied the LSP with some definitions, before the real
 collection is generated.
@@ -88,15 +73,15 @@
 your previously defined `PluginCollection` as argument:
 ```python
 # plugins.py
 
 from injector_collections import CollectionItem
 # the following line will import PluginCollection from stubs, if not yet
 # existing or from the generated collections, if they were already generated.
-from collections import PluginCollection
+from my_collections import PluginCollection
 
 @CollectionItem(PluginCollection)
 class HelloPlugin:
     def run(self):
         print("Hello Friends!")
 
 @CollectionItem(PluginCollection)
@@ -113,53 +98,54 @@
 **before** the application runs. Let's create first another module for this:
 ``` python
 # generate_collections.py
 
 import os
 from injector import inject
 from injector_collections import generateCollections
-import collections
+import my_collections
 
 scandir = os.path.dirname(__file__)
 # This auto-generates the real collections from the stubs. You need to provide
-# the collections-module You created during setup and a list of directories to
+# the my_collections-module You created during setup and a list of directories to
 # scan (recursively) for your collection items.
-generateCollections(inject, collections, [scandir])
+generateCollections(inject, my_collections, [scandir])
 ```
 
 Now you only need to import `generate_collections` and of course the collection
 itself to your `App` and use it:
 
 ```python
 # app.py
 
 import generate_collections
-from collections import PluginCollection
+from my_collections import PluginCollection
 
 from plugins import HelloPlugin
 
 from injector import inject
 
 class App:
     @inject
      def __init__(self, plugins: PluginCollection, '''some other injected classes'''):
          # here comes some code
          self.plugins = plugins
 
          def run(self):
              # plugins.items contains a dict containing the plugins:
-             for plugin in plugins.items.values():
+             for plugin in self.plugins.items.values():
                  plugin.run() # prints "Hello Friends!" and "Goodby Friends!"
              # Or just call a single plugin from the collection:
-             plugins[HelloPlugin].run()
+             self.plugins[HelloPlugin].run()
              # runs the app
 ...
 ```
 **Important:** `PluginCollection` and other collections must be imported only
 after they were generated (by `generate_collections`). Otherwise You will just
 have the stubs imported (if not generated previously).
 
 ### In Production
 
-For a production system, just remove the generation of collections and just
-make sure to check in the generated collections module. Because it suffices to
-generate the collections once.
+For a production system, just remove the generation of collections (in the
+example remove the `import generate_collections` line) and just make sure to
+check in the `my_collections` module. Because it suffices to generate the
+collections once.
```

