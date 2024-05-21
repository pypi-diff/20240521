# Comparing `tmp/injector_collections-0.0.3.tar.gz` & `tmp/injector_collections-0.0.5.tar.gz`

## Comparing `injector_collections-0.0.3.tar` & `injector_collections-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 injector_collections-0.0.3/src/injector_collections/Collection.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 injector_collections-0.0.3/src/injector_collections/CollectionItem.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 injector_collections-0.0.3/src/injector_collections/Generator.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 injector_collections-0.0.3/src/injector_collections/__init__.py
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 injector_collections-0.0.3/src/injector_collections/collections.jinja
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 injector_collections-0.0.3/.gitignore
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 injector_collections-0.0.3/LICENSE
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 injector_collections-0.0.3/README.md
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 injector_collections-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 injector_collections-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      444 2020-02-02 00:00:00.000000 injector_collections-0.0.5/src/injector_collections/Collection.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 injector_collections-0.0.5/src/injector_collections/CollectionItem.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 injector_collections-0.0.5/src/injector_collections/Generator.py
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 injector_collections-0.0.5/src/injector_collections/__init__.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 injector_collections-0.0.5/src/injector_collections/collections.jinja
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 injector_collections-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 injector_collections-0.0.5/LICENSE
+-rw-r--r--   0        0        0     5028 2020-02-02 00:00:00.000000 injector_collections-0.0.5/README.md
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 injector_collections-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5605 2020-02-02 00:00:00.000000 injector_collections-0.0.5/PKG-INFO
```

### Comparing `injector_collections-0.0.3/src/injector_collections/CollectionItem.py` & `injector_collections-0.0.5/src/injector_collections/CollectionItem.py`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.3/src/injector_collections/Generator.py` & `injector_collections-0.0.5/src/injector_collections/Generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,50 @@
 import os
 import pkgutil
 import importlib
-import importlib.util as iutil
 from types import ModuleType
 from typing import Any, Callable, Iterable, Type
 from jinja2 import FileSystemLoader
 from jinja2 import Environment
 from injector_collections.CollectionItem import CollectionItem
 import injector_collections
+from importlib import util
 
 class Generator:
     generatedCollectionsFileName = 'generated.py'
     collectionsTemplateFilename = 'collections.jinja'
     def generate(
             self,
             inject: Callable,
-            collectionModule: ModuleType,
-            scanPathes: Iterable[str]
+            collectionModule: str,
+            scannedModules: Iterable[str]
             ):
         collectionModuleDirectory = self.getModuleDirectory(collectionModule)
         # empty collections module to avoid circular imports
         with open(f'{collectionModuleDirectory}/{self.generatedCollectionsFileName}', 'w') as f:
             pass
 
-        collectionMetadata = self.gatherCollectionMetadata(scanPathes)
+        collectionMetadata = self.gatherCollectionMetadata(scannedModules)
 
         with open(f'{collectionModuleDirectory}/{self.generatedCollectionsFileName}', 'w') as f:
             f.write(self.renderCollectionsTemplate(inject, collectionMetadata))
 
         # reload the collections module to make generated collections
         # visible when using import from other places
-        importlib.reload(collectionModule.generated)
-        importlib.reload(collectionModule)
-
-    def getModuleDirectory(self, module: ModuleType) -> str:
-        modulePath = module.__file__
+        # collectionModule = importlib.import_module(collectionModule)
+        # importlib.reload(collectionModule.generated)
+        # importlib.reload(collectionModule)
+
+    def getModuleDirectory(self, module: str|ModuleType) -> str:
+        print(module)
+        if isinstance(module, str):
+            moduleSpec = util.find_spec(module)
+            modulePath = moduleSpec.origin
+        else:
+            modulePath = module.__file__
         assert(modulePath is not None)
         return os.path.dirname(modulePath)
 
     def renderCollectionsTemplate(
             self,
             inject: Callable,
             collectionsMetadata: dict[Type, list[tuple[Any, Any]]]
@@ -52,23 +58,37 @@
         return template.render(
             collectionItems = collectionsMetadata,
             inject = inject
             )
 
     def gatherCollectionMetadata(
             self,
-            scanPathes: Iterable[str],
+            scannedModules: Iterable[str],
             ) -> dict[Type, list[tuple[Any, Any]]]:
-        # Import all classes decorated with @CollectionItem. The import will
-        # trigger the __call__ method of the decorator and this will populate
-        # the metadata dict, which this method returns.
-        for modinfo in pkgutil.walk_packages(scanPathes):
-            spec = iutil.find_spec(modinfo.name)
-            assert(spec is not None)
-            filepath = spec.origin
-            assert(filepath is not None)
-            with open(filepath, 'r') as f:
-                if '@CollectionItem' in f.read():
-                    importlib.import_module(modinfo.name)
+        ''' Gather Metadata for Collection generation with template
+
+        Recursively walks through all modules in 'scannedModules' and gathers
+        metadata for every class decorated with '@CollectionItem'.
+        '''
+        for m in scannedModules:
+            for spec in self.walkModules(m):
+                with open(spec.origin, 'r') as f:
+                    if '@CollectionItem' in f.read():
+                        importlib.import_module(spec.name)
 
         return CollectionItem.getItems()
 
+    def walkModules(self, rootModule: str):
+        info = util.find_spec(rootModule)
+        yield info
+
+        if info.submodule_search_locations is None:
+            return
+
+        #for modinfo in pkgutil.walk_packages(info.submodule_search_locations):
+        for modinfo in pkgutil.iter_modules(info.submodule_search_locations):
+            name = f'{info.name}.{modinfo.name}'
+            yield util.find_spec(name)
+            submods = self.walkModules(name)
+            next(submods) # remove the root, which was just yielded
+            for mi in submods:
+                yield mi
```

