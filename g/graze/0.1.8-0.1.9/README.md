# Comparing `tmp/graze-0.1.8.tar.gz` & `tmp/graze-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graze-0.1.8.tar", last modified: Wed Jan  5 19:19:32 2022, max compression
+gzip compressed data, was "graze-0.1.9.tar", last modified: Tue Feb 28 11:21:16 2023, max compression
```

## Comparing `graze-0.1.8.tar` & `graze-0.1.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 19:19:32.084204 graze-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-01-05 19:19:10.000000 graze-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7783 2022-01-05 19:19:32.084204 graze-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5845 2022-01-05 19:19:10.000000 graze-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 19:19:32.084204 graze-0.1.8/graze/
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-01-05 19:19:10.000000 graze-0.1.8/graze/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13619 2022-01-05 19:19:10.000000 graze-0.1.8/graze/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3722 2022-01-05 19:19:10.000000 graze-0.1.8/graze/migration_tools.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-01-05 19:19:10.000000 graze-0.1.8/graze/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-05 19:19:32.084204 graze-0.1.8/graze.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7783 2022-01-05 19:19:31.000000 graze-0.1.8/graze.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-01-05 19:19:31.000000 graze-0.1.8/graze.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-05 19:19:31.000000 graze-0.1.8/graze.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-05 19:19:31.000000 graze-0.1.8/graze.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-05 19:19:31.000000 graze-0.1.8/graze.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-05 19:19:31.000000 graze-0.1.8/graze.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      514 2022-01-05 19:19:32.084204 graze-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-01-05 19:19:10.000000 graze-0.1.8/setup.py
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-02-28 11:21:16.533875 graze-0.1.9/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     1069 2022-10-25 12:59:08.000000 graze-0.1.9/LICENSE
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     6619 2023-02-28 11:21:16.536305 graze-0.1.9/PKG-INFO
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     6368 2023-02-28 11:14:59.000000 graze-0.1.9/README.md
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-02-28 11:21:15.423168 graze-0.1.9/graze/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      269 2022-10-25 12:59:08.000000 graze-0.1.9/graze/__init__.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)    16617 2023-02-28 11:14:59.000000 graze-0.1.9/graze/base.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     3722 2022-10-25 12:59:08.000000 graze-0.1.9/graze/migration_tools.py
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     1743 2022-10-25 12:59:08.000000 graze-0.1.9/graze/util.py
+drwxr-xr-x   0 thorwhalen   (501) staff       (20)        0 2023-02-28 11:21:15.481621 graze-0.1.9/graze.egg-info/
+-rw-r--r--   0 thorwhalen   (501) staff       (20)     6619 2023-02-28 11:21:11.000000 graze-0.1.9/graze.egg-info/PKG-INFO
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      279 2023-02-28 11:21:13.000000 graze-0.1.9/graze.egg-info/SOURCES.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2023-02-28 11:21:11.000000 graze-0.1.9/graze.egg-info/dependency_links.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        1 2023-02-28 11:21:11.000000 graze-0.1.9/graze.egg-info/not-zip-safe
+-rw-r--r--   0 thorwhalen   (501) staff       (20)       18 2023-02-28 11:21:11.000000 graze-0.1.9/graze.egg-info/requires.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)        6 2023-02-28 11:21:11.000000 graze-0.1.9/graze.egg-info/top_level.txt
+-rw-r--r--   0 thorwhalen   (501) staff       (20)      514 2023-02-28 11:21:16.550144 graze-0.1.9/setup.cfg
+-rw-r--r--   0 thorwhalen   (501) staff       (20)       91 2022-10-25 12:59:08.000000 graze-0.1.9/setup.py
```

### Comparing `graze-0.1.8/LICENSE` & `graze-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `graze-0.1.8/README.md` & `graze-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,25 @@
+Metadata-Version: 2.1
+Name: graze
+Version: 0.1.9
+Summary: Cache (a tiny part of) the internet
+Home-page: https://github.com/thorwhalen/graze
+Author: Thor Whalen
+License: mit
+Platform: any
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # graze
 
 Cache (a tiny part of) the internet.
 
+(For the technically inclined, graze is meant to enable the separation of the concerns 
+of getting and caching data from the internet.)
+
 ## install
 
 ```pip install graze```
 
 # Example
 
 ```python
@@ -82,14 +96,15 @@
 ```python
 del g[url]
 ```
 
 
 # Q&A
 
+
 ## The pages I need to slurp need to be rendered, can I use selenium of other such engines?
 
 Sure!
 
 We understand that sometimes you might have special slurping needs -- such 
 as needing to let the JS render the page fully, and/or extract something 
 specific, in a specific way, from the page.
