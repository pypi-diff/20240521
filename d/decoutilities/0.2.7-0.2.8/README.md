# Comparing `tmp/decoutilities-0.2.7.tar.gz` & `tmp/decoutilities-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.2.7.tar", last modified: Mon May 20 12:18:46 2024, max compression
+gzip compressed data, was "decoutilities-0.2.8.tar", last modified: Mon May 20 22:21:50 2024, max compression
```

## Comparing `decoutilities-0.2.7.tar` & `decoutilities-0.2.8.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.399621 decoutilities-0.2.7/
--rw-rw-rw-   0        0        0     1089 2024-05-08 11:01:18.000000 decoutilities-0.2.7/LICENSE
--rw-rw-rw-   0        0        0    15668 2024-05-20 12:18:46.383619 decoutilities-0.2.7/PKG-INFO
--rw-rw-rw-   0        0        0    15197 2024-05-20 11:56:43.000000 decoutilities-0.2.7/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.023620 decoutilities-0.2.7/decoutilities/
--rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.2.7/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.181621 decoutilities-0.2.7/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.7/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.7/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.7/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.248620 decoutilities-0.2.7/decoutilities/data/
--rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.2.7/decoutilities/data/__init__.py
--rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.2.7/decoutilities/data/dataEncryptor.py
--rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.2.7/decoutilities/data/keyManager.py
-drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.284620 decoutilities-0.2.7/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.7/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      569 2024-05-20 10:37:54.000000 decoutilities-0.2.7/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.301620 decoutilities-0.2.7/decoutilities/logger/
--rw-rw-rw-   0        0        0     1272 2024-05-20 12:16:35.000000 decoutilities-0.2.7/decoutilities/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.320621 decoutilities-0.2.7/decoutilities/queue/
--rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.2.7/decoutilities/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.334620 decoutilities-0.2.7/decoutilities/textUtils/
--rw-rw-rw-   0        0        0     2427 2024-05-20 10:37:30.000000 decoutilities-0.2.7/decoutilities/textUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 12:18:46.367620 decoutilities-0.2.7/decoutilities.egg-info/
--rw-rw-rw-   0        0        0    15668 2024-05-20 12:18:45.000000 decoutilities-0.2.7/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2024-05-20 12:18:45.000000 decoutilities-0.2.7/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 12:18:45.000000 decoutilities-0.2.7/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-20 12:18:45.000000 decoutilities-0.2.7/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 12:18:46.399621 decoutilities-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-20 12:18:16.000000 decoutilities-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.423959 decoutilities-0.2.8/
+-rw-rw-rw-   0        0        0     1089 2024-05-08 22:21:06.000000 decoutilities-0.2.8/LICENSE
+-rw-rw-rw-   0        0        0    15668 2024-05-20 22:21:50.422903 decoutilities-0.2.8/PKG-INFO
+-rw-rw-rw-   0        0        0    15197 2024-05-20 22:20:37.000000 decoutilities-0.2.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.403977 decoutilities-0.2.8/decoutilities/
+-rw-rw-rw-   0        0        0     4740 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.410290 decoutilities-0.2.8/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2736 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.413965 decoutilities-0.2.8/decoutilities/data/
+-rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/data/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/data/dataEncryptor.py
+-rw-rw-rw-   0        0        0     1671 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/data/keyManager.py
+drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.417125 decoutilities-0.2.8/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-05-18 20:23:23.000000 decoutilities-0.2.8/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.418176 decoutilities-0.2.8/decoutilities/logger/
+-rw-rw-rw-   0        0        0     1244 2024-05-20 22:20:37.000000 decoutilities-0.2.8/decoutilities/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.419232 decoutilities-0.2.8/decoutilities/queue/
+-rw-rw-rw-   0        0        0     1043 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.420291 decoutilities-0.2.8/decoutilities/textUtils/
+-rw-rw-rw-   0        0        0     2427 2024-05-20 22:20:37.000000 decoutilities-0.2.8/decoutilities/textUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.421337 decoutilities-0.2.8/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0    15668 2024-05-20 22:21:50.000000 decoutilities-0.2.8/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-05-20 22:21:50.000000 decoutilities-0.2.8/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 22:21:50.000000 decoutilities-0.2.8/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-20 22:21:50.000000 decoutilities-0.2.8/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-20 22:21:50.423959 decoutilities-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-20 22:20:37.000000 decoutilities-0.2.8/setup.py
```

### Comparing `decoutilities-0.2.7/LICENSE` & `decoutilities-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.7/PKG-INFO` & `decoutilities-0.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.7
+Version: 0.2.8
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.2.7/README.md` & `decoutilities-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.7/decoutilities/__init__.py` & `decoutilities-0.2.8/decoutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.7/decoutilities/config/config.py` & `decoutilities-0.2.8/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.7/decoutilities/config/configContainer.py` & `decoutilities-0.2.8/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.7/decoutilities/data/dataEncryptor.py` & `decoutilities-0.2.8/decoutilities/data/dataEncryptor.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.7/decoutilities/data/keyManager.py` & `decoutilities-0.2.8/decoutilities/data/keyManager.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.7/decoutilities/inject/injector.py` & `decoutilities-0.2.8/decoutilities/inject/injector.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.7/decoutilities/logger/__init__.py` & `decoutilities-0.2.8/decoutilities/logger/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             with open(self.log, "a") as file:
                 file.write(message + "\n")
 
     def __log(self, event, message):
         if self.prefix is not None:
             event = self.prefix + " " + event
         message = self.text_utils.format(message)
-        formatted_message = self.format.format(event=event, message=message)
+        formatted_message = f"{event} {message}"
         print(formatted_message)
         self.__toLogFile(formatted_message)
     
     def info(self, message):
         self.__log("INFO", message)
 
     def warning(self, message):
```

### Comparing `decoutilities-0.2.7/decoutilities/queue/__init__.py` & `decoutilities-0.2.8/decoutilities/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.7/decoutilities/textUtils/__init__.py` & `decoutilities-0.2.8/decoutilities/textUtils/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.7/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.2.8/decoutilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.7
+Version: 0.2.8
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.2.7/decoutilities.egg-info/SOURCES.txt` & `decoutilities-0.2.8/decoutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.7/setup.py` & `decoutilities-0.2.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.2.7',
+version='0.2.8',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