### Comparing `injector_collections-0.0.3/src/injector_collections/collections.jinja` & `injector_collections-0.0.5/src/injector_collections/collections.jinja`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.3/LICENSE` & `injector_collections-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `injector_collections-0.0.3/README.md` & `injector_collections-0.0.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,33 @@
 tagged using the `@CollectionItem` keyword and a designated `Collection`-class.
 
 ## Setup
 
 To be able to use this package, You must create a new module-directory inside
 your python project. The name of this module-directory does not matter, let's
 name it `my_collections` here. Inside this module-directory the two submodules
-(python-files) `generated.py` and `stubs.py` must be created. The following
-file-tree will be the result:
+(python-files) `generated.py` and `stubs.py` must be created. Also a module-file
+`generate-collections.py` should be created.
+The following file-tree will be the result:
 ```
 my_collections
-├── generated.py
 ├── __init__.py
-└── stubs.py
+├── generate_collections.py
+├── stubs.py
+└── generated.py
 ```
 Then include into `__init__.py` everything from `stubs` and `generated`:
 ```python
-from my_collections.stubs import *
-from my_collections.generated import *
-```
-Make sure, that `my_collections.generated` is imported last, since it shall
-overwrite the collections from `my_collections.stubs`.
+from injection.collections.stubs import *
+import injection.collections.generate_collections
+from injection.collections.generated import *
+```
+**Important:** Make sure, that You import the `generate_collections` module
+before importing the generated collections, since otherwise of course you will
+only have stubs on the first invokation.
 
 ## Usage / Example
 
 Be sure to have done everything described in [Setup](#setup).
 
 Let's say You have an application and want to add several plugins which are all
 used in the app afterwards, but of course this list of plugins must be easily
@@ -87,41 +91,39 @@
 @CollectionItem(PluginCollection)
 class GoodbyPlugin:
     def run(self):
         print("Goodby Friends!")
 ```
 
 **Important:** Currently you need to import `CollectionItem` literally, as the
-code will be scanned for files containing the `CollectionItem` keyword, which
-must then be imported to auto-generate the collections!
+code will be scanned for files containing the `@CollectionItem` string, which
+will then be imported to auto-generate the collections!
 
 Now we're almost done. We just have to make sure the plugins are generated when
-**before** the application runs. Let's create first another module for this:
+**before** the application runs. Now we will edit the
+`my_collections/generate_collections.py` to have it generate our
+`PluginCollection`:
 ``` python
 # generate_collections.py
 
-import os
 from injector import inject
 from injector_collections import generateCollections
-import my_collections
 
-scandir = os.path.dirname(__file__)
 # This auto-generates the real collections from the stubs. You need to provide
-# the my_collections-module You created during setup and a list of directories to
-# scan (recursively) for your collection items.
-generateCollections(inject, my_collections, [scandir])
+# the my_collections-module and a list of modules to scan for your collection
+# items (in this case the plugins module suffices). If those modules are
+# directories, all modules in them will be scanned recursively.
+generateCollections(inject, "my_collections", ['plugins'])
 ```
 
-Now you only need to import `generate_collections` and of course the collection
-itself to your `App` and use it:
+Now you just need to import the `PluginCollection` to your `App` and use it:
 
 ```python
 # app.py
 
-import generate_collections
 from my_collections import PluginCollection
 
 from plugins import HelloPlugin
 
 from injector import inject
 
 class App:
@@ -135,17 +137,14 @@
              for plugin in self.plugins.items.values():
                  plugin.run() # prints "Hello Friends!" and "Goodby Friends!"
              # Or just call a single plugin from the collection:
              self.plugins[HelloPlugin].run()
              # runs the app
 ...
 ```