@@ -128,15 +143,14 @@
 
 # and then you can just do
 g = my_graze()
 # and get on with the fun...
 ```
 
 
-
 ## What if I want a fresh copy of the data?
 
 Classic caching problem. 
 You like the convenience of having a local copy, but then how do you keep in sync with the data source if it changes?
 
 If you KNOW the source data changed and want to sync, it's easy. You delete the local copy 
 (like deleting a key from a dict: `del Graze()[url]`)
@@ -158,15 +172,26 @@
 
 ```
 from graze import graze
 
 content_bytes = graze(url, max_age=in_seconds)
 ```
 
-## Does it work for dropbox links?
+## Can I make graze notify me when it gets a new copy of the data?
+
+Sure! Just specify a `preget` function when you make your `Graze` object, or 
+call `graze`. This function will be called on the key (the url) just before contents 
+are being downloaded from the internet. The typical function would be:
+
+```python
+preget = lambda key: print(f"Getting {key} from the internet")
+```
+
+
+## Does graze work for dropbox links?
 
 Yes it does, but you need to be aware that dropbox systematically send the data as a zip, **even if there's only one file in it**.
 
 Here's some code that can help.
 
 ```python
 def zip_store_of_gropbox_url(dropbox_url: str):
```

### Comparing `graze-0.1.8/graze/base.py` & `graze-0.1.9/graze/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     'http/www.example.com_f/subdir1_f/subdir2_f/file.txt'
     >>> _url_to_localpath('https://www.example.com/subdir1/subdir2/file.txt/')
     'https/www.example.com_f/subdir1_f/subdir2_f/file.txt_f/'
     >>> _url_to_localpath('www.example.com/subdir1/subdir2/file.txt')
     'www.example.com/subdir1_f/subdir2_f/file.txt'
     """
     path = url.replace('https://', 'https/').replace('http://', 'http/')
-    path_subdirs = path.split(psep)
+    path_subdirs = list(filter(None, path.split(psep)))
     path_subdirs[1:-1] = [x + '_f' for x in path_subdirs[1:-1]]
     return pjoin(*path_subdirs)
 
 
 def _localpath_to_url(path: str) -> str:
     """
     >>> _localpath_to_url('http/www.example.com_f/subdir1_f/subdir2_f/file.txt')
