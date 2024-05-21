# Comparing `tmp/netbox_attachments-5.0.0.tar.gz` & `tmp/netbox_attachments-5.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_attachments-5.0.0.tar", last modified: Tue May 21 09:25:52 2024, max compression
+gzip compressed data, was "netbox_attachments-5.0.0b1.tar", last modified: Tue May 14 11:56:54 2024, max compression
```

## Comparing `netbox_attachments-5.0.0.tar` & `netbox_attachments-5.0.0b1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:25:52.674389 netbox_attachments-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-21 09:25:52.670389 netbox_attachments-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:25:52.666389 netbox_attachments-5.0.0/netbox_attachments/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:25:52.670389 netbox_attachments-5.0.0/netbox_attachments/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/filtersets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:25:52.670389 netbox_attachments-5.0.0/netbox_attachments/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/migrations/0002_alter_netboxattachment_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/migrations/0003_alter_netboxattachment_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/migrations/0004_netboxattachment_size_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/migrations/0005_netboxattachment_description.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/models.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:25:52.666389 netbox_attachments-5.0.0/netbox_attachments/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:25:52.670389 netbox_attachments-5.0.0/netbox_attachments/templates/netbox_attachments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/templates/netbox_attachments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/templates/netbox_attachments/add_attachment_button.html
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/templates/netbox_attachments/generic_tab_list.html
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/templates/netbox_attachments/netbox_attachment_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/templates/netbox_attachments/netbox_attachment_panel.html
--rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/templates/netbox_attachments/netboxattachment.html
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/netbox_attachments/views.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:25:52.670389 netbox_attachments-5.0.0/netbox_attachments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3892 2024-05-21 09:25:52.000000 netbox_attachments-5.0.0/netbox_attachments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-21 09:25:52.000000 netbox_attachments-5.0.0/netbox_attachments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:25:52.000000 netbox_attachments-5.0.0/netbox_attachments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:25:52.000000 netbox_attachments-5.0.0/netbox_attachments.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 09:25:52.000000 netbox_attachments-5.0.0/netbox_attachments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:25:52.674389 netbox_attachments-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-21 09:25:49.000000 netbox_attachments-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.255107 netbox_attachments-5.0.0b1/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-05-14 11:56:54.251108 netbox_attachments-5.0.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.251108 netbox_attachments-5.0.0b1/netbox_attachments/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.251108 netbox_attachments-5.0.0b1/netbox_attachments/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/filtersets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.251108 netbox_attachments-5.0.0b1/netbox_attachments/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/migrations/0002_alter_netboxattachment_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/migrations/0003_alter_netboxattachment_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/migrations/0004_netboxattachment_size_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/migrations/0005_netboxattachment_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6365 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.247107 netbox_attachments-5.0.0b1/netbox_attachments/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.251108 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/add_attachment_button.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/generic_tab_list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/netbox_attachment_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/netbox_attachment_panel.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/netboxattachment.html
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/netbox_attachments/views.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 11:56:54.251108 netbox_attachments-5.0.0b1/netbox_attachments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3894 2024-05-14 11:56:54.000000 netbox_attachments-5.0.0b1/netbox_attachments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-05-14 11:56:54.000000 netbox_attachments-5.0.0b1/netbox_attachments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:56:54.000000 netbox_attachments-5.0.0b1/netbox_attachments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 11:56:54.000000 netbox_attachments-5.0.0b1/netbox_attachments.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-14 11:56:54.000000 netbox_attachments-5.0.0b1/netbox_attachments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 11:56:54.255107 netbox_attachments-5.0.0b1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-14 11:56:50.000000 netbox_attachments-5.0.0b1/setup.py
```

### Comparing `netbox_attachments-5.0.0/PKG-INFO` & `netbox_attachments-5.0.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-attachments
-Version: 5.0.0
+Version: 5.0.0b1
 Summary: Netbox plugin to manage attachments for any model
 Home-page: https://github.com/Kani999/netbox-attachments
 Author: Jan Krupa
 Keywords: netbox,netbox-plugin
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -26,15 +26,15 @@
 | -------- | --------------- |
 | >= 3.3.4 | 0.0.0 <-> 0.0.5 |
 | >= 3.4.0 | 0.0.6 <-> 1.0.6 |
 | >= 3.4.3 | 1.0.7 <-> 1.1.X |
 | >= 3.5.0 | 2.0.0           |
 | >= 3.6.0 | 3.0.0           |
 | >= 3.7.0 | 4.0.0           |
