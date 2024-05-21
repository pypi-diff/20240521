# Comparing `tmp/fast_bitrix24-1.7.2.tar.gz` & `tmp/fast_bitrix24-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fast_bitrix24-1.7.2.tar", last modified: Mon May 20 10:39:36 2024, max compression
+gzip compressed data, was "fast_bitrix24-1.7.3.tar", last modified: Tue May 21 14:39:35 2024, max compression
```

## Comparing `fast_bitrix24-1.7.2.tar` & `fast_bitrix24-1.7.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:39:36.694682 fast_bitrix24-1.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21752 2024-05-20 10:39:36.694682 fast_bitrix24-1.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:39:36.690682 fast_bitrix24-1.7.2/fast_bitrix24/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/bitrix.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/correct_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/mult_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/server_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/srh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)    15389 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/user_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/fast_bitrix24/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:39:36.694682 fast_bitrix24-1.7.2/fast_bitrix24.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21752 2024-05-20 10:39:36.000000 fast_bitrix24-1.7.2/fast_bitrix24.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-20 10:39:36.000000 fast_bitrix24-1.7.2/fast_bitrix24.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 10:39:36.000000 fast_bitrix24-1.7.2/fast_bitrix24.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-20 10:39:36.000000 fast_bitrix24-1.7.2/fast_bitrix24.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-20 10:39:36.000000 fast_bitrix24-1.7.2/fast_bitrix24.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 10:39:36.694682 fast_bitrix24-1.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 10:39:36.694682 fast_bitrix24-1.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7869 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_server_responses.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_srh.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_throttle.py
--rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-20 10:39:25.000000 fast_bitrix24-1.7.2/tests/test_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:39:35.295163 fast_bitrix24-1.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21752 2024-05-21 14:39:35.295163 fast_bitrix24-1.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20848 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:39:35.291163 fast_bitrix24-1.7.3/fast_bitrix24/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/fast_bitrix24/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/fast_bitrix24/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/fast_bitrix24/bitrix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/fast_bitrix24/correct_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/fast_bitrix24/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/fast_bitrix24/mult_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/fast_bitrix24/server_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/fast_bitrix24/srh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4056 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/fast_bitrix24/throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15363 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/fast_bitrix24/user_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/fast_bitrix24/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:39:35.291163 fast_bitrix24-1.7.3/fast_bitrix24.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21752 2024-05-21 14:39:35.000000 fast_bitrix24-1.7.3/fast_bitrix24.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-21 14:39:35.000000 fast_bitrix24-1.7.3/fast_bitrix24.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:39:35.000000 fast_bitrix24-1.7.3/fast_bitrix24.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-21 14:39:35.000000 fast_bitrix24-1.7.3/fast_bitrix24.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-21 14:39:35.000000 fast_bitrix24-1.7.3/fast_bitrix24.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 14:39:35.295163 fast_bitrix24-1.7.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:39:35.291163 fast_bitrix24-1.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1213 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8195 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/tests/test_server_responses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/tests/test_srh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/tests/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/tests/test_throttle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3317 2024-05-21 14:39:19.000000 fast_bitrix24-1.7.3/tests/test_warnings.py
```

### Comparing `fast_bitrix24-1.7.2/LICENSE` & `fast_bitrix24-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/PKG-INFO` & `fast_bitrix24-1.7.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_bitrix24
-Version: 1.7.2
+Version: 1.7.3
 Summary: API wrapper для быстрого получения данных от Битрикс24 через REST API. Параллельные запросы к серверу, упаковка запросов в батчи, контроль скорости запросов, есть синхронный и асинхронный клиенты.
 Home-page: https://github.com/leshchenko1979/fast_bitrix24
 Author: Alexey Leshchenko
 Author-email: leshchenko@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fast_bitrix24-1.7.2/README.md` & `fast_bitrix24-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/fast_bitrix24/bitrix.py` & `fast_bitrix24-1.7.3/fast_bitrix24/bitrix.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/fast_bitrix24/logger.py` & `fast_bitrix24-1.7.3/fast_bitrix24/logger.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/fast_bitrix24/mult_request.py` & `fast_bitrix24-1.7.3/fast_bitrix24/mult_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,15 +99,15 @@
             if self.results is None:
                 self.results = extracted
             elif isinstance(extracted, list):
                 self.results.extend(extracted)
             elif isinstance(extracted, dict):
                 self.results.update(extracted)
 
-            extracted_len += len(extracted)
+            extracted_len += len(extracted) if isinstance(extracted, list) else 1
 
         return extracted_len
 
     def get_pbar(self):
         """Возвращает прогресс бар `tqdm()` или пустышку,
         если `self.bitrix.verbose is False`."""
```

### Comparing `fast_bitrix24-1.7.2/fast_bitrix24/server_response.py` & `fast_bitrix24-1.7.3/fast_bitrix24/server_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,37 +66,27 @@
 
         return None
 
     def is_batch(self) -> bool:
         return isinstance(self.result, dict) and "result" in self.result
 
     def extract_from_single_response(self, result: dict):
