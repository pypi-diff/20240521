# Comparing `tmp/smo_rejection-0.4.3.tar.gz` & `tmp/smo_rejection-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smo_rejection-0.4.3.tar", max compression
+gzip compressed data, was "smo_rejection-0.4.4.tar", max compression
```

## Comparing `smo_rejection-0.4.3.tar` & `smo_rejection-0.4.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      283 2024-05-20 15:05:06.949138 smo_rejection-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    16387 2024-05-20 07:59:33.306860 smo_rejection-0.4.3/README.md
--rw-r--r--   0        0        0      496 2024-05-20 15:04:59.554803 smo_rejection-0.4.3/smo_rejection/__init__.py
--rw-r--r--   0        0        0     1709 2024-05-18 10:29:03.257241 smo_rejection-0.4.3/smo_rejection/exception.py
--rw-r--r--   0        0        0     1628 2024-05-18 10:29:03.257241 smo_rejection-0.4.3/smo_rejection/models.py
--rw-r--r--   0        0        0     4236 2024-05-20 07:59:33.326861 smo_rejection-0.4.3/smo_rejection/pdf_export.py
--rw-r--r--   0        0        0     4419 2024-05-18 10:29:03.257241 smo_rejection-0.4.3/smo_rejection/processing.py
--rw-r--r--   0        0        0     4307 2024-05-18 10:29:03.258245 smo_rejection-0.4.3/smo_rejection/simulation.py
--rw-r--r--   0        0        0     2471 2024-05-18 10:29:03.258245 smo_rejection-0.4.3/smo_rejection/utils.py
--rw-r--r--   0        0        0     4797 2024-05-20 14:59:05.590827 smo_rejection-0.4.3/smo_rejection/xml_export.py
--rw-r--r--   0        0        0    16485 1970-01-01 00:00:00.000000 smo_rejection-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      283 2024-05-21 11:14:25.971590 smo_rejection-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    16387 2024-05-21 11:13:02.127103 smo_rejection-0.4.4/README.md
+-rw-r--r--   0        0        0      496 2024-05-21 11:13:02.130096 smo_rejection-0.4.4/smo_rejection/__init__.py
+-rw-r--r--   0        0        0     1709 2024-05-21 11:13:02.136049 smo_rejection-0.4.4/smo_rejection/exception.py
+-rw-r--r--   0        0        0     1628 2024-05-21 11:13:02.136049 smo_rejection-0.4.4/smo_rejection/models.py
+-rw-r--r--   0        0        0     4236 2024-05-21 11:13:02.137051 smo_rejection-0.4.4/smo_rejection/pdf_export.py
+-rw-r--r--   0        0        0     4403 2024-05-21 11:13:28.975815 smo_rejection-0.4.4/smo_rejection/processing.py
+-rw-r--r--   0        0        0     4306 2024-05-21 11:13:02.137051 smo_rejection-0.4.4/smo_rejection/simulation.py
+-rw-r--r--   0        0        0     2471 2024-05-21 11:13:02.138052 smo_rejection-0.4.4/smo_rejection/utils.py
+-rw-r--r--   0        0        0     4797 2024-05-21 11:13:02.138052 smo_rejection-0.4.4/smo_rejection/xml_export.py
+-rw-r--r--   0        0        0    16485 1970-01-01 00:00:00.000000 smo_rejection-0.4.4/PKG-INFO
```

### Comparing `smo_rejection-0.4.3/README.md` & `smo_rejection-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.3/smo_rejection/exception.py` & `smo_rejection-0.4.4/smo_rejection/exception.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.3/smo_rejection/models.py` & `smo_rejection-0.4.4/smo_rejection/models.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.3/smo_rejection/pdf_export.py` & `smo_rejection-0.4.4/smo_rejection/pdf_export.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.3/smo_rejection/processing.py` & `smo_rejection-0.4.4/smo_rejection/processing.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,16 @@
 
         # Сформировать словарь с информацией о текущей заявке
         entry = {
             'index': len(request_times) + 1,
             'rand_value': round(rand_value, 4),
             'iba': round(inter_arrival_time, 4),
             'app_time': round(request_time, 4),
-            'Обслужено': serviced,
-            'Отказов': rejected,
+            'serviced': serviced,
+            'rejected': rejected,
         }
 
         # Добавить информацию о времени окончания обслуживания на каждом канале
         for i in range(num_channels):
             key = f'server_{i + 1}'
             if serviced == 1 and available_server == i:
                 entry[key] = round(service_end_times[i], 4)
```

### Comparing `smo_rejection-0.4.3/smo_rejection/simulation.py` & `smo_rejection-0.4.4/smo_rejection/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     2. Создает объект `SimulationParameters` с заданными параметрами.
     3. Запускает цикл по количеству итераций, на каждой итерации вызывая функцию `process_iteration` и сохраняя ее результат.
     4. Возвращает список объектов `SimulationResult`, содержащих результаты каждой итерации симуляции.
     """
     # Проверка корректности входных параметров
     if T <= 0:
         raise MaxTimeNegative("Максимальное время симуляции должно быть положительным числом.")
-    if num_channels <= 0:
+    if num_channels < 0:
         raise NumChannelsNegative("Количество каналов должно быть положительным числом.")
     if num_channels == 0:
         raise NumChannelsIsZero("Количество каналов не может быть нулевым.")
     if service_time <= 0:
         raise ServiceTimeNegative("Время обслуживания должно быть положительным числом.")
     if num_iterations < 0:
         raise NumIterationsNegative("Количество итераций не может быть отрицательным.")
```

### Comparing `smo_rejection-0.4.3/smo_rejection/utils.py` & `smo_rejection-0.4.4/smo_rejection/utils.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.3/smo_rejection/xml_export.py` & `smo_rejection-0.4.4/smo_rejection/xml_export.py`

 * *Files identical despite different names*

### Comparing `smo_rejection-0.4.3/PKG-INFO` & `smo_rejection-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smo_rejection
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 Author: mbtmrw
 Author-email: keks2324098@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

