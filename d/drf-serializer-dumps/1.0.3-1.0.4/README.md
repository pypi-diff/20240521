# Comparing `tmp/drf_serializer_dumps-1.0.3.tar.gz` & `tmp/drf_serializer_dumps-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_serializer_dumps-1.0.3.tar", last modified: Thu May  2 17:17:38 2024, max compression
+gzip compressed data, was "drf_serializer_dumps-1.0.4.tar", last modified: Tue May 21 19:24:17 2024, max compression
```

## Comparing `drf_serializer_dumps-1.0.3.tar` & `drf_serializer_dumps-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.782069 drf_serializer_dumps-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.774069 drf_serializer_dumps-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.778069 drf_serializer_dumps-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-05-02 17:17:38.778069 drf_serializer_dumps-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)    12272 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-02 17:17:38.782069 drf_serializer_dumps-1.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.774069 drf_serializer_dumps-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.778069 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10088 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.778069 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-05-02 17:17:38.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-02 17:17:38.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 17:17:38.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-02 17:17:38.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-02 17:17:38.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-02 17:17:38.000000 drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:38.778069 drf_serializer_dumps-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/tests/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-02 17:17:34.000000 drf_serializer_dumps-1.0.3/tests/test_decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:24:17.193174 drf_serializer_dumps-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:24:17.189174 drf_serializer_dumps-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:24:17.189174 drf_serializer_dumps-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3771 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-05-21 19:24:17.193174 drf_serializer_dumps-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8350 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12521 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-21 19:24:17.193174 drf_serializer_dumps-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:24:17.189174 drf_serializer_dumps-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:24:17.189174 drf_serializer_dumps-1.0.4/src/drf_serializer_dumps/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/src/drf_serializer_dumps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10303 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/src/drf_serializer_dumps/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:24:17.193174 drf_serializer_dumps-1.0.4/src/drf_serializer_dumps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11652 2024-05-21 19:24:17.000000 drf_serializer_dumps-1.0.4/src/drf_serializer_dumps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-05-21 19:24:17.000000 drf_serializer_dumps-1.0.4/src/drf_serializer_dumps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 19:24:17.000000 drf_serializer_dumps-1.0.4/src/drf_serializer_dumps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-21 19:24:17.000000 drf_serializer_dumps-1.0.4/src/drf_serializer_dumps.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-21 19:24:17.000000 drf_serializer_dumps-1.0.4/src/drf_serializer_dumps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 19:24:17.000000 drf_serializer_dumps-1.0.4/src/drf_serializer_dumps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 19:24:17.193174 drf_serializer_dumps-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/tests/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-21 19:24:13.000000 drf_serializer_dumps-1.0.4/tests/test_decorators.py
```

### Comparing `drf_serializer_dumps-1.0.3/.editorconfig` & `drf_serializer_dumps-1.0.4/.editorconfig`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.3/.github/workflows/publish-to-pypi.yml` & `drf_serializer_dumps-1.0.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.3/.pre-commit-config.yaml` & `drf_serializer_dumps-1.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.3/CONTRIBUTING.md` & `drf_serializer_dumps-1.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.3/LICENSE` & `drf_serializer_dumps-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.3/PKG-INFO` & `drf_serializer_dumps-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf_serializer_dumps
-Version: 1.0.3
+Version: 1.0.4
 Summary: Decorator for creating dict based on the drf serializer class for swagger
 Home-page: https://github.com/Friskes/drf-serializer-dumps
 Author: Friskes
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
```

### Comparing `drf_serializer_dumps-1.0.3/README.md` & `drf_serializer_dumps-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.3/pyproject.toml` & `drf_serializer_dumps-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -175,25 +175,26 @@
     "RET",    # https://docs.astral.sh/ruff/rules/#flake8-return-ret
     "SLF",    # https://docs.astral.sh/ruff/rules/#flake8-self-slf
     "SLOT",   # https://docs.astral.sh/ruff/rules/#flake8-slots-slot
     "SIM",    # https://docs.astral.sh/ruff/rules/#flake8-simplify-sim
     "TID",    # https://docs.astral.sh/ruff/rules/#flake8-tidy-imports-tid
     "TCH",    # https://docs.astral.sh/ruff/rules/#flake8-type-checking-tch
     "INT",    # https://docs.astral.sh/ruff/rules/#flake8-gettext-int
