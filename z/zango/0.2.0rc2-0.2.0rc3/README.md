# Comparing `tmp/zango-0.2.0rc2.tar.gz` & `tmp/zango-0.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zango-0.2.0rc2.tar", last modified: Tue May 21 11:52:32 2024, max compression
+gzip compressed data, was "zango-0.2.0rc3.tar", last modified: Tue May 21 13:14:55 2024, max compression
```

## Comparing `zango-0.2.0rc2.tar` & `zango-0.2.0rc3.tar`

### file list

```diff
@@ -1,302 +1,302 @@
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.620587 zango-0.2.0rc2/
--rw-r--r--   0 harshshah   (501) staff       (20)    10873 2024-05-21 11:25:52.000000 zango-0.2.0rc2/LICENSE
--rw-r--r--   0 harshshah   (501) staff       (20)     5993 2024-05-21 11:52:32.592220 zango-0.2.0rc2/PKG-INFO
--rw-r--r--   0 harshshah   (501) staff       (20)     4307 2024-05-21 11:19:53.000000 zango-0.2.0rc2/README.md
--rw-r--r--   0 harshshah   (501) staff       (20)       38 2024-05-21 11:52:32.620844 zango-0.2.0rc2/setup.cfg
--rw-r--r--   0 harshshah   (501) staff       (20)     1444 2024-05-21 11:51:52.000000 zango-0.2.0rc2/setup.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.248702 zango-0.2.0rc2/src/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.371166 zango-0.2.0rc2/src/zango/
--rw-r--r--   0 harshshah   (501) staff       (20)       64 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.402592 zango-0.2.0rc2/src/zango/api/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.403513 zango-0.2.0rc2/src/zango/api/app_auth/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/app_auth/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.404400 zango-0.2.0rc2/src/zango/api/app_auth/profile/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/app_auth/profile/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.419944 zango-0.2.0rc2/src/zango/api/app_auth/profile/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/app_auth/profile/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      237 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/app_auth/profile/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      281 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/app_auth/profile/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5419 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/app_auth/profile/v1/utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2753 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/app_auth/profile/v1/views.py
--rw-r--r--   0 harshshah   (501) staff       (20)      156 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/app_auth/urls.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.434996 zango-0.2.0rc2/src/zango/api/platform/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.436477 zango-0.2.0rc2/src/zango/api/platform/auditlogs/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/api/platform/auditlogs/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.451819 zango-0.2.0rc2/src/zango/api/platform/auditlogs/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/api/platform/auditlogs/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1799 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/api/platform/auditlogs/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      200 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/api/platform/auditlogs/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     6762 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/api/platform/auditlogs/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.452792 zango-0.2.0rc2/src/zango/api/platform/auth/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/auth/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.473072 zango-0.2.0rc2/src/zango/api/platform/auth/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/auth/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      558 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/auth/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      537 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/auth/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     6079 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/auth/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.475829 zango-0.2.0rc2/src/zango/api/platform/codeassist/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/codeassist/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.533326 zango-0.2.0rc2/src/zango/api/platform/codeassist/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/codeassist/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      369 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/codeassist/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)      254 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/codeassist/v1/utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)    11926 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/codeassist/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.535133 zango-0.2.0rc2/src/zango/api/platform/packages/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/packages/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.539580 zango-0.2.0rc2/src/zango/api/platform/packages/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/packages/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      217 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/packages/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2601 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/packages/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.540982 zango-0.2.0rc2/src/zango/api/platform/permissions/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/permissions/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.551070 zango-0.2.0rc2/src/zango/api/platform/permissions/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/permissions/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1945 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/permissions/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      583 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/permissions/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     6507 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/permissions/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.553937 zango-0.2.0rc2/src/zango/api/platform/tasks/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/tasks/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.558872 zango-0.2.0rc2/src/zango/api/platform/tasks/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/tasks/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1366 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/tasks/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      213 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/tasks/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     4914 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/tasks/v1/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.559841 zango-0.2.0rc2/src/zango/api/platform/tenancy/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/tenancy/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.570259 zango-0.2.0rc2/src/zango/api/platform/tenancy/v1/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/tenancy/v1/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     4832 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/tenancy/v1/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2071 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/api/platform/tenancy/v1/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)    21220 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/api/platform/tenancy/v1/views.py
--rw-r--r--   0 harshshah   (501) staff       (20)      241 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/api/platform/urls.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.571236 zango-0.2.0rc2/src/zango/apps/
--rw-r--r--   0 harshshah   (501) staff       (20)      176 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.591196 zango-0.2.0rc2/src/zango/apps/appauth/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      124 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      221 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/apps.py
--rw-r--r--   0 harshshah   (501) staff       (20)      929 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/auth_backend.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.738983 zango-0.2.0rc2/src/zango/apps/appauth/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)     7465 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)      618 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/migrations/0002_default_user_roles.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1124 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1633 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/migrations/0004_oldpasswords.py
--rw-r--r--   0 harshshah   (501) staff       (20)      325 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/migrations/0005_remove_appusermodel_user.py
--rw-r--r--   0 harshshah   (501) staff       (20)      396 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/migrations/0006_appusermodel_app_objects.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     9431 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/appauth/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)      356 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/serializers.py
--rw-r--r--   0 harshshah   (501) staff       (20)      477 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/signals.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.750658 zango-0.2.0rc2/src/zango/apps/appauth/templates/
--rw-r--r--   0 harshshah   (501) staff       (20)      738 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/templates/app.html
--rw-r--r--   0 harshshah   (501) staff       (20)      919 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/templates/app_login_signup.html
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)      203 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)      682 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/appauth/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.866758 zango-0.2.0rc2/src/zango/apps/auditlogs/
--rw-r--r--   0 harshshah   (501) staff       (20)        1 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1870 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      473 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/apps.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2151 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/cid.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1451 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/conf.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2744 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/context.py
--rw-r--r--   0 harshshah   (501) staff       (20)     7934 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/diff.py
--rw-r--r--   0 harshshah   (501) staff       (20)      982 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/filters.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.872419 zango-0.2.0rc2/src/zango/apps/auditlogs/management/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/management/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.882389 zango-0.2.0rc2/src/zango/apps/auditlogs/management/commands/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/management/commands/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1681 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/management/commands/auditlogflush.py
--rw-r--r--   0 harshshah   (501) staff       (20)     4608 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/management/commands/auditlogmigratejson.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2135 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/middleware.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.889134 zango-0.2.0rc2/src/zango/apps/auditlogs/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)     5014 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     6136 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/mixins.py
--rw-r--r--   0 harshshah   (501) staff       (20)    24158 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5398 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/receivers.py
--rw-r--r--   0 harshshah   (501) staff       (20)    13367 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/registry.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2369 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/auditlogs/signals.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.955775 zango-0.2.0rc2/src/zango/apps/dynamic_models/
--rw-r--r--   0 harshshah   (501) staff       (20)       59 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1063 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.957368 zango-0.2.0rc2/src/zango/apps/dynamic_models/fields/
--rw-r--r--   0 harshshah   (501) staff       (20)     4411 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/fields/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.958364 zango-0.2.0rc2/src/zango/apps/dynamic_models/management/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/management/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.962540 zango-0.2.0rc2/src/zango/apps/dynamic_models/management/commands/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/management/commands/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      326 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/management/commands/reload_tenant.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.987207 zango-0.2.0rc2/src/zango/apps/dynamic_models/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)    15126 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)      694 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/permissions.py
--rw-r--r--   0 harshshah   (501) staff       (20)      350 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/registry.py
--rw-r--r--   0 harshshah   (501) staff       (20)      871 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/signals.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.989411 zango-0.2.0rc2/src/zango/apps/dynamic_models/templates/
--rw-r--r--   0 harshshah   (501) staff       (20)    29251 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/templates/default_landing.html
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)      224 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     3141 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.009895 zango-0.2.0rc2/src/zango/apps/dynamic_models/workspace/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/workspace/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)    18528 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/workspace/base.py
--rw-r--r--   0 harshshah   (501) staff       (20)      326 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/workspace/lifecycle.py
--rw-r--r--   0 harshshah   (501) staff       (20)      897 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/dynamic_models/workspace/wtree.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.036930 zango-0.2.0rc2/src/zango/apps/object_store/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/object_store/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      130 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/object_store/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      166 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/object_store/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.038477 zango-0.2.0rc2/src/zango/apps/object_store/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)      784 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/object_store/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/object_store/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2485 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/object_store/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/object_store/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/object_store/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.054243 zango-0.2.0rc2/src/zango/apps/permissions/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/permissions/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      242 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/permissions/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      165 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/permissions/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.082101 zango-0.2.0rc2/src/zango/apps/permissions/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)     3203 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/permissions/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)      678 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py
--rw-r--r--   0 harshshah   (501) staff       (20)      669 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/permissions/migrations/0003_default_policy.py
--rw-r--r--   0 harshshah   (501) staff       (20)      762 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/permissions/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5117 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/permissions/mixin.py
--rw-r--r--   0 harshshah   (501) staff       (20)     3904 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/permissions/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/permissions/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/permissions/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.083578 zango-0.2.0rc2/src/zango/apps/shared/
--rw-r--r--   0 harshshah   (501) staff       (20)      454 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.119671 zango-0.2.0rc2/src/zango/apps/shared/platformauth/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/platformauth/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2578 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/platformauth/abstract_model.py
--rw-r--r--   0 harshshah   (501) staff       (20)      140 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/platformauth/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      267 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/platformauth/apps.py
--rw-r--r--   0 harshshah   (501) staff       (20)      940 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/platformauth/auth_backend.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.125486 zango-0.2.0rc2/src/zango/apps/shared/platformauth/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)     5327 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/platformauth/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)      914 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/platformauth/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     7168 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/platformauth/models.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.289265 zango-0.2.0rc2/src/zango/apps/shared/platformauth/templates/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.129842 zango-0.2.0rc2/src/zango/apps/shared/platformauth/templates/app_panel/
--rw-r--r--   0 harshshah   (501) staff       (20)     4952 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/shared/platformauth/templates/app_panel/app_panel_login.html
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/platformauth/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)      379 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/shared/platformauth/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)      627 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/shared/platformauth/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.149124 zango-0.2.0rc2/src/zango/apps/shared/tenancy/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      180 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/admin.py
--rw-r--r--   0 harshshah   (501) staff       (20)      161 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.150357 zango-0.2.0rc2/src/zango/apps/shared/tenancy/management/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/management/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.156846 zango-0.2.0rc2/src/zango/apps/shared/tenancy/management/commands/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/management/commands/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2263 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/management/commands/sync_static.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2780 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/management/commands/ws_makemigration.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1457 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/management/commands/ws_migrate.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.171260 zango-0.2.0rc2/src/zango/apps/shared/tenancy/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)    54320 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)      363 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/migrations/0002_rename_is_default_themesmodel_is_active.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1095 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1136 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5622 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1890 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/tasks.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.171877 zango-0.2.0rc2/src/zango/apps/shared/tenancy/templates/
--rw-r--r--   0 harshshah   (501) staff       (20)      728 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/templates/app_panel.html
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.174035 zango-0.2.0rc2/src/zango/apps/shared/tenancy/templatetags/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/templatetags/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      560 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/templatetags/zstatic.py
--rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/tests.py
--rw-r--r--   0 harshshah   (501) staff       (20)      137 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1554 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)      450 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/views.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.174816 zango-0.2.0rc2/src/zango/apps/shared/tenancy/workspace_folder_template/
--rw-r--r--   0 harshshah   (501) staff       (20)       30 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/workspace_folder_template/cookiecutter.json
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.183656 zango-0.2.0rc2/src/zango/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/
--rw-r--r--   0 harshshah   (501) staff       (20)       22 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/manifest.json
--rw-r--r--   0 harshshah   (501) staff       (20)       93 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/settings.json
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.214364 zango-0.2.0rc2/src/zango/apps/tasks/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/tasks/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      153 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/tasks/apps.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.220081 zango-0.2.0rc2/src/zango/apps/tasks/migrations/
--rw-r--r--   0 harshshah   (501) staff       (20)     2952 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/tasks/migrations/0001_initial.py
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/tasks/migrations/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2786 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/apps/tasks/models.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2649 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/apps/tasks/utils.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.339011 zango-0.2.0rc2/src/zango/assets/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.317545 zango-0.2.0rc2/src/zango/assets/app_landing/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.221076 zango-0.2.0rc2/src/zango/assets/app_landing/css/
--rw-r--r--   0 harshshah   (501) staff       (20)     5763 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/assets/app_landing/css/styles.css
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.336050 zango-0.2.0rc2/src/zango/assets/app_panel/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.222768 zango-0.2.0rc2/src/zango/assets/app_panel/css/
--rw-r--r--   0 harshshah   (501) staff       (20)    10247 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/assets/app_panel/css/styles.css
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.224686 zango-0.2.0rc2/src/zango/assets/app_panel/images/
--rw-r--r--   0 harshshah   (501) staff       (20)     3903 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/assets/app_panel/images/zangoLogo.svg
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.226315 zango-0.2.0rc2/src/zango/assets/app_panel/js/
--rw-r--r--   0 harshshah   (501) staff       (20)  6319876 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/assets/app_panel/js/build.v1.1.1.min.js
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.339647 zango-0.2.0rc2/src/zango/assets/js/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:31.340020 zango-0.2.0rc2/src/zango/assets/js/jquery/
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.264254 zango-0.2.0rc2/src/zango/assets/js/jquery/3.7.1/
--rw-r--r--   0 harshshah   (501) staff       (20)    87532 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/assets/js/jquery/3.7.1/jquery.min.js
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.341119 zango-0.2.0rc2/src/zango/cli/
--rw-r--r--   0 harshshah   (501) staff       (20)      331 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/cli/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      617 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/cli/install_package.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1201 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/cli/package_info.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.358535 zango-0.2.0rc2/src/zango/cli/project_template/
--rwxr-xr-x   0 harshshah   (501) staff       (20)      672 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/cli/project_template/manage.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.451689 zango-0.2.0rc2/src/zango/cli/project_template/project_name/
--rw-r--r--   0 harshshah   (501) staff       (20)       76 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/cli/project_template/project_name/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      404 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/cli/project_template/project_name/asgi.py
--rw-r--r--   0 harshshah   (501) staff       (20)     4205 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/cli/project_template/project_name/settings.py
--rw-r--r--   0 harshshah   (501) staff       (20)      767 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/cli/project_template/project_name/urls.py
--rw-r--r--   0 harshshah   (501) staff       (20)      179 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/cli/project_template/project_name/urls_public.py
--rw-r--r--   0 harshshah   (501) staff       (20)      179 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/cli/project_template/project_name/urls_tenants.py
--rw-r--r--   0 harshshah   (501) staff       (20)      404 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/cli/project_template/project_name/wsgi.py
--rw-r--r--   0 harshshah   (501) staff       (20)     7354 2024-05-21 11:51:49.000000 zango-0.2.0rc2/src/zango/cli/start_project.py
--rw-r--r--   0 harshshah   (501) staff       (20)      688 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/cli/utils.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.474202 zango-0.2.0rc2/src/zango/config/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/config/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)      552 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/config/celery.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.491302 zango-0.2.0rc2/src/zango/config/settings/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/config/settings/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5025 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/config/settings/base.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1045 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/config/urls_public.py
--rw-r--r--   0 harshshah   (501) staff       (20)      708 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/config/urls_tenants.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.549895 zango-0.2.0rc2/src/zango/core/
--rw-r--r--   0 harshshah   (501) staff       (20)       39 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/__init__.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.555082 zango-0.2.0rc2/src/zango/core/api/
--rw-r--r--   0 harshshah   (501) staff       (20)      211 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/api/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2104 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/api/base.py
--rw-r--r--   0 harshshah   (501) staff       (20)      846 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/api/utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1097 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/common_utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)      810 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/custom_pluginbase.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1033 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/core/decorators.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.559582 zango-0.2.0rc2/src/zango/core/generic_views/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/generic_views/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1538 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/core/generic_views/base.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5955 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/internal_requests.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1096 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/model_mixins.py
--rw-r--r--   0 harshshah   (501) staff       (20)     6345 2024-05-21 11:19:53.000000 zango-0.2.0rc2/src/zango/core/package_utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2576 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/permissions.py
--rw-r--r--   0 harshshah   (501) staff       (20)     2100 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/storage_utils.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1237 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/tasks.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1803 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/template_loader.py
--rw-r--r--   0 harshshah   (501) staff       (20)     3014 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/core/utils.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.587782 zango-0.2.0rc2/src/zango/middleware/
--rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/middleware/__init__.py
--rw-r--r--   0 harshshah   (501) staff       (20)     1772 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/middleware/request.py
--rw-r--r--   0 harshshah   (501) staff       (20)     5455 2024-05-15 11:27:55.000000 zango-0.2.0rc2/src/zango/middleware/tenant.py
-drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 11:52:32.589448 zango-0.2.0rc2/src/zango.egg-info/
--rw-r--r--   0 harshshah   (501) staff       (20)     5993 2024-05-21 11:52:28.000000 zango-0.2.0rc2/src/zango.egg-info/PKG-INFO
--rw-r--r--   0 harshshah   (501) staff       (20)     9893 2024-05-21 11:52:29.000000 zango-0.2.0rc2/src/zango.egg-info/SOURCES.txt
--rw-r--r--   0 harshshah   (501) staff       (20)        1 2024-05-21 11:52:28.000000 zango-0.2.0rc2/src/zango.egg-info/dependency_links.txt
--rw-r--r--   0 harshshah   (501) staff       (20)       40 2024-05-21 11:52:28.000000 zango-0.2.0rc2/src/zango.egg-info/entry_points.txt
--rw-r--r--   0 harshshah   (501) staff       (20)      728 2024-05-21 11:52:28.000000 zango-0.2.0rc2/src/zango.egg-info/requires.txt
--rw-r--r--   0 harshshah   (501) staff       (20)        6 2024-05-21 11:52:28.000000 zango-0.2.0rc2/src/zango.egg-info/top_level.txt
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.773748 zango-0.2.0rc3/
+-rw-r--r--   0 harshshah   (501) staff       (20)    10873 2024-05-21 11:25:52.000000 zango-0.2.0rc3/LICENSE
+-rw-r--r--   0 harshshah   (501) staff       (20)     5993 2024-05-21 13:14:55.770655 zango-0.2.0rc3/PKG-INFO
+-rw-r--r--   0 harshshah   (501) staff       (20)     4307 2024-05-21 11:19:53.000000 zango-0.2.0rc3/README.md
+-rw-r--r--   0 harshshah   (501) staff       (20)       38 2024-05-21 13:14:55.773979 zango-0.2.0rc3/setup.cfg
+-rw-r--r--   0 harshshah   (501) staff       (20)     1444 2024-05-21 13:14:19.000000 zango-0.2.0rc3/setup.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.031164 zango-0.2.0rc3/src/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.288384 zango-0.2.0rc3/src/zango/
+-rw-r--r--   0 harshshah   (501) staff       (20)       64 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.303193 zango-0.2.0rc3/src/zango/api/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.307791 zango-0.2.0rc3/src/zango/api/app_auth/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/app_auth/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.309251 zango-0.2.0rc3/src/zango/api/app_auth/profile/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/app_auth/profile/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.322789 zango-0.2.0rc3/src/zango/api/app_auth/profile/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/app_auth/profile/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      237 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/app_auth/profile/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      281 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/app_auth/profile/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5419 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/app_auth/profile/v1/utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2753 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/app_auth/profile/v1/views.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      156 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/app_auth/urls.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.328668 zango-0.2.0rc3/src/zango/api/platform/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.339011 zango-0.2.0rc3/src/zango/api/platform/auditlogs/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/api/platform/auditlogs/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.358412 zango-0.2.0rc3/src/zango/api/platform/auditlogs/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/api/platform/auditlogs/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1799 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/api/platform/auditlogs/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      200 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/api/platform/auditlogs/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     6762 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/api/platform/auditlogs/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.359330 zango-0.2.0rc3/src/zango/api/platform/auth/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/auth/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.381395 zango-0.2.0rc3/src/zango/api/platform/auth/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/auth/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      558 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/auth/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      537 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/auth/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     6079 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/auth/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.392189 zango-0.2.0rc3/src/zango/api/platform/codeassist/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/codeassist/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.415206 zango-0.2.0rc3/src/zango/api/platform/codeassist/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/codeassist/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      369 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/codeassist/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      254 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/codeassist/v1/utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    11926 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/codeassist/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.419302 zango-0.2.0rc3/src/zango/api/platform/packages/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/packages/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.448746 zango-0.2.0rc3/src/zango/api/platform/packages/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/packages/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      217 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/packages/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2601 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/packages/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.461419 zango-0.2.0rc3/src/zango/api/platform/permissions/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/permissions/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.501531 zango-0.2.0rc3/src/zango/api/platform/permissions/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/permissions/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1945 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/permissions/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      583 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/permissions/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     6507 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/permissions/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.502774 zango-0.2.0rc3/src/zango/api/platform/tasks/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/tasks/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.509277 zango-0.2.0rc3/src/zango/api/platform/tasks/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/tasks/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1366 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/tasks/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      213 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/tasks/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     4914 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/tasks/v1/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.519260 zango-0.2.0rc3/src/zango/api/platform/tenancy/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/tenancy/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.592639 zango-0.2.0rc3/src/zango/api/platform/tenancy/v1/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/tenancy/v1/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     4832 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/tenancy/v1/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2071 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/api/platform/tenancy/v1/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    21220 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/api/platform/tenancy/v1/views.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      241 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/api/platform/urls.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.597076 zango-0.2.0rc3/src/zango/apps/
+-rw-r--r--   0 harshshah   (501) staff       (20)      176 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.694016 zango-0.2.0rc3/src/zango/apps/appauth/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      124 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      221 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/apps.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      929 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/auth_backend.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.741824 zango-0.2.0rc3/src/zango/apps/appauth/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)     7465 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      618 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/migrations/0002_default_user_roles.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1124 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1633 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/migrations/0004_oldpasswords.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      325 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/migrations/0005_remove_appusermodel_user.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      396 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/migrations/0006_appusermodel_app_objects.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     9431 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/appauth/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      356 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/serializers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      477 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/signals.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.745296 zango-0.2.0rc3/src/zango/apps/appauth/templates/
+-rw-r--r--   0 harshshah   (501) staff       (20)      738 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/templates/app.html
+-rw-r--r--   0 harshshah   (501) staff       (20)      919 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/templates/app_login_signup.html
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      203 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      682 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/appauth/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.856939 zango-0.2.0rc3/src/zango/apps/auditlogs/
+-rw-r--r--   0 harshshah   (501) staff       (20)        1 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1870 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      473 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/apps.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2151 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/cid.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1451 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/conf.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2744 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/context.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     7934 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/diff.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      982 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/filters.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.857728 zango-0.2.0rc3/src/zango/apps/auditlogs/management/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/management/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.860119 zango-0.2.0rc3/src/zango/apps/auditlogs/management/commands/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/management/commands/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1681 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/management/commands/auditlogflush.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     4608 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/management/commands/auditlogmigratejson.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2135 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/middleware.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.862604 zango-0.2.0rc3/src/zango/apps/auditlogs/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)     5014 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     6136 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/mixins.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    24158 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5398 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/receivers.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    13367 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/registry.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2369 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/auditlogs/signals.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.906206 zango-0.2.0rc3/src/zango/apps/dynamic_models/
+-rw-r--r--   0 harshshah   (501) staff       (20)       59 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1063 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.957499 zango-0.2.0rc3/src/zango/apps/dynamic_models/fields/
+-rw-r--r--   0 harshshah   (501) staff       (20)     4411 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/fields/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.962010 zango-0.2.0rc3/src/zango/apps/dynamic_models/management/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/management/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.986333 zango-0.2.0rc3/src/zango/apps/dynamic_models/management/commands/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/management/commands/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      326 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/management/commands/reload_tenant.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.988537 zango-0.2.0rc3/src/zango/apps/dynamic_models/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    15126 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      694 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/permissions.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      350 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/registry.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      871 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/signals.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.989223 zango-0.2.0rc3/src/zango/apps/dynamic_models/templates/
+-rw-r--r--   0 harshshah   (501) staff       (20)    29251 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/templates/default_landing.html
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      224 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     3141 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.009086 zango-0.2.0rc3/src/zango/apps/dynamic_models/workspace/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/workspace/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)    18528 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/workspace/base.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      326 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/workspace/lifecycle.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      897 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/dynamic_models/workspace/wtree.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.028703 zango-0.2.0rc3/src/zango/apps/object_store/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/object_store/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      130 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/object_store/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      166 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/object_store/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.039168 zango-0.2.0rc3/src/zango/apps/object_store/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)      784 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/object_store/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/object_store/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2485 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/object_store/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/object_store/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/object_store/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.057939 zango-0.2.0rc3/src/zango/apps/permissions/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/permissions/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      242 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/permissions/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      165 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/permissions/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.072901 zango-0.2.0rc3/src/zango/apps/permissions/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)     3203 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/permissions/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      678 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      669 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/permissions/migrations/0003_default_policy.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      762 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/permissions/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5117 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/permissions/mixin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     3904 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/permissions/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/permissions/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       63 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/permissions/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.075373 zango-0.2.0rc3/src/zango/apps/shared/
+-rw-r--r--   0 harshshah   (501) staff       (20)      454 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.132791 zango-0.2.0rc3/src/zango/apps/shared/platformauth/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/platformauth/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2578 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/platformauth/abstract_model.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      140 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/platformauth/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      267 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/platformauth/apps.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      940 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/platformauth/auth_backend.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.136246 zango-0.2.0rc3/src/zango/apps/shared/platformauth/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)     5327 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/platformauth/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      914 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/platformauth/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     7168 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/platformauth/models.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.166885 zango-0.2.0rc3/src/zango/apps/shared/platformauth/templates/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.137643 zango-0.2.0rc3/src/zango/apps/shared/platformauth/templates/app_panel/
+-rw-r--r--   0 harshshah   (501) staff       (20)     4952 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/shared/platformauth/templates/app_panel/app_panel_login.html
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/platformauth/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      379 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/shared/platformauth/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      627 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/shared/platformauth/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.188443 zango-0.2.0rc3/src/zango/apps/shared/tenancy/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      180 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/admin.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      161 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.190475 zango-0.2.0rc3/src/zango/apps/shared/tenancy/management/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/management/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.257818 zango-0.2.0rc3/src/zango/apps/shared/tenancy/management/commands/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/management/commands/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2263 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/management/commands/sync_static.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2780 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/management/commands/ws_makemigration.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1457 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/management/commands/ws_migrate.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.292484 zango-0.2.0rc3/src/zango/apps/shared/tenancy/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)    54320 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      363 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/migrations/0002_rename_is_default_themesmodel_is_active.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1095 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1136 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5622 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1890 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/tasks.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.312990 zango-0.2.0rc3/src/zango/apps/shared/tenancy/templates/
+-rw-r--r--   0 harshshah   (501) staff       (20)      728 2024-05-21 13:14:10.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/templates/app_panel.html
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.320009 zango-0.2.0rc3/src/zango/apps/shared/tenancy/templatetags/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/templatetags/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      560 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/templatetags/zstatic.py
+-rw-r--r--   0 harshshah   (501) staff       (20)       60 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/tests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      137 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1554 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      450 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/views.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.321249 zango-0.2.0rc3/src/zango/apps/shared/tenancy/workspace_folder_template/
+-rw-r--r--   0 harshshah   (501) staff       (20)       30 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/workspace_folder_template/cookiecutter.json
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.324565 zango-0.2.0rc3/src/zango/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/
+-rw-r--r--   0 harshshah   (501) staff       (20)       22 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/manifest.json
+-rw-r--r--   0 harshshah   (501) staff       (20)       93 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/shared/tenancy/workspace_folder_template/{{cookiecutter.app_name}}/settings.json
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.350364 zango-0.2.0rc3/src/zango/apps/tasks/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/tasks/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      153 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/tasks/apps.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.353452 zango-0.2.0rc3/src/zango/apps/tasks/migrations/
+-rw-r--r--   0 harshshah   (501) staff       (20)     2952 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/tasks/migrations/0001_initial.py
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/tasks/migrations/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2786 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/apps/tasks/models.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2649 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/apps/tasks/utils.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.252834 zango-0.2.0rc3/src/zango/assets/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.238991 zango-0.2.0rc3/src/zango/assets/app_landing/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.354693 zango-0.2.0rc3/src/zango/assets/app_landing/css/
+-rw-r--r--   0 harshshah   (501) staff       (20)     5763 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/assets/app_landing/css/styles.css
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.246246 zango-0.2.0rc3/src/zango/assets/app_panel/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.364014 zango-0.2.0rc3/src/zango/assets/app_panel/css/
+-rw-r--r--   0 harshshah   (501) staff       (20)    10247 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/assets/app_panel/css/styles.css
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.366352 zango-0.2.0rc3/src/zango/assets/app_panel/images/
+-rw-r--r--   0 harshshah   (501) staff       (20)     3903 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/assets/app_panel/images/zangoLogo.svg
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.378425 zango-0.2.0rc3/src/zango/assets/app_panel/js/
+-rw-r--r--   0 harshshah   (501) staff       (20)  6319925 2024-05-21 13:14:10.000000 zango-0.2.0rc3/src/zango/assets/app_panel/js/build.v1.1.2.min.js
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.254073 zango-0.2.0rc3/src/zango/assets/js/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:54.254570 zango-0.2.0rc3/src/zango/assets/js/jquery/
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.409340 zango-0.2.0rc3/src/zango/assets/js/jquery/3.7.1/
+-rw-r--r--   0 harshshah   (501) staff       (20)    87532 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/assets/js/jquery/3.7.1/jquery.min.js
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.423976 zango-0.2.0rc3/src/zango/cli/
+-rw-r--r--   0 harshshah   (501) staff       (20)      331 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/cli/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      617 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/cli/install_package.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1201 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/cli/package_info.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.425309 zango-0.2.0rc3/src/zango/cli/project_template/
+-rwxr-xr-x   0 harshshah   (501) staff       (20)      672 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/cli/project_template/manage.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.455127 zango-0.2.0rc3/src/zango/cli/project_template/project_name/
+-rw-r--r--   0 harshshah   (501) staff       (20)       76 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/cli/project_template/project_name/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      404 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/cli/project_template/project_name/asgi.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     4205 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/cli/project_template/project_name/settings.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      767 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/cli/project_template/project_name/urls.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      179 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/cli/project_template/project_name/urls_public.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      179 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/cli/project_template/project_name/urls_tenants.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      404 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/cli/project_template/project_name/wsgi.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     7354 2024-05-21 11:51:49.000000 zango-0.2.0rc3/src/zango/cli/start_project.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      688 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/cli/utils.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.461547 zango-0.2.0rc3/src/zango/config/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/config/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      552 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/config/celery.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.463682 zango-0.2.0rc3/src/zango/config/settings/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/config/settings/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5025 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/config/settings/base.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1045 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/config/urls_public.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      708 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/config/urls_tenants.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.542996 zango-0.2.0rc3/src/zango/core/
+-rw-r--r--   0 harshshah   (501) staff       (20)       39 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/__init__.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.683110 zango-0.2.0rc3/src/zango/core/api/
+-rw-r--r--   0 harshshah   (501) staff       (20)      211 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/api/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2104 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/api/base.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      846 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/api/utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1097 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/common_utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)      810 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/custom_pluginbase.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1033 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/core/decorators.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.760040 zango-0.2.0rc3/src/zango/core/generic_views/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/generic_views/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1538 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/core/generic_views/base.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5955 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/internal_requests.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1096 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/model_mixins.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     6345 2024-05-21 11:19:53.000000 zango-0.2.0rc3/src/zango/core/package_utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2576 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/permissions.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     2100 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/storage_utils.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1237 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/tasks.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1803 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/template_loader.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     3014 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/core/utils.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.764860 zango-0.2.0rc3/src/zango/middleware/
+-rw-r--r--   0 harshshah   (501) staff       (20)        0 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/middleware/__init__.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     1772 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/middleware/request.py
+-rw-r--r--   0 harshshah   (501) staff       (20)     5455 2024-05-15 11:27:55.000000 zango-0.2.0rc3/src/zango/middleware/tenant.py
+drwxr-xr-x   0 harshshah   (501) staff       (20)        0 2024-05-21 13:14:55.767004 zango-0.2.0rc3/src/zango.egg-info/
+-rw-r--r--   0 harshshah   (501) staff       (20)     5993 2024-05-21 13:14:47.000000 zango-0.2.0rc3/src/zango.egg-info/PKG-INFO
+-rw-r--r--   0 harshshah   (501) staff       (20)     9893 2024-05-21 13:14:47.000000 zango-0.2.0rc3/src/zango.egg-info/SOURCES.txt
+-rw-r--r--   0 harshshah   (501) staff       (20)        1 2024-05-21 13:14:47.000000 zango-0.2.0rc3/src/zango.egg-info/dependency_links.txt
+-rw-r--r--   0 harshshah   (501) staff       (20)       40 2024-05-21 13:14:47.000000 zango-0.2.0rc3/src/zango.egg-info/entry_points.txt
+-rw-r--r--   0 harshshah   (501) staff       (20)      728 2024-05-21 13:14:47.000000 zango-0.2.0rc3/src/zango.egg-info/requires.txt
+-rw-r--r--   0 harshshah   (501) staff       (20)        6 2024-05-21 13:14:47.000000 zango-0.2.0rc3/src/zango.egg-info/top_level.txt
```

### Comparing `zango-0.2.0rc2/LICENSE` & `zango-0.2.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/PKG-INFO` & `zango-0.2.0rc3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zango
-Version: 0.2.0rc2
+Version: 0.2.0rc3
 Summary: Zango: multi-tenant Django framework for building business apps
 Home-page: https://github.com/Healthlane-Technologies/zelthy3
 Author: Zelthy ("Healthlane Technologies")
 Author-email: maintainers@zelthy.com
 License: Apache License 2.0
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zango Version: 0.2.0rc2 Summary: Zango: multi-
+Metadata-Version: 2.1 Name: zango Version: 0.2.0rc3 Summary: Zango: multi-
 tenant Django framework for building business apps Home-page: https://
 github.com/Healthlane-Technologies/zelthy3 Author: Zelthy ("Healthlane
 Technologies") Author-email: maintainers@zelthy.com License: Apache License 2.0
 Classifier: Framework :: Django Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 django==4.2.11 Requires-Dist: psycopg2-binary Requires-Dist: django-tenants
 Requires-Dist: djangorestframework Requires-Dist: django-rest-knox Requires-
```

### Comparing `zango-0.2.0rc2/README.md` & `zango-0.2.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/setup.py` & `zango-0.2.0rc3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 PROJECT_DIR = os.path.dirname(__file__)
 REQUIREMENTS_DIR = os.path.join(PROJECT_DIR, "requirements")
 
 README = os.path.join(PROJECT_DIR, "README.md")
 
-PLATFORM_VERSION = "0.2.0-rc2"
+PLATFORM_VERSION = "0.2.0-rc3"
 
 
 def get_requirements(env):
     with open(os.path.join(REQUIREMENTS_DIR, f"{env}.txt")) as fp:
         return [x.strip() for x in fp.read().split("\n") if not x.startswith("#")]
```

### Comparing `zango-0.2.0rc2/src/zango/api/app_auth/profile/v1/utils.py` & `zango-0.2.0rc3/src/zango/api/app_auth/profile/v1/utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/app_auth/profile/v1/views.py` & `zango-0.2.0rc3/src/zango/api/app_auth/profile/v1/views.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/auditlogs/v1/serializers.py` & `zango-0.2.0rc3/src/zango/api/platform/auditlogs/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/auditlogs/v1/views.py` & `zango-0.2.0rc3/src/zango/api/platform/auditlogs/v1/views.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/auth/v1/serializers.py` & `zango-0.2.0rc3/src/zango/api/platform/auth/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/auth/v1/urls.py` & `zango-0.2.0rc3/src/zango/api/platform/auth/v1/urls.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/auth/v1/views.py` & `zango-0.2.0rc3/src/zango/api/platform/auth/v1/views.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/codeassist/v1/views.py` & `zango-0.2.0rc3/src/zango/api/platform/codeassist/v1/views.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/packages/v1/views.py` & `zango-0.2.0rc3/src/zango/api/platform/packages/v1/views.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/permissions/v1/serializers.py` & `zango-0.2.0rc3/src/zango/api/platform/permissions/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/permissions/v1/urls.py` & `zango-0.2.0rc3/src/zango/api/platform/permissions/v1/urls.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/permissions/v1/views.py` & `zango-0.2.0rc3/src/zango/api/platform/permissions/v1/views.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/tasks/v1/serializers.py` & `zango-0.2.0rc3/src/zango/api/platform/tasks/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/tasks/v1/views.py` & `zango-0.2.0rc3/src/zango/api/platform/tasks/v1/views.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/tenancy/v1/serializers.py` & `zango-0.2.0rc3/src/zango/api/platform/tenancy/v1/serializers.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/tenancy/v1/urls.py` & `zango-0.2.0rc3/src/zango/api/platform/tenancy/v1/urls.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/api/platform/tenancy/v1/views.py` & `zango-0.2.0rc3/src/zango/api/platform/tenancy/v1/views.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/appauth/auth_backend.py` & `zango-0.2.0rc3/src/zango/apps/appauth/auth_backend.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/appauth/migrations/0001_initial.py` & `zango-0.2.0rc3/src/zango/apps/appauth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/appauth/migrations/0002_default_user_roles.py` & `zango-0.2.0rc3/src/zango/apps/appauth/migrations/0002_default_user_roles.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py` & `zango-0.2.0rc3/src/zango/apps/appauth/migrations/0003_remove_userrolemodel_temp_field_appusermodel_mobile_and_more.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/appauth/migrations/0004_oldpasswords.py` & `zango-0.2.0rc3/src/zango/apps/appauth/migrations/0004_oldpasswords.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/appauth/models.py` & `zango-0.2.0rc3/src/zango/apps/appauth/models.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/appauth/templates/app.html` & `zango-0.2.0rc3/src/zango/apps/appauth/templates/app.html`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/appauth/templates/app_login_signup.html` & `zango-0.2.0rc3/src/zango/apps/appauth/templates/app_login_signup.html`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/appauth/views.py` & `zango-0.2.0rc3/src/zango/apps/appauth/views.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/admin.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/admin.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/cid.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/cid.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/conf.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/conf.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/context.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/context.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/diff.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/diff.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/filters.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/filters.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/management/commands/auditlogflush.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/management/commands/auditlogflush.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/management/commands/auditlogmigratejson.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/management/commands/auditlogmigratejson.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/middleware.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/middleware.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/migrations/0001_initial.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/mixins.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/mixins.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/models.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/models.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/receivers.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/receivers.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/registry.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/registry.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/auditlogs/signals.py` & `zango-0.2.0rc3/src/zango/apps/auditlogs/signals.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/dynamic_models/apps.py` & `zango-0.2.0rc3/src/zango/apps/dynamic_models/apps.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/dynamic_models/fields/__init__.py` & `zango-0.2.0rc3/src/zango/apps/dynamic_models/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/dynamic_models/models.py` & `zango-0.2.0rc3/src/zango/apps/dynamic_models/models.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/dynamic_models/permissions.py` & `zango-0.2.0rc3/src/zango/apps/dynamic_models/permissions.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/dynamic_models/signals.py` & `zango-0.2.0rc3/src/zango/apps/dynamic_models/signals.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/dynamic_models/templates/default_landing.html` & `zango-0.2.0rc3/src/zango/apps/dynamic_models/templates/default_landing.html`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/dynamic_models/views.py` & `zango-0.2.0rc3/src/zango/apps/dynamic_models/views.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/dynamic_models/workspace/base.py` & `zango-0.2.0rc3/src/zango/apps/dynamic_models/workspace/base.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/dynamic_models/workspace/wtree.py` & `zango-0.2.0rc3/src/zango/apps/dynamic_models/workspace/wtree.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/object_store/migrations/0001_initial.py` & `zango-0.2.0rc3/src/zango/apps/object_store/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/object_store/models.py` & `zango-0.2.0rc3/src/zango/apps/object_store/models.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/permissions/migrations/0001_initial.py` & `zango-0.2.0rc3/src/zango/apps/permissions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py` & `zango-0.2.0rc3/src/zango/apps/permissions/migrations/0002_policymodel_type_alter_policymodel_expiry.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/permissions/migrations/0003_default_policy.py` & `zango-0.2.0rc3/src/zango/apps/permissions/migrations/0003_default_policy.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py` & `zango-0.2.0rc3/src/zango/apps/permissions/migrations/0004_policymodel_path_alter_policymodel_name_and_more.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/permissions/mixin.py` & `zango-0.2.0rc3/src/zango/apps/permissions/mixin.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/permissions/models.py` & `zango-0.2.0rc3/src/zango/apps/permissions/models.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/platformauth/abstract_model.py` & `zango-0.2.0rc3/src/zango/apps/shared/platformauth/abstract_model.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/platformauth/auth_backend.py` & `zango-0.2.0rc3/src/zango/apps/shared/platformauth/auth_backend.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/platformauth/migrations/0001_initial.py` & `zango-0.2.0rc3/src/zango/apps/shared/platformauth/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py` & `zango-0.2.0rc3/src/zango/apps/shared/platformauth/migrations/0002_platformusermodel_is_superadmin_and_more.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/platformauth/models.py` & `zango-0.2.0rc3/src/zango/apps/shared/platformauth/models.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/platformauth/templates/app_panel/app_panel_login.html` & `zango-0.2.0rc3/src/zango/apps/shared/platformauth/templates/app_panel/app_panel_login.html`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/platformauth/views.py` & `zango-0.2.0rc3/src/zango/apps/shared/platformauth/views.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/tenancy/management/commands/sync_static.py` & `zango-0.2.0rc3/src/zango/apps/shared/tenancy/management/commands/sync_static.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/tenancy/management/commands/ws_makemigration.py` & `zango-0.2.0rc3/src/zango/apps/shared/tenancy/management/commands/ws_makemigration.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/tenancy/management/commands/ws_migrate.py` & `zango-0.2.0rc3/src/zango/apps/shared/tenancy/management/commands/ws_migrate.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/tenancy/migrations/0001_initial.py` & `zango-0.2.0rc3/src/zango/apps/shared/tenancy/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py` & `zango-0.2.0rc3/src/zango/apps/shared/tenancy/migrations/0003_themesmodel_created_at_themesmodel_created_by_and_more.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py` & `zango-0.2.0rc3/src/zango/apps/shared/tenancy/migrations/0004_tenantmodel_fav_icon_alter_tenantmodel_logo.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/tenancy/models.py` & `zango-0.2.0rc3/src/zango/apps/shared/tenancy/models.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/tenancy/tasks.py` & `zango-0.2.0rc3/src/zango/apps/shared/tenancy/tasks.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/tenancy/templates/app_panel.html` & `zango-0.2.0rc3/src/zango/apps/shared/tenancy/templates/app_panel.html`

 * *Files 19% similar despite different names*

```diff
@@ -14,13 +14,13 @@
 <body>
   <noscript>You need to enable JavaScript to run this app.</noscript>
   <div id="root"></div>
   <script>
     var csrf_token = "{{ csrf_token }}";
     var platform_version = "{{ platform_version }}";
   </script>
-  <script src="{% static 'app_panel/js/build.v1.1.1.min.js' %}"></script>
+  <script src="{% static 'app_panel/js/build.v1.1.2.min.js' %}"></script>
   <script src="{% static 'js/jquery/3.7.1/jquery.min.js' %}"></script>
   {% include 'session_security/all.html' %}
 </body>
 
 </html>
```

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/tenancy/templatetags/zstatic.py` & `zango-0.2.0rc3/src/zango/apps/shared/tenancy/templatetags/zstatic.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/shared/tenancy/utils.py` & `zango-0.2.0rc3/src/zango/apps/shared/tenancy/utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/tasks/migrations/0001_initial.py` & `zango-0.2.0rc3/src/zango/apps/tasks/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/tasks/models.py` & `zango-0.2.0rc3/src/zango/apps/tasks/models.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/apps/tasks/utils.py` & `zango-0.2.0rc3/src/zango/apps/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/assets/app_landing/css/styles.css` & `zango-0.2.0rc3/src/zango/assets/app_landing/css/styles.css`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/assets/app_panel/css/styles.css` & `zango-0.2.0rc3/src/zango/assets/app_panel/css/styles.css`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/assets/app_panel/images/zangoLogo.svg` & `zango-0.2.0rc3/src/zango/assets/app_panel/images/zangoLogo.svg`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/assets/app_panel/js/build.v1.1.1.min.js` & `zango-0.2.0rc3/src/zango/assets/app_panel/js/build.v1.1.2.min.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
-/*! For license information please see build.v1.1.1.min.js.LICENSE.txt */
+/*! For license information please see build.v1.1.2.min.js.LICENSE.txt */
 (() => {
     var __webpack_modules__ = {
-            900: (module, exports, __webpack_require__) => {
+            296: (module, exports, __webpack_require__) => {
                 module = __webpack_require__.nmd(module), (() => {
                     var __webpack_modules__ = {
                             54371: (e, t, a) => {
                                 "use strict";
                                 var n = Object.assign || function(e) {
                                         for (var t = 1; t < arguments.length; t++) {
                                             var a, n = arguments[t];
@@ -120972,34 +120972,34 @@
                                     })]
                                 }), (0, ge.jsx)("main", {
                                     className: "small-device-height-fix flex grow overflow-y-auto",
                                     children: e
                                 }), (0, ge.jsxs)("footer", {
                                     ref: n,
                                     className: "flex items-center justify-center gap-[8px] border-t-[1px] border-[#DDE2E5] p-[8px]",
-                                    children: [(0, ge.jsx)("span", {
+                                    children: [(0, ge.jsxs)("span", {
                                         className: "font-lato text-[11px] leading-[16px] text-[#495057]",
-                                        children: "V 3.0"
+                                        children: ["V ", "undefined" !== platform_version ? platform_version : ""]
                                     }), (0, ge.jsx)("span", {
                                         className: "font-lato text-[12px] font-bold leading-[16px] text-[#C7CED3]",
                                         children: "•"
                                     }), (0, ge.jsxs)("span", {
                                         className: "font-lato text-[11px] leading-[16px] text-[#495057]",
                                         children: ["© ", (new Date).getFullYear(), " HEALTHLANE TECHNOLOGIES PVT. LTD"]
                                     }), (0, ge.jsx)("span", {
                                         className: "font-lato text-[12px] font-bold leading-[16px] text-[#C7CED3]",
                                         children: "•"
                                     }), (0, ge.jsx)("a", {
-                                        href: "https://docs.zelthy.com/",
+                                        href: "https://www.zango.dev/docs/",
                                         alt: "#",
                                         target: "_blank",
                                         className: "m-0 inline-flex p-0",
                                         children: (0, ge.jsx)("span", {
                                             className: "font-lato text-[11px] leading-[16px] text-[#495057]",
-                                            children: "Documents"
+                                            children: "Docs"
                                         })
                                     })]
                                 })]
                             })
                         }
 
                         function TP() {
@@ -126898,9 +126898,9 @@
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
     }(), __webpack_require__.o = (e, t) => Object.prototype.hasOwnProperty.call(e, t), __webpack_require__.nmd = e => (e.paths = [], e.children || (e.children = []), e), __webpack_require__.b = document.baseURI || self.location.href, __webpack_require__.nc = void 0, __webpack_require__(637);
-    var __webpack_exports__ = __webpack_require__(900)
+    var __webpack_exports__ = __webpack_require__(296)
 })();
```

### Comparing `zango-0.2.0rc2/src/zango/assets/js/jquery/3.7.1/jquery.min.js` & `zango-0.2.0rc3/src/zango/assets/js/jquery/3.7.1/jquery.min.js`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/cli/install_package.py` & `zango-0.2.0rc3/src/zango/cli/install_package.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/cli/package_info.py` & `zango-0.2.0rc3/src/zango/cli/package_info.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/cli/project_template/manage.py` & `zango-0.2.0rc3/src/zango/cli/project_template/manage.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/cli/project_template/project_name/settings.py` & `zango-0.2.0rc3/src/zango/cli/project_template/project_name/settings.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/cli/project_template/project_name/urls.py` & `zango-0.2.0rc3/src/zango/cli/project_template/project_name/urls.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/cli/start_project.py` & `zango-0.2.0rc3/src/zango/cli/start_project.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/cli/utils.py` & `zango-0.2.0rc3/src/zango/cli/utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/config/celery.py` & `zango-0.2.0rc3/src/zango/config/celery.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/config/settings/base.py` & `zango-0.2.0rc3/src/zango/config/settings/base.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/config/urls_public.py` & `zango-0.2.0rc3/src/zango/config/urls_public.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/config/urls_tenants.py` & `zango-0.2.0rc3/src/zango/config/urls_tenants.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/api/base.py` & `zango-0.2.0rc3/src/zango/core/api/base.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/api/utils.py` & `zango-0.2.0rc3/src/zango/core/api/utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/common_utils.py` & `zango-0.2.0rc3/src/zango/core/common_utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/custom_pluginbase.py` & `zango-0.2.0rc3/src/zango/core/custom_pluginbase.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/decorators.py` & `zango-0.2.0rc3/src/zango/core/decorators.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/generic_views/base.py` & `zango-0.2.0rc3/src/zango/core/generic_views/base.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/internal_requests.py` & `zango-0.2.0rc3/src/zango/core/internal_requests.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/model_mixins.py` & `zango-0.2.0rc3/src/zango/core/model_mixins.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/package_utils.py` & `zango-0.2.0rc3/src/zango/core/package_utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/permissions.py` & `zango-0.2.0rc3/src/zango/core/permissions.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/storage_utils.py` & `zango-0.2.0rc3/src/zango/core/storage_utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/tasks.py` & `zango-0.2.0rc3/src/zango/core/tasks.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/template_loader.py` & `zango-0.2.0rc3/src/zango/core/template_loader.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/core/utils.py` & `zango-0.2.0rc3/src/zango/core/utils.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/middleware/request.py` & `zango-0.2.0rc3/src/zango/middleware/request.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango/middleware/tenant.py` & `zango-0.2.0rc3/src/zango/middleware/tenant.py`

 * *Files identical despite different names*

### Comparing `zango-0.2.0rc2/src/zango.egg-info/PKG-INFO` & `zango-0.2.0rc3/src/zango.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zango
-Version: 0.2.0rc2
+Version: 0.2.0rc3
 Summary: Zango: multi-tenant Django framework for building business apps
 Home-page: https://github.com/Healthlane-Technologies/zelthy3
 Author: Zelthy ("Healthlane Technologies")
 Author-email: maintainers@zelthy.com
 License: Apache License 2.0
 Classifier: Framework :: Django
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: zango Version: 0.2.0rc2 Summary: Zango: multi-
+Metadata-Version: 2.1 Name: zango Version: 0.2.0rc3 Summary: Zango: multi-
 tenant Django framework for building business apps Home-page: https://
 github.com/Healthlane-Technologies/zelthy3 Author: Zelthy ("Healthlane
 Technologies") Author-email: maintainers@zelthy.com License: Apache License 2.0
 Classifier: Framework :: Django Classifier: Programming Language :: Python
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 django==4.2.11 Requires-Dist: psycopg2-binary Requires-Dist: django-tenants
 Requires-Dist: djangorestframework Requires-Dist: django-rest-knox Requires-
```

### Comparing `zango-0.2.0rc2/src/zango.egg-info/SOURCES.txt` & `zango-0.2.0rc3/src/zango.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -177,15 +177,15 @@
 src/zango/apps/tasks/models.py
 src/zango/apps/tasks/utils.py
 src/zango/apps/tasks/migrations/0001_initial.py
 src/zango/apps/tasks/migrations/__init__.py
 src/zango/assets/app_landing/css/styles.css
 src/zango/assets/app_panel/css/styles.css
 src/zango/assets/app_panel/images/zangoLogo.svg
-src/zango/assets/app_panel/js/build.v1.1.1.min.js
+src/zango/assets/app_panel/js/build.v1.1.2.min.js
 src/zango/assets/js/jquery/3.7.1/jquery.min.js
 src/zango/cli/__init__.py
 src/zango/cli/install_package.py
 src/zango/cli/package_info.py
 src/zango/cli/start_project.py
 src/zango/cli/utils.py
 src/zango/cli/project_template/manage.py
```

### Comparing `zango-0.2.0rc2/src/zango.egg-info/requires.txt` & `zango-0.2.0rc3/src/zango.egg-info/requires.txt`

 * *Files identical despite different names*