-**Important:** `PluginCollection` and other collections must be imported only
-after they were generated (by `generate_collections`). Otherwise You will just
-have the stubs imported (if not generated previously).
 
 ### In Production
 
 For a production system, just remove the generation of collections (in the
 example remove the `import generate_collections` line) and just make sure to
 check in the `my_collections` module. Because it suffices to generate the
 collections once.
```

### Comparing `injector_collections-0.0.3/pyproject.toml` & `injector_collections-0.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "injector_collections"
-version = "0.0.3"
+version = "0.0.5"
 authors = [
   { name="Benjamin Schnitzler", email="regenbogenbauer@web.de" },
 ]
 description = "Collections for the Injector Package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `injector_collections-0.0.3/PKG-INFO` & `injector_collections-0.0.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: injector_collections
-Version: 0.0.3
+Version: 0.0.5
 Summary: Collections for the Injector Package
 Project-URL: Homepage, https://github.com/bschnitz/injector_collections
 Project-URL: Issues, https://github.com/bschnitz/injector_collections/issues
 Author-email: Benjamin Schnitzler <regenbogenbauer@web.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -21,29 +21,33 @@
 tagged using the `@CollectionItem` keyword and a designated `Collection`-class.
 
 ## Setup
 
 To be able to use this package, You must create a new module-directory inside
 your python project. The name of this module-directory does not matter, let's
 name it `my_collections` here. Inside this module-directory the two submodules
-(python-files) `generated.py` and `stubs.py` must be created. The following
-file-tree will be the result:
+(python-files) `generated.py` and `stubs.py` must be created. Also a module-file
+`generate-collections.py` should be created.
+The following file-tree will be the result:
 ```
 my_collections
-├── generated.py
 ├── __init__.py
-└── stubs.py
+├── generate_collections.py
+├── stubs.py
+└── generated.py
 ```
 Then include into `__init__.py` everything from `stubs` and `generated`:
 ```python
-from my_collections.stubs import *
-from my_collections.generated import *
-```
-Make sure, that `my_collections.generated` is imported last, since it shall
-overwrite the collections from `my_collections.stubs`.
+from injection.collections.stubs import *
+import injection.collections.generate_collections
+from injection.collections.generated import *
+```
+**Important:** Make sure, that You import the `generate_collections` module
+before importing the generated collections, since otherwise of course you will
+only have stubs on the first invokation.
 
 ## Usage / Example
 
 Be sure to have done everything described in [Setup](#setup).
 
 Let's say You have an application and want to add several plugins which are all
 used in the app afterwards, but of course this list of plugins must be easily
@@ -102,41 +106,39 @@
 @CollectionItem(PluginCollection)
 class GoodbyPlugin:
     def run(self):
         print("Goodby Friends!")
 ```
 
 **Important:** Currently you need to import `CollectionItem` literally, as the
-code will be scanned for files containing the `CollectionItem` keyword, which
-must then be imported to auto-generate the collections!
+code will be scanned for files containing the `@CollectionItem` string, which
+will then be imported to auto-generate the collections!
 
 Now we're almost done. We just have to make sure the plugins are generated when
-**before** the application runs. Let's create first another module for this:
+**before** the application runs. Now we will edit the
+`my_collections/generate_collections.py` to have it generate our
+`PluginCollection`:
 ``` python
 # generate_collections.py
 
-import os
 from injector import inject
 from injector_collections import generateCollections
-import my_collections
 
-scandir = os.path.dirname(__file__)
 # This auto-generates the real collections from the stubs. You need to provide
-# the my_collections-module You created during setup and a list of directories to
-# scan (recursively) for your collection items.
-generateCollections(inject, my_collections, [scandir])
+# the my_collections-module and a list of modules to scan for your collection
+# items (in this case the plugins module suffices). If those modules are
+# directories, all modules in them will be scanned recursively.
+generateCollections(inject, "my_collections", ['plugins'])
 ```
 
-Now you only need to import `generate_collections` and of course the collection
-itself to your `App` and use it:
+Now you just need to import the `PluginCollection` to your `App` and use it:
 
 ```python
 # app.py
 
-import generate_collections
 from my_collections import PluginCollection
 
 from plugins import HelloPlugin
 
 from injector import inject
 
 class App:
@@ -150,17 +152,14 @@
              for plugin in self.plugins.items.values():
                  plugin.run() # prints "Hello Friends!" and "Goodby Friends!"
              # Or just call a single plugin from the collection:
              self.plugins[HelloPlugin].run()
              # runs the app
 ...
 ```
-**Important:** `PluginCollection` and other collections must be imported only
-after they were generated (by `generate_collections`). Otherwise You will just
-have the stubs imported (if not generated previously).
 
 ### In Production
 
 For a production system, just remove the generation of collections (in the
 example remove the `import generate_collections` line) and just make sure to
 check in the `my_collections` module. Because it suffices to generate the
 collections once.
```