+    "TD",     # https://docs.astral.sh/ruff/rules/#flake8-todos-td
     "FLY",    # https://docs.astral.sh/ruff/rules/#flynt-fly
     "PERF",   # https://docs.astral.sh/ruff/rules/#perflint-perf
     "LOG",    # https://docs.astral.sh/ruff/rules/#flake8-logging-log
     "RUF",    # https://docs.astral.sh/ruff/rules/#ruff-specific-rules-ruf
     #! https://docs.astral.sh/ruff/rules/#refurb-furb
     #! "FURB",  # refurb  (пока что не стабильно 29.03.2024)
 ]
 ignore = [
     # https://docs.astral.sh/ruff/rules/#pyflakes-f
-    "F401",    # (не ругаться на неиспользуемые импорты)
-    "F841",    # (не ругаться на неиспользуемые переменные)
+    # "F401",    # (не ругаться на неиспользуемые импорты)
+    # "F841",    # (не ругаться на неиспользуемые переменные)
     "F403",    # (не ругаться на использование from ... import *)
     # https://docs.astral.sh/ruff/rules/#pyupgrade-up
     "UP031",   # (не ругаться на форматирование с помощью %s)
     # https://docs.astral.sh/ruff/rules/#flake8-logging-format-g
     "G004",    # (не ругаться на использование f-строк для сообщения лога)
     # https://docs.astral.sh/ruff/rules/#ruff-specific-rules-ruf
     "RUF001",  # (не ругаться на кириллицу в строках)
@@ -217,14 +218,16 @@
     # https://docs.astral.sh/ruff/rules/#flake8-blind-except-ble
     "BLE001",  # (не ругаться на обработку обычного Exception)
     # https://docs.astral.sh/ruff/rules/#flake8-django-dj  #! (ВРЕМЕННО)
     "DJ001",   # (не ругаться на использование null в моделях для текстовых полей)
     # https://docs.astral.sh/ruff/rules/#flake8-comprehensions-c4
     # {} VS dict()  # https://switowski.com/blog/dict-function-vs-literal-syntax/
     "C408",    # (не ругаться на использование классов коллекций вместо их литералов)
+    "TD001",   # (не ругаться на использование FIXME и XXX)
+    "TD003",   # (не ругаться на отсутствие ссылки на issues)
 ]
 # Не давать исправлять эти ошибки в тултипе, и в том числе автоматически при линте через команду
 unfixable = [
 ]
 
 
 [tool.ruff.lint.per-file-ignores]
```

### Comparing `drf_serializer_dumps-1.0.3/src/drf_serializer_dumps/decorators.py` & `drf_serializer_dumps-1.0.4/src/drf_serializer_dumps/decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,14 +90,15 @@
     if renew_type_value:
         global _uuid
         global _now
         _uuid = uuid4()
         _now = timezone.now()
 
     field_type_mapping = {
+        serializers.ChoiceField: 'string',
         serializers.CharField: 'string',
         serializers.FloatField: 1.0,
         serializers.BooleanField: False,
         serializers.IntegerField: 1,
         serializers.UUIDField: _uuid,
         serializers.DateTimeField: _now,
         serializers.DateField: _now.date(),
@@ -192,15 +193,19 @@
                 example_val[field_name] = [type_mapping.get(type(field_instance.child))]
 
             elif not isinstance(field_instance, serializers.SerializerMethodField):
                 base_field_cls = type(field_instance).__bases__[0]  # __mro__
                 if base_field_cls is not serializers.Field and not issubclass(
                     base_field_cls, serializers.Serializer
                 ):
-                    example_val[field_name] = base_field_cls().to_representation(
+                    kwargs = {}
+                    if isinstance(field_instance, serializers.ChoiceField):
+                        kwargs.update({'choices': ()})
+
+                    example_val[field_name] = base_field_cls(**kwargs).to_representation(
                         type_mapping.get(base_field_cls)
                     )
                 elif isinstance(field_instance, serializers.Serializer):
                     example_val[field_name] = _walk_fields_recursively(
                         type(field_instance), exclude_fields
                     )
                 else:
```

### Comparing `drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/PKG-INFO` & `drf_serializer_dumps-1.0.4/src/drf_serializer_dumps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf_serializer_dumps
-Version: 1.0.3
+Version: 1.0.4
 Summary: Decorator for creating dict based on the drf serializer class for swagger
 Home-page: https://github.com/Friskes/drf-serializer-dumps
 Author: Friskes
 Author-email: Friskes <friskesx@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Friskes
```

### Comparing `drf_serializer_dumps-1.0.3/src/drf_serializer_dumps.egg-info/SOURCES.txt` & `drf_serializer_dumps-1.0.4/src/drf_serializer_dumps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `drf_serializer_dumps-1.0.3/tests/serializers.py` & `drf_serializer_dumps-1.0.4/tests/serializers.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 class PersonCars(serializers.Serializer):
     car_name = serializers.CharField()
     car_price = serializers.IntegerField()
 
 
 class PersonHouse(serializers.Serializer):
     address = serializers.CharField()
+    cfield = serializers.ChoiceField(choices=())
 
 
 class PersonSerializer1(serializers.Serializer):
     name = serializers.CharField()
     age = serializers.IntegerField()
     birthday = serializers.DateTimeField()
```

### Comparing `drf_serializer_dumps-1.0.3/tests/test_decorators.py` & `drf_serializer_dumps-1.0.4/tests/test_decorators.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     assert result == {
         'name': 'string',
         'birthday': ANY,
         'field_without_annotation': None,
         'height': 1,
         'weight': 1,
         'cars': [{'car_name': 'string', 'car_price': 1}],
-        'house': {'address': 'string'},
+        'house': {'address': 'string', 'cfield': 'string'},
     }
 
 
 def test_model_serializer_dumps() -> None:
     """"""
     result = serializer_dumps(PersonSerializer2)
     assert result == {'id': 1, 'name': 'string', 'phones': ['string']}
@@ -34,15 +34,15 @@
         'name': 'string',
         'age': 1,
         'birthday': ANY,
         'field_without_annotation': None,
         'height': 1,
         'weight': 1,
         'cars': [{'car_name': 'string', 'car_price': 1}],
-        'house': {'address': 'string'},
+        'house': {'address': 'string', 'cfield': 'string'},
     }
 
     result1 = serializer_dumps(PersonSerializer1, renew_type_value=True)
     assert result1 == expected
 
     sleep(0.01)
```

