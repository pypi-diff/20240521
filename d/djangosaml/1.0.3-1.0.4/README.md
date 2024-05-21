# Comparing `tmp/djangosaml-1.0.3.tar.gz` & `tmp/djangosaml-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangosaml-1.0.3.tar", last modified: Wed Apr  3 09:10:22 2024, max compression
+gzip compressed data, was "djangosaml-1.0.4.tar", last modified: Tue May 21 09:38:09 2024, max compression
```

## Comparing `djangosaml-1.0.3.tar` & `djangosaml-1.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-04-03 09:10:22.105614 djangosaml-1.0.3/
--rw-rw-r--   0 suhail    (1001) suhail    (1001)      745 2024-04-02 09:26:36.000000 djangosaml-1.0.3/AUTHORS.rst
--rw-rw-r--   0 suhail    (1001) suhail    (1001)      552 2024-04-01 03:53:09.000000 djangosaml-1.0.3/LICENSE
--rw-rw-r--   0 suhail    (1001) suhail    (1001)      120 2024-04-01 03:53:09.000000 djangosaml-1.0.3/MANIFEST.in
--rw-r--r--   0 suhail    (1001) suhail    (1001)     2711 2024-04-03 09:10:22.105614 djangosaml-1.0.3/PKG-INFO
--rw-rw-r--   0 suhail    (1001) suhail    (1001)     1783 2024-04-02 09:26:36.000000 djangosaml-1.0.3/README.md
-drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-04-03 09:10:22.101611 djangosaml-1.0.3/djangosaml/
--rw-rw-r--   0 suhail    (1001) suhail    (1001)       24 2024-04-01 03:53:09.000000 djangosaml-1.0.3/djangosaml/__init__.py
-drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-04-03 09:10:22.101611 djangosaml-1.0.3/djangosaml/templates/
-drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-04-03 09:10:22.105614 djangosaml-1.0.3/djangosaml/templates/djangosaml/
--rw-rw-r--   0 suhail    (1001) suhail    (1001)      327 2024-04-01 03:53:09.000000 djangosaml-1.0.3/djangosaml/templates/djangosaml/denied.html
--rw-rw-r--   0 suhail    (1001) suhail    (1001)      308 2024-04-01 03:53:09.000000 djangosaml-1.0.3/djangosaml/templates/djangosaml/signout.html
--rw-rw-r--   0 suhail    (1001) suhail    (1001)      295 2024-04-02 09:26:32.000000 djangosaml-1.0.3/djangosaml/urls.py
--rw-rw-r--   0 suhail    (1001) suhail    (1001)     9148 2024-04-03 09:08:30.000000 djangosaml-1.0.3/djangosaml/views.py
-drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-04-03 09:10:22.105614 djangosaml-1.0.3/djangosaml.egg-info/
--rw-r--r--   0 suhail    (1001) suhail    (1001)     2711 2024-04-03 09:10:22.000000 djangosaml-1.0.3/djangosaml.egg-info/PKG-INFO
--rw-rw-r--   0 suhail    (1001) suhail    (1001)      380 2024-04-03 09:10:22.000000 djangosaml-1.0.3/djangosaml.egg-info/SOURCES.txt
--rw-rw-r--   0 suhail    (1001) suhail    (1001)        1 2024-04-03 09:10:22.000000 djangosaml-1.0.3/djangosaml.egg-info/dependency_links.txt
--rw-rw-r--   0 suhail    (1001) suhail    (1001)       15 2024-04-03 09:10:22.000000 djangosaml-1.0.3/djangosaml.egg-info/requires.txt
--rw-rw-r--   0 suhail    (1001) suhail    (1001)       11 2024-04-03 09:10:22.000000 djangosaml-1.0.3/djangosaml.egg-info/top_level.txt
--rw-rw-r--   0 suhail    (1001) suhail    (1001)       67 2024-04-03 09:10:22.105614 djangosaml-1.0.3/setup.cfg
--rw-rw-r--   0 suhail    (1001) suhail    (1001)     1342 2024-04-03 09:08:26.000000 djangosaml-1.0.3/setup.py
+drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-05-21 09:38:09.555616 djangosaml-1.0.4/
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      745 2024-04-02 09:26:36.000000 djangosaml-1.0.4/AUTHORS.rst
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      552 2024-04-01 03:53:09.000000 djangosaml-1.0.4/LICENSE
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      120 2024-04-01 03:53:09.000000 djangosaml-1.0.4/MANIFEST.in
+-rw-r--r--   0 suhail    (1001) suhail    (1001)     2711 2024-05-21 09:38:09.555616 djangosaml-1.0.4/PKG-INFO
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)     1783 2024-04-02 09:26:36.000000 djangosaml-1.0.4/README.md
+drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-05-21 09:38:09.551616 djangosaml-1.0.4/djangosaml/
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)       24 2024-04-01 03:53:09.000000 djangosaml-1.0.4/djangosaml/__init__.py
+drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-05-21 09:38:09.547616 djangosaml-1.0.4/djangosaml/templates/
+drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-05-21 09:38:09.551616 djangosaml-1.0.4/djangosaml/templates/djangosaml/
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      327 2024-04-01 03:53:09.000000 djangosaml-1.0.4/djangosaml/templates/djangosaml/denied.html
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      308 2024-04-01 03:53:09.000000 djangosaml-1.0.4/djangosaml/templates/djangosaml/signout.html
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      365 2024-05-10 12:22:14.000000 djangosaml-1.0.4/djangosaml/urls.py
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)     9262 2024-05-21 09:33:09.000000 djangosaml-1.0.4/djangosaml/views.py
+drwxrwxr-x   0 suhail    (1001) suhail    (1001)        0 2024-05-21 09:38:09.551616 djangosaml-1.0.4/djangosaml.egg-info/
+-rw-r--r--   0 suhail    (1001) suhail    (1001)     2711 2024-05-21 09:38:09.000000 djangosaml-1.0.4/djangosaml.egg-info/PKG-INFO
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)      380 2024-05-21 09:38:09.000000 djangosaml-1.0.4/djangosaml.egg-info/SOURCES.txt
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)        1 2024-05-21 09:38:09.000000 djangosaml-1.0.4/djangosaml.egg-info/dependency_links.txt
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)       15 2024-05-21 09:38:09.000000 djangosaml-1.0.4/djangosaml.egg-info/requires.txt
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)       11 2024-05-21 09:38:09.000000 djangosaml-1.0.4/djangosaml.egg-info/top_level.txt
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)       67 2024-05-21 09:38:09.555616 djangosaml-1.0.4/setup.cfg
+-rw-rw-r--   0 suhail    (1001) suhail    (1001)     1342 2024-05-21 09:36:54.000000 djangosaml-1.0.4/setup.py
```

### Comparing `djangosaml-1.0.3/AUTHORS.rst` & `djangosaml-1.0.4/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `djangosaml-1.0.3/LICENSE` & `djangosaml-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `djangosaml-1.0.3/PKG-INFO` & `djangosaml-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml
-Version: 1.0.3
+Version: 1.0.4
 Summary: Django SAML2 Authentication Made Easy. Easily integrate with SAML2 SSO identity providers like Okta
 Home-page: https://djangosaml.readthedocs.io/en/latest/
 Author: Fang Li
 Author-email: lorenzo.gil.sanchez@gmail.com
 License: Apache 2.0
 Keywords: Django SAML2 Authentication Made Easy,integrate with SAML2 SSO such as Okta easily
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `djangosaml-1.0.3/README.md` & `djangosaml-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `djangosaml-1.0.3/djangosaml/views.py` & `djangosaml-1.0.4/djangosaml/views.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                         (acs_url, BINDING_HTTP_REDIRECT),
                         (acs_url, BINDING_HTTP_POST)
                     ],
                 },
                 'allow_unsolicited': True,
                 'authn_requests_signed': False,
                 'logout_requests_signed': True,
