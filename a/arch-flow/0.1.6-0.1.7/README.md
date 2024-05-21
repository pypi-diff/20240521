# Comparing `tmp/arch_flow-0.1.6.tar.gz` & `tmp/arch_flow-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch_flow-0.1.6.tar", last modified: Tue May  7 14:35:01 2024, max compression
+gzip compressed data, was "arch_flow-0.1.7.tar", last modified: Tue May 21 01:26:44 2024, max compression
```

## Comparing `arch_flow-0.1.6.tar` & `arch_flow-0.1.7.tar`

### file list

```diff
@@ -1,31 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-07 14:35:01.308359 arch_flow-0.1.6/
--rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.6/LICENCE
--rw-rw-rw-   0        0        0      981 2024-05-07 14:35:01.306848 arch_flow-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     6622 2024-04-25 23:30:53.000000 arch_flow-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-07 14:35:01.216693 arch_flow-0.1.6/arch_flow/
--rw-rw-rw-   0        0        0     4328 2024-05-07 14:34:58.000000 arch_flow-0.1.6/arch_flow/ArchFlow.py
--rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.6/arch_flow/DirectoryCreator.py
--rw-rw-rw-   0        0        0     3301 2024-05-04 03:27:18.000000 arch_flow-0.1.6/arch_flow/DirectoryExplorer.py
--rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.6/arch_flow/StringManipulator.py
--rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.6/arch_flow/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-07 14:35:01.254910 arch_flow-0.1.6/arch_flow/exceptions/
--rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.6/arch_flow/exceptions/ExceptionHandler.py
--rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.6/arch_flow/exceptions/FileOrDirectoryExistsError.py
--rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.6/arch_flow/exceptions/NotFoundException.py
-drwxrwxrwx   0        0        0        0 2024-05-07 14:35:01.280526 arch_flow-0.1.6/arch_flow/implementations/
--rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.6/arch_flow/implementations/DirectoryCreatorImplementation.py
--rw-rw-rw-   0        0        0     7196 2024-04-21 05:43:57.000000 arch_flow-0.1.6/arch_flow/implementations/DirectoryExplorerImplementation.py
--rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.6/arch_flow/implementations/StringManipulatorImplementation.py
-drwxrwxrwx   0        0        0        0 2024-05-07 14:35:01.289594 arch_flow-0.1.6/arch_flow/output/
--rw-rw-rw-   0        0        0     2372 2024-03-15 22:56:29.000000 arch_flow-0.1.6/arch_flow/output/OutputHandler.py
-drwxrwxrwx   0        0        0        0 2024-05-07 14:35:01.303849 arch_flow-0.1.6/arch_flow/utils/
--rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.6/arch_flow/utils/DirectoryExplorerUtil.py
--rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.6/arch_flow/utils/Filter.py
-drwxrwxrwx   0        0        0        0 2024-05-07 14:35:01.305849 arch_flow-0.1.6/arch_flow.egg-info/
--rw-rw-rw-   0        0        0      981 2024-05-07 14:35:00.000000 arch_flow-0.1.6/arch_flow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      743 2024-05-07 14:35:01.000000 arch_flow-0.1.6/arch_flow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-07 14:35:00.000000 arch_flow-0.1.6/arch_flow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-07 14:35:00.000000 arch_flow-0.1.6/arch_flow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-07 14:35:00.000000 arch_flow-0.1.6/arch_flow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-07 14:35:01.308359 arch_flow-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1182 2024-05-07 14:34:58.000000 arch_flow-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.731464 arch_flow-0.1.7/
+-rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.7/LICENCE
+-rw-rw-rw-   0        0        0      981 2024-05-21 01:26:44.729466 arch_flow-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6622 2024-04-25 23:30:53.000000 arch_flow-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.638187 arch_flow-0.1.7/arch_flow/
+-rw-rw-rw-   0        0        0     4601 2024-05-21 01:17:31.000000 arch_flow-0.1.7/arch_flow/ArchFlow.py
+-rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/DirectoryCreator.py
+-rw-rw-rw-   0        0        0     3301 2024-05-04 03:27:18.000000 arch_flow-0.1.7/arch_flow/DirectoryExplorer.py
+-rw-rw-rw-   0        0        0      291 2024-05-21 01:26:37.000000 arch_flow-0.1.7/arch_flow/Run.py
+-rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/StringManipulator.py
+-rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.7/arch_flow/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.686347 arch_flow-0.1.7/arch_flow/exceptions/
+-rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/exceptions/ExceptionHandler.py
+-rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/exceptions/FileOrDirectoryExistsError.py
+-rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/exceptions/NotFoundException.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.708897 arch_flow-0.1.7/arch_flow/implementations/
+-rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/implementations/DirectoryCreatorImplementation.py
+-rw-rw-rw-   0        0        0     7196 2024-04-21 05:43:57.000000 arch_flow-0.1.7/arch_flow/implementations/DirectoryExplorerImplementation.py
+-rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.7/arch_flow/implementations/StringManipulatorImplementation.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.718408 arch_flow-0.1.7/arch_flow/output/
+-rw-rw-rw-   0        0        0     2372 2024-03-15 22:56:29.000000 arch_flow-0.1.7/arch_flow/output/OutputHandler.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.727409 arch_flow-0.1.7/arch_flow/utils/
+-rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.7/arch_flow/utils/DirectoryExplorerUtil.py
+-rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/utils/Filter.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.728462 arch_flow-0.1.7/arch_flow.egg-info/
+-rw-rw-rw-   0        0        0      981 2024-05-21 01:26:44.000000 arch_flow-0.1.7/arch_flow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      760 2024-05-21 01:26:44.000000 arch_flow-0.1.7/arch_flow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 01:26:44.000000 arch_flow-0.1.7/arch_flow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-21 01:26:44.000000 arch_flow-0.1.7/arch_flow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 01:26:44.000000 arch_flow-0.1.7/arch_flow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 01:26:44.731464 arch_flow-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1182 2024-05-21 01:26:37.000000 arch_flow-0.1.7/setup.py
```

### Comparing `arch_flow-0.1.6/LICENCE` & `arch_flow-0.1.7/LICENCE`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.6/PKG-INFO` & `arch_flow-0.1.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.6
+Version: 0.1.7
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `arch_flow-0.1.6/README.md` & `arch_flow-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.6/arch_flow/ArchFlow.py` & `arch_flow-0.1.7/arch_flow/ArchFlow.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,20 @@
         content = self.StringManipulator.replace_tags(content)
         self.DirectoryCreator.create_file(file_destination, file_name, content)
 
     @staticmethod
     def handle_args():
         return sys.argv[1:]
 
