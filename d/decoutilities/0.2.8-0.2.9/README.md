# Comparing `tmp/decoutilities-0.2.8.tar.gz` & `tmp/decoutilities-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoutilities-0.2.8.tar", last modified: Mon May 20 22:21:50 2024, max compression
+gzip compressed data, was "decoutilities-0.2.9.tar", last modified: Tue May 21 06:17:47 2024, max compression
```

## Comparing `decoutilities-0.2.8.tar` & `decoutilities-0.2.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.423959 decoutilities-0.2.8/
--rw-rw-rw-   0        0        0     1089 2024-05-08 22:21:06.000000 decoutilities-0.2.8/LICENSE
--rw-rw-rw-   0        0        0    15668 2024-05-20 22:21:50.422903 decoutilities-0.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    15197 2024-05-20 22:20:37.000000 decoutilities-0.2.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.403977 decoutilities-0.2.8/decoutilities/
--rw-rw-rw-   0        0        0     4740 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.410290 decoutilities-0.2.8/decoutilities/config/
--rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/config/__init__.py
--rw-rw-rw-   0        0        0      994 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/config/config.py
--rw-rw-rw-   0        0        0     2736 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/config/configContainer.py
-drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.413965 decoutilities-0.2.8/decoutilities/data/
--rw-rw-rw-   0        0        0      104 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/data/__init__.py
--rw-rw-rw-   0        0        0     2154 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/data/dataEncryptor.py
--rw-rw-rw-   0        0        0     1671 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/data/keyManager.py
-drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.417125 decoutilities-0.2.8/decoutilities/inject/
--rw-rw-rw-   0        0        0       44 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/inject/__init__.py
--rw-rw-rw-   0        0        0      569 2024-05-18 20:23:23.000000 decoutilities-0.2.8/decoutilities/inject/injector.py
-drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.418176 decoutilities-0.2.8/decoutilities/logger/
--rw-rw-rw-   0        0        0     1244 2024-05-20 22:20:37.000000 decoutilities-0.2.8/decoutilities/logger/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.419232 decoutilities-0.2.8/decoutilities/queue/
--rw-rw-rw-   0        0        0     1043 2024-05-08 22:21:06.000000 decoutilities-0.2.8/decoutilities/queue/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.420291 decoutilities-0.2.8/decoutilities/textUtils/
--rw-rw-rw-   0        0        0     2427 2024-05-20 22:20:37.000000 decoutilities-0.2.8/decoutilities/textUtils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-20 22:21:50.421337 decoutilities-0.2.8/decoutilities.egg-info/
--rw-rw-rw-   0        0        0    15668 2024-05-20 22:21:50.000000 decoutilities-0.2.8/decoutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      571 2024-05-20 22:21:50.000000 decoutilities-0.2.8/decoutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-20 22:21:50.000000 decoutilities-0.2.8/decoutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-05-20 22:21:50.000000 decoutilities-0.2.8/decoutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-20 22:21:50.423959 decoutilities-0.2.8/setup.cfg
--rw-rw-rw-   0        0        0      729 2024-05-20 22:20:37.000000 decoutilities-0.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.777485 decoutilities-0.2.9/
+-rw-rw-rw-   0        0        0     1089 2024-05-08 11:01:18.000000 decoutilities-0.2.9/LICENSE
+-rw-rw-rw-   0        0        0    15668 2024-05-21 06:17:47.765488 decoutilities-0.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    15197 2024-05-20 11:56:43.000000 decoutilities-0.2.9/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.342487 decoutilities-0.2.9/decoutilities/
+-rw-rw-rw-   0        0        0     4740 2024-05-07 07:54:09.000000 decoutilities-0.2.9/decoutilities/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.507487 decoutilities-0.2.9/decoutilities/config/
+-rw-rw-rw-   0        0        0      104 2024-04-29 13:15:34.000000 decoutilities-0.2.9/decoutilities/config/__init__.py
+-rw-rw-rw-   0        0        0      994 2024-04-26 08:33:42.000000 decoutilities-0.2.9/decoutilities/config/config.py
+-rw-rw-rw-   0        0        0     2736 2024-04-30 08:27:33.000000 decoutilities-0.2.9/decoutilities/config/configContainer.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.577489 decoutilities-0.2.9/decoutilities/data/
+-rw-rw-rw-   0        0        0      104 2024-05-08 07:57:21.000000 decoutilities-0.2.9/decoutilities/data/__init__.py
+-rw-rw-rw-   0        0        0     2154 2024-05-08 07:56:33.000000 decoutilities-0.2.9/decoutilities/data/dataEncryptor.py
+-rw-rw-rw-   0        0        0     1671 2024-05-08 07:52:43.000000 decoutilities-0.2.9/decoutilities/data/keyManager.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.613488 decoutilities-0.2.9/decoutilities/inject/
+-rw-rw-rw-   0        0        0       44 2024-04-29 13:15:19.000000 decoutilities-0.2.9/decoutilities/inject/__init__.py
+-rw-rw-rw-   0        0        0      569 2024-05-20 10:37:54.000000 decoutilities-0.2.9/decoutilities/inject/injector.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.625488 decoutilities-0.2.9/decoutilities/logger/
+-rw-rw-rw-   0        0        0     1221 2024-05-21 05:28:53.000000 decoutilities-0.2.9/decoutilities/logger/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.682487 decoutilities-0.2.9/decoutilities/queue/
+-rw-rw-rw-   0        0        0     1043 2024-05-07 08:05:33.000000 decoutilities-0.2.9/decoutilities/queue/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.701488 decoutilities-0.2.9/decoutilities/textUtils/
+-rw-rw-rw-   0        0        0     2832 2024-05-21 06:12:32.000000 decoutilities-0.2.9/decoutilities/textUtils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-21 06:17:47.720487 decoutilities-0.2.9/decoutilities.egg-info/
+-rw-rw-rw-   0        0        0    15668 2024-05-21 06:17:46.000000 decoutilities-0.2.9/decoutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      571 2024-05-21 06:17:47.000000 decoutilities-0.2.9/decoutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 06:17:46.000000 decoutilities-0.2.9/decoutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-05-21 06:17:46.000000 decoutilities-0.2.9/decoutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 06:17:47.778488 decoutilities-0.2.9/setup.cfg
+-rw-rw-rw-   0        0        0      729 2024-05-21 05:29:14.000000 decoutilities-0.2.9/setup.py
```

### Comparing `decoutilities-0.2.8/LICENSE` & `decoutilities-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.8/PKG-INFO` & `decoutilities-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.8
+Version: 0.2.9
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.2.8/README.md` & `decoutilities-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.8/decoutilities/__init__.py` & `decoutilities-0.2.9/decoutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.8/decoutilities/config/config.py` & `decoutilities-0.2.9/decoutilities/config/config.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.8/decoutilities/config/configContainer.py` & `decoutilities-0.2.9/decoutilities/config/configContainer.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.8/decoutilities/data/dataEncryptor.py` & `decoutilities-0.2.9/decoutilities/data/dataEncryptor.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.8/decoutilities/data/keyManager.py` & `decoutilities-0.2.9/decoutilities/data/keyManager.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.8/decoutilities/inject/injector.py` & `decoutilities-0.2.9/decoutilities/inject/injector.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.8/decoutilities/logger/__init__.py` & `decoutilities-0.2.9/decoutilities/logger/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,25 +2,24 @@
 
 class Logger:
     def __init__(self, prefix = None, debug=False, log = None, format = "{event} {white}| {message}"):
         self.prefix = prefix
         self.log = log
         self.format = format
         self.debug = debug
