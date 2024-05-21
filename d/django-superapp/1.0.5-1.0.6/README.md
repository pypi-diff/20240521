# Comparing `tmp/django_superapp-1.0.5.tar.gz` & `tmp/django_superapp-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_superapp-1.0.5.tar", last modified: Mon May 20 09:12:30 2024, max compression
+gzip compressed data, was "django_superapp-1.0.6.tar", last modified: Tue May 21 08:51:20 2024, max compression
```

## Comparing `django_superapp-1.0.5.tar` & `django_superapp-1.0.6.tar`

### file list

```diff
@@ -1,35 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:12:30.156592 django_superapp-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-20 09:12:15.000000 django_superapp-1.0.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-20 09:12:30.156592 django_superapp-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-20 09:12:15.000000 django_superapp-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-20 09:12:15.000000 django_superapp-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      279 2024-05-20 09:12:30.156592 django_superapp-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-20 09:12:15.000000 django_superapp-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:12:30.148591 django_superapp-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:12:30.152592 django_superapp-1.0.5/src/django_superapp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      118 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/db_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/decorators.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      826 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/forms.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:12:30.156592 django_superapp-1.0.5/src/django_superapp/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:12:30.156592 django_superapp-1.0.5/src/django_superapp/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/management/commands/list_all_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/management/commands/list_all_urls_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/management/commands/truncate_all_models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:12:30.156592 django_superapp-1.0.5/src/django_superapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1267 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/sites.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1443 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-20 09:12:15.000000 django_superapp-1.0.5/src/django_superapp/widgets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:12:30.156592 django_superapp-1.0.5/src/django_superapp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-20 09:12:30.000000 django_superapp-1.0.5/src/django_superapp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-20 09:12:30.000000 django_superapp-1.0.5/src/django_superapp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:12:30.000000 django_superapp-1.0.5/src/django_superapp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-20 09:12:30.000000 django_superapp-1.0.5/src/django_superapp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-20 09:12:30.000000 django_superapp-1.0.5/src/django_superapp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:51:20.843950 django_superapp-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-21 08:51:10.000000 django_superapp-1.0.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-21 08:51:20.843950 django_superapp-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-21 08:51:10.000000 django_superapp-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 08:51:10.000000 django_superapp-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-21 08:51:20.843950 django_superapp-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-21 08:51:10.000000 django_superapp-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:51:20.839950 django_superapp-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:51:20.839950 django_superapp-1.0.6/src/django_superapp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      118 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/autocomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:51:20.843950 django_superapp-1.0.6/src/django_superapp/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/db_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/decorators.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      826 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/forms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6321 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:51:20.843950 django_superapp-1.0.6/src/django_superapp/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:51:20.843950 django_superapp-1.0.6/src/django_superapp/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/management/commands/list_all_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/management/commands/list_all_urls_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/management/commands/truncate_all_models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:51:20.843950 django_superapp-1.0.6/src/django_superapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1267 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/sites.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/types.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1438 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-21 08:51:10.000000 django_superapp-1.0.6/src/django_superapp/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:51:20.843950 django_superapp-1.0.6/src/django_superapp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2018 2024-05-21 08:51:20.000000 django_superapp-1.0.6/src/django_superapp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-21 08:51:20.000000 django_superapp-1.0.6/src/django_superapp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:51:20.000000 django_superapp-1.0.6/src/django_superapp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 08:51:20.000000 django_superapp-1.0.6/src/django_superapp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-21 08:51:20.000000 django_superapp-1.0.6/src/django_superapp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-21 08:51:20.000000 django_superapp-1.0.6/src/django_superapp.egg-info/top_level.txt
```

### Comparing `django_superapp-1.0.5/LICENSE.md` & `django_superapp-1.0.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.5/PKG-INFO` & `django_superapp-1.0.6/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django_superapp
-Version: 1.0.5
-Summary: Build your startup application faster with django-superapp
+Version: 1.0.6
+Summary: Build your startup's product faster.
 Home-page: https://github.com/django-superapp/django-superapp
 Author: Django SuperApp
 Author-email: django-superapp@bringes.io
 License: MIT
 Project-URL: Bug Reports, https://github.com/django-superapp/django-superapp/issues
 Project-URL: Source, https://github.com/django-superapp/django-superapp
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,16 +30,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: Django>=5.0.0
 Requires-Dist: django-unfold>=0.22.0
 Requires-Dist: django-svelte-jsoneditor>=0.4.2
 Requires-Dist: django-import-export>=4.0.3
 Requires-Dist: django-admin-confirm>=1.0.0
