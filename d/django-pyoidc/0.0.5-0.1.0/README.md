# Comparing `tmp/django_pyoidc-0.0.5.tar.gz` & `tmp/django_pyoidc-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pyoidc-0.0.5.tar", last modified: Tue May 21 12:55:59 2024, max compression
+gzip compressed data, was "django_pyoidc-0.1.0.tar", last modified: Tue May 21 12:33:26 2024, max compression
```

## Comparing `django_pyoidc-0.0.5.tar` & `django_pyoidc-0.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:55:59.163474 django_pyoidc-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-21 12:55:59.163474 django_pyoidc-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:55:59.151474 django_pyoidc-0.0.5/django_pyoidc/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:55:59.155474 django_pyoidc-0.0.5/django_pyoidc/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:55:59.155474 django_pyoidc-0.0.5/django_pyoidc/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/providers/keycloak.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/providers/keycloak_10.py
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/providers/keycloak_17.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/providers/keycloak_18.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/providers/lemonldapng.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/providers/lemonldapng2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21342 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/django_pyoidc/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:55:59.155474 django_pyoidc-0.0.5/django_pyoidc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-21 12:55:59.000000 django_pyoidc-0.0.5/django_pyoidc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-21 12:55:59.000000 django_pyoidc-0.0.5/django_pyoidc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:55:59.000000 django_pyoidc-0.0.5/django_pyoidc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 12:55:59.000000 django_pyoidc-0.0.5/django_pyoidc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 12:55:59.000000 django_pyoidc-0.0.5/django_pyoidc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/requirements.in
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:55:59.163474 django_pyoidc-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:55:59.155474 django_pyoidc-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/tests/tests_pyoidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/tests/tests_session.py
--rw-r--r--   0 runner    (1001) docker     (127)    23027 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/tests/tests_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-21 12:55:54.000000 django_pyoidc-0.0.5/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:33:26.800425 django_pyoidc-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-21 12:33:26.800425 django_pyoidc-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:33:26.788425 django_pyoidc-0.1.0/django_pyoidc/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:33:26.792425 django_pyoidc-0.1.0/django_pyoidc/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:33:26.792425 django_pyoidc-0.1.0/django_pyoidc/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/providers/keycloak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/providers/keycloak_10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/providers/keycloak_17.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/providers/keycloak_18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/providers/lemonldapng.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/providers/lemonldapng2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21342 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/django_pyoidc/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:33:26.792425 django_pyoidc-0.1.0/django_pyoidc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-05-21 12:33:26.000000 django_pyoidc-0.1.0/django_pyoidc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-21 12:33:26.000000 django_pyoidc-0.1.0/django_pyoidc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 12:33:26.000000 django_pyoidc-0.1.0/django_pyoidc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 12:33:26.000000 django_pyoidc-0.1.0/django_pyoidc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 12:33:26.000000 django_pyoidc-0.1.0/django_pyoidc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 12:33:26.800425 django_pyoidc-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 12:33:26.792425 django_pyoidc-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/tests/tests_pyoidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/tests/tests_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23027 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/tests/tests_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-05-21 12:33:22.000000 django_pyoidc-0.1.0/tests/utils.py
```

### Comparing `django_pyoidc-0.0.5/LICENSE` & `django_pyoidc-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/PKG-INFO` & `django_pyoidc-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pyoidc
-Version: 0.0.5
+Version: 0.1.0
 Summary: Authenticate your users using OpenID Connect (OIDC)
 Author-email: "Régis Leroy (Makina Corpus)" <django_pyoidc@makina-corpus.net>, "Paul Florence (Makina Corpus)" <django_pyoidc@makina-corpus.net>
 Project-URL: repository, https://gitlab.makina-corpus.net/pfl/django-pyoidc
 Keywords: openid,oidc,django,sso,single-sign-on,openid-connect
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-pyoidc Version: 0.0.5 Summary: Authenticate
+Metadata-Version: 2.1 Name: django-pyoidc Version: 0.1.0 Summary: Authenticate
 your users using OpenID Connect (OIDC) Author-email: "RÃ©gis Leroy (Makina
 Corpus)"
 makina-corpus.net>, "Paul Florence (Makina Corpus)"
 makina-corpus.net> Project-URL: repository, https://gitlab.makina-corpus.net/
 pfl/django-pyoidc Keywords: openid,oidc,django,sso,single-sign-on,openid-
 connect Classifier: Topic :: Utilities Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