-                'want_assertions_signed': True,
+                'want_assertions_signed': False,
                 'want_response_signed': False,
             },
         },
     }
 
     if 'ENTITY_ID' in settings.SAML2_AUTH:
         saml_settings['entityid'] = settings.SAML2_AUTH['ENTITY_ID']
@@ -164,30 +164,32 @@
         resp, entity.BINDING_HTTP_POST)
     if authn_response is None:
         return HttpResponseRedirect(get_reverse([denied, 'denied', 'djangosaml:denied']))
 
     user_identity = authn_response.get_identity()
     if user_identity is None:
         return HttpResponseRedirect(get_reverse([denied, 'denied', 'djangosaml:denied']))
-
-    user_email = user_identity[settings.SAML2_AUTH.get('ATTRIBUTES_MAP', {}).get('email', 'Email')][0]
+    print('Django SAML User details')
+    print('='*100)    
+    print(user_identity)
+    
     user_name = user_identity[settings.SAML2_AUTH.get('ATTRIBUTES_MAP', {}).get('username', 'UserName')][0]
-    user_first_name = user_identity[settings.SAML2_AUTH.get('ATTRIBUTES_MAP', {}).get('first_name', 'FirstName')][0]
-    user_last_name = user_identity[settings.SAML2_AUTH.get('ATTRIBUTES_MAP', {}).get('last_name', 'LastName')][0]
-
     target_user = None
     is_new_user = False
 
     try:
         target_user = User.objects.get(username=user_name)
         if settings.SAML2_AUTH.get('TRIGGER', {}).get('BEFORE_LOGIN', None):
             import_string(settings.SAML2_AUTH['TRIGGER']['BEFORE_LOGIN'])(user_identity)
     except User.DoesNotExist:
         new_user_should_be_created = settings.SAML2_AUTH.get('CREATE_USER', True)
         if new_user_should_be_created: 
