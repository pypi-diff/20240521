# Comparing `tmp/arch_flow-0.1.7.tar.gz` & `tmp/arch_flow-0.1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arch_flow-0.1.7.tar", last modified: Tue May 21 01:26:44 2024, max compression
+gzip compressed data, was "arch_flow-0.1.7.1.tar", last modified: Tue May 21 01:50:17 2024, max compression
```

## Comparing `arch_flow-0.1.7.tar` & `arch_flow-0.1.7.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.731464 arch_flow-0.1.7/
--rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.7/LICENCE
--rw-rw-rw-   0        0        0      981 2024-05-21 01:26:44.729466 arch_flow-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     6622 2024-04-25 23:30:53.000000 arch_flow-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.638187 arch_flow-0.1.7/arch_flow/
--rw-rw-rw-   0        0        0     4601 2024-05-21 01:17:31.000000 arch_flow-0.1.7/arch_flow/ArchFlow.py
--rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/DirectoryCreator.py
--rw-rw-rw-   0        0        0     3301 2024-05-04 03:27:18.000000 arch_flow-0.1.7/arch_flow/DirectoryExplorer.py
--rw-rw-rw-   0        0        0      291 2024-05-21 01:26:37.000000 arch_flow-0.1.7/arch_flow/Run.py
--rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/StringManipulator.py
--rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.7/arch_flow/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.686347 arch_flow-0.1.7/arch_flow/exceptions/
--rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/exceptions/ExceptionHandler.py
--rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/exceptions/FileOrDirectoryExistsError.py
--rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/exceptions/NotFoundException.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.708897 arch_flow-0.1.7/arch_flow/implementations/
--rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/implementations/DirectoryCreatorImplementation.py
--rw-rw-rw-   0        0        0     7196 2024-04-21 05:43:57.000000 arch_flow-0.1.7/arch_flow/implementations/DirectoryExplorerImplementation.py
--rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.7/arch_flow/implementations/StringManipulatorImplementation.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.718408 arch_flow-0.1.7/arch_flow/output/
--rw-rw-rw-   0        0        0     2372 2024-03-15 22:56:29.000000 arch_flow-0.1.7/arch_flow/output/OutputHandler.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.727409 arch_flow-0.1.7/arch_flow/utils/
--rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.7/arch_flow/utils/DirectoryExplorerUtil.py
--rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.7/arch_flow/utils/Filter.py
-drwxrwxrwx   0        0        0        0 2024-05-21 01:26:44.728462 arch_flow-0.1.7/arch_flow.egg-info/
--rw-rw-rw-   0        0        0      981 2024-05-21 01:26:44.000000 arch_flow-0.1.7/arch_flow.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      760 2024-05-21 01:26:44.000000 arch_flow-0.1.7/arch_flow.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 01:26:44.000000 arch_flow-0.1.7/arch_flow.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-21 01:26:44.000000 arch_flow-0.1.7/arch_flow.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-21 01:26:44.000000 arch_flow-0.1.7/arch_flow.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 01:26:44.731464 arch_flow-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1182 2024-05-21 01:26:37.000000 arch_flow-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:50:17.252970 arch_flow-0.1.7.1/
+-rw-rw-rw-   0        0        0     1109 2024-04-16 05:07:31.000000 arch_flow-0.1.7.1/LICENCE
+-rw-rw-rw-   0        0        0      983 2024-05-21 01:50:17.251971 arch_flow-0.1.7.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6622 2024-04-25 23:30:53.000000 arch_flow-0.1.7.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 01:50:17.213835 arch_flow-0.1.7.1/arch_flow/
+-rw-rw-rw-   0        0        0     4601 2024-05-21 01:17:31.000000 arch_flow-0.1.7.1/arch_flow/ArchFlow.py
+-rw-rw-rw-   0        0        0      216 2024-05-21 01:50:14.000000 arch_flow-0.1.7.1/arch_flow/ArchFlowCli.py
+-rw-rw-rw-   0        0        0      877 2024-04-16 07:34:12.000000 arch_flow-0.1.7.1/arch_flow/DirectoryCreator.py
+-rw-rw-rw-   0        0        0     3301 2024-05-04 03:27:18.000000 arch_flow-0.1.7.1/arch_flow/DirectoryExplorer.py
+-rw-rw-rw-   0        0        0      291 2024-05-21 01:26:37.000000 arch_flow-0.1.7.1/arch_flow/Run.py
+-rw-rw-rw-   0        0        0     3130 2024-04-16 07:34:12.000000 arch_flow-0.1.7.1/arch_flow/StringManipulator.py
+-rw-rw-rw-   0        0        0       32 2024-04-16 07:33:26.000000 arch_flow-0.1.7.1/arch_flow/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:50:17.241451 arch_flow-0.1.7.1/arch_flow/exceptions/
+-rw-rw-rw-   0        0        0      594 2024-04-16 07:34:12.000000 arch_flow-0.1.7.1/arch_flow/exceptions/ExceptionHandler.py
+-rw-rw-rw-   0        0        0     1132 2024-04-16 07:34:12.000000 arch_flow-0.1.7.1/arch_flow/exceptions/FileOrDirectoryExistsError.py
+-rw-rw-rw-   0        0        0      631 2024-04-16 07:34:12.000000 arch_flow-0.1.7.1/arch_flow/exceptions/NotFoundException.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:50:17.245450 arch_flow-0.1.7.1/arch_flow/implementations/
+-rw-rw-rw-   0        0        0     2191 2024-04-16 07:34:12.000000 arch_flow-0.1.7.1/arch_flow/implementations/DirectoryCreatorImplementation.py
+-rw-rw-rw-   0        0        0     7196 2024-04-21 05:43:57.000000 arch_flow-0.1.7.1/arch_flow/implementations/DirectoryExplorerImplementation.py
+-rw-rw-rw-   0        0        0     7653 2024-03-15 22:56:29.000000 arch_flow-0.1.7.1/arch_flow/implementations/StringManipulatorImplementation.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:50:17.246957 arch_flow-0.1.7.1/arch_flow/output/
+-rw-rw-rw-   0        0        0     2372 2024-03-15 22:56:29.000000 arch_flow-0.1.7.1/arch_flow/output/OutputHandler.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:50:17.248973 arch_flow-0.1.7.1/arch_flow/utils/
+-rw-rw-rw-   0        0        0      470 2024-03-15 22:56:29.000000 arch_flow-0.1.7.1/arch_flow/utils/DirectoryExplorerUtil.py
+-rw-rw-rw-   0        0        0     1801 2024-04-16 07:34:12.000000 arch_flow-0.1.7.1/arch_flow/utils/Filter.py
+drwxrwxrwx   0        0        0        0 2024-05-21 01:50:17.250974 arch_flow-0.1.7.1/arch_flow.egg-info/
+-rw-rw-rw-   0        0        0      983 2024-05-21 01:50:17.000000 arch_flow-0.1.7.1/arch_flow.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      785 2024-05-21 01:50:17.000000 arch_flow-0.1.7.1/arch_flow.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 01:50:17.000000 arch_flow-0.1.7.1/arch_flow.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-21 01:50:17.000000 arch_flow-0.1.7.1/arch_flow.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 01:50:17.000000 arch_flow-0.1.7.1/arch_flow.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 01:50:17.253970 arch_flow-0.1.7.1/setup.cfg
+-rw-rw-rw-   0        0        0     1184 2024-05-21 01:50:14.000000 arch_flow-0.1.7.1/setup.py
```

### Comparing `arch_flow-0.1.7/LICENCE` & `arch_flow-0.1.7.1/LICENCE`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/PKG-INFO` & `arch_flow-0.1.7.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `arch_flow-0.1.7/README.md` & `arch_flow-0.1.7.1/README.md`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/arch_flow/ArchFlow.py` & `arch_flow-0.1.7.1/arch_flow/ArchFlow.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/arch_flow/DirectoryCreator.py` & `arch_flow-0.1.7.1/arch_flow/DirectoryCreator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/arch_flow/DirectoryExplorer.py` & `arch_flow-0.1.7.1/arch_flow/DirectoryExplorer.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/arch_flow/StringManipulator.py` & `arch_flow-0.1.7.1/arch_flow/StringManipulator.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/arch_flow/exceptions/ExceptionHandler.py` & `arch_flow-0.1.7.1/arch_flow/exceptions/ExceptionHandler.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/arch_flow/exceptions/FileOrDirectoryExistsError.py` & `arch_flow-0.1.7.1/arch_flow/exceptions/FileOrDirectoryExistsError.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/arch_flow/exceptions/NotFoundException.py` & `arch_flow-0.1.7.1/arch_flow/exceptions/NotFoundException.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/arch_flow/implementations/DirectoryCreatorImplementation.py` & `arch_flow-0.1.7.1/arch_flow/implementations/DirectoryCreatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/arch_flow/implementations/DirectoryExplorerImplementation.py` & `arch_flow-0.1.7.1/arch_flow/implementations/DirectoryExplorerImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/arch_flow/implementations/StringManipulatorImplementation.py` & `arch_flow-0.1.7.1/arch_flow/implementations/StringManipulatorImplementation.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/arch_flow/output/OutputHandler.py` & `arch_flow-0.1.7.1/arch_flow/output/OutputHandler.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/arch_flow/utils/Filter.py` & `arch_flow-0.1.7.1/arch_flow/utils/Filter.py`

 * *Files identical despite different names*

