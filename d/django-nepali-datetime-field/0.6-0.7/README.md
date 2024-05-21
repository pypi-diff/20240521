# Comparing `tmp/django-nepali-datetime-field-0.6.tar.gz` & `tmp/django_nepali_datetime_field-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-nepali-datetime-field-0.6.tar", last modified: Sat May  7 11:38:09 2022, max compression
+gzip compressed data, was "django_nepali_datetime_field-0.7.tar", last modified: Tue May 21 19:15:26 2024, max compression
```

## Comparing `django-nepali-datetime-field-0.6.tar` & `django_nepali_datetime_field-0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxr-x   0 dxillar   (1000) dxillar   (1000)        0 2022-05-07 11:38:09.717525 django-nepali-datetime-field-0.6/
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)     1066 2022-05-07 10:37:21.000000 django-nepali-datetime-field-0.6/LICENSE
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)      136 2022-05-07 10:37:21.000000 django-nepali-datetime-field-0.6/MANIFEST.in
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)     3509 2022-05-07 11:38:09.717525 django-nepali-datetime-field-0.6/PKG-INFO
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)     2262 2022-05-07 11:36:47.000000 django-nepali-datetime-field-0.6/README.rst
-drwxrwxr-x   0 dxillar   (1000) dxillar   (1000)        0 2022-05-07 11:38:09.717525 django-nepali-datetime-field-0.6/django_nepali_datetime_field.egg-info/
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)     3509 2022-05-07 11:38:09.000000 django-nepali-datetime-field-0.6/django_nepali_datetime_field.egg-info/PKG-INFO
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)      824 2022-05-07 11:38:09.000000 django-nepali-datetime-field-0.6/django_nepali_datetime_field.egg-info/SOURCES.txt
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)        1 2022-05-07 11:38:09.000000 django-nepali-datetime-field-0.6/django_nepali_datetime_field.egg-info/dependency_links.txt
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)       28 2022-05-07 11:38:09.000000 django-nepali-datetime-field-0.6/django_nepali_datetime_field.egg-info/requires.txt
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)       22 2022-05-07 11:38:09.000000 django-nepali-datetime-field-0.6/django_nepali_datetime_field.egg-info/top_level.txt
-drwxrwxr-x   0 dxillar   (1000) dxillar   (1000)        0 2022-05-07 11:38:09.717525 django-nepali-datetime-field-0.6/nepali_datetime_field/
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)       67 2022-05-07 11:34:56.000000 django-nepali-datetime-field-0.6/nepali_datetime_field/__init__.py
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)       63 2022-05-07 10:39:06.000000 django-nepali-datetime-field-0.6/nepali_datetime_field/admin.py
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)      172 2022-05-07 10:39:06.000000 django-nepali-datetime-field-0.6/nepali_datetime_field/apps.py
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)     1430 2022-05-07 11:18:29.000000 django-nepali-datetime-field-0.6/nepali_datetime_field/forms.py
-drwxrwxr-x   0 dxillar   (1000) dxillar   (1000)        0 2022-05-07 11:38:09.717525 django-nepali-datetime-field-0.6/nepali_datetime_field/migrations/
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)        0 2022-05-07 10:39:06.000000 django-nepali-datetime-field-0.6/nepali_datetime_field/migrations/__init__.py
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)     1678 2022-05-07 10:39:06.000000 django-nepali-datetime-field-0.6/nepali_datetime_field/models.py
-drwxrwxr-x   0 dxillar   (1000) dxillar   (1000)        0 2022-05-07 11:38:09.717525 django-nepali-datetime-field-0.6/nepali_datetime_field/static/
-drwxrwxr-x   0 dxillar   (1000) dxillar   (1000)        0 2022-05-07 11:38:09.717525 django-nepali-datetime-field-0.6/nepali_datetime_field/static/nepali_datetime_field/
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)      246 2022-05-07 11:18:18.000000 django-nepali-datetime-field-0.6/nepali_datetime_field/static/nepali_datetime_field/init.js
-drwxrwxr-x   0 dxillar   (1000) dxillar   (1000)        0 2022-05-07 11:38:09.717525 django-nepali-datetime-field-0.6/nepali_datetime_field/templates/
-drwxrwxr-x   0 dxillar   (1000) dxillar   (1000)        0 2022-05-07 11:38:09.717525 django-nepali-datetime-field-0.6/nepali_datetime_field/templates/nepali_datetime_field/
-drwxrwxr-x   0 dxillar   (1000) dxillar   (1000)        0 2022-05-07 11:38:09.717525 django-nepali-datetime-field-0.6/nepali_datetime_field/templates/nepali_datetime_field/forms/
-drwxrwxr-x   0 dxillar   (1000) dxillar   (1000)        0 2022-05-07 11:38:09.717525 django-nepali-datetime-field-0.6/nepali_datetime_field/templates/nepali_datetime_field/forms/widgets/
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)      254 2022-05-07 10:39:06.000000 django-nepali-datetime-field-0.6/nepali_datetime_field/templates/nepali_datetime_field/forms/widgets/nepali_date.html
-drwxrwxr-x   0 dxillar   (1000) dxillar   (1000)        0 2022-05-07 11:38:09.717525 django-nepali-datetime-field-0.6/nepali_datetime_field/templatetags/
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)        0 2022-05-07 10:39:06.000000 django-nepali-datetime-field-0.6/nepali_datetime_field/templatetags/__init__.py
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)      192 2022-05-07 10:39:06.000000 django-nepali-datetime-field-0.6/nepali_datetime_field/templatetags/nepali_datetime_field.py
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)       60 2022-05-07 10:39:06.000000 django-nepali-datetime-field-0.6/nepali_datetime_field/tests.py
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)       63 2022-05-07 10:39:06.000000 django-nepali-datetime-field-0.6/nepali_datetime_field/views.py
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)     1283 2022-05-07 11:38:09.721525 django-nepali-datetime-field-0.6/setup.cfg
--rw-rw-r--   0 dxillar   (1000) dxillar   (1000)       38 2022-05-07 10:37:21.000000 django-nepali-datetime-field-0.6/setup.py
+drwxr-xr-x   0 agaru     (1000) agaru     (1000)        0 2024-05-21 19:15:26.153109 django_nepali_datetime_field-0.7/
+-rw-r--r--   0 agaru     (1000) agaru     (1000)     1066 2024-05-21 18:38:33.000000 django_nepali_datetime_field-0.7/LICENSE
+-rw-r--r--   0 agaru     (1000) agaru     (1000)      136 2024-05-21 18:38:33.000000 django_nepali_datetime_field-0.7/MANIFEST.in
+-rw-r--r--   0 agaru     (1000) agaru     (1000)     3580 2024-05-21 19:15:26.153109 django_nepali_datetime_field-0.7/PKG-INFO
+-rw-r--r--   0 agaru     (1000) agaru     (1000)     2262 2024-05-21 19:12:22.000000 django_nepali_datetime_field-0.7/README.rst
+drwxr-xr-x   0 agaru     (1000) agaru     (1000)        0 2024-05-21 19:15:26.153109 django_nepali_datetime_field-0.7/django_nepali_datetime_field.egg-info/
+-rw-r--r--   0 agaru     (1000) agaru     (1000)     3580 2024-05-21 19:15:26.000000 django_nepali_datetime_field-0.7/django_nepali_datetime_field.egg-info/PKG-INFO
+-rw-r--r--   0 agaru     (1000) agaru     (1000)      814 2024-05-21 19:15:26.000000 django_nepali_datetime_field-0.7/django_nepali_datetime_field.egg-info/SOURCES.txt
+-rw-r--r--   0 agaru     (1000) agaru     (1000)        1 2024-05-21 19:15:26.000000 django_nepali_datetime_field-0.7/django_nepali_datetime_field.egg-info/dependency_links.txt
+-rw-r--r--   0 agaru     (1000) agaru     (1000)       28 2024-05-21 19:15:26.000000 django_nepali_datetime_field-0.7/django_nepali_datetime_field.egg-info/requires.txt
+-rw-r--r--   0 agaru     (1000) agaru     (1000)       22 2024-05-21 19:15:26.000000 django_nepali_datetime_field-0.7/django_nepali_datetime_field.egg-info/top_level.txt
+drwxr-xr-x   0 agaru     (1000) agaru     (1000)        0 2024-05-21 19:15:26.153109 django_nepali_datetime_field-0.7/nepali_datetime_field/
+-rw-r--r--   0 agaru     (1000) agaru     (1000)       67 2024-05-21 18:53:55.000000 django_nepali_datetime_field-0.7/nepali_datetime_field/__init__.py
+-rw-r--r--   0 agaru     (1000) agaru     (1000)       63 2024-05-21 18:38:33.000000 django_nepali_datetime_field-0.7/nepali_datetime_field/admin.py
+-rw-r--r--   0 agaru     (1000) agaru     (1000)      172 2024-05-21 18:38:33.000000 django_nepali_datetime_field-0.7/nepali_datetime_field/apps.py
+-rw-r--r--   0 agaru     (1000) agaru     (1000)     1430 2024-05-21 18:38:33.000000 django_nepali_datetime_field-0.7/nepali_datetime_field/forms.py
+drwxr-xr-x   0 agaru     (1000) agaru     (1000)        0 2024-05-21 19:15:26.153109 django_nepali_datetime_field-0.7/nepali_datetime_field/migrations/
+-rw-r--r--   0 agaru     (1000) agaru     (1000)        0 2024-05-21 18:38:33.000000 django_nepali_datetime_field-0.7/nepali_datetime_field/migrations/__init__.py
+-rw-r--r--   0 agaru     (1000) agaru     (1000)     1823 2024-05-21 18:52:04.000000 django_nepali_datetime_field-0.7/nepali_datetime_field/models.py
+drwxr-xr-x   0 agaru     (1000) agaru     (1000)        0 2024-05-21 19:15:26.143109 django_nepali_datetime_field-0.7/nepali_datetime_field/static/
+drwxr-xr-x   0 agaru     (1000) agaru     (1000)        0 2024-05-21 19:15:26.153109 django_nepali_datetime_field-0.7/nepali_datetime_field/static/nepali_datetime_field/
+-rw-r--r--   0 agaru     (1000) agaru     (1000)      246 2024-05-21 18:38:33.000000 django_nepali_datetime_field-0.7/nepali_datetime_field/static/nepali_datetime_field/init.js
+drwxr-xr-x   0 agaru     (1000) agaru     (1000)        0 2024-05-21 19:15:26.143109 django_nepali_datetime_field-0.7/nepali_datetime_field/templates/
+drwxr-xr-x   0 agaru     (1000) agaru     (1000)        0 2024-05-21 19:15:26.143109 django_nepali_datetime_field-0.7/nepali_datetime_field/templates/nepali_datetime_field/
+drwxr-xr-x   0 agaru     (1000) agaru     (1000)        0 2024-05-21 19:15:26.143109 django_nepali_datetime_field-0.7/nepali_datetime_field/templates/nepali_datetime_field/forms/
+drwxr-xr-x   0 agaru     (1000) agaru     (1000)        0 2024-05-21 19:15:26.153109 django_nepali_datetime_field-0.7/nepali_datetime_field/templates/nepali_datetime_field/forms/widgets/
+-rw-r--r--   0 agaru     (1000) agaru     (1000)      254 2024-05-21 18:38:33.000000 django_nepali_datetime_field-0.7/nepali_datetime_field/templates/nepali_datetime_field/forms/widgets/nepali_date.html
+drwxr-xr-x   0 agaru     (1000) agaru     (1000)        0 2024-05-21 19:15:26.153109 django_nepali_datetime_field-0.7/nepali_datetime_field/templatetags/
+-rw-r--r--   0 agaru     (1000) agaru     (1000)        0 2024-05-21 18:38:33.000000 django_nepali_datetime_field-0.7/nepali_datetime_field/templatetags/__init__.py
+-rw-r--r--   0 agaru     (1000) agaru     (1000)      192 2024-05-21 18:38:33.000000 django_nepali_datetime_field-0.7/nepali_datetime_field/templatetags/nepali_datetime_field.py
+-rw-r--r--   0 agaru     (1000) agaru     (1000)       60 2024-05-21 18:38:33.000000 django_nepali_datetime_field-0.7/nepali_datetime_field/tests.py
+-rw-r--r--   0 agaru     (1000) agaru     (1000)       63 2024-05-21 18:38:33.000000 django_nepali_datetime_field-0.7/nepali_datetime_field/views.py
+-rw-r--r--   0 agaru     (1000) agaru     (1000)       38 2024-05-21 19:15:26.153109 django_nepali_datetime_field-0.7/setup.cfg
+-rw-r--r--   0 agaru     (1000) agaru     (1000)     1653 2024-05-21 19:15:14.000000 django_nepali_datetime_field-0.7/setup.py
```

### Comparing `django-nepali-datetime-field-0.6/LICENSE` & `django_nepali_datetime_field-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-nepali-datetime-field-0.6/PKG-INFO` & `django_nepali_datetime_field-0.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-nepali-datetime-field
-Version: 0.6
-Summary: Django nepali datetime helpers.
+Version: 0.7
+Summary: Django nepali datetime fields and helpers.
 Home-page: https://github.com/dxillar/django-nepali-datetime-field
