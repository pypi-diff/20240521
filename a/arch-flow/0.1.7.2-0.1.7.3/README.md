# Comparing `tmp/arch_flow-0.1.7.2.tar.gz` & `tmp/arch_flow-0.1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch_flow-0.1.7.2.tar", last modified: Tue May 21 01:57:38 2024, max compression
+gzip compressed data, was "arch_flow-0.1.7.3.tar", last modified: Tue May 21 02:25:01 2024, max compression
```

## Comparing `arch_flow-0.1.7.2.tar` & `arch_flow-0.1.7.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 01:57:38.543101 arch_flow-0.1.7.2/
--rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.7.2/LICENCE
--rw-rw-rw-   0        0        0      983 2024-05-21 01:57:38.542102 arch_flow-0.1.7.2/PKG-INFO
--rw-rw-rw-   0        0        0     6622 2024-04-25 23:30:53.000000 arch_flow-0.1.7.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 01:57:38.509862 arch_flow-0.1.7.2/arch_flow/
--rw-rw-rw-   0        0        0     4601 2024-05-21 01:17:31.000000 arch_flow-0.1.7.2/arch_flow/ArchFlow.py
--rw-rw-rw-   0        0        0      216 2024-05-21 01:50:14.000000 arch_flow-0.1.7.2/arch_flow/ArchFlowCli.py
--rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.7.2/arch_flow/DirectoryCreator.py
--rw-rw-rw-   0        0        0     3301 2024-05-04 03:27:18.000000 arch_flow-0.1.7.2/arch_flow/DirectoryExplorer.py
--rw-rw-rw-   0        0        0      363 2024-05-21 01:57:35.000000 arch_flow-0.1.7.2/arch_flow/Run.py
--rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.7.2/arch_flow/StringManipulator.py
--rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.7.2/arch_flow/__init__.py
--rw-rw-rw-   0        0        0      143 2024-05-21 01:50:14.000000 arch_flow-0.1.7.2/arch_flow/db.json
-drwxrwxrwx   0        0        0        0 2024-05-21 01:57:38.531910 arch_flow-0.1.7.2/arch_flow/exceptions/
--rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.7.2/arch_flow/exceptions/ExceptionHandler.py
--rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.7.2/arch_flow/exceptions/FileOrDirectoryExistsError.py
--rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.7.2/arch_flow/exceptions/NotFoundException.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:57:38.536909 arch_flow-0.1.7.2/arch_flow/implementations/
--rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.7.2/arch_flow/implementations/DirectoryCreatorImplementation.py
--rw-rw-rw-   0        0        0     7196 2024-04-21 05:43:57.000000 arch_flow-0.1.7.2/arch_flow/implementations/DirectoryExplorerImplementation.py
--rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.7.2/arch_flow/implementations/StringManipulatorImplementation.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:57:38.538094 arch_flow-0.1.7.2/arch_flow/output/
--rw-rw-rw-   0        0        0     2372 2024-03-15 22:56:29.000000 arch_flow-0.1.7.2/arch_flow/output/OutputHandler.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:57:38.540104 arch_flow-0.1.7.2/arch_flow/utils/
--rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.7.2/arch_flow/utils/DirectoryExplorerUtil.py
--rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.7.2/arch_flow/utils/Filter.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:57:38.542102 arch_flow-0.1.7.2/arch_flow.egg-info/
--rw-rw-rw-   0        0        0      983 2024-05-21 01:57:38.000000 arch_flow-0.1.7.2/arch_flow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      803 2024-05-21 01:57:38.000000 arch_flow-0.1.7.2/arch_flow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 01:57:38.000000 arch_flow-0.1.7.2/arch_flow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-21 01:57:38.000000 arch_flow-0.1.7.2/arch_flow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-21 01:57:38.000000 arch_flow-0.1.7.2/arch_flow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 01:57:38.544102 arch_flow-0.1.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1246 2024-05-21 01:57:35.000000 arch_flow-0.1.7.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:25:01.264645 arch_flow-0.1.7.3/
+-rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.7.3/LICENCE
+-rw-rw-rw-   0        0        0      983 2024-05-21 02:25:01.262642 arch_flow-0.1.7.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6622 2024-04-25 23:30:53.000000 arch_flow-0.1.7.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 02:25:01.236841 arch_flow-0.1.7.3/arch_flow/
+-rw-rw-rw-   0        0        0     5165 2024-05-21 02:24:38.000000 arch_flow-0.1.7.3/arch_flow/ArchFlow.py
+-rw-rw-rw-   0        0        0      216 2024-05-21 01:50:14.000000 arch_flow-0.1.7.3/arch_flow/ArchFlowCli.py
+-rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.7.3/arch_flow/DirectoryCreator.py
+-rw-rw-rw-   0        0        0     3301 2024-05-04 03:27:18.000000 arch_flow-0.1.7.3/arch_flow/DirectoryExplorer.py
+-rw-rw-rw-   0        0        0      363 2024-05-21 01:57:35.000000 arch_flow-0.1.7.3/arch_flow/Run.py
+-rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.7.3/arch_flow/StringManipulator.py
+-rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.7.3/arch_flow/__init__.py
+-rw-rw-rw-   0        0        0      143 2024-05-21 01:50:14.000000 arch_flow-0.1.7.3/arch_flow/db.json
+drwxrwxrwx   0        0        0        0 2024-05-21 02:25:01.253374 arch_flow-0.1.7.3/arch_flow/exceptions/
+-rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.7.3/arch_flow/exceptions/ExceptionHandler.py
+-rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.7.3/arch_flow/exceptions/FileOrDirectoryExistsError.py
+-rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.7.3/arch_flow/exceptions/NotFoundException.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:25:01.256371 arch_flow-0.1.7.3/arch_flow/implementations/
+-rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.7.3/arch_flow/implementations/DirectoryCreatorImplementation.py
+-rw-rw-rw-   0        0        0     7196 2024-04-21 05:43:57.000000 arch_flow-0.1.7.3/arch_flow/implementations/DirectoryExplorerImplementation.py
+-rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.7.3/arch_flow/implementations/StringManipulatorImplementation.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:25:01.257646 arch_flow-0.1.7.3/arch_flow/output/
+-rw-rw-rw-   0        0        0     2372 2024-03-15 22:56:29.000000 arch_flow-0.1.7.3/arch_flow/output/OutputHandler.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:25:01.260643 arch_flow-0.1.7.3/arch_flow/utils/
+-rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.7.3/arch_flow/utils/DirectoryExplorerUtil.py
+-rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.7.3/arch_flow/utils/Filter.py
+drwxrwxrwx   0        0        0        0 2024-05-21 02:25:01.261643 arch_flow-0.1.7.3/arch_flow.egg-info/
+-rw-rw-rw-   0        0        0      983 2024-05-21 02:25:01.000000 arch_flow-0.1.7.3/arch_flow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      803 2024-05-21 02:25:01.000000 arch_flow-0.1.7.3/arch_flow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 02:25:01.000000 arch_flow-0.1.7.3/arch_flow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-21 02:25:01.000000 arch_flow-0.1.7.3/arch_flow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 02:25:01.000000 arch_flow-0.1.7.3/arch_flow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 02:25:01.264645 arch_flow-0.1.7.3/setup.cfg
+-rw-rw-rw-   0        0        0     1246 2024-05-21 02:24:58.000000 arch_flow-0.1.7.3/setup.py
```

### Comparing `arch_flow-0.1.7.2/LICENCE` & `arch_flow-0.1.7.3/LICENCE`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/PKG-INFO` & `arch_flow-0.1.7.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.7.2
+Version: 0.1.7.3
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `arch_flow-0.1.7.2/README.md` & `arch_flow-0.1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/arch_flow/ArchFlow.py` & `arch_flow-0.1.7.3/arch_flow/ArchFlow.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from arch_flow.DirectoryCreator import DirectoryCreator
 from arch_flow.DirectoryExplorer import DirectoryExplorer
 from arch_flow.StringManipulator import StringManipulator
 from arch_flow.utils.Filter import Filter
 from arch_flow.output.OutputHandler import OutputHandler
 import sys
 import os
