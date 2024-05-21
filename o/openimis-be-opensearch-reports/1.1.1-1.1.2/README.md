# Comparing `tmp/openimis_be_opensearch_reports-1.1.1.tar.gz` & `tmp/openimis_be_opensearch_reports-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openimis_be_opensearch_reports-1.1.1.tar", last modified: Wed May  1 05:26:59 2024, max compression
+gzip compressed data, was "openimis_be_opensearch_reports-1.1.2.tar", last modified: Tue May 21 09:30:49 2024, max compression
```

## Comparing `openimis_be_opensearch_reports-1.1.1.tar` & `openimis_be_opensearch_reports-1.1.2.tar`

### file list

```diff
@@ -1,33 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:26:59.274199 openimis_be_opensearch_reports-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-01 05:26:59.274199 openimis_be_opensearch_reports-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5555 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:26:59.274199 openimis_be_opensearch_reports-1.1.1/openimis_be_opensearch_reports.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6396 2024-05-01 05:26:59.000000 openimis_be_opensearch_reports-1.1.1/openimis_be_opensearch_reports.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-01 05:26:59.000000 openimis_be_opensearch_reports-1.1.1/openimis_be_opensearch_reports.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 05:26:59.000000 openimis_be_opensearch_reports-1.1.1/openimis_be_opensearch_reports.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-01 05:26:59.000000 openimis_be_opensearch_reports-1.1.1/openimis_be_opensearch_reports.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 05:26:59.000000 openimis_be_opensearch_reports-1.1.1/openimis_be_opensearch_reports.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:26:59.274199 openimis_be_opensearch_reports-1.1.1/opensearch_reports/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/gql_mutations.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/gql_queries.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 05:26:59.274199 openimis_be_opensearch_reports-1.1.1/opensearch_reports/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/migrations/0002_default_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/migrations/0003_individuals_groups_dashboards.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/migrations/0004_alter_historicalopensearchdashboard_date_created_and_more.py
--rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/migrations/0005_add_opensearch_rights.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/service.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/validations.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-01 05:26:50.000000 openimis_be_opensearch_reports-1.1.1/opensearch_reports/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 05:26:59.274199 openimis_be_opensearch_reports-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-01 05:26:59.000000 openimis_be_opensearch_reports-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:30:49.179521 openimis_be_opensearch_reports-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-05-21 09:30:49.179521 openimis_be_opensearch_reports-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:30:49.179521 openimis_be_opensearch_reports-1.1.2/openimis_be_opensearch_reports.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6967 2024-05-21 09:30:49.000000 openimis_be_opensearch_reports-1.1.2/openimis_be_opensearch_reports.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-21 09:30:49.000000 openimis_be_opensearch_reports-1.1.2/openimis_be_opensearch_reports.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 09:30:49.000000 openimis_be_opensearch_reports-1.1.2/openimis_be_opensearch_reports.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-21 09:30:49.000000 openimis_be_opensearch_reports-1.1.2/openimis_be_opensearch_reports.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 09:30:49.000000 openimis_be_opensearch_reports-1.1.2/openimis_be_opensearch_reports.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:30:49.175521 openimis_be_opensearch_reports-1.1.2/opensearch_reports/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/gql_mutations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/gql_queries.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:30:49.179521 openimis_be_opensearch_reports-1.1.2/opensearch_reports/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:30:49.179521 openimis_be_opensearch_reports-1.1.2/opensearch_reports/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/management/commands/upload_opensearch_dashboards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 09:30:49.179521 openimis_be_opensearch_reports-1.1.2/opensearch_reports/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4604 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/migrations/0002_default_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/migrations/0003_individuals_groups_dashboards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/migrations/0004_alter_historicalopensearchdashboard_date_created_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1018 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/migrations/0005_add_opensearch_rights.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/validations.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 09:30:37.000000 openimis_be_opensearch_reports-1.1.2/opensearch_reports/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 09:30:49.179521 openimis_be_opensearch_reports-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-05-21 09:30:48.000000 openimis_be_opensearch_reports-1.1.2/setup.py
```

### Comparing `openimis_be_opensearch_reports-1.1.1/LICENSE` & `openimis_be_opensearch_reports-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openimis_be_opensearch_reports-1.1.1/LICENSE.md` & `openimis_be_opensearch_reports-1.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `openimis_be_opensearch_reports-1.1.1/PKG-INFO` & `openimis_be_opensearch_reports-1.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-opensearch_reports
-Version: 1.1.1
+Version: 1.1.2
 Summary: The openIMIS Backend opensearch_reports reference module.
 Home-page: https://openimis.org/
 Author: sniedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -137,7 +137,17 @@
 * At the top-right corner of the table, click on `Export <N> objects`.
 * Ensure that you have selected dashboards only. Additionally, choose the option to 
 include related objects, and then click export all.
 * You should have downloaded file in `.ndjson` format. 
 * Save file in the business model for initialization after deployment in 
 `openimis-be_<module-name>/import_data`.
 * Rename filename into `opensearch_<model-name>_dashboard.ndjson`
+
+## Developer tools
+
+### To upload opensearch configuration
+
+- from `/openimis-be_py/openIMIS`:
+  - run this command: `python manage.py upload_opensearch_dashboards --host-domain <host-domain> --imis-password <password>`. This command will This command will upload dashboards config 
+  including charts, visualizations, indexes if the opensearch is available in package.
+  - `<password>` - password necessary to log as admin user to obtain token to connect with API
+  - `<host-domain>` is a hostname with http or https protocol for example `https://release.openimis.org`
```

### Comparing `openimis_be_opensearch_reports-1.1.1/README.md` & `openimis_be_opensearch_reports-1.1.2/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -113,7 +113,17 @@
 * At the top-right corner of the table, click on `Export <N> objects`.
 * Ensure that you have selected dashboards only. Additionally, choose the option to 
 include related objects, and then click export all.
 * You should have downloaded file in `.ndjson` format. 
 * Save file in the business model for initialization after deployment in 
 `openimis-be_<module-name>/import_data`.
 * Rename filename into `opensearch_<model-name>_dashboard.ndjson`
