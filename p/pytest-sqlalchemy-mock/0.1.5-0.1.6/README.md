# Comparing `tmp/pytest-sqlalchemy-mock-0.1.5.tar.gz` & `tmp/pytest_sqlalchemy_mock-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-sqlalchemy-mock-0.1.5.tar", last modified: Wed Mar 15 16:52:53 2023, max compression
+gzip compressed data, was "pytest_sqlalchemy_mock-0.1.6.tar", last modified: Tue May 21 11:13:59 2024, max compression
```

## Comparing `pytest-sqlalchemy-mock-0.1.5.tar` & `pytest_sqlalchemy_mock-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:52:53.841323 pytest-sqlalchemy-mock-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-15 16:52:44.000000 pytest-sqlalchemy-mock-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-15 16:52:53.841323 pytest-sqlalchemy-mock-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-03-15 16:52:44.000000 pytest-sqlalchemy-mock-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:52:53.837323 pytest-sqlalchemy-mock-0.1.5/pytest_sqlalchemy_mock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 16:52:44.000000 pytest-sqlalchemy-mock-0.1.5/pytest_sqlalchemy_mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-03-15 16:52:44.000000 pytest-sqlalchemy-mock-0.1.5/pytest_sqlalchemy_mock/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-03-15 16:52:44.000000 pytest-sqlalchemy-mock-0.1.5/pytest_sqlalchemy_mock/model_mocker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:52:53.841323 pytest-sqlalchemy-mock-0.1.5/pytest_sqlalchemy_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-15 16:52:53.000000 pytest-sqlalchemy-mock-0.1.5/pytest_sqlalchemy_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      456 2023-03-15 16:52:53.000000 pytest-sqlalchemy-mock-0.1.5/pytest_sqlalchemy_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 16:52:53.000000 pytest-sqlalchemy-mock-0.1.5/pytest_sqlalchemy_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-15 16:52:53.000000 pytest-sqlalchemy-mock-0.1.5/pytest_sqlalchemy_mock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-15 16:52:53.000000 pytest-sqlalchemy-mock-0.1.5/pytest_sqlalchemy_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-15 16:52:53.000000 pytest-sqlalchemy-mock-0.1.5/pytest_sqlalchemy_mock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-03-15 16:52:53.841323 pytest-sqlalchemy-mock-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-15 16:52:44.000000 pytest-sqlalchemy-mock-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:52:53.841323 pytest-sqlalchemy-mock-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-03-15 16:52:44.000000 pytest-sqlalchemy-mock-0.1.5/tests/test_pytest_sqlalchemy_mock.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:13:59.604983 pytest_sqlalchemy_mock-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-21 11:13:50.000000 pytest_sqlalchemy_mock-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-21 11:13:59.604983 pytest_sqlalchemy_mock-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-05-21 11:13:50.000000 pytest_sqlalchemy_mock-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-21 11:13:50.000000 pytest_sqlalchemy_mock-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:13:59.604983 pytest_sqlalchemy_mock-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:13:59.600983 pytest_sqlalchemy_mock-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:13:59.600983 pytest_sqlalchemy_mock-0.1.6/src/pytest_sqlalchemy_mock/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:13:50.000000 pytest_sqlalchemy_mock-0.1.6/src/pytest_sqlalchemy_mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-21 11:13:50.000000 pytest_sqlalchemy_mock-0.1.6/src/pytest_sqlalchemy_mock/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-21 11:13:50.000000 pytest_sqlalchemy_mock-0.1.6/src/pytest_sqlalchemy_mock/model_mocker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:13:59.604983 pytest_sqlalchemy_mock-0.1.6/src/pytest_sqlalchemy_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5381 2024-05-21 11:13:59.000000 pytest_sqlalchemy_mock-0.1.6/src/pytest_sqlalchemy_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-21 11:13:59.000000 pytest_sqlalchemy_mock-0.1.6/src/pytest_sqlalchemy_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:13:59.000000 pytest_sqlalchemy_mock-0.1.6/src/pytest_sqlalchemy_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-21 11:13:59.000000 pytest_sqlalchemy_mock-0.1.6/src/pytest_sqlalchemy_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 11:13:59.000000 pytest_sqlalchemy_mock-0.1.6/src/pytest_sqlalchemy_mock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:13:59.604983 pytest_sqlalchemy_mock-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-21 11:13:50.000000 pytest_sqlalchemy_mock-0.1.6/tests/test_pytest_sqlalchemy_mock.py
```

### Comparing `pytest-sqlalchemy-mock-0.1.5/LICENSE` & `pytest_sqlalchemy_mock-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-sqlalchemy-mock-0.1.5/PKG-INFO` & `pytest_sqlalchemy_mock-0.1.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,94 +1,115 @@
-Metadata-Version: 2.1
-Name: pytest-sqlalchemy-mock
-Version: 0.1.5
-Summary: pytest sqlalchemy plugin for mock
-Home-page: https://github.com/resulyrt93/pytest-sqlalchemy-mock
-Author: Resul Yurttakalan
-Author-email: resulyrt93@gmail.com
-License: MIT
-Classifier: Framework :: Pytest
-Classifier: Development Status :: 3 - Alpha
-Classifier: Topic :: Software Development :: Testing
-Classifier: Intended Audience :: Developers
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
+# pytest-sqlalchemy-mock
 
