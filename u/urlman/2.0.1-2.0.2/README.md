# Comparing `tmp/urlman-2.0.1.tar.gz` & `tmp/urlman-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/andrew/Programs/urlman/dist/tmpnzyr7sdi/urlman-2.0.1.tar", last modified: Fri Jun 11 02:46:31 2021, max compression
+gzip compressed data, was "urlman-2.0.2.tar", last modified: Tue May 21 14:57:26 2024, max compression
```

## Comparing `urlman-2.0.1.tar` & `urlman-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2021-06-11 02:46:31.336421 urlman-2.0.1/
--rw-r--r--   0 andrew    (1000) andrew    (1000)    10172 2021-06-06 05:53:51.000000 urlman-2.0.1/LICENSE
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3354 2021-06-11 02:46:31.336421 urlman-2.0.1/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)     2274 2021-06-06 05:53:51.000000 urlman-2.0.1/README.rst
--rw-r--r--   0 andrew    (1000) andrew    (1000)      189 2021-06-11 02:46:31.336421 urlman-2.0.1/setup.cfg
--rw-r--r--   0 andrew    (1000) andrew    (1000)     1256 2021-06-11 02:42:01.000000 urlman-2.0.1/setup.py
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2021-06-11 02:46:31.336421 urlman-2.0.1/urlman/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     4793 2021-06-11 02:43:38.000000 urlman-2.0.1/urlman/__init__.py
--rw-r--r--   0 andrew    (1000) andrew    (1000)      704 2021-06-06 05:53:51.000000 urlman-2.0.1/urlman/serializers.py
-drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2021-06-11 02:46:31.336421 urlman-2.0.1/urlman.egg-info/
--rw-r--r--   0 andrew    (1000) andrew    (1000)     3354 2021-06-11 02:46:31.000000 urlman-2.0.1/urlman.egg-info/PKG-INFO
--rw-r--r--   0 andrew    (1000) andrew    (1000)      198 2021-06-11 02:46:31.000000 urlman-2.0.1/urlman.egg-info/SOURCES.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2021-06-11 02:46:31.000000 urlman-2.0.1/urlman.egg-info/dependency_links.txt
--rw-r--r--   0 andrew    (1000) andrew    (1000)        7 2021-06-11 02:46:31.000000 urlman-2.0.1/urlman.egg-info/top_level.txt
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2024-05-21 14:57:26.968923 urlman-2.0.2/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)    10172 2024-05-21 14:55:08.000000 urlman-2.0.2/LICENSE
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3317 2024-05-21 14:57:26.972923 urlman-2.0.2/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     2274 2024-05-21 14:55:08.000000 urlman-2.0.2/README.rst
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      189 2024-05-21 14:57:26.972923 urlman-2.0.2/setup.cfg
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     1256 2024-05-21 14:55:53.000000 urlman-2.0.2/setup.py
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2024-05-21 14:57:26.968923 urlman-2.0.2/urlman/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     4336 2024-05-21 14:56:08.000000 urlman-2.0.2/urlman/__init__.py
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      844 2024-05-21 14:55:08.000000 urlman-2.0.2/urlman/serializers.py
+drwxr-xr-x   0 andrew    (1000) andrew    (1000)        0 2024-05-21 14:57:26.968923 urlman-2.0.2/urlman.egg-info/
+-rw-r--r--   0 andrew    (1000) andrew    (1000)     3317 2024-05-21 14:57:26.000000 urlman-2.0.2/urlman.egg-info/PKG-INFO
+-rw-r--r--   0 andrew    (1000) andrew    (1000)      198 2024-05-21 14:57:26.000000 urlman-2.0.2/urlman.egg-info/SOURCES.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        1 2024-05-21 14:57:26.000000 urlman-2.0.2/urlman.egg-info/dependency_links.txt
+-rw-r--r--   0 andrew    (1000) andrew    (1000)        7 2024-05-21 14:57:26.000000 urlman-2.0.2/urlman.egg-info/top_level.txt
```

### Comparing `urlman-2.0.1/LICENSE` & `urlman-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `urlman-2.0.1/PKG-INFO` & `urlman-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: urlman
-Version: 2.0.1
+Version: 2.0.2
 Summary: Django URL pattern helpers
 Home-page: https://github.com/andrewgodwin/urlman
 Author: Andrew Godwin
 Author-email: andrew@aeracode.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -96,9 +94,7 @@
 
 .. code-block:: python
 
    from urlman.serializers import UrlManField
 
    class MySerializer(ModelSerializer):
        urls = UrlManField(urls=['view', 'edit'], attribute='urls', full=True)
-
-
```