+
+## Developer tools
+
+### To upload opensearch configuration
+
+- from `/openimis-be_py/openIMIS`:
+  - run this command: `python manage.py upload_opensearch_dashboards --host-domain <host-domain> --imis-password <password>`. This command will This command will upload dashboards config 
+  including charts, visualizations, indexes if the opensearch is available in package.
+  - `<password>` - password necessary to log as admin user to obtain token to connect with API
+  - `<host-domain>` is a hostname with http or https protocol for example `https://release.openimis.org`
```

### Comparing `openimis_be_opensearch_reports-1.1.1/openimis_be_opensearch_reports.egg-info/PKG-INFO` & `openimis_be_opensearch_reports-1.1.2/openimis_be_opensearch_reports.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openimis-be-opensearch_reports
-Version: 1.1.1
+Version: 1.1.2
 Summary: The openIMIS Backend opensearch_reports reference module.
 Home-page: https://openimis.org/
 Author: sniedzielski
 Author-email: sniedzielski@soldevelo.com
 License: GNU AGPL v3
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -137,7 +137,17 @@
 * At the top-right corner of the table, click on `Export <N> objects`.
 * Ensure that you have selected dashboards only. Additionally, choose the option to 
 include related objects, and then click export all.
 * You should have downloaded file in `.ndjson` format. 
 * Save file in the business model for initialization after deployment in 
 `openimis-be_<module-name>/import_data`.
 * Rename filename into `opensearch_<model-name>_dashboard.ndjson`
+
+## Developer tools
+
+### To upload opensearch configuration
+
+- from `/openimis-be_py/openIMIS`:
+  - run this command: `python manage.py upload_opensearch_dashboards --host-domain <host-domain> --imis-password <password>`. This command will This command will upload dashboards config 
+  including charts, visualizations, indexes if the opensearch is available in package.
+  - `<password>` - password necessary to log as admin user to obtain token to connect with API
+  - `<host-domain>` is a hostname with http or https protocol for example `https://release.openimis.org`
```

### Comparing `openimis_be_opensearch_reports-1.1.1/openimis_be_opensearch_reports.egg-info/SOURCES.txt` & `openimis_be_opensearch_reports-1.1.2/openimis_be_opensearch_reports.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,13 +15,16 @@
 opensearch_reports/models.py
 opensearch_reports/schema.py
 opensearch_reports/service.py
 opensearch_reports/tests.py
 opensearch_reports/urls.py
 opensearch_reports/validations.py
 opensearch_reports/views.py