-Author: Amit Garu
+Author: Amit Garu <amitgaru2@gmail.com>
 Author-email: amitgaru2@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
@@ -26,14 +25,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: Django>=2.0
+Requires-Dist: nepali_datetime
 
 =====================
 Nepali DateTime Field
 =====================
 
 Highly motivated package from Django's DateField & DateTimeField. The library is intended to provide
 Bikram Sambat Date Time fields for Django's Model and Form.
@@ -114,9 +115,7 @@
 ----------
 Check some of the usage details in `example_app/tests.py <https://github.com/dxillar/django-nepali-datetime-field/blob/main/example_app/tests.py>`__.
 
 
 Demo
 ----
 Play around with the live demo `here <https://nepali-datetime-field.herokuapp.com/example/create>`__.
-
-
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: django-nepali-datetime-field Version: 0.6 Summary:
-Django nepali datetime helpers. Home-page: https://github.com/dxillar/django-
-nepali-datetime-field Author: Amit Garu Author-email: amitgaru2@gmail.com
-License: MIT Platform: UNKNOWN Classifier: Environment :: Web Environment
-Classifier: Framework :: Django Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1 Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2 Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: BSD License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/
-HTTP :: Dynamic Content Requires-Python: >=3.6 Description-Content-Type: text/
-x-rst License-File: LICENSE ===================== Nepali DateTime Field
+Metadata-Version: 2.1 Name: django-nepali-datetime-field Version: 0.7 Summary:
+Django nepali datetime fields and helpers. Home-page: https://github.com/
+dxillar/django-nepali-datetime-field Author: Amit Garu
+gmail.com> Author-email: amitgaru2@gmail.com License: MIT Classifier:
+Environment :: Web Environment Classifier: Framework :: Django Classifier:
+Framework :: Django :: 2.0 Classifier: Framework :: Django :: 2.1 Classifier:
+Framework :: Django :: 2.2 Classifier: Framework :: Django :: 3.0 Classifier:
+Framework :: Django :: 3.1 Classifier: Framework :: Django :: 3.2 Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
+License Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
+Internet :: WWW/HTTP :: Dynamic Content Requires-Python: >=3.6 Description-
+Content-Type: text/x-rst License-File: LICENSE Requires-Dist: Django>=2.0
+Requires-Dist: nepali_datetime ===================== Nepali DateTime Field
 ===================== Highly motivated package from Django's DateField &
 DateTimeField. The library is intended to provide Bikram Sambat Date Time
 fields for Django's Model and Form. :code:`Note: Currently only supports
 DateField. DateTimeField will be supported soon in future releases.` The
 package is dependent on `nepali-datetime
 github.com/dxillar/nepali-datetime>`_ package and the UI for the date picker is
 implemented from https://github.com/leapfrogtechnology/nepali-date-picker.
```

