# Comparing `tmp/datapad-0.6.9.tar.gz` & `tmp/datapad-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/datapad-0.6.9.tar", last modified: Fri May 20 01:14:56 2022, max compression
+gzip compressed data, was "datapad-0.7.1.tar", last modified: Tue May 21 19:20:57 2024, max compression
```

## Comparing `datapad-0.6.9.tar` & `datapad-0.7.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2022-05-20 01:14:56.906931 datapad-0.6.9/
--rw-r--r--   0 huy        (501) staff       (20)     4693 2022-05-20 01:14:56.906633 datapad-0.6.9/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)     3519 2020-01-02 18:43:22.000000 datapad-0.6.9/README.md
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2022-05-20 01:14:56.904878 datapad-0.6.9/datapad/
--rw-r--r--   0 huy        (501) staff       (20)      608 2019-12-30 21:14:31.000000 datapad-0.6.9/datapad/__init__.py
--rw-r--r--   0 huy        (501) staff       (20)    13199 2020-01-08 20:06:49.000000 datapad-0.6.9/datapad/fields.py
--rw-r--r--   0 huy        (501) staff       (20)     4658 2019-12-30 21:14:21.000000 datapad-0.6.9/datapad/io.py
--rw-r--r--   0 huy        (501) staff       (20)    23690 2022-05-20 01:13:00.000000 datapad-0.6.9/datapad/sequence.py
--rw-r--r--   0 huy        (501) staff       (20)     1014 2020-01-02 00:52:45.000000 datapad-0.6.9/datapad/tests.py
-drwxr-xr-x   0 huy        (501) staff       (20)        0 2022-05-20 01:14:56.906016 datapad-0.6.9/datapad.egg-info/
--rw-r--r--   0 huy        (501) staff       (20)     4693 2022-05-20 01:14:56.000000 datapad-0.6.9/datapad.egg-info/PKG-INFO
--rw-r--r--   0 huy        (501) staff       (20)      231 2022-05-20 01:14:56.000000 datapad-0.6.9/datapad.egg-info/SOURCES.txt
--rw-r--r--   0 huy        (501) staff       (20)        1 2022-05-20 01:14:56.000000 datapad-0.6.9/datapad.egg-info/dependency_links.txt
--rw-r--r--   0 huy        (501) staff       (20)        8 2022-05-20 01:14:56.000000 datapad-0.6.9/datapad.egg-info/top_level.txt
--rw-r--r--   0 huy        (501) staff       (20)       38 2022-05-20 01:14:56.907026 datapad-0.6.9/setup.cfg
--rw-r--r--   0 huy        (501) staff       (20)     1317 2022-05-20 01:13:48.000000 datapad-0.6.9/setup.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-21 19:20:57.024995 datapad-0.7.1/
+-rw-r--r--   0 huy        (501) staff       (20)    11340 2019-12-30 21:17:14.000000 datapad-0.7.1/LICENSE
+-rw-r--r--   0 huy        (501) staff       (20)     4350 2024-05-21 19:20:57.024506 datapad-0.7.1/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)     3176 2024-05-21 19:05:30.000000 datapad-0.7.1/README.md
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-21 19:20:57.021139 datapad-0.7.1/datapad/
+-rw-r--r--   0 huy        (501) staff       (20)      608 2024-05-21 18:56:15.000000 datapad-0.7.1/datapad/__init__.py
+-rw-r--r--   0 huy        (501) staff       (20)    13199 2020-01-08 20:06:49.000000 datapad-0.7.1/datapad/fields.py
+-rw-r--r--   0 huy        (501) staff       (20)     7091 2024-05-21 14:12:40.000000 datapad-0.7.1/datapad/io.py
+-rw-r--r--   0 huy        (501) staff       (20)    25915 2024-05-21 19:08:51.000000 datapad-0.7.1/datapad/sequence.py
+-rw-r--r--   0 huy        (501) staff       (20)     2047 2024-05-21 19:01:19.000000 datapad-0.7.1/datapad/tests.py
+drwxr-xr-x   0 huy        (501) staff       (20)        0 2024-05-21 19:20:57.023663 datapad-0.7.1/datapad.egg-info/
+-rw-r--r--   0 huy        (501) staff       (20)     4350 2024-05-21 19:20:56.000000 datapad-0.7.1/datapad.egg-info/PKG-INFO
+-rw-r--r--   0 huy        (501) staff       (20)      239 2024-05-21 19:20:56.000000 datapad-0.7.1/datapad.egg-info/SOURCES.txt
+-rw-r--r--   0 huy        (501) staff       (20)        1 2024-05-21 19:20:56.000000 datapad-0.7.1/datapad.egg-info/dependency_links.txt
+-rw-r--r--   0 huy        (501) staff       (20)        8 2024-05-21 19:20:56.000000 datapad-0.7.1/datapad.egg-info/top_level.txt
+-rw-r--r--   0 huy        (501) staff       (20)       38 2024-05-21 19:20:57.025150 datapad-0.7.1/setup.cfg
+-rw-r--r--   0 huy        (501) staff       (20)     1317 2024-05-21 19:03:02.000000 datapad-0.7.1/setup.py
```

### Comparing `datapad-0.6.9/PKG-INFO` & `datapad-0.7.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapad
-Version: 0.6.9
+Version: 0.7.1
 Summary: Datapad is a library of lazy data transformations for sequences; similar to spark and linq
 Home-page: https://github.com/huyng/datapad
 Author: Huy Nguyen
 Author-email: 
 License: UNKNOWN
 Description: <!--
         Copyright 2019 Huy Nguyen