+Requires-Dist: click>=8.1.7
+Requires-Dist: copier>=9.2.0
+Requires-Dist: requests>=2.31.0
+Requires-Dist: pydantic>=2.7.1
 
-# django-superapp-core
+# Django SuperApp
+
+### Getting Started
+```bash
+pipx install django_superapp
+django_superapp create-project test_project
+cd test_project
+django_superapp add-app --app-name sample_app
+```
 
 ### Development
 ```bash
 make install-requirements
 make install
 make release
 ```
```

### Comparing `django_superapp-1.0.5/setup.py` & `django_superapp-1.0.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,27 +3,37 @@
 this_directory = Path(__file__).parent
 
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="django_superapp",
     packages=find_packages(where="src"),
+    description="Build your startup's product faster.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     url="https://github.com/django-superapp/django-superapp",
     author="Django SuperApp",
     author_email="django-superapp@bringes.io",
     license="MIT",
     package_dir={"": "src"},
+    entry_points={
+        'console_scripts': [
+            'django_superapp=django_superapp.cli.main:cli',
+        ],
+    },
     install_requires=[
         "Django >= 5.0.0",
         "django-unfold >= 0.22.0",
         "django-svelte-jsoneditor >= 0.4.2",
         "django-import-export >= 4.0.3",
         "django-admin-confirm >= 1.0.0",
+        "click >= 8.1.7",
+        "copier >= 9.2.0",
+        "requests >= 2.31.0",
+        "pydantic >= 2.7.1",
     ],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "Intended Audience :: System Administrators",
         "License :: OSI Approved :: MIT License",
```

### Comparing `django_superapp-1.0.5/src/django_superapp/autocomplete.py` & `django_superapp-1.0.6/src/django_superapp/autocomplete.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.5/src/django_superapp/decorators.py` & `django_superapp-1.0.6/src/django_superapp/decorators.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.5/src/django_superapp/forms.py` & `django_superapp-1.0.6/src/django_superapp/forms.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.5/src/django_superapp/helpers.py` & `django_superapp-1.0.6/src/django_superapp/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import copy
 from typing import List, Optional, Dict, Any
 
 from django.contrib.admin import helpers
 from django.contrib.admin.utils import lookup_field
-from django.core.exceptions import ObjectDoesNotExist
+from django.core.exceptions import ObjectDoesNotExist, ValidationError
 from django.db.models import ForeignKey
 from django.forms import ModelChoiceField
 from django.http import HttpRequest
 from django.urls import reverse, URLPattern, path
 from django.utils.text import wrap
 from django_svelte_jsoneditor.widgets import SvelteJSONEditorWidget
 from import_export.admin import ImportExportModelAdmin
@@ -15,15 +15,16 @@
 from unfold.contrib.forms.widgets import WysiwygWidget
 from unfold.dataclasses import UnfoldAction
 from unfold.widgets import UnfoldBooleanSwitchWidget, UnfoldAdminFileFieldWidget
 from django.db import models
 
 from admin_confirm import AdminConfirmMixin
 