-        # если результат вызова содержит только словарь {ключ: список},
-        # то вернуть этот список.
+        # если результат вызова содержит только словарь из одного элемента {ключ: содержимое},
+        # то вернуть это содержимое.
         # См. https://github.com/leshchenko1979/fast_bitrix24/issues/132
 
         # метод `crm.stagehistory.list` возвращает dict["items", list] --
         # разворачиваем его в список
 
-        if self.is_nested(result):
-            contents = self.extract_from_nested(result)
-            if isinstance(contents, list):
-                return contents
-
-        return result
+        return next(iter(result.values())) if self.is_nested(result) else result
 
     @staticmethod
     def is_nested(result) -> bool:
         return isinstance(result, dict) and len(result) == 1
 
-    @staticmethod
-    def extract_from_nested(result: dict):
-        return next(iter(result.values()))
-
-
     def extract_from_batch_response(self, result) -> list:
 
         if not result:
             return []
 
         # если результат вызова содержит только словарь c одним ключом
         # и списком у него внутри, то вернуть этот список.
@@ -107,13 +97,15 @@
         # если внутри - списки, то вернуть их в одном плоском списке
         if self.is_nested(first_item) or isinstance(first_item, list):
             result_list = [
                 self.extract_from_single_response(element)
                 for element in result.values()
             ]
 
-            result_list = list(chain(*result_list))
+            # если получился вложенный список, то уплощаем
+            if isinstance(result_list[0], list):
+                result_list = list(chain(*result_list))
 
             return result_list
 
         # иначе (если внутри - dict), то вернуть в сам dict
         return result
```

### Comparing `fast_bitrix24-1.7.2/fast_bitrix24/srh.py` & `fast_bitrix24-1.7.3/fast_bitrix24/srh.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/fast_bitrix24/throttle.py` & `fast_bitrix24-1.7.3/fast_bitrix24/throttle.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/fast_bitrix24/user_request.py` & `fast_bitrix24-1.7.3/fast_bitrix24/user_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,21 +323,20 @@
             self.bitrix,
             self.method,
             self.item_list,
             ID_field=self.ID_field_name,
             get_by_ID=False,
         ).run()
 
-        if isinstance(raw_results, dict):
-            results = tuple(raw_results.values())
+        if isinstance(raw_results, dict) and not is_single_item:
+            return tuple(raw_results.values())
+        elif raw_results and isinstance(raw_results, list) and is_single_item:
+            return raw_results[0]
         else:
-            # бывают случаи, что возвращается список
-            results = raw_results
-
-        return results[0] if results and is_single_item else results
+            return raw_results
 
     def prepare_item_list(self):
         # При отправке батчей на сервер результаты приходят не в том порядке,
         # в котором они отправлялись. Для того, чтобы пользователь мог понять,
         # какой результат пришел по каждому конкретному элементу списка,
         # переданному в call(), нужно возвращать не результаты запроса общим списком,
         # где может быть нарушен порядок, а словарь, содержащий на результаты запроса
```

### Comparing `fast_bitrix24-1.7.2/fast_bitrix24/utils.py` & `fast_bitrix24-1.7.3/fast_bitrix24/utils.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/fast_bitrix24.egg-info/PKG-INFO` & `fast_bitrix24-1.7.3/fast_bitrix24.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast_bitrix24
-Version: 1.7.2
+Version: 1.7.3
 Summary: API wrapper для быстрого получения данных от Битрикс24 через REST API. Параллельные запросы к серверу, упаковка запросов в батчи, контроль скорости запросов, есть синхронный и асинхронный клиенты.
 Home-page: https://github.com/leshchenko1979/fast_bitrix24
 Author: Alexey Leshchenko
 Author-email: leshchenko@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `fast_bitrix24-1.7.2/fast_bitrix24.egg-info/SOURCES.txt` & `fast_bitrix24-1.7.3/fast_bitrix24.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/setup.py` & `fast_bitrix24-1.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/tests/test_async.py` & `fast_bitrix24-1.7.3/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/tests/test_exceptions.py` & `fast_bitrix24-1.7.3/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/tests/test_helpers.py` & `fast_bitrix24-1.7.3/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/tests/test_server_responses.py` & `fast_bitrix24-1.7.3/tests/test_server_responses.py`

 * *Files 4% similar despite different names*

```diff
@@ -256,7 +256,17 @@
                 "SPAM_PERMS",
                 "SUBJECT_NAME",
             ]
         },
     )
 
     assert len(results) == 50
+
+
+def test_crm_add_item(bx_dummy):
+    from tests.real_responses.crm_item_add import response
+
+    bx_dummy.srh = MockSRH(response)
+    result = bx_dummy.call(
+        "crm.item.add", {"entityTypeId": 1, "fields": {"first_name": "first_name"}}
+    )
+    assert result != "item" and isinstance(result, dict) and "id" in result
```

### Comparing `fast_bitrix24-1.7.2/tests/test_srh.py` & `fast_bitrix24-1.7.3/tests/test_srh.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/tests/test_sync.py` & `fast_bitrix24-1.7.3/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/tests/test_throttle.py` & `fast_bitrix24-1.7.3/tests/test_throttle.py`

 * *Files identical despite different names*

### Comparing `fast_bitrix24-1.7.2/tests/test_warnings.py` & `fast_bitrix24-1.7.3/tests/test_warnings.py`

 * *Files identical despite different names*