+    def handler_functions_flow(self, args, json_functions=None):
+        json_content = ""
+        for json_root_path in json_functions:
+            json_content += self.DirectoryExplorer.read_json_file(json_root_path)
+        self.handler_input(args, json_content)
+
     def handler_input(self, args, json_content):
         if len(args) == 0:
             self.OutputHandler.information_message("Whoopsie-daisy! It seems like you forgot to provide a function. "
                                                "How about trying --help for some magic commands?")
             return None
         name_function = args[0]
```

### Comparing `arch_flow-0.1.6/arch_flow/DirectoryCreator.py` & `arch_flow-0.1.7/arch_flow/DirectoryCreator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.6/arch_flow/DirectoryExplorer.py` & `arch_flow-0.1.7/arch_flow/DirectoryExplorer.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.6/arch_flow/StringManipulator.py` & `arch_flow-0.1.7/arch_flow/StringManipulator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.6/arch_flow/exceptions/ExceptionHandler.py` & `arch_flow-0.1.7/arch_flow/exceptions/ExceptionHandler.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.6/arch_flow/exceptions/FileOrDirectoryExistsError.py` & `arch_flow-0.1.7/arch_flow/exceptions/FileOrDirectoryExistsError.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.6/arch_flow/exceptions/NotFoundException.py` & `arch_flow-0.1.7/arch_flow/exceptions/NotFoundException.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.6/arch_flow/implementations/DirectoryCreatorImplementation.py` & `arch_flow-0.1.7/arch_flow/implementations/DirectoryCreatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.6/arch_flow/implementations/DirectoryExplorerImplementation.py` & `arch_flow-0.1.7/arch_flow/implementations/DirectoryExplorerImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.6/arch_flow/implementations/StringManipulatorImplementation.py` & `arch_flow-0.1.7/arch_flow/implementations/StringManipulatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.6/arch_flow/output/OutputHandler.py` & `arch_flow-0.1.7/arch_flow/output/OutputHandler.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.6/arch_flow/utils/Filter.py` & `arch_flow-0.1.7/arch_flow/utils/Filter.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.6/arch_flow.egg-info/PKG-INFO` & `arch_flow-0.1.7/arch_flow.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.6
+Version: 0.1.7
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `arch_flow-0.1.6/arch_flow.egg-info/SOURCES.txt` & `arch_flow-0.1.7/arch_flow.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 LICENCE
 README.md
 setup.py
 arch_flow/ArchFlow.py
 arch_flow/DirectoryCreator.py
 arch_flow/DirectoryExplorer.py
+arch_flow/Run.py
 arch_flow/StringManipulator.py
 arch_flow/__init__.py
 arch_flow.egg-info/PKG-INFO
 arch_flow.egg-info/SOURCES.txt
 arch_flow.egg-info/dependency_links.txt
 arch_flow.egg-info/requires.txt
 arch_flow.egg-info/top_level.txt
```

### Comparing `arch_flow-0.1.6/setup.py` & `arch_flow-0.1.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='arch-flow',
-    version='0.1.6',
+    version='0.1.7',
     license='MIT License',
     author='Carlos Vinicius Da Silva',
     long_description="O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações. Inspirado no conceito de peças de Lego, o ArchFlow oferece uma variedade de módulos independentes, cada um com funcionalidades específicas. Esses módulos podem ser combinados de forma flexível para atender às necessidades de automação de diferentes projetos. Com uma arquitetura modular e uma ampla gama de funções, o ArchFlow permite aos desenvolvedores criar soluções eficientes e personalizadas, reduzindo o tempo e esforço necessários para o desenvolvimento de software.",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='arch flow',
     description=u'O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.',
```