-from django_superapp_core.db_fields import ChainedForeignKey
+from django_superapp.db_fields import ChainedForeignKey
+from django_superapp.widgets import ChainedAdminSelect
 
 
 class SuperAppAdminReadonlyField(UnfoldAdminReadonlyField):
 
     def is_custom_html_field(self) -> bool:
         field, obj, model_admin = (
             self.field["field"],
```

### Comparing `django_superapp-1.0.5/src/django_superapp/management/commands/list_all_urls_patterns.py` & `django_superapp-1.0.6/src/django_superapp/management/commands/list_all_urls_patterns.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.5/src/django_superapp/management/commands/truncate_all_models.py` & `django_superapp-1.0.6/src/django_superapp/management/commands/truncate_all_models.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.5/src/django_superapp/settings.py` & `django_superapp-1.0.6/src/django_superapp/settings.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.5/src/django_superapp/sites.py` & `django_superapp-1.0.6/src/django_superapp/sites.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.5/src/django_superapp/urls.py` & `django_superapp-1.0.6/src/django_superapp/urls.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,13 +29,13 @@
             urls_module.extend_superapp_admin_urlpatterns(main_admin_urlpatterns)
 
 
 main_admin_urlpatterns = []
 
 
 def extend_with_superapp_urlpatterns(main_urlpatterns, superapp_apps):
-    from django_superapp_core.sites import superapp_admin_site
+    from django_superapp.sites import superapp_admin_site
     main_urlpatterns += [
         path("portal/", superapp_admin_site.urls),
     ]
     extend_superapp_urlpatterns(main_urlpatterns, superapp_apps)
     extend_superapp_admin_urlpatterns(main_admin_urlpatterns, superapp_apps)
```

### Comparing `django_superapp-1.0.5/src/django_superapp/widgets.py` & `django_superapp-1.0.6/src/django_superapp/widgets.py`

 * *Files identical despite different names*

### Comparing `django_superapp-1.0.5/src/django_superapp.egg-info/PKG-INFO` & `django_superapp-1.0.6/src/django_superapp.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: django_superapp
-Version: 1.0.5
-Summary: Build your startup application faster with django-superapp
+Version: 1.0.6
+Summary: Build your startup's product faster.
 Home-page: https://github.com/django-superapp/django-superapp
 Author: Django SuperApp
 Author-email: django-superapp@bringes.io
 License: MIT
 Project-URL: Bug Reports, https://github.com/django-superapp/django-superapp/issues
 Project-URL: Source, https://github.com/django-superapp/django-superapp
 Classifier: Development Status :: 5 - Production/Stable
@@ -30,16 +30,28 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: Django>=5.0.0
 Requires-Dist: django-unfold>=0.22.0
 Requires-Dist: django-svelte-jsoneditor>=0.4.2
 Requires-Dist: django-import-export>=4.0.3
 Requires-Dist: django-admin-confirm>=1.0.0
+Requires-Dist: click>=8.1.7
+Requires-Dist: copier>=9.2.0
+Requires-Dist: requests>=2.31.0
+Requires-Dist: pydantic>=2.7.1
 
-# django-superapp-core
+# Django SuperApp
+
+### Getting Started
+```bash
+pipx install django_superapp
+django_superapp create-project test_project
+cd test_project
+django_superapp add-app --app-name sample_app
+```
 
 ### Development
 ```bash
 make install-requirements
 make install
 make release
 ```
```

### Comparing `django_superapp-1.0.5/src/django_superapp.egg-info/SOURCES.txt` & `django_superapp-1.0.6/src/django_superapp.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -8,20 +8,24 @@
 src/django_superapp/autocomplete.py
 src/django_superapp/db_fields.py
 src/django_superapp/decorators.py
 src/django_superapp/forms.py
 src/django_superapp/helpers.py
 src/django_superapp/settings.py
 src/django_superapp/sites.py
+src/django_superapp/types.py
 src/django_superapp/urls.py
 src/django_superapp/widgets.py
 src/django_superapp.egg-info/PKG-INFO
 src/django_superapp.egg-info/SOURCES.txt
 src/django_superapp.egg-info/dependency_links.txt
+src/django_superapp.egg-info/entry_points.txt
 src/django_superapp.egg-info/requires.txt
 src/django_superapp.egg-info/top_level.txt
+src/django_superapp/cli/__init__.py
+src/django_superapp/cli/main.py
 src/django_superapp/management/__init__.py
 src/django_superapp/management/commands/__init__.py
 src/django_superapp/management/commands/list_all_permissions.py
 src/django_superapp/management/commands/list_all_urls_patterns.py
 src/django_superapp/management/commands/truncate_all_models.py
 src/django_superapp/migrations/__init__.py
```