### Comparing `django-nepali-datetime-field-0.6/README.rst` & `django_nepali_datetime_field-0.7/README.rst`

 * *Files identical despite different names*

### Comparing `django-nepali-datetime-field-0.6/django_nepali_datetime_field.egg-info/PKG-INFO` & `django_nepali_datetime_field-0.7/django_nepali_datetime_field.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-nepali-datetime-field
-Version: 0.6
-Summary: Django nepali datetime helpers.
+Version: 0.7
+Summary: Django nepali datetime fields and helpers.
 Home-page: https://github.com/dxillar/django-nepali-datetime-field
-Author: Amit Garu
+Author: Amit Garu <amitgaru2@gmail.com>
 Author-email: amitgaru2@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 2.0
 Classifier: Framework :: Django :: 2.1
 Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
@@ -26,14 +25,16 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE
+Requires-Dist: Django>=2.0
+Requires-Dist: nepali_datetime
 
 =====================
 Nepali DateTime Field
 =====================
 
 Highly motivated package from Django's DateField & DateTimeField. The library is intended to provide
 Bikram Sambat Date Time fields for Django's Model and Form.
@@ -114,9 +115,7 @@
 ----------
 Check some of the usage details in `example_app/tests.py <https://github.com/dxillar/django-nepali-datetime-field/blob/main/example_app/tests.py>`__.
 
 
 Demo
 ----
 Play around with the live demo `here <https://nepali-datetime-field.herokuapp.com/example/create>`__.