+            user_email = user_identity[settings.SAML2_AUTH.get('ATTRIBUTES_MAP', {}).get('email', 'Email')][0]
+            user_first_name = user_identity[settings.SAML2_AUTH.get('ATTRIBUTES_MAP', {}).get('first_name', 'FirstName')][0]
+            user_last_name = user_identity[settings.SAML2_AUTH.get('ATTRIBUTES_MAP', {}).get('last_name', 'LastName')][0]
             target_user = _create_new_user(user_name, user_email, user_first_name, user_last_name)
             if settings.SAML2_AUTH.get('TRIGGER', {}).get('CREATE_USER', None):
                 import_string(settings.SAML2_AUTH['TRIGGER']['CREATE_USER'])(user_identity)
             is_new_user = True
         else:
             return HttpResponseRedirect(get_reverse([denied, 'denied', 'djangosaml:denied']))
```

### Comparing `djangosaml-1.0.3/djangosaml.egg-info/PKG-INFO` & `djangosaml-1.0.4/djangosaml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangosaml
-Version: 1.0.3
+Version: 1.0.4
 Summary: Django SAML2 Authentication Made Easy. Easily integrate with SAML2 SSO identity providers like Okta
 Home-page: https://djangosaml.readthedocs.io/en/latest/
 Author: Fang Li
 Author-email: lorenzo.gil.sanchez@gmail.com
 License: Apache 2.0
 Keywords: Django SAML2 Authentication Made Easy,integrate with SAML2 SSO such as Okta easily
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `djangosaml-1.0.3/setup.py` & `djangosaml-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Get the long description from the README file
 def read(f):
     with open(f, 'r', encoding='utf-8') as file:
         return file.read()
     
 setup(
     name='djangosaml',
-    version='1.0.3',
+    version='1.0.4',
     description='Django SAML2 Authentication Made Easy. Easily integrate with SAML2 SSO identity providers like Okta',
     long_description=read('README.md'),
     long_description_content_type='text/markdown',
 
     url='https://djangosaml.readthedocs.io/en/latest/',
 
     author='Fang Li',
```