@@ -208,14 +208,15 @@
 
         :param url_to_contents: The function that gets you the contents from the url
         """
         self.url_to_contents = url_to_contents
 
     # TODO: implement the key-specific getitem mapping externally to make it open-closed
     def __getitem__(self, k):
+        k = k.strip()
         if k.endswith('/'):
             # because it shouldn't matter as url (?) and having it leads to dirs (not
             # files) being created:
             k = k[:-1]
 
         if is_dropbox_url(k):
             return bytes_from_dropbox(k)
@@ -225,23 +226,58 @@
     def _get_contents_of_url(self, url):
         try:
             return self.url_to_contents(url)
         except RequestFailure as e:
             raise KeyError(e.args[0])
 
 
+# Typical function to use as a preget to Graze
+def preget_print_downloading_message(key):
+    print(f"The contents of {key} are being downloaded")
+
 # TODO: Use reususable caching decorator?
 # TODO: Not seeing the right signature, but the LocalGrazed one!
 class Graze(LocalGrazed):
-    def __init__(self, rootdir=DFLT_GRAZE_DIR, source=Internet()):
+    """A data access object that will get data from the internet if it's not
+    already stored locally.
+
+    The interface of ``Graze`` instances is a ``typing.Mapping`` (i.e. ``dict``-like).
+    When you list (or iterate over) keys, you'll get the urls
+    whose contents are stored locally.
+    When you get a value, you'll get the contents of the url (in bytes).
+    ``Graze`` will first look if the contents are stored locally, and return that,
+    if not it will get the contents from the internet and store it locally,
+    then return those bytes.
+    """
+    def __init__(
+            self,
+            rootdir=DFLT_GRAZE_DIR,
+            source=Internet(),
+            *,
+            preget: Optional[Callable] = None
+    ):
+        """
+        :param rootdir: Where to store the contents locally.
+        :param source: Where to get the contents from if they're not already stored
+            locally. By default, it's an ``Internet`` instance, but can be a custom
+            object that has a ``__getitem__`` method that takes a url and returns
+            its contents.
+        :param preget: A function to call on the key before getting the contents from
+            ``source``. Typically, this is used to notify the user that the contents
+            are being downloaded. For example, you could use
+            ``preget=lambda k: print(f"The contents of {k} are being downloaded")``.
+        """
         super().__init__(rootdir)
         self.source = source
         self.rootdir = rootdir
+        self.preget = preget
 
     def __missing__(self, k):
+        if self.preget:
+            self.preget(k)
         # if you didn't have it "locally", ask src for it
         v = self.source[k]  # ... get it from _src,
         self[k] = v  # ... store it in self
         return v  # ... and return it.
 
     filepath_of = partialmethod(inner_most_key)
     filepath_of.__doc__ = (
@@ -279,30 +315,35 @@
 A_WEEK_IN_SECONDS = 7 * 24 * 60 * 60  # one week
 
 
 # TODO: Would be nicer to solve this with a reusable ttl caching decorator!
 class GrazeWithDataRefresh(Graze):
     def __init__(
         self,
+        rootdir=DFLT_GRAZE_DIR,
+        source=Internet(),
+        *,
+        preget: Optional[Callable] = None,
         time_to_live: Union[int, float] = A_WEEK_IN_SECONDS,
         on_error: str = 'warn',
     ):
         """Like Graze, but where you can specify a time_to_live "freshness threshold" to trigger the re-download of data
 
         :param time_to_live: In seconds.
         :param on_error: What to do if there's an error when fetching the new data.
             'raise' raise an error (but keep the cached data)
             'warn' warn the user of the stale data (but return anyway)
             'ignore' ignore the error, and return the stale data
         """
-        super().__init__()
+        super().__init__(rootdir, source=source, preget=preget)
         self.time_to_live = time_to_live
         self.on_error = on_error
 
     def __getitem__(self, k):
+        k = k.strip()
         v = None
         if k in self:
             # TODO: Use info store that is not necessarily a local files sys?
             filepath = inner_most_key(self, k)
             age = (
                 time.time() - os.stat(filepath).st_mtime
             )  # Note: local file sys cache is assumed here!
@@ -327,21 +368,44 @@
         return v
 
 
 def graze(
     url: str,
     rootdir: str = DFLT_GRAZE_DIR,
     source=Internet(),
+    *,
+    preget: Optional[Callable] = None,
     max_age: Optional[Union[int, float]] = None,
 ):
-    """Get the contents of the url (persisting the results in a local file, for next time you'll ask for it)"""
+    """Get the contents of the url (persisting the results in a local file,
+    for next time you'll ask for it)
+
+    :param rootdir: Where to store the contents locally.
+    :param source: Where to get the contents from if they're not already stored
+        locally. By default, it's an ``Internet`` instance, but can be a custom
+        object that has a ``__getitem__`` method that takes a url and returns
+        its contents.
+    :param preget: A function to call on the key before getting the contents from
+        ``source``. Typically, this is used to notify the user that the contents
+        are being downloaded. For example, you could use
+        ``preget="The contents of {} are being downloaded".format``.
+    :param time_to_live: If not None, should be a number specifying the number of
+    seconds a the cached data is considered "fresh". If the cached data is older
+    than this, then it will be re-downloaded from the source.
+    :param on_error: What to do if there's an error when fetching the new data.
+        'raise' raise an error (but keep the cached data)
+        'warn' warn the user of the stale data (but return anyway)
+        'ignore' ignore the error, and return the stale data
+    """
+    _kwargs = dict(rootdir=rootdir, source=source, preget=preget)
     if max_age is None:
-        return Graze(rootdir=rootdir, source=source)[url]
+        g = Graze(**_kwargs)
     else:
-        return GrazeWithDataRefresh(time_to_live=max_age)[url]
+        g = GrazeWithDataRefresh(**_kwargs, time_to_live=max_age)
+    return g[url]
 
 
 def url_to_filepath(url: str, rootdir: str = DFLT_GRAZE_DIR):
     """Get the file path for the url, downloading contents before hand if necessary.
 
     Use case:
```

### Comparing `graze-0.1.8/graze/migration_tools.py` & `graze-0.1.9/graze/migration_tools.py`

 * *Files identical despite different names*

### Comparing `graze-0.1.8/graze/util.py` & `graze-0.1.9/graze/util.py`

 * *Files identical despite different names*

### Comparing `graze-0.1.8/setup.cfg` & `graze-0.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = graze
-version = 0.1.8
+version = 0.1.9
 url = https://github.com/thorwhalen/graze
 platforms = any
 description_file = README.md
 description = Cache (a tiny part of) the internet
 root_url = https://github.com/thorwhalen
 author = Thor Whalen
 license = mit
```