-
-
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: django-nepali-datetime-field Version: 0.6 Summary:
-Django nepali datetime helpers. Home-page: https://github.com/dxillar/django-
-nepali-datetime-field Author: Amit Garu Author-email: amitgaru2@gmail.com
-License: MIT Platform: UNKNOWN Classifier: Environment :: Web Environment
-Classifier: Framework :: Django Classifier: Framework :: Django :: 2.0
-Classifier: Framework :: Django :: 2.1 Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.0 Classifier: Framework :: Django :: 3.1
-Classifier: Framework :: Django :: 3.2 Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: BSD License Classifier:
-Operating System :: OS Independent Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3 :: Only Classifier: Programming Language :: Python ::
-3.6 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic :: Internet :: WWW/
-HTTP :: Dynamic Content Requires-Python: >=3.6 Description-Content-Type: text/
-x-rst License-File: LICENSE ===================== Nepali DateTime Field
+Metadata-Version: 2.1 Name: django-nepali-datetime-field Version: 0.7 Summary:
+Django nepali datetime fields and helpers. Home-page: https://github.com/
+dxillar/django-nepali-datetime-field Author: Amit Garu
+gmail.com> Author-email: amitgaru2@gmail.com License: MIT Classifier:
+Environment :: Web Environment Classifier: Framework :: Django Classifier:
+Framework :: Django :: 2.0 Classifier: Framework :: Django :: 2.1 Classifier:
+Framework :: Django :: 2.2 Classifier: Framework :: Django :: 3.0 Classifier:
+Framework :: Django :: 3.1 Classifier: Framework :: Django :: 3.2 Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
+License Classifier: Operating System :: OS Independent Classifier: Programming
+Language :: Python Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3 :: Only Classifier: Programming Language ::
+Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Topic :: Internet :: WWW/HTTP Classifier: Topic ::
+Internet :: WWW/HTTP :: Dynamic Content Requires-Python: >=3.6 Description-
+Content-Type: text/x-rst License-File: LICENSE Requires-Dist: Django>=2.0
+Requires-Dist: nepali_datetime ===================== Nepali DateTime Field
 ===================== Highly motivated package from Django's DateField &
 DateTimeField. The library is intended to provide Bikram Sambat Date Time
 fields for Django's Model and Form. :code:`Note: Currently only supports
 DateField. DateTimeField will be supported soon in future releases.` The
 package is dependent on `nepali-datetime
 github.com/dxillar/nepali-datetime>`_ package and the UI for the date picker is
 implemented from https://github.com/leapfrogtechnology/nepali-date-picker.
```