-# pytest-sqlalchemy-mock  👋
 [![PyPI version](https://badge.fury.io/py/pytest-sqlalchemy-mock.svg)](https://badge.fury.io/py/pytest-sqlalchemy-mock)
 [![codecov](https://codecov.io/gh/resulyrt93/pytest-sqlalchemy-mock/branch/dev/graph/badge.svg?token=RUQ4DN3CH9)](https://codecov.io/gh/resulyrt93/pytest-sqlalchemy-mock)
 [![CI](https://github.com/resulyrt93/pytest-sqlalchemy-mock/actions/workflows/tests.yaml/badge.svg?branch=dev)](https://github.com/resulyrt93/pytest-sqlalchemy-mock/actions/workflows/tests.yaml)
 [![Supported Python Version](https://img.shields.io/pypi/pyversions/pytest-sqlalchemy-mock)](https://github.com/resulyrt93/pytest-sqlalchemy-mock)
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 
 This plugin provides pytest fixtures to create an in-memory DB instance on tests and dump your raw test data.
 
+## Supported Python versions
+
+Python 3.12 or later highly recommended but also might work on Python 3.11.
+
 ## Installation
-```
+
+### Download from PyPI
+
+```python
 pip install pytest-sqlalchemy-mock
 ```
 
+### Building from source
+
+At the top direcotry,
+
+```sh
+python3 -m build
+python3 -m pip install dist/pytest_sqlalchemy_mock-*.whl
+```
+
+or
+
+```sh
+python3 -m pip install .
+```
+
+## Uninstall
+
+```sh
+python3 -m pip uninstall pytest_sqlalchemy_mock
+```
+
 ## Usage
+
 Let's assume you have a SQLAlchemy declarative base and some models with it.
 
-**models.py**
+### models.py
+
 ```python
 from sqlalchemy import Column, Integer, String
 from sqlalchemy.orm import declarative_base
 
 Base = declarative_base()
 
 
 class User(Base):
     __tablename__ = "user"
 
     id = Column(Integer, primary_key=True)
     name = Column(String)
 ```
+
 Firstly SQLAlchemy base class which is used for declare models should be passed with `sqlalchemy_declarative_base` fixture in `conftest.py`
 
-**conftest.py**
+### conftest.py
+
 ```python
 @pytest.fixture(scope="function")
 def sqlalchemy_declarative_base():
     return Base
 ```
+
 Then in test functions you can use `mocked_session` fixture to make query in mocked DB.
 
-**test_user_table.py**
+### test_user_table.py
+
 ```python
 def test_mocked_session_user_table(mocked_session):
     user_data = mocked_session.execute("SELECT * from user;").all()
     assert user_data == []
 ```
+
 Also, you can dump your mock data to DB before start testing via `sqlalchemy_mock_config` fixture like following.
 
-**conftest.py**
+### conftest.py
+
 ```python
 @pytest.fixture(scope="function")
 def sqlalchemy_mock_config():
     return [("user", [
         {
             "id": 1,
             "name": "Kevin"
         },
         {
             "id": 2,
             "name": "Dwight"
         }
     ])]
 ```
-**test_user_table.py**
+
+### test_user_table.py
+
 ```python
 def test_mocked_session_user_class(mocked_session):
     user = mocked_session.query(User).filter_by(id=2).first()
     assert user.name == "Dwight"
 ```
 
 ## Upcoming Features
+
 * Mock with decorator for specific DB states for specific cases.
 * Support to load data from `.json` and `.csv`
 * Async SQLAlchemy support
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytest-sqlalchemy-mock-0.1.5/pytest_sqlalchemy_mock/base.py` & `pytest_sqlalchemy_mock-0.1.6/src/pytest_sqlalchemy_mock/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,19 +41,15 @@
 def session(connection):
     session: Session = sessionmaker()(bind=connection)
     yield session
     session.close()
 
 
 @pytest.fixture(scope="function")
-def mocked_session(
-    connection, sqlalchemy_declarative_base, sqlalchemy_mock_config
-):
+def mocked_session(connection, sqlalchemy_declarative_base, sqlalchemy_mock_config):
     session: Session = sessionmaker()(bind=connection)
 
     if sqlalchemy_declarative_base and sqlalchemy_mock_config:
-        ModelMocker(
-            session, sqlalchemy_declarative_base, sqlalchemy_mock_config
-        ).create_all()
+        ModelMocker(session, sqlalchemy_declarative_base, sqlalchemy_mock_config).create_all()
 
     yield session
     session.close()
```

### Comparing `pytest-sqlalchemy-mock-0.1.5/pytest_sqlalchemy_mock/model_mocker.py` & `pytest_sqlalchemy_mock-0.1.6/src/pytest_sqlalchemy_mock/model_mocker.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
-    from typing import List, Tuple
+    from typing import (
+        List,
+        Tuple,
+    )
 
     from sqlalchemy import Table
     from sqlalchemy.orm import Session
 
     MOCK_CONFIG_TYPE = List[Tuple[str, List]]
```

### Comparing `pytest-sqlalchemy-mock-0.1.5/tests/test_pytest_sqlalchemy_mock.py` & `pytest_sqlalchemy_mock-0.1.6/tests/test_pytest_sqlalchemy_mock.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from sqlalchemy import text
 
 from .data import MockData
-from .db import Department, User
+from .db import (
+    Department,
+    User,
+)
 
 
 def test_get_session(session):
     assert session.execute(text("SELECT 5")).scalar() == 5
 
 
 def test_session_user_table(session):
     assert session.execute(text("SELECT count(*) from user")).scalar() == 0
 
 
 def test_session_query_for_assocation_table(session):
-    assert (
-        session.execute(text("SELECT count(*) from user_department")).scalar()
-        == 0
-    )
+    assert session.execute(text("SELECT count(*) from user_department")).scalar() == 0
 
 
 def test_mocked_session_user_table(mocked_session):
     user_data = mocked_session.execute(text("SELECT * from user;")).first()
     raw_data = MockData.USER_DATA[0]
     assert user_data[0] == raw_data["id"]
     assert user_data[1] == raw_data["name"]
```