-| >= 4.0.0 | 5.0.0           |
+| >= 4.0.0 | 5.0.0-beta1     |
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```
 pip install netbox-attachments
```

### Comparing `netbox_attachments-5.0.0/README.md` & `netbox_attachments-5.0.0b1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 | -------- | --------------- |
 | >= 3.3.4 | 0.0.0 <-> 0.0.5 |
 | >= 3.4.0 | 0.0.6 <-> 1.0.6 |
 | >= 3.4.3 | 1.0.7 <-> 1.1.X |
 | >= 3.5.0 | 2.0.0           |
 | >= 3.6.0 | 3.0.0           |
 | >= 3.7.0 | 4.0.0           |
-| >= 4.0.0 | 5.0.0           |
+| >= 4.0.0 | 5.0.0-beta1     |
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```
 pip install netbox-attachments
```

### Comparing `netbox_attachments-5.0.0/netbox_attachments/__init__.py` & `netbox_attachments-5.0.0b1/netbox_attachments/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/api/serializers.py` & `netbox_attachments-5.0.0b1/netbox_attachments/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/filtersets.py` & `netbox_attachments-5.0.0b1/netbox_attachments/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/forms.py` & `netbox_attachments-5.0.0b1/netbox_attachments/forms.py`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/migrations/0001_initial.py` & `netbox_attachments-5.0.0b1/netbox_attachments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/migrations/0002_alter_netboxattachment_options_and_more.py` & `netbox_attachments-5.0.0b1/netbox_attachments/migrations/0002_alter_netboxattachment_options_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/migrations/0004_netboxattachment_size_and_more.py` & `netbox_attachments-5.0.0b1/netbox_attachments/migrations/0004_netboxattachment_size_and_more.py`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/models.py` & `netbox_attachments-5.0.0b1/netbox_attachments/models.py`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/tables.py` & `netbox_attachments-5.0.0b1/netbox_attachments/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/template_content.py` & `netbox_attachments-5.0.0b1/netbox_attachments/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/templates/netbox_attachments/generic_tab_list.html` & `netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/generic_tab_list.html`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/templates/netbox_attachments/netbox_attachment_edit.html` & `netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/netbox_attachment_edit.html`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/templates/netbox_attachments/netbox_attachment_panel.html` & `netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/netbox_attachment_panel.html`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/templates/netbox_attachments/netboxattachment.html` & `netbox_attachments-5.0.0b1/netbox_attachments/templates/netbox_attachments/netboxattachment.html`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/urls.py` & `netbox_attachments-5.0.0b1/netbox_attachments/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments/views.py` & `netbox_attachments-5.0.0b1/netbox_attachments/views.py`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/netbox_attachments.egg-info/PKG-INFO` & `netbox_attachments-5.0.0b1/netbox_attachments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-attachments
-Version: 5.0.0
+Version: 5.0.0b1
 Summary: Netbox plugin to manage attachments for any model
 Home-page: https://github.com/Kani999/netbox-attachments
 Author: Jan Krupa
 Keywords: netbox,netbox-plugin
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
@@ -26,15 +26,15 @@
 | -------- | --------------- |
 | >= 3.3.4 | 0.0.0 <-> 0.0.5 |
 | >= 3.4.0 | 0.0.6 <-> 1.0.6 |
 | >= 3.4.3 | 1.0.7 <-> 1.1.X |
 | >= 3.5.0 | 2.0.0           |
 | >= 3.6.0 | 3.0.0           |
 | >= 3.7.0 | 4.0.0           |
-| >= 4.0.0 | 5.0.0           |
+| >= 4.0.0 | 5.0.0-beta1     |
 
 ## Installation
 
 The plugin is available as a Python package in pypi and can be installed with pip
 
 ```
 pip install netbox-attachments
```

### Comparing `netbox_attachments-5.0.0/netbox_attachments.egg-info/SOURCES.txt` & `netbox_attachments-5.0.0b1/netbox_attachments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox_attachments-5.0.0/setup.py` & `netbox_attachments-5.0.0b1/setup.py`

 * *Files identical despite different names*