### Comparing `django-nepali-datetime-field-0.6/django_nepali_datetime_field.egg-info/SOURCES.txt` & `django_nepali_datetime_field-0.7/django_nepali_datetime_field.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 LICENSE
 MANIFEST.in
 README.rst
-setup.cfg
 setup.py
 django_nepali_datetime_field.egg-info/PKG-INFO
 django_nepali_datetime_field.egg-info/SOURCES.txt
 django_nepali_datetime_field.egg-info/dependency_links.txt
 django_nepali_datetime_field.egg-info/requires.txt
 django_nepali_datetime_field.egg-info/top_level.txt
 nepali_datetime_field/__init__.py
```

### Comparing `django-nepali-datetime-field-0.6/nepali_datetime_field/forms.py` & `django_nepali_datetime_field-0.7/nepali_datetime_field/forms.py`

 * *Files identical despite different names*

### Comparing `django-nepali-datetime-field-0.6/nepali_datetime_field/models.py` & `django_nepali_datetime_field-0.7/nepali_datetime_field/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,38 +22,41 @@
 class NepaliDateField(models.DateField):
     description = "Nepali Date Field"
 
     def formfield(self, **kwargs):
         return super().formfield(**{
             'form_class': forms.NepaliDateField,
             **kwargs,
+
         })
 
     def from_db_value(self, value, expression, connection):
+        if value is None or value == '':
+            return value
         return nepali_datetime.date.from_datetime_date(value)
 
     def get_prep_value(self, value):
+        if value is None or value == '':
+            return value
         value = super().get_prep_value(value)
         return self.to_python(value).to_datetime_date()
 
     def to_python(self, value):
-        if value is None:
-            return value
+        if value is None or value == '':
+            return None
         if isinstance(value, nepali_datetime.date):
             return value
         try:
             parsed = parse_date(value)
             if parsed is not None:
                 return parsed
-
         except ValueError:
             raise ValidationError(
                 self.error_messages['invalid_date'],
                 code='invalid_date',
                 params={'value': value},
             )
-
         raise ValidationError(
             self.error_messages['invalid'],
             code='invalid',
             params={'value': value},
         )
```