@@ -65,15 +65,15 @@
          ('c', 3)]
         ```
         
         **Transform individual fields in a sequence:**
         
         ```python
         >>> import datapad as dp
-        >>> import datapad.fields as F
+        >>> F = datapad.fields
         >>> data = [
         ...     {'a': 1, 'b': 2},
         ...     {'a': 4, 'b': 4},
         ...     {'a': 5, 'b': 7}
         ... ]
         >>> seq = dp.Sequence(data)
         >>> seq.map(F.apply('a', lambda x: x*2)) \
@@ -101,18 +101,18 @@
         
         Check out our documentation below to see what else is possible with Datapad:
         
         **[Documentation](https://datapad.readthedocs.io/en/latest/quickstart.html)**
         
         ---
         
-        This project incorporates ideas from:
+        ### Development
         
-        * [LINQ](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/standard-query-operators-overview)
-        * [Spark](https://spark.apache.org/)
-        * [Python Itertools](https://docs.python.org/3/library/itertools.html)
-        * [Pandas](https://pandas.pydata.org/)
-        * [Dask](https://dask.org/)
-        * [Tensorflow tf.data.Datasets](https://www.tensorflow.org/api_docs/python/tf/data/Dataset)
+        Run tests from the root of repo using
+        
+        ```
+        pip install pytest
+        sh test.sh
+        ```
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datapad Version: 0.6.9 Summary: Datapad is a
+Metadata-Version: 2.1 Name: datapad Version: 0.7.1 Summary: Datapad is a
 library of lazy data transformations for sequences; similar to spark and linq
 Home-page: https://github.com/huyng/datapad Author: Huy Nguyen Author-email:
 License: UNKNOWN Description: # Datapad: A Fluent API for Exploratory Data
 Analysis
 [https://user-images.githubusercontent.com/121183/71599089-4cfe1080-2afe-11ea-
                             8852-81f00ed8c3fa.jpg]
 _[_h_t_t_p_s_:_/_/_t_r_a_v_i_s_-_c_i_._o_r_g_/_h_u_y_n_g_/_d_a_t_a_p_a_d_._s_v_g_?_b_r_a_n_c_h_=_m_a_s_t_e_r_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/
@@ -18,25 +18,20 @@
 quickstart.html#structured-sequences) data. [Learn more in Documentation]
 (https://datapad.readthedocs.io/en/latest/quickstart.html) --- ### Install ```
 pip install datapad ``` ### Exploratory data analysis with Datapad See what you
 can do with `datapad` in the examples below. **Count all unique items in a
 sequence:** ```python >>> import datapad as dp >>> data = ['a', 'b', 'b', 'c',
 'c', 'c'] >>> seq = dp.Sequence(data) >>> seq.count(distinct=True) \ ...
 .collect() [('a', 1), ('b', 2), ('c', 3)] ``` **Transform individual fields in
-a sequence:** ```python >>> import datapad as dp >>> import datapad.fields as F
->>> data = [ ... {'a': 1, 'b': 2}, ... {'a': 4, 'b': 4}, ... {'a': 5, 'b': 7}
-... ] >>> seq = dp.Sequence(data) >>> seq.map(F.apply('a', lambda x: x*2)) \
-... .map(F.apply('b', lambda x: x*3)) \ ... .collect() [{'a': 2, 'b': 6}, {'a':
-8, 'b': 12}, {'a': 10, 'b': 21}] ``` **Chain together multiple transforms for
-the elements of a sequence:** ```python >>> import datapad as dp >>> data =
-['a', 'b', 'b', 'c', 'c', 'c'] >>> seq = dp.Sequence(data) >>> seq.distinct() \
-... .map(lambda x: x+'z') \ ... .map(lambda x: (x, len(x))) \ ... .collect() [
+a sequence:** ```python >>> import datapad as dp >>> F = datapad.fields >>>
+data = [ ... {'a': 1, 'b': 2}, ... {'a': 4, 'b': 4}, ... {'a': 5, 'b': 7} ... ]
+>>> seq = dp.Sequence(data) >>> seq.map(F.apply('a', lambda x: x*2)) \ ... .map
+(F.apply('b', lambda x: x*3)) \ ... .collect() [{'a': 2, 'b': 6}, {'a': 8, 'b':
+12}, {'a': 10, 'b': 21}] ``` **Chain together multiple transforms for the
+elements of a sequence:** ```python >>> import datapad as dp >>> data = ['a',
+'b', 'b', 'c', 'c', 'c'] >>> seq = dp.Sequence(data) >>> seq.distinct() \ ...
+.map(lambda x: x+'z') \ ... .map(lambda x: (x, len(x))) \ ... .collect() [
 ('az', 2), ('bz', 2), ('cz', 2)] ``` Check out our documentation below to see
 what else is possible with Datapad: **[Documentation](https://
-datapad.readthedocs.io/en/latest/quickstart.html)** --- This project
-incorporates ideas from: * [LINQ](https://docs.microsoft.com/en-us/dotnet/
-csharp/programming-guide/concepts/linq/standard-query-operators-overview) *
-[Spark](https://spark.apache.org/) * [Python Itertools](https://
-docs.python.org/3/library/itertools.html) * [Pandas](https://pandas.pydata.org/
-) * [Dask](https://dask.org/) * [Tensorflow tf.data.Datasets](https://
-www.tensorflow.org/api_docs/python/tf/data/Dataset) Platform: UNKNOWN
-Description-Content-Type: text/markdown
+datapad.readthedocs.io/en/latest/quickstart.html)** --- ### Development Run
+tests from the root of repo using ``` pip install pytest sh test.sh ```
+Platform: UNKNOWN Description-Content-Type: text/markdown
```

### Comparing `datapad-0.6.9/README.md` & `datapad-0.7.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -57,15 +57,15 @@
  ('c', 3)]
 ```
 
 **Transform individual fields in a sequence:**
 
 ```python
 >>> import datapad as dp
->>> import datapad.fields as F
+>>> F = datapad.fields
 >>> data = [
 ...     {'a': 1, 'b': 2},
 ...     {'a': 4, 'b': 4},
 ...     {'a': 5, 'b': 7}
 ... ]
 >>> seq = dp.Sequence(data)
 >>> seq.map(F.apply('a', lambda x: x*2)) \
@@ -93,15 +93,15 @@
 
 Check out our documentation below to see what else is possible with Datapad:
 
 **[Documentation](https://datapad.readthedocs.io/en/latest/quickstart.html)**
 
 ---
 
-This project incorporates ideas from:
+### Development
 
-* [LINQ](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/standard-query-operators-overview)
-* [Spark](https://spark.apache.org/)
-* [Python Itertools](https://docs.python.org/3/library/itertools.html)
-* [Pandas](https://pandas.pydata.org/)
-* [Dask](https://dask.org/)
-* [Tensorflow tf.data.Datasets](https://www.tensorflow.org/api_docs/python/tf/data/Dataset)
+Run tests from the root of repo using
+
+```
+pip install pytest
+sh test.sh
+```
```

#### html2text {}

```diff
@@ -14,24 +14,19 @@
 quickstart.html#structured-sequences) data. [Learn more in Documentation]
 (https://datapad.readthedocs.io/en/latest/quickstart.html) --- ### Install ```
 pip install datapad ``` ### Exploratory data analysis with Datapad See what you
 can do with `datapad` in the examples below. **Count all unique items in a
 sequence:** ```python >>> import datapad as dp >>> data = ['a', 'b', 'b', 'c',
 'c', 'c'] >>> seq = dp.Sequence(data) >>> seq.count(distinct=True) \ ...
 .collect() [('a', 1), ('b', 2), ('c', 3)] ``` **Transform individual fields in
-a sequence:** ```python >>> import datapad as dp >>> import datapad.fields as F
->>> data = [ ... {'a': 1, 'b': 2}, ... {'a': 4, 'b': 4}, ... {'a': 5, 'b': 7}
-... ] >>> seq = dp.Sequence(data) >>> seq.map(F.apply('a', lambda x: x*2)) \
-... .map(F.apply('b', lambda x: x*3)) \ ... .collect() [{'a': 2, 'b': 6}, {'a':
-8, 'b': 12}, {'a': 10, 'b': 21}] ``` **Chain together multiple transforms for
-the elements of a sequence:** ```python >>> import datapad as dp >>> data =
-['a', 'b', 'b', 'c', 'c', 'c'] >>> seq = dp.Sequence(data) >>> seq.distinct() \
-... .map(lambda x: x+'z') \ ... .map(lambda x: (x, len(x))) \ ... .collect() [
+a sequence:** ```python >>> import datapad as dp >>> F = datapad.fields >>>
+data = [ ... {'a': 1, 'b': 2}, ... {'a': 4, 'b': 4}, ... {'a': 5, 'b': 7} ... ]
+>>> seq = dp.Sequence(data) >>> seq.map(F.apply('a', lambda x: x*2)) \ ... .map
+(F.apply('b', lambda x: x*3)) \ ... .collect() [{'a': 2, 'b': 6}, {'a': 8, 'b':
+12}, {'a': 10, 'b': 21}] ``` **Chain together multiple transforms for the
+elements of a sequence:** ```python >>> import datapad as dp >>> data = ['a',
+'b', 'b', 'c', 'c', 'c'] >>> seq = dp.Sequence(data) >>> seq.distinct() \ ...
+.map(lambda x: x+'z') \ ... .map(lambda x: (x, len(x))) \ ... .collect() [
 ('az', 2), ('bz', 2), ('cz', 2)] ``` Check out our documentation below to see
 what else is possible with Datapad: **[Documentation](https://
-datapad.readthedocs.io/en/latest/quickstart.html)** --- This project
-incorporates ideas from: * [LINQ](https://docs.microsoft.com/en-us/dotnet/
-csharp/programming-guide/concepts/linq/standard-query-operators-overview) *
-[Spark](https://spark.apache.org/) * [Python Itertools](https://
-docs.python.org/3/library/itertools.html) * [Pandas](https://pandas.pydata.org/
-) * [Dask](https://dask.org/) * [Tensorflow tf.data.Datasets](https://
-www.tensorflow.org/api_docs/python/tf/data/Dataset)
+datapad.readthedocs.io/en/latest/quickstart.html)** --- ### Development Run
+tests from the root of repo using ``` pip install pytest sh test.sh ```
```

### Comparing `datapad-0.6.9/datapad/__init__.py` & `datapad-0.7.1/datapad/__init__.py`

 * *Files identical despite different names*

### Comparing `datapad-0.6.9/datapad/fields.py` & `datapad-0.7.1/datapad/fields.py`

 * *Files identical despite different names*

### Comparing `datapad-0.6.9/datapad/sequence.py` & `datapad-0.7.1/datapad/sequence.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,15 +118,16 @@
             b_index = collections.OrderedDict(b_index)
 
             for k, v_a in a_index.items():
                 if k in b_index:
                     v_b = b_index[k]
                     yield (v_a, v_b)
 
-        seq = Sequence(_iterable=_inner_join_iterator(self, other, key, other_key))
+        seq = Sequence(_iterable=_inner_join_iterator(self, other, key,
+                                                      other_key))
         return seq
 
     def reduce(self, fn, initial=None):
         """
         Eagerly apply a function of two arguments cumulatively to the items of a sequence,
         from left to right, so as to reduce the sequence to a single value.
         For example, reduce(lambda x, y: x+y, [1, 2, 3, 4, 5]) calculates
@@ -221,57 +222,76 @@
         [1, 2, 3]
         >>> _  = seq.reset()
         >>> seq.collect()
         [1, 2, 3]
 
         """
         if not hasattr(self, "_cache"):
-            raise Exception("Internal cache has never been created for this Sequence")
+            raise Exception(
+                "Internal cache has never been created for this Sequence")
 
         self._iterable = Sequence(_iterable=self._cache)
         return self
 
-    def pmap(self, fn, workers=3, ordered=True):
+    def pmap(self, fn, workers=3, ordered=True, wtype="thread"):
         """
-        Lazily apply fn function to every element of iterable, in parallel using
-        multiprocess.dummy.Pool . The returned sequence may appear in a
-        different order than the input sequence if you set `ordered` to False
-
-        THIS FUNCTION IS EXPERIMENTAL
+        Lazily apply fn function to every element of iterable, in
+        parallel using python's multiprocessing package. The returned
+        sequence may appear in a different order than the input
+        sequence if you set `ordered` to False.
 
         Args:
             fn (function):
-                Function with signature fn(element) -> element to apply to every
-                element of sequence.
+                Function with signature fn(element) -> element to apply to
+                every element of sequence.
             workers (int):
                 Number of parallel workers to use (default: 3). These
                 workers are implemented as python threads.
             ordered (bool):
                 Whether to yield results in the same order in which items
-                arrive. You may get better performance by setting this to false (default: True).
+                arrive. You may get better performance by setting this to
+                false (default: True).
+            wtype ("thread" | "process"):
+                The worker type to use (default: "thread"). Please
+                note, if you are using "process", any functions passed
+                to pmap must be defined concretely inside your script.
+                lambda functions can not be used due to limitations of
+                python multiprocess pickling. The worker type "thread"
+                is good for use with io-bound tasks (such as reading data)
+                from urls.
 
         >>> seq = Sequence(range(10))
         >>> seq = seq.pmap(lambda v: v*2)
         >>> seq.collect()
         [0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
 
         >>> seq = Sequence(range(10))
         >>> seq = seq.pmap(lambda v: v*2, workers=1, ordered=False)
         >>> seq.collect()
         [0, 2, 4, 6, 8, 10, 12, 14, 16, 18]
+
         """
+
         from multiprocessing.dummy import Pool as ThreadPool
-        pool = ThreadPool(workers)
-        apply = pool.imap_unordered if not ordered else pool.imap
+        from multiprocessing import Pool as ProcessPool
 
-        def _pmap(seq):
-            for result in apply(fn, seq):
-                yield result
+        def _pmap(seq, fn):
+            if wtype == "process":
+                Pool = ProcessPool
+            elif wtype == "thread":
+                Pool = ThreadPool
+            else:
+                raise Exception("Unknown worker type '%s'" % wtype)
+
+            with Pool(workers) as pool:
+                apply = pool.imap_unordered if not ordered else pool.imap
+                for result in apply(fn, seq):
+                    yield result
 
-        seq = Sequence(_iterable=_pmap(self._iterable))
+        seq = Sequence(_iterable=_pmap(self._iterable, fn))
         return seq
 
     def flatmap(self, fn):
         """
         Lazily apply fn function to every element of iterable and chain the output
         into a single flattend sequence.
 
@@ -731,15 +751,16 @@
             windows = 0
             for element in iterable:
                 windows += 1
                 queue.append(element)
                 if windows % stride == 0:
                     yield list(queue)
 
-        seq = Sequence(_iterable=_window_iterator(self._iterable, size=size, stride=stride))
+        seq = Sequence(_iterable=_window_iterator(
+            self._iterable, size=size, stride=stride))
         return seq
 
     def batch(self, size):
         """
         Lazily combines elements in sequence into a list of length `size`.
         This function will drop any remainder if the sequence ends before
         a batch with `size` has been created.
@@ -792,14 +813,56 @@
             self._iterable = it.chain(elements, self._iterable)
             return elements
         else:
             element = self.first()
             self._iterable = it.chain([element], self._iterable)
             return element
 
+    def progress(self):
+        """
+        Output progess and transparently pass through elements
+        of sequence.
+
+        >>> seq = Sequence(range(1000))
+        >>> _ = seq.map(lambda x: x*2).progress().collect()
+        """
+
+        def _report(iterable):
+            import time
+            import sys
+            t0 = time.time()
+            for i, elem in enumerate(iterable):
+                yield elem
+                t1 = time.time()
+                print('- secs/element: %.6fs, processed: %d' %
+                      ((t1-t0)/(i+1), (i+1)), end='\r', file=sys.stderr)
+
+            print("", file=sys.stderr)
+            print('- total time: %.3fs' % (time.time()-t0), file=sys.stderr)
+
+        seq = Sequence(_iterable=_report(self._iterable))
+        return seq
+
+    def dump(self, sink):
+        """
+        Dump sequence into a sink function that will greedily consume
+        elements. The purpose of this function is mainly to be used as
+        a way to write files or other external system output.
+
+        Args:
+            sink:
+                Any callable that will take a sequence to
+                consume as its first argument.
+
+        >>> sink = dp.io.JsonSink("data.jsonl", lines=True) # doctest: +SKIP
+        >>> seq.dump(sink) # doctest: +SKIP
+        """
+
+        return sink(self)
+
     def __repr__(self):
         return '<Sequence at %s>' % hex(id(self))
 
 
 if __name__ == "__main__":
     import doctest
     doctest.testmod()
```

### Comparing `datapad-0.6.9/datapad.egg-info/PKG-INFO` & `datapad-0.7.1/datapad.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datapad
-Version: 0.6.9
+Version: 0.7.1
 Summary: Datapad is a library of lazy data transformations for sequences; similar to spark and linq
 Home-page: https://github.com/huyng/datapad
 Author: Huy Nguyen
 Author-email: 
 License: UNKNOWN
 Description: <!--
         Copyright 2019 Huy Nguyen
@@ -65,15 +65,15 @@
          ('c', 3)]
         ```
         
         **Transform individual fields in a sequence:**
         
         ```python
         >>> import datapad as dp
-        >>> import datapad.fields as F
+        >>> F = datapad.fields
         >>> data = [
         ...     {'a': 1, 'b': 2},
         ...     {'a': 4, 'b': 4},
         ...     {'a': 5, 'b': 7}
         ... ]
         >>> seq = dp.Sequence(data)
         >>> seq.map(F.apply('a', lambda x: x*2)) \
@@ -101,18 +101,18 @@
         
         Check out our documentation below to see what else is possible with Datapad:
         
         **[Documentation](https://datapad.readthedocs.io/en/latest/quickstart.html)**
         
         ---
         
-        This project incorporates ideas from:
+        ### Development
         
-        * [LINQ](https://docs.microsoft.com/en-us/dotnet/csharp/programming-guide/concepts/linq/standard-query-operators-overview)
-        * [Spark](https://spark.apache.org/)
-        * [Python Itertools](https://docs.python.org/3/library/itertools.html)
-        * [Pandas](https://pandas.pydata.org/)
-        * [Dask](https://dask.org/)
-        * [Tensorflow tf.data.Datasets](https://www.tensorflow.org/api_docs/python/tf/data/Dataset)
+        Run tests from the root of repo using
+        
+        ```
+        pip install pytest
+        sh test.sh
+        ```
         
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: datapad Version: 0.6.9 Summary: Datapad is a
+Metadata-Version: 2.1 Name: datapad Version: 0.7.1 Summary: Datapad is a
 library of lazy data transformations for sequences; similar to spark and linq
 Home-page: https://github.com/huyng/datapad Author: Huy Nguyen Author-email:
 License: UNKNOWN Description: # Datapad: A Fluent API for Exploratory Data
 Analysis
 [https://user-images.githubusercontent.com/121183/71599089-4cfe1080-2afe-11ea-
                             8852-81f00ed8c3fa.jpg]
 _[_h_t_t_p_s_:_/_/_t_r_a_v_i_s_-_c_i_._o_r_g_/_h_u_y_n_g_/_d_a_t_a_p_a_d_._s_v_g_?_b_r_a_n_c_h_=_m_a_s_t_e_r_]_[_h_t_t_p_s_:_/_/_b_a_d_g_e_._f_u_r_y_._i_o_/
@@ -18,25 +18,20 @@
 quickstart.html#structured-sequences) data. [Learn more in Documentation]
 (https://datapad.readthedocs.io/en/latest/quickstart.html) --- ### Install ```
 pip install datapad ``` ### Exploratory data analysis with Datapad See what you
 can do with `datapad` in the examples below. **Count all unique items in a
 sequence:** ```python >>> import datapad as dp >>> data = ['a', 'b', 'b', 'c',
 'c', 'c'] >>> seq = dp.Sequence(data) >>> seq.count(distinct=True) \ ...
 .collect() [('a', 1), ('b', 2), ('c', 3)] ``` **Transform individual fields in
-a sequence:** ```python >>> import datapad as dp >>> import datapad.fields as F
->>> data = [ ... {'a': 1, 'b': 2}, ... {'a': 4, 'b': 4}, ... {'a': 5, 'b': 7}
-... ] >>> seq = dp.Sequence(data) >>> seq.map(F.apply('a', lambda x: x*2)) \
-... .map(F.apply('b', lambda x: x*3)) \ ... .collect() [{'a': 2, 'b': 6}, {'a':
-8, 'b': 12}, {'a': 10, 'b': 21}] ``` **Chain together multiple transforms for
-the elements of a sequence:** ```python >>> import datapad as dp >>> data =
-['a', 'b', 'b', 'c', 'c', 'c'] >>> seq = dp.Sequence(data) >>> seq.distinct() \
-... .map(lambda x: x+'z') \ ... .map(lambda x: (x, len(x))) \ ... .collect() [
+a sequence:** ```python >>> import datapad as dp >>> F = datapad.fields >>>
+data = [ ... {'a': 1, 'b': 2}, ... {'a': 4, 'b': 4}, ... {'a': 5, 'b': 7} ... ]
+>>> seq = dp.Sequence(data) >>> seq.map(F.apply('a', lambda x: x*2)) \ ... .map
+(F.apply('b', lambda x: x*3)) \ ... .collect() [{'a': 2, 'b': 6}, {'a': 8, 'b':
+12}, {'a': 10, 'b': 21}] ``` **Chain together multiple transforms for the
+elements of a sequence:** ```python >>> import datapad as dp >>> data = ['a',
+'b', 'b', 'c', 'c', 'c'] >>> seq = dp.Sequence(data) >>> seq.distinct() \ ...
+.map(lambda x: x+'z') \ ... .map(lambda x: (x, len(x))) \ ... .collect() [
 ('az', 2), ('bz', 2), ('cz', 2)] ``` Check out our documentation below to see
 what else is possible with Datapad: **[Documentation](https://
-datapad.readthedocs.io/en/latest/quickstart.html)** --- This project
-incorporates ideas from: * [LINQ](https://docs.microsoft.com/en-us/dotnet/
-csharp/programming-guide/concepts/linq/standard-query-operators-overview) *
-[Spark](https://spark.apache.org/) * [Python Itertools](https://
-docs.python.org/3/library/itertools.html) * [Pandas](https://pandas.pydata.org/
-) * [Dask](https://dask.org/) * [Tensorflow tf.data.Datasets](https://
-www.tensorflow.org/api_docs/python/tf/data/Dataset) Platform: UNKNOWN
-Description-Content-Type: text/markdown
+datapad.readthedocs.io/en/latest/quickstart.html)** --- ### Development Run
+tests from the root of repo using ``` pip install pytest sh test.sh ```
+Platform: UNKNOWN Description-Content-Type: text/markdown
```

### Comparing `datapad-0.6.9/setup.py` & `datapad-0.7.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     name='datapad',
-    version='0.6.9',
+    version='0.7.1',
     description='Datapad is a library of lazy data transformations for sequences; similar to spark and linq',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Huy Nguyen',
     author_email='',
     url='https://github.com/huyng/datapad',
     packages=['datapad'],
```

