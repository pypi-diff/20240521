# Comparing `tmp/pynest_api-0.2.2.tar.gz` & `tmp/pynest_api-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynest_api-0.2.2.tar", last modified: Wed Apr 24 08:19:33 2024, max compression
+gzip compressed data, was "pynest_api-0.2.3.tar", last modified: Tue May 21 05:59:14 2024, max compression
```

## Comparing `pynest_api-0.2.2.tar` & `pynest_api-0.2.3.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.427373 pynest_api-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-24 08:18:56.000000 pynest_api-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-24 08:19:33.427373 pynest_api-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-24 08:18:56.000000 pynest_api-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.415373 pynest_api-0.2.2/nest/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.415373 pynest_api-0.2.2/nest/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/cli/click_handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.419373 pynest_api-0.2.2/nest/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/module.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/route_resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.419373 pynest_api-0.2.2/nest/common/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/base_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/blank_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/mongo_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/mysql_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/orm_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/postgres_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/sqlite_template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/common/templates/templates_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.419373 pynest_api-0.2.2/nest/core/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.419373 pynest_api-0.2.2/nest/core/database/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/database/base_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/database/odm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/database/odm_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/database/orm_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/database/orm_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/core/decorators/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/class_based_view.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/database.py
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/http_method.py
--rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/http_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/injectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/module.py
--rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/decorators/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/pynest_app_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/pynest_application.py
--rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/pynest_container.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/core/pynest_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/plugins/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/controllers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/plugins/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/plugins/modules/auth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/auth/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/plugins/modules/redis/
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/redis/redis_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/redis/redis_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/redis/redis_module.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/modules/redis/redis_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/nest/plugins/services/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:56.000000 pynest_api-0.2.2/nest/plugins/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:19:33.423373 pynest_api-0.2.2/pynest_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-04-24 08:19:33.000000 pynest_api-0.2.2/pynest_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-24 08:19:33.000000 pynest_api-0.2.2/pynest_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:19:33.000000 pynest_api-0.2.2/pynest_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 08:19:33.000000 pynest_api-0.2.2/pynest_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      297 2024-04-24 08:19:33.000000 pynest_api-0.2.2/pynest_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-24 08:19:33.000000 pynest_api-0.2.2/pynest_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-04-24 08:18:56.000000 pynest_api-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:19:33.427373 pynest_api-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.698174 pynest_api-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-21 05:58:47.000000 pynest_api-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-05-21 05:59:14.694173 pynest_api-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-05-21 05:58:47.000000 pynest_api-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.686173 pynest_api-0.2.3/nest/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.686173 pynest_api-0.2.3/nest/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/cli/click_handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.686173 pynest_api-0.2.3/nest/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/route_resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.686173 pynest_api-0.2.3/nest/common/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10224 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/templates/base_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/templates/blank_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4552 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/templates/mongo_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/templates/mysql_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9720 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/templates/orm_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/templates/postgres_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/templates/sqlite_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/common/templates/templates_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.690173 pynest_api-0.2.3/nest/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.690173 pynest_api-0.2.3/nest/core/database/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/database/base_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/database/odm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/database/odm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7075 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/database/orm_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/database/orm_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.690173 pynest_api-0.2.3/nest/core/decorators/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4086 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/decorators/class_based_view.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/decorators/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/decorators/database.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/decorators/http_method.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/decorators/http_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/decorators/injectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/decorators/module.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2902 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/decorators/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3744 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/pynest_app_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/pynest_application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6678 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/pynest_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/core/pynest_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.690173 pynest_api-0.2.3/nest/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.690173 pynest_api-0.2.3/nest/plugins/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/plugins/controllers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.694173 pynest_api-0.2.3/nest/plugins/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/plugins/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.694173 pynest_api-0.2.3/nest/plugins/modules/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/plugins/modules/auth/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.694173 pynest_api-0.2.3/nest/plugins/modules/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/plugins/modules/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/plugins/modules/redis/redis_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/plugins/modules/redis/redis_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/plugins/modules/redis/redis_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/plugins/modules/redis/redis_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.694173 pynest_api-0.2.3/nest/plugins/services/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 05:58:47.000000 pynest_api-0.2.3/nest/plugins/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 05:59:14.694173 pynest_api-0.2.3/pynest_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8959 2024-05-21 05:59:14.000000 pynest_api-0.2.3/pynest_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-21 05:59:14.000000 pynest_api-0.2.3/pynest_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 05:59:14.000000 pynest_api-0.2.3/pynest_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-21 05:59:14.000000 pynest_api-0.2.3/pynest_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      297 2024-05-21 05:59:14.000000 pynest_api-0.2.3/pynest_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 05:59:14.000000 pynest_api-0.2.3/pynest_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-21 05:58:47.000000 pynest_api-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 05:59:14.698174 pynest_api-0.2.3/setup.cfg
```

### Comparing `pynest_api-0.2.2/LICENSE` & `pynest_api-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/PKG-INFO` & `pynest_api-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynest-api
-Version: 0.2.2
+Version: 0.2.3
 Summary: PyNest is a FastAPI Abstraction for building microservices, influenced by NestJS.
 Author-email: Itay Dar <itay2803@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 PyNest
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynest-api Version: 0.2.2 Summary: PyNest is a
+Metadata-Version: 2.1 Name: pynest-api Version: 0.2.3 Summary: PyNest is a
 FastAPI Abstraction for building microservices, influenced by NestJS. Author-
 email: Itay Dar
 gmail.com> License: MIT License Copyright (c) 2023 PyNest Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

