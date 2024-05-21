# Comparing `tmp/some_aiohttp_middleware-0.1.6.tar.gz` & `tmp/some_aiohttp_middleware-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "some_aiohttp_middleware-0.1.6.tar", max compression
+gzip compressed data, was "some_aiohttp_middleware-0.1.7.tar", max compression
```

## Comparing `some_aiohttp_middleware-0.1.6.tar` & `some_aiohttp_middleware-0.1.7.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1065 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/LICENSE
--rw-r--r--   0        0        0      563 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/README.md
--rw-r--r--   0        0        0     1547 2024-05-17 12:09:09.971817 some_aiohttp_middleware-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      196 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/__init__.py
--rw-r--r--   0        0        0     1762 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/admin_auth_handler.py
--rw-r--r--   0        0        0     4854 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/base.py
--rw-r--r--   0        0        0     2760 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/db.py
--rw-r--r--   0        0        0     2441 2024-05-17 12:08:49.595529 some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/s3.py
--rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 some_aiohttp_middleware-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-05-21 08:37:18.368099 some_aiohttp_middleware-0.1.7/LICENSE
+-rw-r--r--   0        0        0      563 2024-05-21 08:37:18.368099 some_aiohttp_middleware-0.1.7/README.md
+-rw-r--r--   0        0        0     1547 2024-05-21 08:37:39.968187 some_aiohttp_middleware-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-05-21 08:37:18.368099 some_aiohttp_middleware-0.1.7/src/some_aiohttp_middleware/__init__.py
+-rw-r--r--   0        0        0     1755 2024-05-21 08:37:18.368099 some_aiohttp_middleware-0.1.7/src/some_aiohttp_middleware/admin_auth.py
+-rw-r--r--   0        0        0     4854 2024-05-21 08:37:18.368099 some_aiohttp_middleware-0.1.7/src/some_aiohttp_middleware/base.py
+-rw-r--r--   0        0        0     2273 2024-05-21 08:37:18.368099 some_aiohttp_middleware-0.1.7/src/some_aiohttp_middleware/basic_auth.py
+-rw-r--r--   0        0        0     2760 2024-05-21 08:37:18.368099 some_aiohttp_middleware-0.1.7/src/some_aiohttp_middleware/db.py
+-rw-r--r--   0        0        0     2441 2024-05-21 08:37:18.368099 some_aiohttp_middleware-0.1.7/src/some_aiohttp_middleware/s3.py
+-rw-r--r--   0        0        0     1649 1970-01-01 00:00:00.000000 some_aiohttp_middleware-0.1.7/PKG-INFO
```

### Comparing `some_aiohttp_middleware-0.1.6/LICENSE` & `some_aiohttp_middleware-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.6/README.md` & `some_aiohttp_middleware-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.6/pyproject.toml` & `some_aiohttp_middleware-0.1.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "some-aiohttp-middleware"
-version = "0.1.6"
+version = "0.1.7"
 license = "MIT"
 description = "Middleware framework for aiohttp"
 authors = ["tommmlij <tommmlij@gmail.com>"]
 readme = "README.md"
 homepage = "https://github.com/tommmlij/some-aiohttp-middleware"
 packages = [{ include = "some_aiohttp_middleware", from = "src" }]
 
@@ -14,17 +14,17 @@
 
 [tool.poetry.dependencies]
 python = ">=3.8.1 <3.13"
 aiohttp = "^3.9.3"
 sqlalchemy = "^2.0.27"
 asyncpg = "^0.29.0"
 pydantic = "^2.6.4"
-aiohttp-pydantic = "^2.0.0"
 pydantic-settings = "^2.2.1"
 aioboto3 = "^12.4.0"
+aiohttp-pydantic = "^2.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 flake8 = "^7.0.0"
 pytest-asyncio = "^0.23.5"
 pytest-aiohttp = "^1.0.5"
 colorlog = "^6.8.2"
```

### Comparing `some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/admin_auth_handler.py` & `some_aiohttp_middleware-0.1.7/src/some_aiohttp_middleware/admin_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         raise HTTPUnprocessableEntity(reason="Malformed bearer token")
 
 
 class Bearer(BaseModel):
     authorization: Annotated[str, AfterValidator(bearer_check)]
 
 
-class AdminAuthHandler(MiddlewareBase):
+class AdminAuth(MiddlewareBase):
 
     @staticmethod
     async def handle(request, *args, admin_token=None, token_location=None, **kwargs):
 
         if token_location is None:
             token_location = ["admin_token"]
```

### Comparing `some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/base.py` & `some_aiohttp_middleware-0.1.7/src/some_aiohttp_middleware/base.py`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/db.py` & `some_aiohttp_middleware-0.1.7/src/some_aiohttp_middleware/db.py`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.6/src/some_aiohttp_middleware/s3.py` & `some_aiohttp_middleware-0.1.7/src/some_aiohttp_middleware/s3.py`

 * *Files identical despite different names*

### Comparing `some_aiohttp_middleware-0.1.6/PKG-INFO` & `some_aiohttp_middleware-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: some-aiohttp-middleware
-Version: 0.1.6
+Version: 0.1.7
 Summary: Middleware framework for aiohttp
 Home-page: https://github.com/tommmlij/some-aiohttp-middleware
 License: MIT
 Author: tommmlij
 Author-email: tommmlij@gmail.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aioboto3 (>=12.4.0,<13.0.0)
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
-Requires-Dist: aiohttp-pydantic (>=2.0.0,<3.0.0)
+Requires-Dist: aiohttp-pydantic (>=2.1.0,<3.0.0)
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
 Requires-Dist: pydantic (>=2.6.4,<3.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: sqlalchemy (>=2.0.27,<3.0.0)
 Project-URL: GitHub: issues, https://github.com/tommmlij/some-aiohttp-middleware/issues
 Project-URL: GitHub: repo, https://github.com/tommmlij/some-aiohttp-middleware
 Description-Content-Type: text/markdown
```