### Comparing `urlman-2.0.1/README.rst` & `urlman-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `urlman-2.0.1/setup.py` & `urlman-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open(os.path.join(os.path.dirname(__file__), "README.rst")) as fh:
     readme_content = fh.read()
 
 setup(
     name="urlman",
-    version="2.0.1",
+    version="2.0.2",
     description="Django URL pattern helpers",
     long_description=readme_content,
     url="https://github.com/andrewgodwin/urlman",
     packages=["urlman"],
     author="Andrew Godwin",
     author_email="andrew@aeracode.org",
     classifiers=[
```

### Comparing `urlman-2.0.1/urlman/__init__.py` & `urlman-2.0.2/urlman/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,31 +2,15 @@
 
 try:
     from urlparse import urlunparse
 except ImportError:  # pragma: no cover
     from urllib.parse import urlunparse
 
 
-__version__ = "2.0.1"
-
-
-def with_metaclass(meta, *bases):
-    """
-    Create a base class with a metaclass.
-
-    For Python 2.x and 3.x compatibility.
-    """
-    # This requires a bit of explanation: the basic idea is to make a dummy
-    # metaclass for one level of class instantiation that replaces itself with
-    # the actual metaclass.
-    class metaclass(meta):
-        def __new__(cls, name, this_bases, d):
-            return meta(name, bases, d)
-
-    return type.__new__(metaclass, "temporary_class", (), {})
+__version__ = "2.0.2"
 
 
 class UrlsMetaclass(type):
     """
     Metaclass which makes attribute access instantiate the class with
     the instance.
     """
@@ -43,15 +27,15 @@
         # Initialise
         return type.__new__(self, name, bases, attrs)
 
     def __get__(self, instance, klass):
         return self(klass, instance, self.__name__)
 
 
-class Urls(with_metaclass(UrlsMetaclass)):
+class Urls(metaclass=UrlsMetaclass):
     """
     Special object which lets you specify URL strings for objects.
 
     Declare urls as string attributes on the object in _python 3_ string
     format. If you need to you can also specify a handler function for a url.
     """
 
@@ -61,15 +45,15 @@
         self.context = {"self": self.instance}
         self.context.update(self.urls)
         self.__qualname__ = ".".join((klass.__qualname__, name))
 
     def __getattr__(self, attr):
         return self.get_url(attr)
 
-    def get_url(self, attr):
+    def get_url(self, attr: str) -> "UrlString":
         # Get the URL value
         try:
             url = self.urls[attr]
         except KeyError:
             raise ValueError(
                 "No URL called %r on %r" % (attr, self.instance.__class__.__name__)
             )
@@ -89,18 +73,18 @@
             raise ValueError("No URL called %r" % attr)
         else:
             if callable(url):
                 url = url(self.instance)
             value = UrlFormatter(self, example=True).vformat(url, [], {})
         return value
 
-    def get_scheme(self, url):
+    def get_scheme(self, url: "UrlString"):
         return "http"
 
-    def get_hostname(self, url):
+    def get_hostname(self, url: "UrlString"):
         return "localhost"
 
 
 class UrlString(str):
     """
     Special string subclass for URLs (for future with/without host modes)
     """
```

### Comparing `urlman-2.0.1/urlman.egg-info/PKG-INFO` & `urlman-2.0.2/urlman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: urlman
-Version: 2.0.1
+Version: 2.0.2
 Summary: Django URL pattern helpers
 Home-page: https://github.com/andrewgodwin/urlman
 Author: Andrew Godwin
 Author-email: andrew@aeracode.org
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
@@ -96,9 +94,7 @@
 
 .. code-block:: python
 
    from urlman.serializers import UrlManField
 
    class MySerializer(ModelSerializer):
        urls = UrlManField(urls=['view', 'edit'], attribute='urls', full=True)
-
-
```