-        self.text_utils = textUtils()
 
     def  __toLogFile(self, message):
         if self.log is not None:
             with open(self.log, "a") as file:
                 file.write(message + "\n")
 
     def __log(self, event, message):
         if self.prefix is not None:
-            event = self.prefix + " " + event
-        message = self.text_utils.format(message)
+            event = textUtils().format(self.prefix + " " + event)
+        message = textUtils().format(message)
         formatted_message = f"{event} {message}"
         print(formatted_message)
         self.__toLogFile(formatted_message)
     
     def info(self, message):
         self.__log("INFO", message)
```

### Comparing `decoutilities-0.2.8/decoutilities/queue/__init__.py` & `decoutilities-0.2.9/decoutilities/queue/__init__.py`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.8/decoutilities/textUtils/__init__.py` & `decoutilities-0.2.9/decoutilities/textUtils/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -42,30 +42,43 @@
             case "italic":
                 return "\033[3m" + text + "\033[0m"
             case _:
                 return text
         
     def format(text):
         aliases = {
-            "bold": "\033[1m",
-            "underline": "\033[4m",
-            "italic": "\033[3m",
-            "red": "\033[91m",
-            "green": "\033[92m",
-            "yellow": "\033[93m",
-            "blue": "\033[94m",
-            "purple": "\033[95m",
-            "cyan": "\033[96m",
-            "white": "\033[97m",
-            "dark_red": "\033[31m",
-            "dark_green": "\033[32m",
-            "gold": "\033[33m",
-            "gray": "\033[37m",
-            "dark_gray": "\033[90m",
-            "black": "\033[30m",
-            "reset": "\033[0m"
+            "{bold}": "\033[1m",
+            "{underline}": "\033[4m",
+            "{italic}": "\033[3m",
+            "{red}": "\033[91m",
+            "{green}": "\033[92m",
+            "{yellow}": "\033[93m",
+            "{blue}": "\033[94m",
+            "{purple}": "\033[95m",
+            "{cyan}": "\033[96m",
+            "{white}": "\033[97m",
+            "{dark_red}": "\033[31m",
+            "{dark_green}": "\033[32m",
+            "{gold}": "\033[33m",
+            "{gray}": "\033[37m",
+            "{dark_gray}": "\033[90m",
+            "{black}": "\033[30m",
+            "{reset}": "\033[0m"
         }
 
         for key, value in aliases.items():
             text = text.replace(key, value)
 
-        return text + "\033[0m"  # reset at the end
+        return text + "\033[0m"  # reset at the end
+def format(text):
+    return textUtils.format(text)
+def color(color, text):
+    return textUtils.color(color, text)
+def decorate(decoration, text):
+    return textUtils.decorate(decoration, text)
+
+# FORMAT DECORATOR
+def formated(func):
+    def wrapper(*args, **kwargs):
+        result = func(*args, **kwargs)
+        return format(result)
+    return wrapper
```

### Comparing `decoutilities-0.2.8/decoutilities.egg-info/PKG-INFO` & `decoutilities-0.2.9/decoutilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoutilities
-Version: 0.2.8
+Version: 0.2.9
 Summary: Enhance the readability of your code with decorators and simplify the creation of configuration files.
 Author: Hugo Torres
 Author-email: contact@redactado.es
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `decoutilities-0.2.8/decoutilities.egg-info/SOURCES.txt` & `decoutilities-0.2.9/decoutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `decoutilities-0.2.8/setup.py` & `decoutilities-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
 name='decoutilities',
-version='0.2.8',
+version='0.2.9',
 author='Hugo Torres',
 author_email='contact@redactado.es',
 description='Enhance the readability of your code with decorators and simplify the creation of configuration files.',
 packages=find_packages(include=['decoutilities', 'decoutilities.*']),
 classifiers=[
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
```