### Comparing `pynest_api-0.2.2/README.md` & `pynest_api-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/cli/cli.py` & `pynest_api-0.2.3/nest/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/cli/click_handlers.py` & `pynest_api-0.2.3/nest/cli/click_handlers.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/common/module.py` & `pynest_api-0.2.3/nest/common/module.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/common/route_resolver.py` & `pynest_api-0.2.3/nest/common/route_resolver.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/common/templates/base_template.py` & `pynest_api-0.2.3/nest/common/templates/base_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/common/templates/blank_template.py` & `pynest_api-0.2.3/nest/common/templates/blank_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/common/templates/mongo_template.py` & `pynest_api-0.2.3/nest/common/templates/mongo_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/common/templates/mysql_template.py` & `pynest_api-0.2.3/nest/common/templates/mysql_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/common/templates/orm_template.py` & `pynest_api-0.2.3/nest/common/templates/orm_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/common/templates/postgres_template.py` & `pynest_api-0.2.3/nest/common/templates/postgres_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/common/templates/sqlite_template.py` & `pynest_api-0.2.3/nest/common/templates/sqlite_template.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/common/templates/templates_factory.py` & `pynest_api-0.2.3/nest/common/templates/templates_factory.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/database/base_config.py` & `pynest_api-0.2.3/nest/core/database/base_config.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/database/odm_config.py` & `pynest_api-0.2.3/nest/core/database/odm_config.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/database/odm_provider.py` & `pynest_api-0.2.3/nest/core/database/odm_provider.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/database/orm_config.py` & `pynest_api-0.2.3/nest/core/database/orm_config.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/database/orm_provider.py` & `pynest_api-0.2.3/nest/core/database/orm_provider.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/decorators/class_based_view.py` & `pynest_api-0.2.3/nest/core/decorators/class_based_view.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/decorators/controller.py` & `pynest_api-0.2.3/nest/core/decorators/controller.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/decorators/database.py` & `pynest_api-0.2.3/nest/core/decorators/database.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/decorators/http_method.py` & `pynest_api-0.2.3/nest/core/decorators/http_method.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/decorators/http_methods.py` & `pynest_api-0.2.3/nest/core/decorators/http_methods.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/decorators/module.py` & `pynest_api-0.2.3/nest/core/decorators/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,14 @@
         self.providers = providers or []
         self.imports = imports or []
         self.exports = exports
         self.is_global = is_global
 
     def __call__(self, cls):
         setattr(cls, ModuleMetadata.CONTROLLERS, self.controllers)
-        setattr(cls, ModuleMetadata.PROVIDER, self.providers)
-        setattr(cls, ModuleMetadata.IMPORT, self.imports)
-        setattr(cls, ModuleMetadata.EXPORTS, self.imports)
+        setattr(cls, ModuleMetadata.PROVIDERS, self.providers)
+        setattr(cls, ModuleMetadata.IMPORTS, self.imports)
+        setattr(cls, ModuleMetadata.EXPORTS, self.exports)
         setattr(cls, "__is_module__", True)
         setattr(cls, "__is_global__", self.is_global)
 
         return cls
```

### Comparing `pynest_api-0.2.2/nest/core/decorators/utils.py` & `pynest_api-0.2.3/nest/core/decorators/utils.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/pynest_app_context.py` & `pynest_api-0.2.3/nest/core/pynest_app_context.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/pynest_application.py` & `pynest_api-0.2.3/nest/core/pynest_application.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/pynest_container.py` & `pynest_api-0.2.3/nest/core/pynest_container.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/core/pynest_factory.py` & `pynest_api-0.2.3/nest/core/pynest_factory.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/plugins/modules/redis/redis_controller.py` & `pynest_api-0.2.3/nest/plugins/modules/redis/redis_controller.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/nest/plugins/modules/redis/redis_service.py` & `pynest_api-0.2.3/nest/plugins/modules/redis/redis_service.py`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/pynest_api.egg-info/PKG-INFO` & `pynest_api-0.2.3/pynest_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynest-api
-Version: 0.2.2
+Version: 0.2.3
 Summary: PyNest is a FastAPI Abstraction for building microservices, influenced by NestJS.
 Author-email: Itay Dar <itay2803@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 PyNest
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pynest-api Version: 0.2.2 Summary: PyNest is a
+Metadata-Version: 2.1 Name: pynest-api Version: 0.2.3 Summary: PyNest is a
 FastAPI Abstraction for building microservices, influenced by NestJS. Author-
 email: Itay Dar
 gmail.com> License: MIT License Copyright (c) 2023 PyNest Permission is hereby
 granted, free of charge, to any person obtaining a copy of this software and
 associated documentation files (the "Software"), to deal in the Software
 without restriction, including without limitation the rights to use, copy,
 modify, merge, publish, distribute, sublicense, and/or sell copies of the
```

### Comparing `pynest_api-0.2.2/pynest_api.egg-info/SOURCES.txt` & `pynest_api-0.2.3/pynest_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pynest_api-0.2.2/pyproject.toml` & `pynest_api-0.2.3/pyproject.toml`

 * *Files identical despite different names*

