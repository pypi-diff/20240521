# Comparing `tmp/decoutilities-0.2.6.tar.gz` & `tmp/decoutilities-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.2.6.tar", last modified: Mon May 20 11:57:12 2024, max compression
+gzip compressed data, was "decoutilities-0.2.7.tar", last modified: Mon May 20 12:18:46 2024, max compression
```

## Comparing `decoutilities-0.2.6.tar` & `decoutilities-0.2.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.375856 decoutilities-0.2.6/
--rw-rw-rw-   0        0        0     1089 2024-05-08 11:01:18.000000 decoutilities-0.2.6/LICENSE
--rw-rw-rw-   0        0        0    15668 2024-05-20 11:57:12.360853 decoutilities-0.2.6/PKG-INFO
--rw-rw-rw-   0        0        0    15197 2024-05-20 11:56:43.000000 decoutilities-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.018468 decoutilities-0.2.6/decoutilities/
--rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.2.6/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.171467 decoutilities-0.2.6/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.6/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.6/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.6/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.225471 decoutilities-0.2.6/decoutilities/data/
--rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.2.6/decoutilities/data/__init__.py
--rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.2.6/decoutilities/data/dataEncryptor.py
--rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.2.6/decoutilities/data/keyManager.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.266468 decoutilities-0.2.6/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.6/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      569 2024-05-20 10:37:54.000000 decoutilities-0.2.6/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.282856 decoutilities-0.2.6/decoutilities/logger/
--rw-rw-rw-   0        0        0     1212 2024-05-20 11:36:36.000000 decoutilities-0.2.6/decoutilities/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.314856 decoutilities-0.2.6/decoutilities/queue/
--rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.2.6/decoutilities/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.326855 decoutilities-0.2.6/decoutilities/textUtils/
--rw-rw-rw-   0        0        0     2427 2024-05-20 10:37:30.000000 decoutilities-0.2.6/decoutilities/textUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 11:57:12.346855 decoutilities-0.2.6/decoutilities.egg-info/
--rw-rw-rw-   0        0        0    15668 2024-05-20 11:57:11.000000 decoutilities-0.2.6/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2024-05-20 11:57:11.000000 decoutilities-0.2.6/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 11:57:11.000000 decoutilities-0.2.6/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-20 11:57:11.000000 decoutilities-0.2.6/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 11:57:12.376853 decoutilities-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-20 11:56:57.000000 decoutilities-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.399621 decoutilities-0.2.7/
+-rw-rw-rw-   0        0        0     1089 2024-05-08 11:01:18.000000 decoutilities-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0    15668 2024-05-20 12:18:46.383619 decoutilities-0.2.7/PKG-INFO
+-rw-rw-rw-   0        0        0    15197 2024-05-20 11:56:43.000000 decoutilities-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.023620 decoutilities-0.2.7/decoutilities/
+-rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.2.7/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.181621 decoutilities-0.2.7/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.7/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.7/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.7/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.248620 decoutilities-0.2.7/decoutilities/data/
+-rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.2.7/decoutilities/data/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.2.7/decoutilities/data/dataEncryptor.py
+-rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.2.7/decoutilities/data/keyManager.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.284620 decoutilities-0.2.7/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.7/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-05-20 10:37:54.000000 decoutilities-0.2.7/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.301620 decoutilities-0.2.7/decoutilities/logger/
+-rw-rw-rw-   0        0        0     1272 2024-05-20 12:16:35.000000 decoutilities-0.2.7/decoutilities/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.320621 decoutilities-0.2.7/decoutilities/queue/
+-rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.2.7/decoutilities/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.334620 decoutilities-0.2.7/decoutilities/textUtils/
+-rw-rw-rw-   0        0        0     2427 2024-05-20 10:37:30.000000 decoutilities-0.2.7/decoutilities/textUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.367620 decoutilities-0.2.7/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0    15668 2024-05-20 12:18:45.000000 decoutilities-0.2.7/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-05-20 12:18:45.000000 decoutilities-0.2.7/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 12:18:45.000000 decoutilities-0.2.7/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 12:18:45.000000 decoutilities-0.2.7/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 12:18:46.399621 decoutilities-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-20 12:18:16.000000 decoutilities-0.2.7/setup.py
```

### Comparing `decoutilities-0.2.6/LICENSE` & `decoutilities-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.6/PKG-INFO` & `decoutilities-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.6
+Version: 0.2.7
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.2.6/README.md` & `decoutilities-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.6/decoutilities/__init__.py` & `decoutilities-0.2.7/decoutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.6/decoutilities/config/config.py` & `decoutilities-0.2.7/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.6/decoutilities/config/configContainer.py` & `decoutilities-0.2.7/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.6/decoutilities/data/dataEncryptor.py` & `decoutilities-0.2.7/decoutilities/data/dataEncryptor.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.6/decoutilities/data/keyManager.py` & `decoutilities-0.2.7/decoutilities/data/keyManager.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.6/decoutilities/inject/injector.py` & `decoutilities-0.2.7/decoutilities/inject/injector.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.6/decoutilities/logger/__init__.py` & `decoutilities-0.2.7/decoutilities/logger/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 from ..textUtils import textUtils
 
 class Logger:
     def __init__(self, prefix = None, debug=False, log = None, format = "{event} {white}| {message}"):
         self.prefix = prefix
         self.log = log
-        self.format = textUtils.format
+        self.format = format
         self.debug = debug
+        self.text_utils = textUtils()
 
     def  __toLogFile(self, message):
         if self.log is not None:
             with open(self.log, "a") as file:
                 file.write(message + "\n")
 
     def __log(self, event, message):
         if self.prefix is not None:
             event = self.prefix + " " + event
-        message = self.format(message)
-        message = self.format(self.format, event = event, message = message)
-        print(message)
-        self.__toLogFile(message)
+        message = self.text_utils.format(message)
+        formatted_message = self.format.format(event=event, message=message)
+        print(formatted_message)
+        self.__toLogFile(formatted_message)
     
     def info(self, message):
         self.__log("INFO", message)
 
     def warning(self, message):
         self.__log("WARNING", message)
```

### Comparing `decoutilities-0.2.6/decoutilities/queue/__init__.py` & `decoutilities-0.2.7/decoutilities/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.6/decoutilities/textUtils/__init__.py` & `decoutilities-0.2.7/decoutilities/textUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.6/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.2.7/decoutilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.6
+Version: 0.2.7
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.2.6/decoutilities.egg-info/SOURCES.txt` & `decoutilities-0.2.7/decoutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.6/setup.py` & `decoutilities-0.2.7/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.2.6',
+version='0.2.7',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