-
+import json
 
 filter = Filter()
 
 
 class ArchFlow(ABC):
     def __init__(self):
         self.DirectoryCreator = DirectoryCreator()
@@ -31,18 +31,29 @@
         self.DirectoryCreator.create_file(file_destination, file_name, content)
 
     @staticmethod
     def handle_args():
         return sys.argv[1:]
 
     def handler_functions_flow(self, args, json_functions=None):
-        json_content = ""
+        combined_json_content = {}
+
         for json_root_path in json_functions:
-            json_content += self.DirectoryExplorer.read_json_file(json_root_path)
-        self.handler_input(args, json_content)
+            json_data = self.DirectoryExplorer.read_json_file(json_root_path)
+            for key, value in json_data.items():
+                if key in combined_json_content:
+                    # Gerencie conflitos de chaves aqui, por exemplo, transformando valores em listas
+                    if isinstance(combined_json_content[key], list):
+                        combined_json_content[key].append(value)
+                    else:
+                        combined_json_content[key] = [combined_json_content[key], value]
+                else:
+                    combined_json_content[key] = value
+
+        self.handler_input(args, combined_json_content)
 
     def handler_input(self, args, json_content):
         if len(args) == 0:
             self.OutputHandler.information_message("Whoopsie-daisy! It seems like you forgot to provide a function. "
                                                "How about trying --help for some magic commands?")
             return None
         name_function = args[0]
