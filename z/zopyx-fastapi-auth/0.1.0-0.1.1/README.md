# Comparing `tmp/zopyx_fastapi_auth-0.1.0.tar.gz` & `tmp/zopyx_fastapi_auth-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zopyx_fastapi_auth-0.1.0.tar", last modified: Tue May 21 17:50:48 2024, max compression
+gzip compressed data, was "zopyx_fastapi_auth-0.1.1.tar", last modified: Tue May 21 18:07:31 2024, max compression
```

## Comparing `zopyx_fastapi_auth-0.1.0.tar` & `zopyx_fastapi_auth-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,74 @@
-drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 17:50:48.580695 zopyx_fastapi_auth-0.1.0/
--rw-r--r--   0 ajung      (501) staff       (20)      460 2024-05-21 17:50:48.579718 zopyx_fastapi_auth-0.1.0/PKG-INFO
--rw-------   0 ajung      (501) staff       (20)     4183 2024-05-21 17:13:14.000000 zopyx_fastapi_auth-0.1.0/README.md
-drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 17:50:48.572648 zopyx_fastapi_auth-0.1.0/fastapi_auth/
--rw-------   0 ajung      (501) staff       (20)       14 2024-05-19 14:39:22.000000 zopyx_fastapi_auth-0.1.0/fastapi_auth/__init__.py
--rw-r--r--   0 ajung      (501) staff       (20)      373 2024-05-21 15:46:25.000000 zopyx_fastapi_auth-0.1.0/fastapi_auth/auth_config.py
--rw-------   0 ajung      (501) staff       (20)     2828 2024-05-21 16:26:03.000000 zopyx_fastapi_auth-0.1.0/fastapi_auth/auth_routes.py
--rw-------   0 ajung      (501) staff       (20)     2849 2024-05-21 16:53:06.000000 zopyx_fastapi_auth-0.1.0/fastapi_auth/demo_app.py
--rw-------   0 ajung      (501) staff       (20)     1972 2024-05-21 17:09:49.000000 zopyx_fastapi_auth-0.1.0/fastapi_auth/dependencies.py
--rw-------   0 ajung      (501) staff       (20)      466 2024-05-21 00:44:36.000000 zopyx_fastapi_auth-0.1.0/fastapi_auth/jinja2_templates.py
--rw-------   0 ajung      (501) staff       (20)      106 2024-05-20 17:48:26.000000 zopyx_fastapi_auth-0.1.0/fastapi_auth/logger.py
--rw-------   0 ajung      (501) staff       (20)      294 2024-05-21 00:42:54.000000 zopyx_fastapi_auth-0.1.0/fastapi_auth/permissions.py
--rw-------   0 ajung      (501) staff       (20)     1722 2024-05-21 00:44:16.000000 zopyx_fastapi_auth-0.1.0/fastapi_auth/roles.py
--rw-------   0 ajung      (501) staff       (20)     2096 2024-05-21 15:48:34.000000 zopyx_fastapi_auth-0.1.0/fastapi_auth/user_cmd.py
--rw-------   0 ajung      (501) staff       (20)     4591 2024-05-21 15:48:28.000000 zopyx_fastapi_auth-0.1.0/fastapi_auth/user_management.py
--rw-------   0 ajung      (501) staff       (20)     1242 2024-05-21 16:49:33.000000 zopyx_fastapi_auth-0.1.0/fastapi_auth/users.py
--rw-------   0 ajung      (501) staff       (20)      705 2024-05-21 17:50:44.000000 zopyx_fastapi_auth-0.1.0/pyproject.toml
--rw-------   0 ajung      (501) staff       (20)       38 2024-05-21 17:50:48.580870 zopyx_fastapi_auth-0.1.0/setup.cfg
-drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 17:50:48.578863 zopyx_fastapi_auth-0.1.0/zopyx_fastapi_auth.egg-info/
--rw-r--r--   0 ajung      (501) staff       (20)      460 2024-05-21 17:50:48.000000 zopyx_fastapi_auth-0.1.0/zopyx_fastapi_auth.egg-info/PKG-INFO
--rw-------   0 ajung      (501) staff       (20)      598 2024-05-21 17:50:48.000000 zopyx_fastapi_auth-0.1.0/zopyx_fastapi_auth.egg-info/SOURCES.txt
--rw-------   0 ajung      (501) staff       (20)        1 2024-05-21 17:50:48.000000 zopyx_fastapi_auth-0.1.0/zopyx_fastapi_auth.egg-info/dependency_links.txt
--rw-------   0 ajung      (501) staff       (20)       71 2024-05-21 17:50:48.000000 zopyx_fastapi_auth-0.1.0/zopyx_fastapi_auth.egg-info/entry_points.txt
--rw-------   0 ajung      (501) staff       (20)      124 2024-05-21 17:50:48.000000 zopyx_fastapi_auth-0.1.0/zopyx_fastapi_auth.egg-info/requires.txt
--rw-------   0 ajung      (501) staff       (20)       13 2024-05-21 17:50:48.000000 zopyx_fastapi_auth-0.1.0/zopyx_fastapi_auth.egg-info/top_level.txt
+drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:07:31.713205 zopyx_fastapi_auth-0.1.1/
+-rw-------   0 ajung      (501) staff       (20)       27 2024-05-21 18:06:00.000000 zopyx_fastapi_auth-0.1.1/MANIFEST.in
+-rw-r--r--   0 ajung      (501) staff       (20)      460 2024-05-21 18:07:31.712798 zopyx_fastapi_auth-0.1.1/PKG-INFO
+-rw-------   0 ajung      (501) staff       (20)     4183 2024-05-21 17:13:14.000000 zopyx_fastapi_auth-0.1.1/README.md
+drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:07:31.645909 zopyx_fastapi_auth-0.1.1/fastapi_auth/
+-rw-------   0 ajung      (501) staff       (20)       14 2024-05-19 14:39:22.000000 zopyx_fastapi_auth-0.1.1/fastapi_auth/__init__.py
+-rw-r--r--   0 ajung      (501) staff       (20)      373 2024-05-21 15:46:25.000000 zopyx_fastapi_auth-0.1.1/fastapi_auth/auth_config.py
+-rw-------   0 ajung      (501) staff       (20)     2828 2024-05-21 16:26:03.000000 zopyx_fastapi_auth-0.1.1/fastapi_auth/auth_routes.py
+-rw-------   0 ajung      (501) staff       (20)     2849 2024-05-21 16:53:06.000000 zopyx_fastapi_auth-0.1.1/fastapi_auth/demo_app.py
+-rw-------   0 ajung      (501) staff       (20)     1972 2024-05-21 17:09:49.000000 zopyx_fastapi_auth-0.1.1/fastapi_auth/dependencies.py
+-rw-------   0 ajung      (501) staff       (20)      466 2024-05-21 00:44:36.000000 zopyx_fastapi_auth-0.1.1/fastapi_auth/jinja2_templates.py
+-rw-------   0 ajung      (501) staff       (20)      106 2024-05-20 17:48:26.000000 zopyx_fastapi_auth-0.1.1/fastapi_auth/logger.py
+-rw-------   0 ajung      (501) staff       (20)      294 2024-05-21 00:42:54.000000 zopyx_fastapi_auth-0.1.1/fastapi_auth/permissions.py
+-rw-------   0 ajung      (501) staff       (20)     1722 2024-05-21 00:44:16.000000 zopyx_fastapi_auth-0.1.1/fastapi_auth/roles.py
+-rw-------   0 ajung      (501) staff       (20)     2096 2024-05-21 15:48:34.000000 zopyx_fastapi_auth-0.1.1/fastapi_auth/user_cmd.py
+-rw-------   0 ajung      (501) staff       (20)     4591 2024-05-21 15:48:28.000000 zopyx_fastapi_auth-0.1.1/fastapi_auth/user_management.py
+-rw-------   0 ajung      (501) staff       (20)     1242 2024-05-21 16:49:33.000000 zopyx_fastapi_auth-0.1.1/fastapi_auth/users.py
+-rw-------   0 ajung      (501) staff       (20)      705 2024-05-21 18:06:27.000000 zopyx_fastapi_auth-0.1.1/pyproject.toml
+-rw-------   0 ajung      (501) staff       (20)       38 2024-05-21 18:07:31.713250 zopyx_fastapi_auth-0.1.1/setup.cfg
+drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:07:31.628517 zopyx_fastapi_auth-0.1.1/static/
+drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:07:31.628943 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/
+drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:07:31.686708 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/
+-rw-------   0 ajung      (501) staff       (20)    70329 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css
+-rw-------   0 ajung      (501) staff       (20)   203221 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.css.map
+-rw-------   0 ajung      (501) staff       (20)    51795 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css
+-rw-------   0 ajung      (501) staff       (20)   115986 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.min.css.map
+-rw-------   0 ajung      (501) staff       (20)    70403 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css
+-rw-------   0 ajung      (501) staff       (20)   203225 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.css.map
+-rw-------   0 ajung      (501) staff       (20)    51870 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css
+-rw-------   0 ajung      (501) staff       (20)   116063 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-grid.rtl.min.css.map
+-rw-------   0 ajung      (501) staff       (20)    12065 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css
+-rw-------   0 ajung      (501) staff       (20)   129371 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.css.map
+-rw-------   0 ajung      (501) staff       (20)    10126 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css
+-rw-------   0 ajung      (501) staff       (20)    51369 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.min.css.map
+-rw-------   0 ajung      (501) staff       (20)    12058 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css
+-rw-------   0 ajung      (501) staff       (20)   129386 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.css.map
+-rw-------   0 ajung      (501) staff       (20)    10198 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css
+-rw-------   0 ajung      (501) staff       (20)    63943 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-reboot.rtl.min.css.map
+-rw-------   0 ajung      (501) staff       (20)   107823 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css
+-rw-------   0 ajung      (501) staff       (20)   267535 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.css.map
+-rw-------   0 ajung      (501) staff       (20)    85352 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css
+-rw-------   0 ajung      (501) staff       (20)   180381 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.min.css.map
+-rw-------   0 ajung      (501) staff       (20)   107691 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css
+-rw-------   0 ajung      (501) staff       (20)   267476 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.css.map
+-rw-------   0 ajung      (501) staff       (20)    85281 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css
+-rw-------   0 ajung      (501) staff       (20)   180217 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap-utilities.rtl.min.css.map
+-rw-------   0 ajung      (501) staff       (20)   281046 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.css
+-rw-------   0 ajung      (501) staff       (20)   679755 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.css.map
+-rw-------   0 ajung      (501) staff       (20)   232803 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css
+-rw-------   0 ajung      (501) staff       (20)   589892 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.min.css.map
+-rw-------   0 ajung      (501) staff       (20)   280259 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css
+-rw-------   0 ajung      (501) staff       (20)   679615 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.css.map
+-rw-------   0 ajung      (501) staff       (20)   232911 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css
+-rw-------   0 ajung      (501) staff       (20)   589087 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/css/bootstrap.rtl.min.css.map
+drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:07:31.703137 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/js/
+-rw-------   0 ajung      (501) staff       (20)   207819 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js
+-rw-------   0 ajung      (501) staff       (20)   444579 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.js.map
+-rw-------   0 ajung      (501) staff       (20)    80721 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js
+-rw-------   0 ajung      (501) staff       (20)   332090 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.bundle.min.js.map
+-rw-------   0 ajung      (501) staff       (20)   135829 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js
+-rw-------   0 ajung      (501) staff       (20)   305438 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.js.map
+-rw-------   0 ajung      (501) staff       (20)    73935 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js
+-rw-------   0 ajung      (501) staff       (20)   222455 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.esm.min.js.map
+-rw-------   0 ajung      (501) staff       (20)   145401 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.js
+-rw-------   0 ajung      (501) staff       (20)   306606 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.js.map
+-rw-------   0 ajung      (501) staff       (20)    60635 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js
+-rw-------   0 ajung      (501) staff       (20)   220561 2024-05-02 16:17:10.000000 zopyx_fastapi_auth-0.1.1/static/bootstrap-5.3.3-dist/js/bootstrap.min.js.map
+drwx------   0 ajung      (501) staff       (20)        0 2024-05-21 18:07:31.712336 zopyx_fastapi_auth-0.1.1/zopyx_fastapi_auth.egg-info/
+-rw-r--r--   0 ajung      (501) staff       (20)      460 2024-05-21 18:07:31.000000 zopyx_fastapi_auth-0.1.1/zopyx_fastapi_auth.egg-info/PKG-INFO
+-rw-------   0 ajung      (501) staff       (20)     3070 2024-05-21 18:07:31.000000 zopyx_fastapi_auth-0.1.1/zopyx_fastapi_auth.egg-info/SOURCES.txt
+-rw-------   0 ajung      (501) staff       (20)        1 2024-05-21 18:07:31.000000 zopyx_fastapi_auth-0.1.1/zopyx_fastapi_auth.egg-info/dependency_links.txt
+-rw-------   0 ajung      (501) staff       (20)       71 2024-05-21 18:07:31.000000 zopyx_fastapi_auth-0.1.1/zopyx_fastapi_auth.egg-info/entry_points.txt
+-rw-------   0 ajung      (501) staff       (20)      124 2024-05-21 18:07:31.000000 zopyx_fastapi_auth-0.1.1/zopyx_fastapi_auth.egg-info/requires.txt
+-rw-------   0 ajung      (501) staff       (20)       13 2024-05-21 18:07:31.000000 zopyx_fastapi_auth-0.1.1/zopyx_fastapi_auth.egg-info/top_level.txt
```

### Comparing `zopyx_fastapi_auth-0.1.0/README.md` & `zopyx_fastapi_auth-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.0/fastapi_auth/auth_routes.py` & `zopyx_fastapi_auth-0.1.1/fastapi_auth/auth_routes.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.0/fastapi_auth/demo_app.py` & `zopyx_fastapi_auth-0.1.1/fastapi_auth/demo_app.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.0/fastapi_auth/dependencies.py` & `zopyx_fastapi_auth-0.1.1/fastapi_auth/dependencies.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.0/fastapi_auth/roles.py` & `zopyx_fastapi_auth-0.1.1/fastapi_auth/roles.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.0/fastapi_auth/user_cmd.py` & `zopyx_fastapi_auth-0.1.1/fastapi_auth/user_cmd.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.0/fastapi_auth/user_management.py` & `zopyx_fastapi_auth-0.1.1/fastapi_auth/user_management.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.0/fastapi_auth/users.py` & `zopyx_fastapi_auth-0.1.1/fastapi_auth/users.py`

 * *Files identical despite different names*

### Comparing `zopyx_fastapi_auth-0.1.0/pyproject.toml` & `zopyx_fastapi_auth-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "zopyx-fastapi-auth"
 description = "FastAPI authentication and authorization"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name = "Andreas Jung", email = "info@zopyx.com" }
 ]
 dependencies = [
     "fastapi",
     "pydantic",
     "pydantic-settings",
```