### Comparing `arch_flow-0.1.7/arch_flow.egg-info/PKG-INFO` & `arch_flow-0.1.7.1/arch_flow.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arch-flow
-Version: 0.1.7
+Version: 0.1.7.1
 Summary: O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.
 Author: Carlos Vinicius Da Silva
 Author-email: vini989073599@gmail.com
 License: MIT License
 Keywords: arch flow
 Description-Content-Type: text/markdown
 License-File: LICENCE
```

### Comparing `arch_flow-0.1.7/arch_flow.egg-info/SOURCES.txt` & `arch_flow-0.1.7.1/arch_flow.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENCE
 README.md
 setup.py
 arch_flow/ArchFlow.py
+arch_flow/ArchFlowCli.py
 arch_flow/DirectoryCreator.py
 arch_flow/DirectoryExplorer.py
 arch_flow/Run.py
 arch_flow/StringManipulator.py
 arch_flow/__init__.py
 arch_flow.egg-info/PKG-INFO
 arch_flow.egg-info/SOURCES.txt
```

### Comparing `arch_flow-0.1.7/setup.py` & `arch_flow-0.1.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='arch-flow',
-    version='0.1.7',
+    version='0.1.7.1',
     license='MIT License',
     author='Carlos Vinicius Da Silva',
     long_description="O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações. Inspirado no conceito de peças de Lego, o ArchFlow oferece uma variedade de módulos independentes, cada um com funcionalidades específicas. Esses módulos podem ser combinados de forma flexível para atender às necessidades de automação de diferentes projetos. Com uma arquitetura modular e uma ampla gama de funções, o ArchFlow permite aos desenvolvedores criar soluções eficientes e personalizadas, reduzindo o tempo e esforço necessários para o desenvolvimento de software.",
     long_description_content_type="text/markdown",
     author_email='vini989073599@gmail.com',
     keywords='arch flow',
     description=u'O ArchFlow é uma plataforma de código aberto projetada para simplificar o desenvolvimento de automações.',
```