+opensearch_reports/management/__init__.py
+opensearch_reports/management/commands/__init__.py
+opensearch_reports/management/commands/upload_opensearch_dashboards.py
 opensearch_reports/migrations/0001_initial.py
 opensearch_reports/migrations/0002_default_dashboards.py
 opensearch_reports/migrations/0003_individuals_groups_dashboards.py
 opensearch_reports/migrations/0004_alter_historicalopensearchdashboard_date_created_and_more.py
 opensearch_reports/migrations/0005_add_opensearch_rights.py
 opensearch_reports/migrations/__init__.py
```

### Comparing `openimis_be_opensearch_reports-1.1.1/opensearch_reports/apps.py` & `openimis_be_opensearch_reports-1.1.2/opensearch_reports/apps.py`

 * *Files identical despite different names*

### Comparing `openimis_be_opensearch_reports-1.1.1/opensearch_reports/gql_mutations.py` & `openimis_be_opensearch_reports-1.1.2/opensearch_reports/gql_mutations.py`

 * *Files identical despite different names*

### Comparing `openimis_be_opensearch_reports-1.1.1/opensearch_reports/gql_queries.py` & `openimis_be_opensearch_reports-1.1.2/opensearch_reports/gql_queries.py`

 * *Files identical despite different names*

### Comparing `openimis_be_opensearch_reports-1.1.1/opensearch_reports/migrations/0001_initial.py` & `openimis_be_opensearch_reports-1.1.2/opensearch_reports/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `openimis_be_opensearch_reports-1.1.1/opensearch_reports/migrations/0002_default_dashboards.py` & `openimis_be_opensearch_reports-1.1.2/opensearch_reports/migrations/0002_default_dashboards.py`

 * *Files identical despite different names*

### Comparing `openimis_be_opensearch_reports-1.1.1/opensearch_reports/migrations/0003_individuals_groups_dashboards.py` & `openimis_be_opensearch_reports-1.1.2/opensearch_reports/migrations/0003_individuals_groups_dashboards.py`

 * *Files identical despite different names*

### Comparing `openimis_be_opensearch_reports-1.1.1/opensearch_reports/migrations/0004_alter_historicalopensearchdashboard_date_created_and_more.py` & `openimis_be_opensearch_reports-1.1.2/opensearch_reports/migrations/0004_alter_historicalopensearchdashboard_date_created_and_more.py`

 * *Files identical despite different names*

### Comparing `openimis_be_opensearch_reports-1.1.1/opensearch_reports/migrations/0005_add_opensearch_rights.py` & `openimis_be_opensearch_reports-1.1.2/opensearch_reports/migrations/0005_add_opensearch_rights.py`

 * *Files identical despite different names*

### Comparing `openimis_be_opensearch_reports-1.1.1/opensearch_reports/schema.py` & `openimis_be_opensearch_reports-1.1.2/opensearch_reports/schema.py`

 * *Files identical despite different names*

### Comparing `openimis_be_opensearch_reports-1.1.1/opensearch_reports/service.py` & `openimis_be_opensearch_reports-1.1.2/opensearch_reports/service.py`

 * *Files identical despite different names*

### Comparing `openimis_be_opensearch_reports-1.1.1/setup.py` & `openimis_be_opensearch_reports-1.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='openimis-be-opensearch_reports',
-    version='v1.1.1',
+    version='v1.1.2',
     packages=find_packages(),
     include_package_data=True,
     license='GNU AGPL v3',
     description='The openIMIS Backend opensearch_reports reference module.',
     long_description=README,
     long_description_content_type='text/markdown',
     url='https://openimis.org/',
```