```

### Comparing `django_pyoidc-0.0.5/README.md` & `django_pyoidc-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/django_pyoidc/__init__.py` & `django_pyoidc-0.1.0/django_pyoidc/__init__.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/django_pyoidc/admin.py` & `django_pyoidc-0.1.0/django_pyoidc/admin.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/django_pyoidc/migrations/0001_initial.py` & `django_pyoidc-0.1.0/django_pyoidc/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/django_pyoidc/models.py` & `django_pyoidc-0.1.0/django_pyoidc/models.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/django_pyoidc/providers/base.py` & `django_pyoidc-0.1.0/django_pyoidc/providers/base.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/django_pyoidc/providers/keycloak_10.py` & `django_pyoidc-0.1.0/django_pyoidc/providers/keycloak_10.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/django_pyoidc/providers/keycloak_18.py` & `django_pyoidc-0.1.0/django_pyoidc/providers/keycloak_18.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/django_pyoidc/providers/lemonldapng2.py` & `django_pyoidc-0.1.0/django_pyoidc/providers/lemonldapng2.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/django_pyoidc/session.py` & `django_pyoidc-0.1.0/django_pyoidc/session.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/django_pyoidc/utils.py` & `django_pyoidc-0.1.0/django_pyoidc/utils.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/django_pyoidc/views.py` & `django_pyoidc-0.1.0/django_pyoidc/views.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/django_pyoidc.egg-info/PKG-INFO` & `django_pyoidc-0.1.0/django_pyoidc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pyoidc
-Version: 0.0.5
+Version: 0.1.0
 Summary: Authenticate your users using OpenID Connect (OIDC)
 Author-email: "Régis Leroy (Makina Corpus)" <django_pyoidc@makina-corpus.net>, "Paul Florence (Makina Corpus)" <django_pyoidc@makina-corpus.net>
 Project-URL: repository, https://gitlab.makina-corpus.net/pfl/django-pyoidc
 Keywords: openid,oidc,django,sso,single-sign-on,openid-connect
 Classifier: Topic :: Utilities
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: django-pyoidc Version: 0.0.5 Summary: Authenticate
+Metadata-Version: 2.1 Name: django-pyoidc Version: 0.1.0 Summary: Authenticate
 your users using OpenID Connect (OIDC) Author-email: "RÃ©gis Leroy (Makina
 Corpus)"
 makina-corpus.net>, "Paul Florence (Makina Corpus)"
 makina-corpus.net> Project-URL: repository, https://gitlab.makina-corpus.net/
 pfl/django-pyoidc Keywords: openid,oidc,django,sso,single-sign-on,openid-
 connect Classifier: Topic :: Utilities Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent Classifier: Intended Audience ::
```

### Comparing `django_pyoidc-0.0.5/django_pyoidc.egg-info/SOURCES.txt` & `django_pyoidc-0.1.0/django_pyoidc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/django_pyoidc.egg-info/requires.txt` & `django_pyoidc-0.1.0/django_pyoidc.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/pyproject.toml` & `django_pyoidc-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/requirements-test.txt` & `django_pyoidc-0.1.0/requirements-test.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #
 # This file is autogenerated by pip-compile with Python 3.12
 # by the following command:
 #
-#    pip-compile --output-file=requirements-test.txt requirements-test.in
+#    pip-compile requirements-test.in
 #
 alabaster==0.7.16
     # via sphinx
 anyio==4.3.0
     # via
     #   starlette
     #   watchfiles
```

### Comparing `django_pyoidc-0.0.5/tests/test_settings.py` & `django_pyoidc-0.1.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/tests/tests_pyoidc.py` & `django_pyoidc-0.1.0/tests/tests_pyoidc.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/tests/tests_session.py` & `django_pyoidc-0.1.0/tests/tests_session.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/tests/tests_views.py` & `django_pyoidc-0.1.0/tests/tests_views.py`

 * *Files identical despite different names*

### Comparing `django_pyoidc-0.0.5/tests/utils.py` & `django_pyoidc-0.1.0/tests/utils.py`

 * *Files identical despite different names*