```

### Comparing `arch_flow-0.1.7.2/arch_flow/DirectoryCreator.py` & `arch_flow-0.1.7.3/arch_flow/DirectoryCreator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/arch_flow/DirectoryExplorer.py` & `arch_flow-0.1.7.3/arch_flow/DirectoryExplorer.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/arch_flow/StringManipulator.py` & `arch_flow-0.1.7.3/arch_flow/StringManipulator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/arch_flow/exceptions/ExceptionHandler.py` & `arch_flow-0.1.7.3/arch_flow/exceptions/ExceptionHandler.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/arch_flow/exceptions/FileOrDirectoryExistsError.py` & `arch_flow-0.1.7.3/arch_flow/exceptions/FileOrDirectoryExistsError.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/arch_flow/exceptions/NotFoundException.py` & `arch_flow-0.1.7.3/arch_flow/exceptions/NotFoundException.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/arch_flow/implementations/DirectoryCreatorImplementation.py` & `arch_flow-0.1.7.3/arch_flow/implementations/DirectoryCreatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/arch_flow/implementations/DirectoryExplorerImplementation.py` & `arch_flow-0.1.7.3/arch_flow/implementations/DirectoryExplorerImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/arch_flow/implementations/StringManipulatorImplementation.py` & `arch_flow-0.1.7.3/arch_flow/implementations/StringManipulatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/arch_flow/output/OutputHandler.py` & `arch_flow-0.1.7.3/arch_flow/output/OutputHandler.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/arch_flow/utils/Filter.py` & `arch_flow-0.1.7.3/arch_flow/utils/Filter.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/arch_flow.egg-info/PKG-INFO` & `arch_flow-0.1.7.3/arch_flow.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.7.2
+Version: 0.1.7.3
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `arch_flow-0.1.7.2/arch_flow.egg-info/SOURCES.txt` & `arch_flow-0.1.7.3/arch_flow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7.2/setup.py` & `arch_flow-0.1.7.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='arch-flow',
-    version='0.1.7.2',
+    version='0.1.7.3',
     license='MIT License',
     author='Carlos Vinicius Da Silva',
     long_description="O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações. Inspirado no conceito de peças de Lego, o ArchFlow oferece uma variedade de módulos independentes, cada um com funcionalidades específicas. Esses módulos podem ser combinados de forma flexível para atender às necessidades de automação de diferentes projetos. Com uma arquitetura modular e uma ampla gama de funções, o ArchFlow permite aos desenvolvedores criar soluções eficientes e personalizadas, reduzindo o tempo e esforço necessários para o desenvolvimento de software.",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='arch flow',
     description=u'O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.',
```

