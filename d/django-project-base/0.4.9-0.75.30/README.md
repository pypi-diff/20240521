# Comparing `tmp/django-project-base-0.4.9.tar.gz` & `tmp/django-project-base-0.75.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-project-base-0.4.9.tar", last modified: Fri Nov 17 14:52:23 2023, max compression
+gzip compressed data, was "django-project-base-0.75.30.tar", last modified: Tue May 21 06:04:06 2024, max compression
```

## Comparing `django-project-base-0.4.9.tar` & `django-project-base-0.75.30.tar`

### file list

```diff
@@ -1,219 +1,222 @@
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.973523 django-project-base-0.4.9/
--rw-rw-r--   0 jure      (1000) jure      (1000)      116 2021-10-28 06:34:59.000000 django-project-base-0.4.9/MANIFEST.in
--rw-rw-r--   0 jure      (1000) jure      (1000)     1585 2023-11-17 14:52:23.973523 django-project-base-0.4.9/PKG-INFO
--rw-rw-r--   0 jure      (1000) jure      (1000)     1006 2023-10-16 12:26:59.000000 django-project-base-0.4.9/README.md
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.949523 django-project-base-0.4.9/django_project_base/
--rw-rw-r--   0 jure      (1000) jure      (1000)      307 2023-11-17 14:52:10.000000 django-project-base-0.4.9/django_project_base/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.949523 django-project-base-0.4.9/django_project_base/account/
--rw-rw-r--   0 jure      (1000) jure      (1000)      161 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/account/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      420 2021-12-10 13:37:27.000000 django-project-base-0.4.9/django_project_base/account/apps.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      182 2023-07-18 11:29:41.000000 django-project-base-0.4.9/django_project_base/account/constants.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.949523 django-project-base-0.4.9/django_project_base/account/management/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.4.9/django_project_base/account/management/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.953523 django-project-base-0.4.9/django_project_base/account/management/commands/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.4.9/django_project_base/account/management/commands/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1832 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/account/management/commands/allauth_to_social_core.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      663 2023-06-20 12:42:50.000000 django-project-base-0.4.9/django_project_base/account/management/commands/delete_users.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3601 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/account/middleware.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.953523 django-project-base-0.4.9/django_project_base/account/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-08-05 09:26:32.000000 django-project-base-0.4.9/django_project_base/account/rest/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    13141 2023-10-26 13:44:43.000000 django-project-base-0.4.9/django_project_base/account/rest/account.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     4541 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/account/rest/impersonate.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     6838 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/account/rest/invite.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5682 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/account/rest/login.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    26708 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/account/rest/profile.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5932 2023-11-16 12:12:19.000000 django-project-base-0.4.9/django_project_base/account/rest/profile_merge.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    11354 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/account/rest/project_profiles.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     6741 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/account/rest/project_profiles_utils.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     6528 2023-08-02 10:50:11.000000 django-project-base-0.4.9/django_project_base/account/rest/reset_password.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2293 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/account/router.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.953523 django-project-base-0.4.9/django_project_base/account/service/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:41.000000 django-project-base-0.4.9/django_project_base/account/service/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5837 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/account/service/merge_users_service.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1392 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/account/service/register_user_service.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2432 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/account/service/reset_password_email_service.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      216 2021-06-29 12:16:02.000000 django-project-base-0.4.9/django_project_base/account/settings.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.953523 django-project-base-0.4.9/django_project_base/account/social_auth/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.4.9/django_project_base/account/social_auth/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1580 2023-03-29 13:29:13.000000 django-project-base-0.4.9/django_project_base/account/social_auth/providers.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2244 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/account/social_auth/settings.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      226 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/account/urls.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      355 2023-07-18 11:29:41.000000 django-project-base-0.4.9/django_project_base/apps.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.953523 django-project-base-0.4.9/django_project_base/auth/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:44.000000 django-project-base-0.4.9/django_project_base/auth/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       77 2023-07-18 12:51:25.000000 django-project-base-0.4.9/django_project_base/auth/admin.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      160 2023-07-18 11:29:44.000000 django-project-base-0.4.9/django_project_base/auth/apps.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.953523 django-project-base-0.4.9/django_project_base/auth/migrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:44.000000 django-project-base-0.4.9/django_project_base/auth/migrations/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      737 2023-08-18 11:58:37.000000 django-project-base-0.4.9/django_project_base/auth/models.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       74 2023-07-18 12:51:25.000000 django-project-base-0.4.9/django_project_base/auth/tests.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       77 2023-07-18 12:51:25.000000 django-project-base-0.4.9/django_project_base/auth/views.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.957523 django-project-base-0.4.9/django_project_base/aws/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-26 14:22:46.000000 django-project-base-0.4.9/django_project_base/aws/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1726 2023-10-17 13:39:09.000000 django-project-base-0.4.9/django_project_base/aws/ses.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.957523 django-project-base-0.4.9/django_project_base/base/
--rw-rw-r--   0 jure      (1000) jure      (1000)       42 2021-06-29 12:16:02.000000 django-project-base-0.4.9/django_project_base/base/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1814 2023-06-16 10:27:37.000000 django-project-base-0.4.9/django_project_base/base/auth_backends.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     9024 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/base/event.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      304 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/base/exceptions.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1794 2023-11-16 12:12:19.000000 django-project-base-0.4.9/django_project_base/base/fields.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1730 2023-09-29 09:40:18.000000 django-project-base-0.4.9/django_project_base/base/middleware.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    12876 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/base/models.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      481 2023-09-04 09:23:53.000000 django-project-base-0.4.9/django_project_base/base/permissions.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1990 2023-07-18 11:29:41.000000 django-project-base-0.4.9/django_project_base/base/queryset_with_cache.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      494 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/base/signals.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.957523 django-project-base-0.4.9/django_project_base/celery/
--rw-rw-r--   0 jure      (1000) jure      (1000)       85 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/celery/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      187 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/celery/apps.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.957523 django-project-base-0.4.9/django_project_base/celery/background_tasks/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/celery/background_tasks/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1619 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/celery/background_tasks/notification_tasks.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2097 2023-08-28 11:05:17.000000 django-project-base-0.4.9/django_project_base/celery/celery.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      327 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/celery/settings.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      447 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/constants.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1335 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/country_holidays.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.957523 django-project-base-0.4.9/django_project_base/licensing/
--rw-rw-r--   0 jure      (1000) jure      (1000)       98 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/licensing/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      190 2023-08-20 09:37:15.000000 django-project-base-0.4.9/django_project_base/licensing/apps.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     4327 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/licensing/logic.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.957523 django-project-base-0.4.9/django_project_base/licensing/migrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)     1767 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/licensing/migrations/0001_initial.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2065 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      550 2023-09-04 09:23:53.000000 django-project-base-0.4.9/django_project_base/licensing/migrations/0005_auto_20230901_0613.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-20 09:37:15.000000 django-project-base-0.4.9/django_project_base/licensing/migrations/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      940 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/licensing/models.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.961523 django-project-base-0.4.9/django_project_base/licensing/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/licensing/rest/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      944 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/licensing/rest/rest.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      243 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/licensing/rest/router.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      175 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/licensing/urls.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.945523 django-project-base-0.4.9/django_project_base/locale/
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.945523 django-project-base-0.4.9/django_project_base/locale/en/
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.961523 django-project-base-0.4.9/django_project_base/locale/en/LC_MESSAGES/
--rw-rw-r--   0 jure      (1000) jure      (1000)      380 2023-08-04 14:40:02.000000 django-project-base-0.4.9/django_project_base/locale/en/LC_MESSAGES/django.mo
--rw-rw-r--   0 jure      (1000) jure      (1000)     7468 2023-08-11 11:07:25.000000 django-project-base-0.4.9/django_project_base/locale/en/LC_MESSAGES/django.po
--rw-rw-r--   0 jure      (1000) jure      (1000)       84 2023-08-04 14:40:02.000000 django-project-base-0.4.9/django_project_base/locale/en/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 jure      (1000) jure      (1000)     4562 2023-08-04 14:39:40.000000 django-project-base-0.4.9/django_project_base/locale/en/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.945523 django-project-base-0.4.9/django_project_base/locale/sl/
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.961523 django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/
--rw-rw-r--   0 jure      (1000) jure      (1000)     4385 2023-08-04 14:40:02.000000 django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/django.mo
--rw-rw-r--   0 jure      (1000) jure      (1000)     8756 2023-08-11 11:07:25.000000 django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/django.po
--rw-rw-r--   0 jure      (1000) jure      (1000)     3731 2023-08-04 14:40:02.000000 django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo
--rw-rw-r--   0 jure      (1000) jure      (1000)     6150 2023-08-04 14:39:32.000000 django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/djangojs.po
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.961523 django-project-base-0.4.9/django_project_base/management/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/management/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.961523 django-project-base-0.4.9/django_project_base/management/commands/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/management/commands/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1790 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/management/commands/confirm_setting.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1657 2023-10-17 07:56:43.000000 django-project-base-0.4.9/django_project_base/management/commands/list_pending_settings.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-20 09:46:16.000000 django-project-base-0.4.9/django_project_base/models.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.961523 django-project-base-0.4.9/django_project_base/notifications/
--rw-rw-r--   0 jure      (1000) jure      (1000)      162 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/notifications/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      449 2021-09-30 06:36:03.000000 django-project-base-0.4.9/django_project_base/notifications/apps.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.965523 django-project-base-0.4.9/django_project_base/notifications/base/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/notifications/base/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.965523 django-project-base-0.4.9/django_project_base/notifications/base/channels/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    10772 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/channel.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.965523 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3550 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/aws_ses.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3070 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2815 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/nexmo_sms.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2914 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/provider_integration.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    10461 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/t2.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1759 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/mail_channel.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1034 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/sms_channel.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/notifications/base/channels/websocket_channel.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1613 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/notifications/base/duplicate_notification_mixin.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1417 2023-09-20 12:31:19.000000 django-project-base-0.4.9/django_project_base/notifications/base/enums.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    11382 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1687 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/phone_number_parser.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1407 2023-08-02 06:59:12.000000 django-project-base-0.4.9/django_project_base/notifications/base/queable_notification_mixin.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5936 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/base/send_notification_mixin.py
--rw-rw-r--   0 jure      (1000) jure      (1000)       59 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/notifications/constants.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5799 2023-10-17 07:56:43.000000 django-project-base-0.4.9/django_project_base/notifications/email_notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      974 2023-08-18 11:58:37.000000 django-project-base-0.4.9/django_project_base/notifications/maintenance_notification.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.965523 django-project-base-0.4.9/django_project_base/notifications/management/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/notifications/management/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.965523 django-project-base-0.4.9/django_project_base/notifications/management/commands/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/notifications/management/commands/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      889 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/notifications/management/commands/resend_notification.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/notifications/migrations/
--rw-rw-r--   0 jure      (1000) jure      (1000)     6404 2023-08-30 15:18:55.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0001_initial.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1086 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      413 2023-09-04 09:23:53.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      393 2023-09-04 09:23:53.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options_and_more.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      412 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2533 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1501 2023-09-20 12:31:19.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0005_merge_20230906_1213.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1458 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1056 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0007_auto_20231026_0555.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      448 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0008_deliveryreport_auxiliary_notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1410 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/0009_auto_20231108_0658.py
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/notifications/migrations/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     9480 2023-11-16 12:12:19.000000 django-project-base-0.4.9/django_project_base/notifications/models.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1200 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/notifications/notification_queryset.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/notifications/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/notifications/rest/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3172 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/notifications/rest/delivery_report.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     9089 2023-08-28 11:05:17.000000 django-project-base-0.4.9/django_project_base/notifications/rest/maintenance_notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    21913 2023-11-16 12:12:19.000000 django-project-base-0.4.9/django_project_base/notifications/rest/notification.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      988 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/notifications/rest/router.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      943 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/notifications/settings.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/notifications/templates/
--rw-rw-r--   0 jure      (1000) jure      (1000)      368 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/notifications/templates/account_created.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     4339 2023-09-21 07:55:00.000000 django-project-base-0.4.9/django_project_base/notifications/templates/notification.html
--rw-rw-r--   0 jure      (1000) jure      (1000)     2614 2023-09-21 07:55:00.000000 django-project-base-0.4.9/django_project_base/notifications/templates/notification_login.html
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/notifications/tests/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/notifications/tests/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/notifications/tests/api/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/notifications/tests/api/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2427 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/tests/api/test_create_mail.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2196 2023-08-28 11:05:17.000000 django-project-base-0.4.9/django_project_base/notifications/tests/api/test_list_mail.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      789 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/tests/api/test_remainig_license.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1485 2023-08-28 11:05:17.000000 django-project-base-0.4.9/django_project_base/notifications/tests/api/test_retrieve_mail.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3332 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/tests/notifications_transaction_test_case.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/notifications/tests/unit/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/notifications/tests/unit/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     2866 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/tests/unit/test_is_mail_sent.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      543 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      177 2023-08-02 05:31:11.000000 django-project-base-0.4.9/django_project_base/notifications/utils.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/permissions/
--rw-rw-r--   0 jure      (1000) jure      (1000)      450 2023-08-01 07:02:58.000000 django-project-base-0.4.9/django_project_base/permissions/__init__.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.969523 django-project-base-0.4.9/django_project_base/profiling/
--rw-rw-r--   0 jure      (1000) jure      (1000)       77 2021-06-29 12:16:02.000000 django-project-base-0.4.9/django_project_base/profiling/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     9788 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/profiling/middleware.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1040 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/profiling/performance_base_command.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3480 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/profiling/views.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.973523 django-project-base-0.4.9/django_project_base/rest/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-03-10 04:17:51.000000 django-project-base-0.4.9/django_project_base/rest/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)    18069 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/rest/project.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3999 2023-09-12 11:16:30.000000 django-project-base-0.4.9/django_project_base/rest/project_role.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     4094 2023-09-11 08:57:16.000000 django-project-base-0.4.9/django_project_base/router.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     3881 2023-11-14 06:52:55.000000 django-project-base-0.4.9/django_project_base/settings.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     1677 2023-11-17 14:51:19.000000 django-project-base-0.4.9/django_project_base/settings_parser.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.945523 django-project-base-0.4.9/django_project_base/static/
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.973523 django-project-base-0.4.9/django_project_base/static/browser-update/
--rw-rw-r--   0 jure      (1000) jure      (1000)      421 2023-07-14 12:32:29.000000 django-project-base-0.4.9/django_project_base/static/browser-update/browser-update.js
--rw-rw-r--   0 jure      (1000) jure      (1000)     9484 2023-07-14 12:32:29.000000 django-project-base-0.4.9/django_project_base/static/browser-update/update.min.js
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.945523 django-project-base-0.4.9/django_project_base/templates/
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.973523 django-project-base-0.4.9/django_project_base/templates/app-debug/
--rw-rw-r--   0 jure      (1000) jure      (1000)     2169 2021-05-19 11:48:39.000000 django-project-base-0.4.9/django_project_base/templates/app-debug/main.html
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.973523 django-project-base-0.4.9/django_project_base/templates/email/
--rw-rw-r--   0 jure      (1000) jure      (1000)      169 2023-06-20 12:45:01.000000 django-project-base-0.4.9/django_project_base/templates/email/base.html
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.973523 django-project-base-0.4.9/django_project_base/templatetags/
--rw-rw-r--   0 jure      (1000) jure      (1000)        0 2022-01-12 07:10:33.000000 django-project-base-0.4.9/django_project_base/templatetags/__init__.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      200 2022-01-12 07:10:33.000000 django-project-base-0.4.9/django_project_base/templatetags/dpb_tags.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      907 2023-10-19 07:08:41.000000 django-project-base-0.4.9/django_project_base/urls.py
--rw-rw-r--   0 jure      (1000) jure      (1000)     5636 2023-10-13 11:01:30.000000 django-project-base-0.4.9/django_project_base/utils.py
--rw-rw-r--   0 jure      (1000) jure      (1000)      912 2023-04-14 14:01:54.000000 django-project-base-0.4.9/django_project_base/views.py
-drwxrwxr-x   0 jure      (1000) jure      (1000)        0 2023-11-17 14:52:23.949523 django-project-base-0.4.9/django_project_base.egg-info/
--rw-rw-r--   0 jure      (1000) jure      (1000)     1585 2023-11-17 14:52:23.000000 django-project-base-0.4.9/django_project_base.egg-info/PKG-INFO
--rw-rw-r--   0 jure      (1000) jure      (1000)     8905 2023-11-17 14:52:23.000000 django-project-base-0.4.9/django_project_base.egg-info/SOURCES.txt
--rw-rw-r--   0 jure      (1000) jure      (1000)        1 2023-11-17 14:52:23.000000 django-project-base-0.4.9/django_project_base.egg-info/dependency_links.txt
--rw-rw-r--   0 jure      (1000) jure      (1000)      297 2023-11-17 14:52:23.000000 django-project-base-0.4.9/django_project_base.egg-info/requires.txt
--rw-rw-r--   0 jure      (1000) jure      (1000)       20 2023-11-17 14:52:23.000000 django-project-base-0.4.9/django_project_base.egg-info/top_level.txt
--rw-rw-r--   0 jure      (1000) jure      (1000)      302 2023-11-14 06:52:55.000000 django-project-base-0.4.9/requirements.txt
--rw-rw-r--   0 jure      (1000) jure      (1000)       38 2023-11-17 14:52:23.973523 django-project-base-0.4.9/setup.cfg
--rwxrwxr-x   0 jure      (1000) jure      (1000)     3354 2023-10-17 07:56:43.000000 django-project-base-0.4.9/setup.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      116 2021-10-28 06:34:59.000000 django-project-base-0.75.30/MANIFEST.in
+-rw-r--r--   0 jure      (1000) jure      (1000)     1567 2024-05-21 06:04:06.191960 django-project-base-0.75.30/PKG-INFO
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1006 2023-10-16 12:26:59.000000 django-project-base-0.75.30/README.md
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.031958 django-project-base-0.75.30/django_project_base/
+-rw-r--r--   0 jure      (1000) jure      (1000)      309 2024-05-21 06:03:51.000000 django-project-base-0.75.30/django_project_base/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.035958 django-project-base-0.75.30/django_project_base/account/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      168 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      420 2021-12-10 13:37:27.000000 django-project-base-0.75.30/django_project_base/account/apps.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      182 2023-07-18 11:29:41.000000 django-project-base-0.75.30/django_project_base/account/constants.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.035958 django-project-base-0.75.30/django_project_base/account/management/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.30/django_project_base/account/management/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.035958 django-project-base-0.75.30/django_project_base/account/management/commands/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.30/django_project_base/account/management/commands/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1834 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/management/commands/allauth_to_social_core.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      664 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/management/commands/delete_users.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3602 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/middleware.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.039959 django-project-base-0.75.30/django_project_base/account/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-08-05 09:26:32.000000 django-project-base-0.75.30/django_project_base/account/rest/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    13904 2024-05-07 13:32:24.000000 django-project-base-0.75.30/django_project_base/account/rest/account.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     5208 2024-04-02 07:52:10.000000 django-project-base-0.75.30/django_project_base/account/rest/impersonate.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6815 2024-05-07 10:48:42.000000 django-project-base-0.75.30/django_project_base/account/rest/invite.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     5766 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/rest/login.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    28708 2024-05-21 06:02:28.000000 django-project-base-0.75.30/django_project_base/account/rest/profile.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6048 2024-05-07 10:47:13.000000 django-project-base-0.75.30/django_project_base/account/rest/profile_merge.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    11582 2024-05-07 10:49:35.000000 django-project-base-0.75.30/django_project_base/account/rest/project_profiles.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6639 2024-05-16 16:41:58.000000 django-project-base-0.75.30/django_project_base/account/rest/project_profiles_utils.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6529 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/rest/reset_password.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2360 2024-03-20 13:38:09.000000 django-project-base-0.75.30/django_project_base/account/router.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.039959 django-project-base-0.75.30/django_project_base/account/service/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:41.000000 django-project-base-0.75.30/django_project_base/account/service/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     5836 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/service/merge_users_service.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1392 2023-10-13 11:01:30.000000 django-project-base-0.75.30/django_project_base/account/service/register_user_service.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2504 2024-04-15 14:09:15.000000 django-project-base-0.75.30/django_project_base/account/service/reset_password_email_service.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      216 2021-06-29 12:16:02.000000 django-project-base-0.75.30/django_project_base/account/settings.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.039959 django-project-base-0.75.30/django_project_base/account/social_auth/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-06-29 12:16:02.000000 django-project-base-0.75.30/django_project_base/account/social_auth/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1581 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/account/social_auth/providers.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2244 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/account/social_auth/settings.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      226 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/account/urls.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      355 2023-07-18 11:29:41.000000 django-project-base-0.75.30/django_project_base/apps.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.039959 django-project-base-0.75.30/django_project_base/auth/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:44.000000 django-project-base-0.75.30/django_project_base/auth/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)       77 2023-07-18 12:51:25.000000 django-project-base-0.75.30/django_project_base/auth/admin.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      160 2023-07-18 11:29:44.000000 django-project-base-0.75.30/django_project_base/auth/apps.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.039959 django-project-base-0.75.30/django_project_base/auth/migrations/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-07-18 11:29:44.000000 django-project-base-0.75.30/django_project_base/auth/migrations/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      738 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/auth/models.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)       74 2023-07-18 12:51:25.000000 django-project-base-0.75.30/django_project_base/auth/tests.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)       77 2023-07-18 12:51:25.000000 django-project-base-0.75.30/django_project_base/auth/views.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.039959 django-project-base-0.75.30/django_project_base/aws/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-26 14:22:46.000000 django-project-base-0.75.30/django_project_base/aws/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1769 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/aws/ses.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.043959 django-project-base-0.75.30/django_project_base/base/
+-rw-rw-r--   0 jure      (1000) jure      (1000)       48 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/base/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1815 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/base/auth_backends.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     9026 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/base/event.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      304 2023-10-13 11:01:30.000000 django-project-base-0.75.30/django_project_base/base/exceptions.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2793 2024-02-15 14:26:52.000000 django-project-base-0.75.30/django_project_base/base/fields.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1731 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/base/middleware.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    12932 2024-02-15 08:50:47.000000 django-project-base-0.75.30/django_project_base/base/models.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3901 2024-02-20 16:52:39.000000 django-project-base-0.75.30/django_project_base/base/permissions.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1991 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/base/queryset_with_cache.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      494 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/base/signals.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.043959 django-project-base-0.75.30/django_project_base/celery/
+-rw-rw-r--   0 jure      (1000) jure      (1000)       85 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/celery/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      187 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/celery/apps.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.043959 django-project-base-0.75.30/django_project_base/celery/background_tasks/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/celery/background_tasks/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1743 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/celery/background_tasks/base_task.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1721 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/celery/background_tasks/notification_tasks.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2533 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/celery/celery.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      327 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/celery/settings.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      447 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/constants.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1336 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/country_holidays.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.043959 django-project-base-0.75.30/django_project_base/licensing/
+-rw-rw-r--   0 jure      (1000) jure      (1000)       98 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/licensing/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      190 2023-08-20 09:37:15.000000 django-project-base-0.75.30/django_project_base/licensing/apps.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4439 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/licensing/logic.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.043959 django-project-base-0.75.30/django_project_base/licensing/migrations/
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1767 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/licensing/migrations/0001_initial.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2065 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      550 2023-09-04 09:23:53.000000 django-project-base-0.75.30/django_project_base/licensing/migrations/0005_auto_20230901_0613.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-20 09:37:15.000000 django-project-base-0.75.30/django_project_base/licensing/migrations/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      940 2023-08-30 15:18:55.000000 django-project-base-0.75.30/django_project_base/licensing/models.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.043959 django-project-base-0.75.30/django_project_base/licensing/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-30 15:18:55.000000 django-project-base-0.75.30/django_project_base/licensing/rest/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      944 2023-10-13 11:01:30.000000 django-project-base-0.75.30/django_project_base/licensing/rest/rest.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      243 2023-08-30 15:18:55.000000 django-project-base-0.75.30/django_project_base/licensing/rest/router.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      175 2023-08-30 15:18:55.000000 django-project-base-0.75.30/django_project_base/licensing/urls.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.027958 django-project-base-0.75.30/django_project_base/locale/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.027958 django-project-base-0.75.30/django_project_base/locale/en/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.047959 django-project-base-0.75.30/django_project_base/locale/en/LC_MESSAGES/
+-rw-r--r--   0 jure      (1000) jure      (1000)      380 2024-02-27 08:45:40.000000 django-project-base-0.75.30/django_project_base/locale/en/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jure      (1000) jure      (1000)    13342 2024-02-27 08:06:33.000000 django-project-base-0.75.30/django_project_base/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 jure      (1000) jure      (1000)       84 2024-02-27 08:45:40.000000 django-project-base-0.75.30/django_project_base/locale/en/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4562 2023-08-04 14:39:40.000000 django-project-base-0.75.30/django_project_base/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.027958 django-project-base-0.75.30/django_project_base/locale/sl/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.047959 django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/
+-rw-r--r--   0 jure      (1000) jure      (1000)     6828 2024-02-27 08:45:40.000000 django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/django.mo
+-rw-rw-r--   0 jure      (1000) jure      (1000)    15563 2024-02-27 08:07:00.000000 django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/django.po
+-rw-r--r--   0 jure      (1000) jure      (1000)     3731 2024-02-27 08:45:40.000000 django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6150 2023-08-04 14:39:32.000000 django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.047959 django-project-base-0.75.30/django_project_base/management/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-10-13 11:01:30.000000 django-project-base-0.75.30/django_project_base/management/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.047959 django-project-base-0.75.30/django_project_base/management/commands/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-10-13 11:01:30.000000 django-project-base-0.75.30/django_project_base/management/commands/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1791 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/management/commands/confirm_setting.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1659 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/management/commands/list_pending_settings.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-20 09:46:16.000000 django-project-base-0.75.30/django_project_base/models.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.051959 django-project-base-0.75.30/django_project_base/notifications/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      162 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/notifications/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      449 2021-09-30 06:36:03.000000 django-project-base-0.75.30/django_project_base/notifications/apps.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.051959 django-project-base-0.75.30/django_project_base/notifications/base/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/notifications/base/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.067959 django-project-base-0.75.30/django_project_base/notifications/base/channels/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    11421 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/channel.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.067959 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     4694 2024-02-26 08:15:05.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/aws_ses.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2832 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2676 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/nexmo_sms.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2980 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/provider_integration.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    10301 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/t2.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2012 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/mail_channel.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1321 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/sms_channel.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/notifications/base/channels/websocket_channel.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1613 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/notifications/base/duplicate_notification_mixin.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1411 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/enums.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    12558 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/notification.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1581 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/phone_number_parser.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1407 2023-08-02 06:59:12.000000 django-project-base-0.75.30/django_project_base/notifications/base/queable_notification_mixin.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     5636 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/base/send_notification_service.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)       59 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/notifications/constants.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     5829 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/email_notification.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      975 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/notifications/maintenance_notification.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.067959 django-project-base-0.75.30/django_project_base/notifications/management/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-11 08:57:16.000000 django-project-base-0.75.30/django_project_base/notifications/management/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.067959 django-project-base-0.75.30/django_project_base/notifications/management/commands/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-09-11 08:57:16.000000 django-project-base-0.75.30/django_project_base/notifications/management/commands/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      900 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/management/commands/resend_notification.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.071959 django-project-base-0.75.30/django_project_base/notifications/migrations/
+-rw-rw-r--   0 jure      (1000) jure      (1000)     6404 2023-08-30 15:18:55.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0001_initial.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1086 2023-09-11 08:57:16.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      413 2023-09-04 09:23:53.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      393 2023-09-04 09:23:53.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0003_alter_djangoprojectbasemessage_options_and_more.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      412 2023-09-11 08:57:16.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2533 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1501 2023-09-20 12:31:19.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0005_merge_20230906_1213.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1458 2023-10-13 11:01:30.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1056 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0007_auto_20231026_0555.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      448 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0008_deliveryreport_auxiliary_notification.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1410 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0009_auto_20231108_0658.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      412 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/0010_djangoprojectbasenotification_extra_data.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/notifications/migrations/__init__.py
+-rw-r--r--   0 jure      (1000) jure      (1000)     9789 2024-05-04 07:03:08.000000 django-project-base-0.75.30/django_project_base/notifications/models.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1201 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/notifications/notification_queryset.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.183960 django-project-base-0.75.30/django_project_base/notifications/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/notifications/rest/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3173 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/notifications/rest/delivery_report.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     9090 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/notifications/rest/maintenance_notification.py
+-rw-r--r--   0 jure      (1000) jure      (1000)    23288 2024-05-16 17:09:01.000000 django-project-base-0.75.30/django_project_base/notifications/rest/notification.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      934 2024-02-05 15:07:30.000000 django-project-base-0.75.30/django_project_base/notifications/rest/router.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      943 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/notifications/settings.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.183960 django-project-base-0.75.30/django_project_base/notifications/templates/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      368 2023-09-11 08:57:16.000000 django-project-base-0.75.30/django_project_base/notifications/templates/account_created.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4339 2023-09-21 07:55:00.000000 django-project-base-0.75.30/django_project_base/notifications/templates/notification.html
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2614 2023-09-21 07:55:00.000000 django-project-base-0.75.30/django_project_base/notifications/templates/notification_login.html
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.183960 django-project-base-0.75.30/django_project_base/notifications/tests/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/notifications/tests/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.187960 django-project-base-0.75.30/django_project_base/notifications/tests/api/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/notifications/tests/api/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2427 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/notifications/tests/api/test_create_mail.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2196 2023-08-28 11:05:17.000000 django-project-base-0.75.30/django_project_base/notifications/tests/api/test_list_mail.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      864 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/tests/api/test_remainig_license.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1485 2023-08-28 11:05:17.000000 django-project-base-0.75.30/django_project_base/notifications/tests/api/test_retrieve_mail.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3332 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/notifications/tests/notifications_transaction_test_case.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.187960 django-project-base-0.75.30/django_project_base/notifications/tests/unit/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2023-08-01 07:02:58.000000 django-project-base-0.75.30/django_project_base/notifications/tests/unit/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2941 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/notifications/tests/unit/test_is_mail_sent.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      543 2023-11-14 06:52:55.000000 django-project-base-0.75.30/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      177 2023-08-02 05:31:11.000000 django-project-base-0.75.30/django_project_base/notifications/utils.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.187960 django-project-base-0.75.30/django_project_base/permissions/
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1082 2023-12-11 12:51:14.000000 django-project-base-0.75.30/django_project_base/permissions/__init__.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/django_project_base/profiling/
+-rw-rw-r--   0 jure      (1000) jure      (1000)       89 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/profiling/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     9791 2024-05-13 14:20:03.000000 django-project-base-0.75.30/django_project_base/profiling/middleware.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1040 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/profiling/performance_base_command.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     3481 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/profiling/views.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/django_project_base/rest/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2021-03-10 04:17:51.000000 django-project-base-0.75.30/django_project_base/rest/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)    18356 2024-05-07 10:45:40.000000 django-project-base-0.75.30/django_project_base/rest/project.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4000 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/rest/project_role.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4094 2023-09-11 08:57:16.000000 django-project-base-0.75.30/django_project_base/router.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     4017 2024-01-10 11:47:45.000000 django-project-base-0.75.30/django_project_base/settings.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1677 2023-11-17 14:51:19.000000 django-project-base-0.75.30/django_project_base/settings_parser.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.031958 django-project-base-0.75.30/django_project_base/static/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/django_project_base/static/browser-update/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      421 2023-07-14 12:32:29.000000 django-project-base-0.75.30/django_project_base/static/browser-update/browser-update.js
+-rw-rw-r--   0 jure      (1000) jure      (1000)     9484 2023-07-14 12:32:29.000000 django-project-base-0.75.30/django_project_base/static/browser-update/update.min.js
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.031958 django-project-base-0.75.30/django_project_base/templates/
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/django_project_base/templates/app-debug/
+-rw-rw-r--   0 jure      (1000) jure      (1000)     2169 2021-05-19 11:48:39.000000 django-project-base-0.75.30/django_project_base/templates/app-debug/main.html
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/django_project_base/templates/email/
+-rw-rw-r--   0 jure      (1000) jure      (1000)      169 2023-06-20 12:45:01.000000 django-project-base-0.75.30/django_project_base/templates/email/base.html
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.191960 django-project-base-0.75.30/django_project_base/templatetags/
+-rw-rw-r--   0 jure      (1000) jure      (1000)        0 2022-01-12 07:10:33.000000 django-project-base-0.75.30/django_project_base/templatetags/__init__.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      200 2022-01-12 07:10:33.000000 django-project-base-0.75.30/django_project_base/templatetags/dpb_tags.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      907 2023-10-19 07:08:41.000000 django-project-base-0.75.30/django_project_base/urls.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)     5824 2024-01-23 09:42:24.000000 django-project-base-0.75.30/django_project_base/utils.py
+-rw-rw-r--   0 jure      (1000) jure      (1000)      913 2023-12-14 13:42:26.000000 django-project-base-0.75.30/django_project_base/views.py
+drwxr-xr-x   0 jure      (1000) jure      (1000)        0 2024-05-21 06:04:06.035958 django-project-base-0.75.30/django_project_base.egg-info/
+-rw-r--r--   0 jure      (1000) jure      (1000)     1567 2024-05-21 06:04:05.000000 django-project-base-0.75.30/django_project_base.egg-info/PKG-INFO
+-rw-r--r--   0 jure      (1000) jure      (1000)     9073 2024-05-21 06:04:05.000000 django-project-base-0.75.30/django_project_base.egg-info/SOURCES.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)        1 2024-05-21 06:04:05.000000 django-project-base-0.75.30/django_project_base.egg-info/dependency_links.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)      308 2024-05-21 06:04:05.000000 django-project-base-0.75.30/django_project_base.egg-info/requires.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)       20 2024-05-21 06:04:05.000000 django-project-base-0.75.30/django_project_base.egg-info/top_level.txt
+-rw-rw-r--   0 jure      (1000) jure      (1000)     1305 2023-12-14 13:42:26.000000 django-project-base-0.75.30/pyproject.toml
+-rw-rw-r--   0 jure      (1000) jure      (1000)      311 2024-05-10 08:57:26.000000 django-project-base-0.75.30/requirements.txt
+-rw-r--r--   0 jure      (1000) jure      (1000)       38 2024-05-21 06:04:06.191960 django-project-base-0.75.30/setup.cfg
+-rwxrwxr-x   0 jure      (1000) jure      (1000)     3354 2023-10-17 07:56:43.000000 django-project-base-0.75.30/setup.py
```

### Comparing `django-project-base-0.4.9/PKG-INFO` & `django-project-base-0.75.30/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-project-base
-Version: 0.4.9
+Version: 0.75.30
 Summary: Everything revolves around it: users, roles, permissions, tags, etc.
 Home-page: https://github.com/velis74/django-project-base
 Author: Jure Erznožnik
 Author-email: jure@velis.si
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -53,9 +52,7 @@
 To generate pdf file. Run:
 
 ```bash 
 $ npm run export-pdf  
 ```
 
 Pdf file is located in docs/pdf folder.
-
-
```

### Comparing `django-project-base-0.4.9/README.md` & `django-project-base-0.75.30/README.md`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/account/management/commands/allauth_to_social_core.py` & `django-project-base-0.75.30/django_project_base/account/management/commands/allauth_to_social_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import json
+
 from typing import Optional
 
 import social_core.backends.facebook
 import social_core.backends.google
 import social_core.backends.microsoft
+
 from django.core.management.base import BaseCommand
 from django.db import connection
 from social_django.models import UserSocialAuth
 
 
 class Command(BaseCommand):
     help = "Migrate social login data from allauth to social_core"
```

### Comparing `django-project-base-0.4.9/django_project_base/account/management/commands/delete_users.py` & `django-project-base-0.75.30/django_project_base/account/management/commands/delete_users.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 import logging
 
 import swapper
+
 from django.core.management.base import BaseCommand
 from django.db import transaction
 
 
 class Command(BaseCommand):
     help = "Deletes users marked for deletion"
```

### Comparing `django-project-base-0.4.9/django_project_base/account/middleware.py` & `django-project-base-0.75.30/django_project_base/account/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 
 import swapper
+
 from django.conf import settings
 from django.contrib.sessions.middleware import SessionMiddleware as SessionMiddlewareBase
 from django.utils.functional import SimpleLazyObject
 from rest_framework.authentication import get_authorization_header
 
 
 class ProjectNotSelectedError(NotImplementedError):
```

### Comparing `django-project-base-0.4.9/django_project_base/account/rest/account.py` & `django-project-base-0.75.30/django_project_base/account/rest/account.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import re
+
 from typing import Optional
 
 import swapper
+
 from django.contrib.auth import get_user_model, login, update_session_auth_hash
 from django.contrib.auth.models import AnonymousUser
 from django.core.cache import cache
 from django.core.exceptions import ValidationError as DjangoValidationError
 from django.core.validators import validate_email
 from django.utils.translation import gettext_lazy as _
 from drf_spectacular.utils import extend_schema, extend_schema_view, OpenApiParameter, OpenApiResponse, OpenApiTypes
 from dynamicforms import fields as df_fields, serializers as df_serializers, viewsets as df_viewsets
 from dynamicforms.action import Actions
 from rest_framework import fields, serializers, status, viewsets
 from rest_framework.decorators import action
 from rest_framework.exceptions import PermissionDenied, ValidationError
-from rest_framework.permissions import IsAdminUser, IsAuthenticated
+from rest_framework.permissions import AllowAny, IsAdminUser, IsAuthenticated
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.serializers import ModelSerializer
 from rest_registration.api.views import change_password, logout, register
 from rest_registration.settings import registration_settings
 from social_django.models import UserSocialAuth
 
@@ -43,25 +45,32 @@
 class SocialAuthSerializer(ModelSerializer):
     class Meta:
         model = UserSocialAuth
         exclude = ("extra_data", "uid")
 
 
 class SocialAuthProvidersViewSet(viewsets.ViewSet):
+    def get_permissions(self):
+        if self.action == "social_auth_providers":
+            return []
+        elif self.action == "social_auth_providers_user":
+            return [IsAuthenticated()]
+        else:
+            return super().get_permissions()
+
     @extend_schema(
         responses={
             status.HTTP_200_OK: OpenApiResponse(description="OK"),
         }
     )
     @action(
         detail=False,
         methods=["get"],
         url_path="social-auth-providers",
         url_name="social-auth-providers",
-        permission_classes=[],
         authentication_classes=[],
     )
     def social_auth_providers(self, request: Request) -> Response:
         return Response(map(lambda item: item._asdict(), get_social_providers()))
 
     @extend_schema(
         responses={
@@ -69,43 +78,49 @@
         }
     )
     @action(
         detail=False,
         methods=["get"],
         url_path="social-auth-providers-user",
         url_name="social-auth-providers-user",
-        permission_classes=[IsAuthenticated],
     )
     def social_auth_providers_user(self, request: Request) -> Response:
         return Response(SocialAuthSerializer(UserSocialAuth.objects.filter(user=self.request.user), many=True).data)
 
 
 class LogoutSerializer(serializers.Serializer):
     revoke_token = fields.BooleanField(required=False)
 
 
 class LogoutViewSet(viewsets.ViewSet):
     serializer_class = LogoutSerializer
 
+    def get_permissions(self):
+        if self.action == "logout":
+            return [IsAuthenticated()]
+        else:
+            return super().get_permissions()
+
+    def initialize_request(self, request, *args, **kwargs):
+        request = super().initialize_request(request, *args, **kwargs)
+        request._dont_enforce_csrf_checks = True
+        return request
+
     @extend_schema(
         description="Logs out the user. Returns an error if the user is not authenticated. "
         "If revoke_token is provided, revokes the given token for a given user. If the token is not  "
         "provided, revoke all tokens for given user. ",
         responses={
             status.HTTP_200_OK: OpenApiResponse(description="OK"),
             status.HTTP_403_FORBIDDEN: OpenApiResponse(description="Not authorised"),
         },
     )
-    @action(
-        detail=False,
-        methods=["post"],
-        url_name="logout",
-        permission_classes=[IsAuthenticated],
-    )
+    @action(detail=False, methods=["post"], url_name="logout")
     def logout(self, request: Request) -> Response:
+        request._request._dont_enforce_csrf_checks = True
         return logout(request._request)
 
 
 class ChangePasswordSerializer(df_serializers.Serializer):
     template_context = dict(
         url_reverse="change-password",
         dialog_classes="modal-lg",
@@ -113,26 +128,27 @@
     )
     form_titles = {
         "table": "",
         "new": _("Change password"),
         "edit": "",
     }
 
-    old_password = df_fields.CharField(required=True, password_field=True)
-    password = df_fields.CharField(required=True, password_field=True)
-    password_confirm = df_fields.CharField(required=True, password_field=True)
+    old_password = df_fields.CharField(label=_("Current password"), required=True, password_field=True)
+    password = df_fields.CharField(label=_("New password"), required=True, password_field=True)
+    password_confirm = df_fields.CharField(label=_("Confirm new password"), required=True, password_field=True)
 
     actions = Actions(add_form_buttons=True)
 
 
 @extend_schema_view(
     retrieve=extend_schema(parameters=[OpenApiParameter("id", OpenApiTypes.STR, OpenApiParameter.PATH, enum=["new"])]),
 )
 class ChangePasswordViewSet(df_viewsets.SingleRecordViewSet):
     serializer_class = ChangePasswordSerializer
+    permission_classes = [AllowAny]
 
     def initialize_request(self, request, *args, **kwargs):
         request = super().initialize_request(request, *args, **kwargs)
         # We need to set following flag (which is used while testing), because otherwise CSRF middleware
         # (django/middleware/csrf.py -> process_view()) would execute request.POST, which would cause
         # "django.http.request.RawPostDataException: You cannot access body after reading from request's data stream"
         # when request will be initialized and authenticated later for rest_registration.api.views.change_password
@@ -181,28 +197,33 @@
         response = change_password(request._request)
         if response.status_code == status.HTTP_200_OK:
             handle_password_changed(request)
         return response
 
 
 class VerifyRegistrationViewSet(viewsets.ViewSet):
+    def get_permissions(self):
+        if self.action == "verify_registration":
+            return []
+        else:
+            return super().get_permissions()
+
     @extend_schema(
         description="Verify registration with signature. The endpoint will generate an e-mail with a confirmation URL "
         "which the user should GET to confirm the account.",
         responses={
             status.HTTP_200_OK: OpenApiResponse(description="OK", response=ResetPasswordSerializer),
             status.HTTP_400_BAD_REQUEST: OpenApiResponse(description="Bad request"),
         },
     )
     @action(
         detail=False,
         methods=["post"],
         url_path="verify-registration",
         url_name="verify-registration",
-        permission_classes=[],
     )
     def verify_registration(self, request: Request) -> Response:
         if (
             (flow_id := request.COOKIES.get("register-flow"))
             and (code := cache.get(flow_id))
             and (req_code := request.data.get("code"))
             and code == req_code
@@ -287,17 +308,15 @@
                        "The password is too similar to the username.",
                        "This password is too short. It must contain at least 8 characters."
                      ],
                      "password_confirm": [
                        "Passwords don't match"
                      ],
                      "non_field_errors": []
-                   }""".replace(
-                    "\n", " "
-                ),
+                   }""".replace("\n", " "),
             )
         ),
     },
 )
 class RegisterViewSet(viewsets.ViewSet):
     serializer_class = RegisterSerializer
```

### Comparing `django-project-base-0.4.9/django_project_base/account/rest/impersonate.py` & `django-project-base-0.75.30/django_project_base/account/rest/impersonate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,25 @@
+from typing import Any, Dict, Optional, Union
+
 from django.contrib.auth import get_user_model
-from django.db.models import Model
+from django.db.models import Model, Q
 from django.shortcuts import get_object_or_404
 from django.utils.translation import gettext_lazy as _
 from drf_spectacular.utils import (
     extend_schema,
     extend_schema_field,
     extend_schema_view,
     OpenApiParameter,
     OpenApiResponse,
     OpenApiTypes,
 )
 from dynamicforms import fields, serializers, viewsets
 from dynamicforms.action import Actions, FormButtonAction, FormButtonTypes
 from hijack.helpers import login_user, release_hijack
 from rest_framework import status
-from rest_framework.decorators import permission_classes
 from rest_framework.exceptions import PermissionDenied
 from rest_framework.permissions import IsAdminUser, IsAuthenticated
 from rest_framework.request import Request
 from rest_framework.response import Response
 
 import django_project_base.base.fields
 
@@ -31,26 +32,35 @@
     id = fields.IntegerField(required=False, label=_("User ID"))
     email = fields.EmailField(required=False, label=_("User email"))
     username = fields.CharField(required=False)
 
 
 @extend_schema_field(OpenApiTypes.NONE)
 class ImpersonateUserIdField(django_project_base.base.fields.UserRelatedField):
-    pass
+    def __init__(
+        self,
+        queryset_filter: Optional[Union[Q, Dict[str, Any]]] = None,
+        queryset_exclude: Optional[Union[Q, Dict[str, Any]]] = None,
+        **kwargs,
+    ):
+        kwargs.setdefault("placeholder", _("Select a user to impersonate"))
+        kwargs.setdefault("label", _("User"))
+        kwargs.setdefault("required", False)
+        kwargs.setdefault("allow_null", True)
+        super().__init__(queryset_filter, queryset_exclude, **kwargs)
+        self.filter_selected_project = False
 
 
 class ImpersonateUserDialogSerializer(serializers.Serializer):
     template_context = dict(
         url_reverse="profile-base-impersonate-user", url_reverse_kwargs=None, dialog_header_classes="bg-info"
     )
-    form_titles = {"new": "Impersonate a user"}
+    form_titles = {"new": _("Impersonate a user")}
 
-    id = ImpersonateUserIdField(
-        placeholder=_("Select a user to impersonate"), label=_("User"), required=False, allow_null=True
-    )
+    id = ImpersonateUserIdField()
 
     actions = Actions(
         FormButtonAction(btn_type=FormButtonTypes.CANCEL, name="cancel", label=_("Cancel")),
         FormButtonAction(btn_type=FormButtonTypes.SUBMIT, name="submit", label=_("Impersonate")),
         add_form_buttons=False,
     )
 
@@ -60,14 +70,29 @@
         description="Retrieves dialog definition for impersonation dialog",
         parameters=[OpenApiParameter("id", OpenApiTypes.STR, OpenApiParameter.PATH, enum=["new"])],
     ),
 )
 class ImpersonateUserViewset(viewsets.SingleRecordViewSet):
     serializer_class = ImpersonateUserDialogSerializer
 
+    def get_permissions(self):
+        if self.action == "destroy":
+            return [
+                IsAuthenticated(),
+            ]
+        elif self.action == "update":
+            return [
+                IsAdminUser(),
+            ]
+        elif self.action == "create":
+            return [
+                IsAdminUser(),
+            ]
+        return super().get_permissions()
+
     def new_object(self):
         return dict(id=None)
 
     # noinspection PyMethodMayBeStatic
     def __validate(self, req_data: dict) -> dict:
         ser: ImpersonateRequestSerializer = ImpersonateRequestSerializer(data=req_data)
         ser.is_valid(raise_exception=True)
@@ -79,21 +104,19 @@
     @extend_schema(
         responses={
             status.HTTP_200_OK: OpenApiResponse(description="OK"),
             status.HTTP_403_FORBIDDEN: OpenApiResponse(description="Forbidden"),
         },
         description="Logout as another user",
     )
-    @permission_classes([IsAuthenticated])
     def destroy(self, request: Request) -> Response:
         release_hijack(request)
         return Response()
 
     @extend_schema(exclude=True)
-    @permission_classes([IsAdminUser])
     def update(self, request: Request, *args, **kwargs) -> Response:
         self._hijack(request=request)
         return Response()
 
     def _hijack(self, request: Request):
         validated_data: dict = self.__validate(request.data)
         hijacked_user: Model = get_object_or_404(get_user_model(), **validated_data)
@@ -109,11 +132,10 @@
                 description="Forbidden. You do not have permission to perform this action or "
                 "Impersonating self is not allowed"
             ),
             status.HTTP_404_NOT_FOUND: OpenApiResponse(description="User matching provided data not found"),
         },
         description="Login as another user and work on behalf of other user without having to know their credentials",
     )
-    @permission_classes([IsAdminUser])
     def create(self, request: Request, *args, **kwargs) -> Response:
         self._hijack(request=request)
         return Response()
```

### Comparing `django-project-base-0.4.9/django_project_base/account/rest/invite.py` & `django-project-base-0.75.30/django_project_base/account/rest/invite.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import swapper
+
 from django.db import transaction
 from django.http import HttpResponse, HttpResponseRedirect
 from django.shortcuts import get_object_or_404
 from django.utils.translation import gettext_lazy as _
 from drf_spectacular.utils import extend_schema
 from dynamicforms import fields
 from dynamicforms.action import Actions, TableAction, TablePosition
 from dynamicforms.mixins import DisplayMode
 from dynamicforms.serializers import ModelSerializer
 from dynamicforms.viewsets import ModelViewSet
-from rest_framework.authentication import SessionAuthentication
 from rest_framework.decorators import action
 from rest_framework.permissions import IsAuthenticated
 from rest_framework.request import Request
 
 from django_project_base.account.middleware import ProjectNotSelectedError
 from django_project_base.base.event import UserInviteFoundEvent
 from django_project_base.base.exceptions import InviteActionNotImplementedException
@@ -88,14 +88,20 @@
 
 
 class ProjectUserInviteViewSet(ModelViewSet):
     # TODO: ADD INVITE SHOULD BE PERMISSION BASED ON ROLE
     permission_classes = (IsAuthenticated,)
     serializer_class = ProjectUserInviteSerializer
 
+    def get_permissions(self):
+        if self.action == "accept":
+            return [IsAuthenticated()]
+        else:
+            return super().get_permissions()
+
     def get_queryset(self):
         project = self.request.selected_project
         try:
             return swapper.load_model("django_project_base", "Invite").objects.filter(project=project)
         except ProjectNotSelectedError:
             return swapper.load_model("django_project_base", "ProjectMember").objects.none()
 
@@ -150,22 +156,15 @@
     def destroy(self, request, *args, **kwargs):
         raise InviteActionNotImplementedException
 
     def list(self, request, *args, **kwargs):
         return super().list(request, *args, **kwargs)
 
     @extend_schema(exclude=True)
-    @action(
-        methods=["GET"],
-        detail=True,
-        permission_classes=[],
-        authentication_classes=[SessionAuthentication],
-        url_name="accept",
-        url_path="accept",
-    )
+    @action(methods=["GET"], detail=True, url_name="accept", url_path="accept")
     def accept(self, request: Request, pk: str, *args, **kwargs) -> HttpResponse:
         invite = get_object_or_404(swapper.load_model("django_project_base", "Invite"), pk=pk)
         response = HttpResponseRedirect(get_host_url(request))
         if not invite.accepted:
             if request.user.is_authenticated:
                 UserInviteFoundEvent(request.user).trigger(payload=invite, request=request)
                 return response
```

### Comparing `django-project-base-0.4.9/django_project_base/account/rest/login.py` & `django-project-base-0.75.30/django_project_base/account/rest/login.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from django.utils.translation import gettext_lazy as _
 from drf_spectacular.utils import extend_schema, extend_schema_view, OpenApiResponse
 from dynamicforms import fields, serializers, viewsets
 from dynamicforms.action import Actions, FormButtonAction, FormButtonTypes
 from dynamicforms.mixins import DisplayMode
 from dynamicforms.template_render.layout import Layout, Row
 from rest_framework import status
+from rest_framework.permissions import AllowAny
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_registration.api.views import login
 
 from django_project_base.account.social_auth.providers import get_social_providers, SocialProviderItem
 from django_project_base.base.event import UserLoginEvent
 
@@ -72,14 +73,15 @@
             ),
             status.HTTP_403_FORBIDDEN: OpenApiResponse(description="Authentication credentials were not provided."),
         },
     ),
 )
 class LoginViewset(viewsets.SingleRecordViewSet):
     serializer_class = LoginSerializer
+    permission_classes = [AllowAny]
 
     def initialize_request(self, request, *args, **kwargs):
         # We need to lie to the CSRF middleware that CSRF processing is done, because otherwise CSRF middleware
         # (django/middleware/csrf.py -> process_view()) would execute request.POST, which would parse request data as
         # empty - because it is not encoded with form url encoding, but with JSON.
         #
         # As a result, DRF then doesn't get the JSON payload and can't process the request
```

### Comparing `django-project-base-0.4.9/django_project_base/account/rest/profile.py` & `django-project-base-0.75.30/django_project_base/account/rest/profile.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,50 @@
 import datetime
 import uuid
+
 from random import randrange
 
 import django
 import swapper
+
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.auth.models import Group, Permission
 from django.core.cache import cache
 from django.db import transaction
 from django.db.models import ForeignKey, Model, QuerySet
 from django.template.loader import render_to_string
 from django.utils import timezone
 from django.utils.crypto import get_random_string
+from django.utils.module_loading import import_string
 from django.utils.translation import gettext_lazy as _
 from drf_spectacular.utils import extend_schema, extend_schema_view, OpenApiParameter, OpenApiResponse
 from dynamicforms import fields
 from dynamicforms.action import TableAction, TablePosition
 from dynamicforms.mixins import DisplayMode
 from dynamicforms.serializers import ModelSerializer
 from dynamicforms.template_render.layout import Column, Layout, Row
 from dynamicforms.template_render.responsive_table_layout import ResponsiveTableLayout, ResponsiveTableLayouts
 from dynamicforms.viewsets import ModelViewSet
 from natural.date import compress
 from rest_framework import exceptions, filters, status
 from rest_framework.decorators import action
 from rest_framework.exceptions import APIException, ValidationError
 from rest_framework.fields import IntegerField
-from rest_framework.permissions import IsAdminUser, IsAuthenticated
+from rest_framework.permissions import IsAuthenticated
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.serializers import Serializer
 from rest_registration.exceptions import UserNotFound
 
 from django_project_base.account.constants import MERGE_USERS_QS_CK
 from django_project_base.account.middleware import ProjectNotSelectedError
 from django_project_base.account.rest.project_profiles_utils import get_project_members
 from django_project_base.base.event import UserRegisteredEvent
+from django_project_base.base.permissions import IsProjectOwner
 from django_project_base.constants import NOTIFY_NEW_USER_SETTING_NAME
 from django_project_base.notifications.email_notification import (
     EMailNotification,
     SystemEMailNotificationWithListOfEmails,
 )
 from django_project_base.notifications.models import DjangoProjectBaseMessage
 from django_project_base.permissions import BasePermissions
@@ -57,17 +61,24 @@
         return {
             get_pk_name(Permission): permission.pk,
             "codename": permission.codename,
             "name": permission.name,
         }
 
     def to_representation(self, value, row_data=None):
+        res = []
         if row_data and row_data.pk:
-            return [ProfilePermissionsField.to_dict(p) for p in row_data.user_permissions.all()]
-        return []
+            if implicit_permissions := getattr(settings, "DJANGO_PROJECT_BASE_IMPLICIT_PERMISSIONS_FUNCTION", None):
+                try:
+                    res.extend(import_string(implicit_permissions)(row_data, self.context["request"].selected_project))
+                except NotImplementedError:
+                    pass
+
+            res.extend([ProfilePermissionsField.to_dict(p) for p in row_data.user_permissions.all()])
+        return res
 
 
 class ProfileGroupsField(fields.ManyRelatedField):
     def to_representation(self, value, row_data=None):
         if row_data and row_data.pk:
             return [
                 {
@@ -102,15 +113,15 @@
     date_joined = fields.AutoGeneratedField(display=DisplayMode.HIDDEN)  # read_only=True,
     is_active = fields.AutoGeneratedField(display=DisplayMode.HIDDEN)  # read_only=True,
     is_superuser = fields.AutoGeneratedField(display=DisplayMode.HIDDEN)  # read_only=True,
     is_staff = fields.AutoGeneratedField(display=DisplayMode.HIDDEN)  # read_only=True,
     avatar = fields.AutoGeneratedField(display_table=DisplayMode.HIDDEN)
     reverse_full_name_order = fields.AutoGeneratedField(display_table=DisplayMode.HIDDEN)
 
-    full_name = fields.CharField(read_only=True, display_form=DisplayMode.HIDDEN)
+    full_name = fields.SerializerMethodField(label=_("Full name"), display_form=DisplayMode.HIDDEN)
     is_impersonated = fields.SerializerMethodField(display=DisplayMode.HIDDEN)
     password_invalid = fields.BooleanField(display_form=DisplayMode.HIDDEN, display_table=DisplayMode.HIDDEN)
 
     delete_at = fields.DateTimeField(read_only=True, display=DisplayMode.HIDDEN)
     permissions = ProfilePermissionsField(
         source="user_permissions",
         child_relation=fields.PrimaryKeyRelatedField(
@@ -182,14 +193,18 @@
                     label=_("Export"),
                     title=_("Export"),
                     name="export",
                     icon="download-outline",
                 )
             )
 
+    def get_full_name(self, obj):
+        # we have made it so that str(UserProfile) returns full_name, but possibly decorated with status (Klubis)
+        return str(obj)
+
     def get_is_impersonated(self, obj):
         try:
             request = self.context["request"]
             session = request.session
             return bool(session.get("hijack_history", [])) and obj.id == request.user.id
         except:
             pass
@@ -207,17 +222,19 @@
             Row("language"),
             Row("avatar"),
             columns=2,
             size="large",
         )
         responsive_columns = ResponsiveTableLayouts(
             auto_generate_single_row_layout=True,
+            auto_generate_single_column_layout=False,
             layouts=[
-                ResponsiveTableLayout(auto_add_non_listed_columns=True),
                 ResponsiveTableLayout("full_name", "email", "#actions-row_end", auto_add_non_listed_columns=False),
+                ResponsiveTableLayout("full_name", "#actions-row_end", auto_add_non_listed_columns=False),
+                ResponsiveTableLayout(["full_name", "#actions-row_end"], auto_add_non_listed_columns=False),
             ],
         )
 
 
 class ProfileRegisterSerializer(ProfileSerializer):
     password = fields.CharField(label=_("Password"), password_field=True)
     password_repeat = fields.CharField(label=_("Repeat Password"), password_field=True)
@@ -277,14 +294,28 @@
 )
 class ProfileViewSet(ModelViewSet):
     filter_backends = [filters.SearchFilter]
     search_fields = search_fields
     permission_classes = (ProfileViewPermissions,)
     pagination_class = ModelViewSet.generate_paged_loader(30, ["un_sort", "id"])
 
+    def get_permissions(self):
+        if self.action == "register_account":
+            return []
+        elif self.action == "get_current_profile":
+            return [IsAuthenticated()]
+        elif self.action == "merge_accounts":
+            return [IsAuthenticated()]
+        elif self.action == "merge":
+            return [IsAuthenticated(), IsProjectOwner()]
+        elif self.action == "reset_user_data":
+            return [IsAuthenticated()]
+        else:
+            return super().get_permissions()
+
     def get_queryset(self):
         return get_project_members(self.request)
 
     def get_serializer_class(self):
         if self.request.query_params.get("select", "") == "1":
 
             class SearchProfileSerializer(ProfileSerializer):
@@ -292,17 +323,31 @@
                     fields = search_fields + [get_pk_name(get_user_model()), "full_name"]
                     exclude = None
 
             return SearchProfileSerializer
 
         return ProfileSerializer
 
+    def filter_queryset(self, queryset, query_params=None):
+        if filter_func := getattr(settings, "DJANGO_PROJECT_BASE_FILTER_PROFILE_QUERYSET_FIELD_FUNCTION", None):
+            try:
+                queryset = import_string(filter_func)(self, queryset, None, query_params)
+            except NotImplementedError:
+                pass
+        return super().filter_queryset(queryset, query_params)
+
     def filter_queryset_field(self, queryset, field, value):
         if field == "full_name":
             return queryset.filter(un__icontains=value)
+        if filter_func := getattr(settings, "DJANGO_PROJECT_BASE_FILTER_PROFILE_QUERYSET_FIELD_FUNCTION", None):
+            try:
+                return import_string(filter_func)(self, queryset, field, value)
+            except NotImplementedError:
+                pass
+
         return super().filter_queryset_field(queryset, field, value)
 
     @extend_schema(
         parameters=[
             OpenApiParameter(
                 "search", description="Search users by all of those fields: username, email, first_name, last_name"
             )
@@ -325,15 +370,14 @@
         },
     )
     @action(
         methods=["GET"],
         detail=False,
         url_path="register",
         url_name="profile-register",
-        permission_classes=[],
     )
     def register_account(self, request: Request, **kwargs):
         register_flow_identifier = str(uuid.uuid4())
         response = Response(ProfileRegisterSerializer(None, context=self.get_serializer_context()).data)
         response.set_cookie(
             "register-flow",
             register_flow_identifier,
@@ -362,16 +406,15 @@
         # call serializer to do the data processing drf way - hijack
         serializer = ProfileRegisterSerializer(
             None, context=self.get_serializer_context(), data=request.data, many=False
         )
         serializer.is_valid(raise_exception=True)
 
         if get_user_model().objects.filter(email=serializer.validated_data["email"]).exists():
-            # TODO: https://taiga.velis.si/project/velis-django-project-admin/issue/711
-            raise ValidationError()
+            raise ValidationError({"email": _("User with this email already exists.")})
 
         user = serializer.save()
         user.set_password(request.data["password"])
         user.save()
         UserRegisteredEvent(user=user).trigger(payload=request)
         return Response(serializer.validated_data)
 
@@ -403,28 +446,33 @@
         },
     )
     @action(
         methods=["GET"],
         detail=False,
         url_path="current",
         url_name="profile-current",
-        permission_classes=[IsAuthenticated],
     )
     def get_current_profile(self, request: Request, **kwargs) -> Response:
         user: Model = request.user
         serializer = self.get_serializer(user)
         response_data: dict = serializer.data
-        if getattr(request, "GET", None) and request.GET.get("decorate", "") == "default-project":
-            try:
-                response_data["default_project"] = ProjectSerializer(request.selected_project).data
-            except ProjectNotSelectedError:
-                if project_object := ProjectViewSet._get_queryset_for_request(request).first():
-                    response_data["default_project"] = ProjectSerializer(project_object).data
-                else:
-                    response_data["default_project"] = None
+        cache_key = f"user-current-project-{user.pk}"
+        try:
+            response_data["default_project"] = ProjectSerializer(request.selected_project).data
+            cache.set(cache_key, request.selected_project.pk, timeout=None)
+        except ProjectNotSelectedError:
+            q = ProjectViewSet._get_queryset_for_request(request)
+            previously_selected_project_pk = cache.get(cache_key)
+            if project_object := q.filter(pk=previously_selected_project_pk).first():
+                response_data["default_project"] = ProjectSerializer(project_object).data
+            elif project_object := q.first():
+                response_data["default_project"] = ProjectSerializer(project_object).data
+            else:
+                response_data["default_project"] = None
+
         return Response(response_data)
 
     @extend_schema(
         description="Marks profile of calling user for deletion in future. Future date is determined " "by settings",
         responses={
             status.HTTP_200_OK: OpenApiResponse(description="OK"),
             status.HTTP_204_NO_CONTENT: OpenApiResponse(description="No content"),
@@ -512,21 +560,15 @@
     )
     def destroy(self, request, *args, **kwargs):
         if self.request.user.is_superuser or self.request.user.is_staff:
             return super().destroy(request, *args, **kwargs)
         raise exceptions.PermissionDenied
 
     @extend_schema(exclude=True)
-    @action(
-        methods=["POST"],
-        detail=False,
-        url_path="merge-accounts",
-        url_name="merge-accounts",
-        permission_classes=[IsAuthenticated],
-    )
+    @action(methods=["POST"], detail=False, url_path="merge-accounts", url_name="merge-accounts")
     def merge_accounts(self, request, *args, **kwargs):
         from rest_registration.settings import registration_settings
 
         serializer = registration_settings.LOGIN_SERIALIZER_CLASS(data=request.data)
         serializer.is_valid(raise_exception=True)
         auth_user = self.request.user
         auth_user_is_main = str(self.request.data.get("account", "false")) in fields.BooleanField.TRUE_VALUES
@@ -551,15 +593,14 @@
 
     @extend_schema(exclude=True)
     @action(
         methods=["POST"],
         detail=False,
         url_path="merge",
         url_name="merge",
-        permission_classes=[IsAuthenticated, IsAdminUser],
     )
     def merge(self, request: Request, **kwargs) -> Response:
         ser = MergeUserRequest(data=request.data)
         ser.is_valid(raise_exception=True)
         ck = MERGE_USERS_QS_CK % self.request.user.pk
         ck_val = cache.get(ck, [])
         ck_val.append(ser.validated_data["user"])
@@ -568,15 +609,14 @@
 
     @extend_schema(exclude=True)
     @action(
         methods=["POST"],
         detail=False,
         url_path="reset-user-data",
         url_name="reset-user-data",
-        permission_classes=[IsAuthenticated],
     )
     @transaction.atomic()
     def reset_user_data(self, request: Request, **kwargs) -> Response:
         profile_model = swapper.load_model("django_project_base", "Profile")
         profile_obj = getattr(request.user, profile_model._meta.model_name)
         if request.data.get("reset"):
             base_user_models = (get_user_model(), profile_model)
```

### Comparing `django-project-base-0.4.9/django_project_base/account/rest/profile_merge.py` & `django-project-base-0.75.30/django_project_base/account/rest/profile_merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List
 
 import swapper
+
 from django.core.cache import cache
 from django.db import transaction
 from django.utils.translation import gettext_lazy as _
 from dynamicforms import fields
 from dynamicforms.action import Actions, TableAction, TablePosition
 from dynamicforms.mixins import DisplayMode
 from dynamicforms.template_render.responsive_table_layout import ResponsiveTableLayout, ResponsiveTableLayouts
@@ -15,15 +16,15 @@
 from rest_framework.permissions import IsAdminUser, IsAuthenticated
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.serializers import Serializer
 
 from django_project_base.account.constants import MERGE_USERS_QS_CK
 from django_project_base.account.rest.profile import ProfileSerializer, ProfileViewSet
-from django_project_base.base.permissions import IsSuperUser
+from django_project_base.base.permissions import IsProjectOwner, IsSuperUser
 from django_project_base.utils import get_pk_name
 
 
 class ProfileMergeSerializer(ProfileSerializer):
     template_context = dict(url_reverse="profile-merge-base-project")
 
     form_titles = {
@@ -87,27 +88,33 @@
             if str(user) in ",".join(MergeUserGroup.objects.values_list("users", flat=True)).split(","):
                 raise ValidationError(dict(users=f"Pk {user} is present in another group of users to be merged"))
         return super().validate(attrs)
 
 
 class ProfileMergeViewSet(ProfileViewSet):
     serializer_class = ProfileMergeSerializer
-    permission_classes = [IsAuthenticated, IsAdminUser | IsSuperUser]
+    permission_classes = [IsAuthenticated, IsAdminUser | IsSuperUser | IsProjectOwner]
 
     schema = None
 
     def get_queryset(self) -> List:
         ck_val = cache.get(MERGE_USERS_QS_CK % self.request.user.pk, [])
         if not ck_val:
             return super().get_queryset().filter(pk=-1)
         return super().get_queryset().filter(pk__in=ck_val)
 
     def get_serializer_class(self):
         return ProfileMergeSerializer
 
+    def get_permissions(self):
+        if self.action == "clear":
+            return [IsAuthenticated(), IsAdminUser()]
+        else:
+            return super().get_permissions()
+
     @transaction.atomic
     def create(self, request: Request, *args, **kwargs) -> Response:
         MergeUserGroup = swapper.load_model("django_project_base", "MergeUserGroup")
         ck = MERGE_USERS_QS_CK % self.request.user.pk
         ser = MergeUsersRequest(data=dict(users=cache.get(ck, [])))
         ser.is_valid(raise_exception=True)
         group, created = MergeUserGroup.objects.get_or_create(
@@ -133,20 +140,14 @@
         ck_val = [i for i in ck_val if i != pk]
         cache.set(ck, list(set(ck_val)), timeout=None)
         return Response(status=status.HTTP_204_NO_CONTENT)
 
     def partial_update(self, request, *args, **kwargs):
         raise APIException(code=status.HTTP_501_NOT_IMPLEMENTED)
 
-    @action(
-        methods=["DELETE"],
-        detail=False,
-        url_path="clear",
-        url_name="clear",
-        permission_classes=[IsAuthenticated, IsAdminUser],
-    )
+    @action(methods=["DELETE"], detail=False, url_path="clear", url_name="clear")
     def clear(self, request: Request, **kwargs) -> Response:
         MergeUserGroup = swapper.load_model("django_project_base", "MergeUserGroup")
 
         cache.set(MERGE_USERS_QS_CK % self.request.user.pk, [])
         MergeUserGroup.objects.filter(created_by=self.request.user.pk).delete()
         return Response(status=status.HTTP_204_NO_CONTENT)
```

### Comparing `django-project-base-0.4.9/django_project_base/account/rest/project_profiles.py` & `django-project-base-0.75.30/django_project_base/account/rest/project_profiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,71 +1,71 @@
 import json
 import re
+
 from io import BytesIO
 
 import pandas as pd
 import swapper
+
 from django.contrib.auth.hashers import make_password
 from django.db import transaction
 from django.http import HttpResponse
 from django.utils.translation import gettext_lazy as _
 from dynamicforms import fields, serializers
 from dynamicforms.action import TableAction, TablePosition
 from dynamicforms.viewsets import SingleRecordViewSet
 from rest_framework.decorators import action
 from rest_framework.exceptions import NotFound, PermissionDenied
+from rest_framework.permissions import IsAuthenticated
 from rest_framework.request import Request
 from rest_framework.response import Response
 from rest_framework.utils import model_meta
 
 from django_project_base.account.rest.profile import ProfileSerializer, ProfileViewSet
+
+from ...base.permissions import is_project_owner, is_superuser, IsProjectOwnerOrMemberReadOnly, project_is_selected
 from ..middleware import ProjectNotSelectedError
 from .project_profiles_utils import filter_project_members_fields, get_project_members
 
 
 class ProjectProfilesSerializer(ProfileSerializer):
     template_context = dict(url_reverse="alc-profiles")
 
     def __init__(self, *args, **kwargs):
         request = kwargs["context"]["request"]
         self.member_fields_read_only = bool(re.findall(r"profile/current", request.path))
 
         user = request.user
-        self.user_is_admin = user.is_superuser
+        project = request.selected_project
+
+        self.user_is_admin = is_superuser(user) or (project_is_selected(project) and is_project_owner(user, project))
         self.user_is_me = (
             len(args) == 1
             and isinstance(args[0], swapper.load_model("django_project_base", "Profile"))
             and user.id == args[0].id
         )
 
         super().__init__(*args, **kwargs)
 
-        # TODO: this permission check should be replaced by role check
-        from django_project_base.base.permissions import can_user_hijack_another_user
-
-        if can_user_hijack_another_user(request.user, None):
-            self.actions.actions.append(
-                TableAction(
-                    TablePosition.ROW_END,
-                    label=_("Reset password"),
-                    title=_("Reset password"),
-                    name="reset-password",
-                    icon="refresh-outline",
-                ),
-            )
-
-        if request.user.is_superuser or request.user.is_staff:
-            self.actions.actions.append(
-                TableAction(
-                    TablePosition.ROW_END,
-                    label=_("Merge"),
-                    title=_("Merge"),
-                    name="add-to-merge",
-                    icon="git-merge-outline",
-                ),
+        if self.user_is_admin:
+            self.actions.actions.extend(
+                [
+                    TableAction(
+                        TablePosition.ROW_END,
+                        label=_("Reset password"),
+                        name="reset-password",
+                        icon="refresh-outline",
+                    ),
+                    TableAction(
+                        TablePosition.ROW_END,
+                        label=_("Merge"),
+                        name="add-to-merge",
+                        icon="git-merge-outline",
+                    ),
+                ]
             )
 
     def get_fields(self):
         ProjectMember = swapper.load_model("django_project_base", "ProjectMember")
         info = model_meta.get_field_info(ProjectMember)
         for field in ProjectMember().project_members_fields:
             source = f"projects.first.{field.name}"
@@ -98,14 +98,16 @@
 
     def get_visible_fields(self):
         return [(name, field) for (name, field) in self.fields.items() if field.display == fields.DisplayMode.FULL]
 
 
 class ProjectProfilesViewSet(ProfileViewSet):
     serializer_class = ProjectProfilesSerializer
+    # see special case in the permission class if you need to change the permission class
+    permission_classes = (IsProjectOwnerOrMemberReadOnly,)
 
     def get_serializer_class(self):
         return ProjectProfilesSerializer
 
     def filter_queryset_field(self, queryset, field, value):
         if field == "state" and value:
             return queryset.filter(projects__state=value)
@@ -195,14 +197,20 @@
         super().__init__(*args, **kwargs)
         self.fields["profile_fields"].choices = visible_profile_fields
 
 
 class ProfileExportViewSet(SingleRecordViewSet):
     serializer_class = ProfileExportSerializer
 
+    def get_permissions(self):
+        if self.action == "download":
+            return [IsAuthenticated()]
+        else:
+            return super().get_permissions()
+
     def new_object(self):
         filter_data = self.request.query_params.get("filter_data", None)
         if filter_data:
             filter_data = json.loads(filter_data)
         return dict(template=None, profile_fields=None, print_filter=True, filter_data=filter_data)
 
     def create(self, request, *args, **kwargs):
@@ -220,21 +228,15 @@
                 file_name += "-" + ",".join(["-".join([name, str(value)]) for name, value in active_filters.items()])
 
         data = dict(ser.data)
         data["file_name"] = file_name
 
         return Response(data)
 
-    @action(
-        methods=["POST"],
-        detail=False,
-        url_path="download",
-        url_name="profile-export-download",
-        permission_classes=[],
-    )
+    @action(methods=["POST"], detail=False, url_path="download", url_name="profile-export-download")
     def download(self, request: Request, **kwargs):
         profile_serializer = ProjectProfilesSerializer(None, context=self.get_serializer_context(), data=request.data)
         visible_profile_fields = {
             name: profile_serializer.translate_relation_fields(name)
             for name, _ in profile_serializer.get_visible_fields()
         }
         column_names = {
```

### Comparing `django-project-base-0.4.9/django_project_base/account/rest/project_profiles_utils.py` & `django-project-base-0.75.30/django_project_base/account/rest/project_profiles_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-from datetime import datetime, timedelta
+from collections.abc import Iterable
 
 import pytz
 import swapper
+
 from django.conf import settings
-from django.core.cache import cache
 from django.db import models
 from django.db.models import Case, CharField, Prefetch, QuerySet, Value, When
 from django.db.models.functions import Coalesce, Concat
 from django.utils.dateparse import (
     datetime_re,
     iso8601_duration_re,
     parse_datetime,
     parse_duration,
     parse_time,
     standard_duration_re,
     time_re,
 )
+from django.utils.timezone import datetime, now, timedelta
 from dynamicforms import fields
 from rest_framework.request import Request
 
-from django_project_base.account.constants import MERGE_USERS_QS_CK
 from django_project_base.account.middleware import ProjectNotSelectedError
 
 
 def get_project_members(request: Request, project=None) -> QuerySet:
     project = project or request.selected_project
     try:
         project_members = swapper.load_model("django_project_base", "ProjectMember").objects.filter(project_id=project)
@@ -55,34 +55,30 @@
                     Case(When(first_name="", then="username"), default="first_name", output_field=CharField()),
                     Value(""),
                 ),
             ),
         )
     )
 
-    qs = qs.exclude(delete_at__isnull=False, delete_at__lt=datetime.now())
+    qs = qs.exclude(delete_at__isnull=False, delete_at__lt=now())
 
     if project is not None:
         # if current project was parsed from request, filter profiles to current project only
         qs = qs.filter(projects__project=project)
-    elif not (request.user.is_staff or request.user.is_superuser):
-        # but if user is not an admin, and the project is not known, only return this user's project
-        qs = qs.filter(pk=request.user.pk)
+    else:
+        qs = qs.none()
 
     if request.query_params.get("remove-merge-users", "false") in fields.BooleanField.TRUE_VALUES:
         MergeUserGroup = swapper.load_model("django_project_base", "MergeUserGroup")
-        exclude_qs = list(
-            map(
-                str,
-                list(MergeUserGroup.objects.filter(created_by=request.user.pk).values_list("users", flat=True))
-                + cache.get(MERGE_USERS_QS_CK % request.user.pk, []),  # noqa: W503
-            )
-        )
+        exclude_qs = set()
+        for mgu in MergeUserGroup.objects.filter(created_by=request.user.pk).values_list("users", flat=True).all():
+            if mgu and mgu.split(","):
+                exclude_qs.update(map(int, mgu.split(",")))
         if exclude_qs:
-            qs = qs.exclude(pk__in=map(int, exclude_qs))
+            qs = qs.exclude(pk__in=exclude_qs)
 
     qs = qs.order_by("un", "id")
     return qs.distinct()
 
 
 def __get_time_resolution(value: str) -> dict:
     try:
@@ -108,14 +104,18 @@
     if value is None or value == "":
         return queryset
 
     if field == "full_name":
         return queryset.filter(un__icontains=value)
     if field == "state":
         return queryset.filter(projects__state=value)
+    if field == "user_groups":
+        if isinstance(value, Iterable):
+            return queryset.filter(members__user_group__in=value)
+        return queryset.filter(members__user_group=value)
 
     model_meta = queryset.model._meta
 
     if field not in (fld.name for fld in model_meta.get_fields()):
         return queryset
 
     try:
@@ -129,15 +129,15 @@
             return queryset.filter(
                 **{
                     field + "__gte": date_time,
                     field + "__lt": date_time + timedelta(**__get_time_resolution(value)),
                 }
             )
         if isinstance(model_meta.get_field(field), (models.TimeField,)):
-            start = datetime.combine(datetime.now().date(), parse_time(value).replace(microsecond=0))
+            start = datetime.combine(now().date(), parse_time(value).replace(microsecond=0))
             end = (start + timedelta(**__get_time_resolution(value))).time()
             return queryset.filter(**{field + "__gte": start, field + "__lt": end})
         if isinstance(model_meta.get_field(field), (models.DurationField,)):
             duration = parse_duration(value)
             duration = duration - timedelta(microseconds=duration.microseconds)
             return queryset.filter(
                 **{
```

### Comparing `django-project-base-0.4.9/django_project_base/account/rest/reset_password.py` & `django-project-base-0.75.30/django_project_base/account/rest/reset_password.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 
 import swapper
+
 from django.core.cache import cache
 from django.shortcuts import get_object_or_404
 from django.utils.translation import gettext_lazy as _
 from drf_spectacular.utils import extend_schema, extend_schema_view, OpenApiParameter, OpenApiResponse, OpenApiTypes
 from dynamicforms import fields as df_fields, serializers as df_serializers, viewsets as df_viewsets
 from dynamicforms.action import Actions
 from rest_framework import fields, serializers, status, viewsets
```

### Comparing `django-project-base-0.4.9/django_project_base/account/router.py` & `django-project-base-0.75.30/django_project_base/account/router.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 
 accounts_router.register(r"", SocialAuthProvidersViewSet, basename="account")
 accounts_router.register(r"change-password", ChangePasswordViewSet, basename="change-password")
 accounts_router.register(
     r"admin-invalidate-password", InvalidatePasswordAdminViewSet, basename="admin-invalidate-password"
 )
 accounts_router.register(r"admin-add-user", AdminAddUserViewSet, basename="admin-add-user")
-accounts_router.register(r"", ResetPasswordViewSet, basename="account")
-accounts_router.register(r"", RegisterViewSet, basename="account")
-accounts_router.register(r"", SendResetPasswordLinkViewSet, basename="account")
-accounts_router.register(r"", VerifyRegistrationViewSet, basename="account")
+accounts_router.register(r"", ResetPasswordViewSet, basename="account-reset-pass")
+accounts_router.register(r"", RegisterViewSet, basename="account-register")
+accounts_router.register(r"", SendResetPasswordLinkViewSet, basename="account-send-reset-pwd-link")
+accounts_router.register(r"", VerifyRegistrationViewSet, basename="account-verify-registration")
 
 profile_router = DFRouter(trailing_slash=False)
 profile_router.register(r"profile", ProfileViewSet, basename="profile-base-project")
 profile_router.register(r"profile-merge", ProfileMergeViewSet, basename="profile-merge-base-project")
 profile_router.register_single_record(r"impersonate", ImpersonateUserViewset, basename="profile-base-impersonate-user")
 profile_router.register_single_record(r"login", LoginViewset, basename="profile-base-login")
-profile_router.register(r"", LogoutViewSet, basename="account")
+profile_router.register(r"", LogoutViewSet, basename="account-logout")
 profile_router.register(r"project-user-invite", ProjectUserInviteViewSet, basename="project-user-invite")
 profile_router.register(r"projects-profile-search", ProjectsProfileSearchViewSet, basename="projects-profile-search")
```

### Comparing `django-project-base-0.4.9/django_project_base/account/service/merge_users_service.py` & `django-project-base-0.75.30/django_project_base/account/service/merge_users_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Optional
 
 import django
 import swapper
+
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.db import connection, transaction
 from django.db.models import ForeignKey
 from django.utils.module_loading import import_string
 
 
@@ -59,15 +60,15 @@
         users_to_merge = list(filter(lambda i: i and str(i) != str(user.pk), group.users.split(",")))
         project_model = swapper.load_model("django_project_base", "Project")
 
         db_tables = connection.introspection.table_names()
 
         for mdl in django.apps.apps.get_models(include_auto_created=True, include_swapped=True):
             if mdl not in base_user_models and not mdl._meta.abstract and not mdl._meta.swapped:
-                if not (mdl._meta.db_table in db_tables):
+                if mdl._meta.db_table not in db_tables:
                     continue
                 is_project_related = [
                     f for f in mdl._meta.fields if isinstance(f, ForeignKey) and f.related_model == project_model
                 ]
                 for fld in [
                     f
                     for f in mdl._meta.fields
```

### Comparing `django-project-base-0.4.9/django_project_base/account/service/register_user_service.py` & `django-project-base-0.75.30/django_project_base/account/service/register_user_service.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/account/service/reset_password_email_service.py` & `django-project-base-0.75.30/django_project_base/account/service/reset_password_email_service.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+
 from typing import Any, Dict
 
 from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.core.cache import cache
 from django.utils.crypto import get_random_string
 from django.utils.translation import gettext as __
@@ -27,27 +28,32 @@
         request=request,
     )
 
     code_ck = RESET_USER_PASSWORD_VERIFICATION_CODE + str(user.pk)
     code = get_random_string(length=6)
     cache.set(code_ck, code, timeout=settings.CONFIRMATION_CODE_TIMEOUT)
 
+    try:
+        project = request.selected_project.slug
+    except:
+        project = None
+
     EMailNotification(
         message=DjangoProjectBaseMessage(
             subject=f"{__('Password recovery for')} {request.META['HTTP_HOST']}",
             body=f"{__('You or someone acting as you requested a password reset for your account at')} "
             f"{request.META['HTTP_HOST']}. "
             f"\n\n{__('Your verification code is')}: "
             f"{code} \n\n {__('Code is valid for')} {compress(settings.CONFIRMATION_CODE_TIMEOUT)}.\n\n"
             f"{__('If this was not you or it was unintentional, you may safely ignore this message.')}",
             footer="",
             content_type=DjangoProjectBaseMessage.PLAIN_TEXT,
         ),
         raw_recipents=[user.pk],
-        project=request.selected_project.slug,
+        project=project,
         delay=int(datetime.datetime.now().timestamp()),
         recipients=[user.pk],
         user=request.user.pk,
     ).send()
 
     return signer.get_signed_data()
```

### Comparing `django-project-base-0.4.9/django_project_base/account/social_auth/providers.py` & `django-project-base-0.75.30/django_project_base/account/social_auth/providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Get enabled social auth providers configuration."""
 import importlib
+
 from collections import namedtuple
 from functools import reduce
 from typing import Iterable, List
 
 from django.conf import settings
 
 from django_project_base.constants import ACCOUNT_URL_PREFIX
```

### Comparing `django-project-base-0.4.9/django_project_base/account/social_auth/settings.py` & `django-project-base-0.75.30/django_project_base/account/social_auth/settings.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/auth/models.py` & `django-project-base-0.75.30/django_project_base/auth/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import swapper
+
 from django.contrib.auth.models import Group, Permission
 
 
 class BaseRole(Group):
     # Right now our role does not do anything more than Django's
     class Meta:
         abstract = True
```

### Comparing `django-project-base-0.4.9/django_project_base/aws/ses.py` & `django-project-base-0.75.30/django_project_base/aws/ses.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import List
 
 import boto3
+
 from django.conf import settings
 from rest_framework import status
 
 
 def get_aws_session():
     if settings.TESTING:
 
         class FakeSession:
             client = lambda t, i: object()  # noqa: E731
 
         return FakeSession()
     return boto3.Session(
-        aws_access_key_id=getattr(settings, "AWS_SES_ACCESS_KEY_ID", None),
-        aws_secret_access_key=getattr(settings, "AWS_SES_SECRET_ACCESS_KEY", None),
-        region_name=getattr(settings, "AWS_SES_REGION_NAME", None),
+        aws_access_key_id=getattr(settings, "NOTIFICATIONS_AWS_SES_ACCESS_KEY_ID", None),
+        aws_secret_access_key=getattr(settings, "NOTIFICATIONS_AWS_SES_SECRET_ACCESS_KEY", None),
+        region_name=getattr(settings, "NOTIFICATIONS_AWS_SES_REGION_NAME", None),
     )
 
 
 class AwsSes:
     client = (lambda: get_aws_session().client("ses"))()
 
     @staticmethod
```

### Comparing `django-project-base-0.4.9/django_project_base/base/auth_backends.py` & `django-project-base-0.75.30/django_project_base/base/auth_backends.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import swapper
+
 from django.contrib.auth import get_user_model
 from django.contrib.auth.backends import ModelBackend
 from django.core.cache import cache
 from django.db.models.signals import post_delete, post_save
 
 from django_project_base.settings import USER_CACHE_KEY
```

### Comparing `django-project-base-0.4.9/django_project_base/base/event.py` & `django-project-base-0.75.30/django_project_base/base/event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import copy
 import datetime
+
 from abc import ABC, abstractmethod
 from gettext import gettext
 
 import swapper
+
 from django.conf import settings
 from django.shortcuts import get_object_or_404
 from rest_registration.settings import registration_settings
 
 from django_project_base.constants import EMAIL_SENDER_ID_SETTING_NAME, SMS_SENDER_ID_SETTING_NAME
 from django_project_base.notifications.email_notification import SystemEMailNotificationWithListOfEmails
 from django_project_base.notifications.models import DjangoProjectBaseMessage
```

### Comparing `django-project-base-0.4.9/django_project_base/base/fields.py` & `django-project-base-0.75.30/django_project_base/base/fields.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+from typing import Any, cast, Dict, Optional, Union
+
 import swapper
+
 from django.core.validators import RegexValidator
-from django.db.models import fields
+from django.db.models import fields, Q, QuerySet
 from django.utils.translation import gettext_lazy as _
 from dynamicforms import fields as df_fields
 
+from django_project_base.account.middleware import ProjectNotSelectedError
 from django_project_base.base.middleware import get_current_request
 
 
 class HexColorField(fields.CharField):
     def __init__(self, *args, **kwargs):
         if "max_length" not in kwargs:
             kwargs["max_length"] = 7
@@ -17,30 +21,50 @@
                 regex="^#([A-Fa-f0-9]{6}|[A-Fa-f0-9]{3})$",
                 message=_("Value is not a hex color (e.g #88f or #8080ff)"),
             )
         )
 
 
 class UserRelatedField(df_fields.PrimaryKeyRelatedField):
-    def __init__(self, **kwargs):
+    def __init__(
+        self,
+        queryset_filter: Optional[Union[Q, Dict[str, Any]]] = None,
+        queryset_exclude: Optional[Union[Q, Dict[str, Any]]] = None,
+        **kwargs,
+    ):
         kwargs["url_reverse"] = "profile-base-project-list"
         kwargs["query_field"] = "full_name"
         kwargs["additional_parameters"] = dict(select=1)
         kwargs["text_field"] = "full_name"
         kwargs["value_field"] = "id"
         super().__init__(**kwargs)
+        self.queryset_filter = queryset_filter or {}
+        self.queryset_exclude = queryset_exclude or {}
+        self.filter_selected_project = True  # ImpersonateUserIdField overrides this (or any other; as needed)
 
     def get_queryset(self):
         # TODO This needs to be amended together with members editor such that it will be possible to specify
         #  in settings.py how to filter and sort project members
-        qs = swapper.load_model("django_project_base", "Profile").objects
-        request = get_current_request()
-        if request and getattr(request, "selected_project_slug", None):
-            # if current project was parsed from request, filter profiles to current project only
-            qs = qs.filter(projects__project__slug=request.selected_project_slug)
-        return qs.all().distinct()
+        qs = cast(QuerySet, swapper.load_model("django_project_base", "Profile").objects)
+
+        if self.filter_selected_project:
+            try:
+                request = get_current_request()
+                # the field only works in currently selected project
+                qs = qs.filter(projects__project=request.selected_project)
+            except ProjectNotSelectedError:
+                qs = qs.none()
+            except AttributeError:
+                # if the middleware setting current project is not even set (request.selected_project will except),
+                #  we just show all users
+                pass
+
+        qs = qs.exclude(**self.queryset_exclude if isinstance(self.queryset_exclude, dict) else self.queryset_exclude)
+        qs = qs.filter(**self.queryset_filter if isinstance(self.queryset_filter, dict) else self.queryset_filter)
+
+        return qs.all()
 
     def display_value(self, instance):
         if not instance:
             return ""
 
-        return instance.get_full_name()
+        return str(instance)
```

### Comparing `django-project-base-0.4.9/django_project_base/base/middleware.py` & `django-project-base-0.75.30/django_project_base/base/middleware.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import threading
+
 from typing import Optional
 
 from django.conf import settings
 from django.core.handlers.wsgi import WSGIRequest
 
 _threadmap = {}
```

### Comparing `django-project-base-0.4.9/django_project_base/base/models.py` & `django-project-base-0.75.30/django_project_base/base/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import uuid
+
 from typing import List
 
 import svgwrite
 import swapper
+
 from django.conf import settings
 from django.contrib.auth import user_logged_in
 from django.contrib.auth.models import User
 from django.core.exceptions import ValidationError
 from django.core.validators import validate_comma_separated_integer_list
 from django.db import models
 from django.db.models.signals import post_save
@@ -78,14 +80,17 @@
 
     def get_users(self):
         objects_all = BaseProfile.objects
         return objects_all
 
     users = property(lambda self: self.get_users())
 
+    def __str__(self):
+        return self.full_name
+
     class Meta:
         abstract = True
 
 
 class Profile(BaseProfile):
     class Meta:
         swappable = swapper.swappable_setting("django_project_base", "Profile")
```

### Comparing `django-project-base-0.4.9/django_project_base/base/queryset_with_cache.py` & `django-project-base-0.75.30/django_project_base/base/queryset_with_cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import hashlib
 import pickle
+
 from typing import Any
 
 from django.core.cache import cache
 from django.db import models
 from django.db.models import Model
```

### Comparing `django-project-base-0.4.9/django_project_base/celery/background_tasks/notification_tasks.py` & `django-project-base-0.75.30/django_project_base/celery/background_tasks/notification_tasks.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-import logging
 import time
+
 from typing import Optional
 
+from django import db
 from django.core.cache import cache
 
+from django_project_base.celery.background_tasks.base_task import BaseTask
 from django_project_base.celery.celery import app
 from django_project_base.celery.settings import NOTIFICATION_QUEABLE_HARD_TIME_LIMIT, NOTIFICATION_SEND_PAUSE_SECONDS
-from django_project_base.notifications.base.send_notification_mixin import SendNotificationMixin
+from django_project_base.notifications.base.send_notification_service import SendNotificationService
 
 LAST_MAIL_SENT_CK = "last-notification-was-sent-timestamp"
 
 
-class SendNotificationTask(app.Task):
+class SendNotificationTask(BaseTask):
     name = "background_tasks.notification_tasks.send_notification_task"
 
     max_retries = 0
     time_limit = NOTIFICATION_QUEABLE_HARD_TIME_LIMIT
     soft_time_limit = NOTIFICATION_QUEABLE_HARD_TIME_LIMIT - 3
     default_retry_delay = 0
 
     def run(self, notification: "DjangoProjectBaseNotification", extra_data):  # noqa: F821
+        super().run()
         try:
             last_sent: Optional[float] = cache.get(LAST_MAIL_SENT_CK)
             time_from_last_sent: float = time.time() - last_sent if last_sent else 0
             if time_from_last_sent < NOTIFICATION_SEND_PAUSE_SECONDS:
                 time.sleep(int(NOTIFICATION_SEND_PAUSE_SECONDS - time_from_last_sent))
-            SendNotificationMixin().make_send(notification=notification, extra_data=extra_data)
+            SendNotificationService(settings=self.settings).make_send(notification=notification, extra_data=extra_data)
         finally:
             cache.set(LAST_MAIL_SENT_CK, time.time(), timeout=NOTIFICATION_SEND_PAUSE_SECONDS + 1)
+            db.connections.close_all()
 
     def on_failure(self, exc, task_id, args, kwargs, einfo):
-        logging.getLogger(__name__).error(
-            f"Exception: {exc} \n\nTask id: {task_id}\n\nArgs: {args}\n\nKwargs: {kwargs}\n\nEInfo: {einfo}"
-        )
+        super().on_failure(exc=exc, task_id=task_id, args=args, kwargs=kwargs, einfo=einfo)
 
 
 send_notification_task = app.register_task(SendNotificationTask())
```

### Comparing `django-project-base-0.4.9/django_project_base/celery/celery.py` & `django-project-base-0.75.30/django_project_base/celery/celery.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 
-from celery import Celery
+from celery import bootsteps, Celery
+from click import Option
 from django.apps import apps
 from django.utils.crypto import get_random_string
 from kombu import Exchange, Queue
 from kombu.entity import TRANSIENT_DELIVERY_MODE
 
 from django_project_base.celery.settings import NOTIFICATIONS_QUEUE_VISIBILITY_TIMEOUT
 from django_project_base.constants import NOTIFICATION_QUEUE_NAME
@@ -34,14 +35,17 @@
         "django_project_base.notifications",
         "django.contrib.contenttypes",
         "django.contrib.auth",
     )
     TESTING = False
 
 
+os.environ.setdefault("DJANGO_SETTINGS_MODULE", "django_project_base.celery.settings")
+apps.populate(CelerySettings().INSTALLED_APPS)
+
 app = Celery(
     "django_project_base",
     config_source=CelerySettings,
     include=[
         "django_project_base.celery.background_tasks.notification_tasks",
     ],
 )
@@ -54,14 +58,21 @@
         durable=False,
     ),
 ]
 
 app.conf.task_ignore_result = True
 app.conf.worker_send_task_events = False
 app.conf.broker_transport_options = {"visibility_timeout": NOTIFICATIONS_QUEUE_VISIBILITY_TIMEOUT}
+setting_option = Option(("--settings",), is_flag=False, help="Django settings file path", default="")
+app.user_options["worker"].add(setting_option)
 
 
-os.environ.setdefault("DJANGO_SETTINGS_MODULE", "django_project_base.celery.settings")
-apps.populate(CelerySettings().INSTALLED_APPS)
+class CeleryBootstep(bootsteps.Step):
+    def __init__(self, parent, **options):
+        super().__init__(parent, **options)
+        app.conf.setdefault("django-settings-module", options.get("settings", ""))
+
+
+app.steps["worker"].add(CeleryBootstep)
 
 # RUN WORKER AS
 # celery -A django_project_base.celery.celery worker -l INFO -Q notification --concurrency=1
```

### Comparing `django-project-base-0.4.9/django_project_base/country_holidays.py` & `django-project-base-0.75.30/django_project_base/country_holidays.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List, Optional
 
 import requests
+
 from django.core.cache import cache
 from django.utils.translation import gettext_lazy as _
 from requests import Timeout
 from rest_framework import status
 
 holidays_api_url: str = "https://date.nager.at/Api/v2/PublicHolidays/%d/%s"
```

### Comparing `django-project-base-0.4.9/django_project_base/licensing/logic.py` & `django-project-base-0.75.30/django_project_base/licensing/logic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List
+from typing import List, Optional
 
 from django.contrib.contenttypes.models import ContentType
 from django.db import connections
 from django.db.models import Model, Sum
 from django.utils.translation import gettext
 from dynamicforms import fields
 from dynamicforms.serializers import Serializer
@@ -21,30 +21,40 @@
     used_credit = fields.FloatField(read_only=True)
     remaining_credit = fields.FloatField(read_only=True)
 
     usage_report = fields.ListField(child=LicenseUsageReport(), allow_empty=True, read_only=True)
 
 
 class LogAccessService:
+    db = "default"
+
+    def __init__(self, db: Optional[str] = None) -> None:
+        super().__init__()
+        if db:
+            self.db = db
+
     def _user_access_user_inflow(self, user_id) -> float:
         return abs(
-            LicenseAccessUse.objects.filter(user_id=str(user_id), amount__lt=0)
+            LicenseAccessUse.objects.using(self.db)
+            .filter(user_id=str(user_id), amount__lt=0)
             .aggregate(Sum("amount"))
             .get("amount__sum", None)
             or 0
         )
 
     def report(self, user: Model) -> dict:
-        user_query = LicenseAccessUse.objects.filter(user_id=str(user.pk), amount__isnull=False, amount__gt=0)
+        user_query = LicenseAccessUse.objects.using(self.db).filter(
+            user_id=str(user.pk), amount__isnull=False, amount__gt=0
+        )
 
         usage_report = []
         added_types = []
         for agg in user_query.values("content_type").annotate(count=Sum("amount")):
             if (
-                content_type := ContentType.objects.get(pk=agg["content_type"])
+                content_type := ContentType.objects.using(self.db).get(pk=agg["content_type"])
             ) and content_type.model_class()._meta.verbose_name not in added_types:
                 usage_report.append(
                     {"item": content_type.model_class()._meta.verbose_name, "usage_sum": round(agg.get("count", 0), 2)}
                 )
                 added_types.append(content_type.model_class()._meta.verbose_name)
         used_credit = 0
         if user_query.exists():
@@ -67,23 +77,19 @@
         notifications_channels_state: List[str],
         record: Model,
         item_price: float,
         comment: str,
         on_sucess=None,
         **kwargs,
     ) -> int:
-        db_connection = "default"
-        if kwargs.get("db") and kwargs["db"] != "default":
-            db_connection = kwargs["db"]
-            connections["default"] = connections[db_connection]
-
+        connections["default"] = connections[self.db]
         content_type = ContentType.objects.get_for_model(model=record._meta.model)
-
         used = (
-            LicenseAccessUse.objects.filter(user_id=str(user_profile_pk), content_type=content_type)
+            LicenseAccessUse.objects.using(self.db)
+            .filter(user_id=str(user_profile_pk), content_type=content_type)
             .aggregate(Sum("amount"))
             .get("amount__sum", None)
             or 0
         )
         if notifications_channels_state:
             items = {i: notifications_channels_state.count(i) for i in notifications_channels_state}
             from django_project_base.notifications.base.enums import ChannelIdentifier
@@ -98,15 +104,15 @@
         if on_sucess:
             accesses_used = on_sucess()
         else:
             accesses_used = 1
 
         amount = accesses_used * item_price
 
-        LicenseAccessUse.objects.using(db_connection).create(
+        LicenseAccessUse.objects.using(self.db).create(
             type=LicenseAccessUse.UseType.USE,
             user_id=str(user_profile_pk),
             content_type_object_id=str(record.pk).replace("-", ""),
             content_type=content_type,
             amount=amount,
             comment=dict(comment=comment, count=accesses_used, item_price=item_price, sender=kwargs.get("sender", "")),
         )
```

### Comparing `django-project-base-0.4.9/django_project_base/licensing/migrations/0001_initial.py` & `django-project-base-0.75.30/django_project_base/licensing/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py` & `django-project-base-0.75.30/django_project_base/licensing/migrations/0002_remove_licenseaccessuse_comment_and_more_squashed_0004_alter_licenseaccessuse_amount.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/licensing/migrations/0005_auto_20230901_0613.py` & `django-project-base-0.75.30/django_project_base/licensing/migrations/0005_auto_20230901_0613.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/licensing/models.py` & `django-project-base-0.75.30/django_project_base/licensing/models.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/licensing/rest/rest.py` & `django-project-base-0.75.30/django_project_base/licensing/rest/rest.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/locale/en/LC_MESSAGES/djangojs.po` & `django-project-base-0.75.30/django_project_base/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo` & `django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/locale/sl/LC_MESSAGES/djangojs.po` & `django-project-base-0.75.30/django_project_base/locale/sl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/management/commands/confirm_setting.py` & `django-project-base-0.75.30/django_project_base/management/commands/confirm_setting.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from gettext import gettext
 
 import swapper
+
 from django.core.management.base import BaseCommand
 from django.shortcuts import get_object_or_404
 
 from django_project_base.base.event import ProjectSettingConfirmedEvent
 from django_project_base.notifications.email_notification import SystemEMailNotification
 from django_project_base.notifications.models import DjangoProjectBaseMessage
```

### Comparing `django-project-base-0.4.9/django_project_base/management/commands/list_pending_settings.py` & `django-project-base-0.75.30/django_project_base/management/commands/list_pending_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import json
+
 from gettext import gettext
 
 import swapper
+
 from django.conf import settings
 from django.core.management.base import BaseCommand
 
 from django_project_base.notifications.email_notification import SystemEMailNotificationWithListOfEmails
 from django_project_base.notifications.models import DjangoProjectBaseMessage
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/base/channels/channel.py` & `django-project-base-0.75.30/django_project_base/notifications/base/channels/channel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import logging
 import uuid
+
 from abc import ABC, abstractmethod
 from typing import List, Optional, Tuple, Union
 
-from django.conf import settings
+from django.conf import Settings, settings
 from django.contrib.auth import get_user_model
 from django.utils.module_loading import import_string
 from django.utils.translation import gettext
 
 from django_project_base.notifications.base.channels.integrations.provider_integration import ProviderIntegration
 from django_project_base.notifications.base.phone_number_parser import PhoneNumberParser
 from django_project_base.notifications.models import (
@@ -21,21 +22,30 @@
 
 class Recipient:
     identifier: str
     phone_number: str
     email: str
     unique_attribute: str
 
-    def __init__(self, identifier: str, phone_number: str, email: str, unique_attribute: str = "identifier") -> None:
+    def __init__(
+        self,
+        identifier: str,
+        phone_number: str,
+        email: str,
+        unique_attribute: str = "identifier",
+        phone_number_validator=None,
+    ) -> None:
         super().__init__()
         self.identifier = identifier
         self.phone_number = (
             next(
                 iter(
-                    PhoneNumberParser.valid_phone_numbers([phone_number]) if phone_number and len(phone_number) else ""
+                    PhoneNumberParser.valid_phone_numbers([phone_number], phone_number_validator)
+                    if phone_number and len(phone_number)
+                    else ""
                 ),
                 None,
             )
             or ""
         )
         self.email = email
         self.unique_attribute = unique_attribute
@@ -69,54 +79,63 @@
     def sender(self, notification: DjangoProjectBaseNotification) -> str:
         _sender = getattr(notification, "sender", {}).get(self.name)
         if not getattr(settings, "TESTING", False):
             assert _sender, "Notification sender is required"
         return _sender
 
     def _find_provider(
-        self, extra_settings: Optional[dict], setting_name: str, exclude: Optional[List[str]] = None
+        self, settings: Optional[Settings], setting_name: str, exclude: Optional[List[str]] = None
     ) -> Optional[ProviderIntegration]:
         if exclude is None:
             exclude = []
 
         def get_first_provider(val: Union[str, List]):
             if val and isinstance(val, (list, tuple)):
                 prov = next(filter(lambda i: i not in exclude, val), None)
 
                 return import_string(prov)() if prov else None
 
-            return import_string(val)() if val not in exclude else None
+            return import_string(val)() if val not in exclude and val else None
 
-        if extra_settings and getattr(extra_settings.get("SETTINGS", object()), setting_name, None):
-            return get_first_provider(getattr(extra_settings["SETTINGS"], setting_name))
-        return get_first_provider(getattr(settings, setting_name, ""))
+        if settings and getattr(settings, setting_name, None):
+            return get_first_provider(getattr(settings, setting_name))
+        return get_first_provider(getattr(settings or object(), setting_name, ""))
 
     def clean_recipients(self, recipients: List[Recipient]) -> List[Recipient]:
         return list(set(recipients))
 
     def create_delivery_report(
         self,
         notification: DjangoProjectBaseNotification,
         recipient: Recipient,
         pk: str,
         channel: Optional[str] = None,
         provider: Optional[str] = None,
         auxiliary_notification: Optional[uuid.UUID] = None,
     ) -> DeliveryReport:
-        return DeliveryReport.objects.create(
-            notification=notification,
-            user_id=recipient.identifier,
-            channel=f"{self.__module__}.{self.__class__.__name__}" if not channel else channel,
-            provider=f"{self.provider.__module__}.{self.provider.__class__.__name__}" if not provider else provider,
-            pk=pk,
-            auxiliary_notification=auxiliary_notification,
+        return next(
+            iter(
+                DeliveryReport.objects.get_or_create(
+                    notification=notification,
+                    user_id=recipient.identifier,
+                    channel=f"{self.__module__}.{self.__class__.__name__}" if not channel else channel,
+                    provider=f"{self.provider.__module__}.{self.provider.__class__.__name__}"
+                    if not provider
+                    else provider,
+                    pk=pk,
+                    auxiliary_notification=auxiliary_notification,
+                )
+            ),
+            None,
         )
 
     @abstractmethod
-    def get_recipients(self, notification: DjangoProjectBaseNotification, unique_identifier="email") -> List[Recipient]:
+    def get_recipients(
+        self, notification: DjangoProjectBaseNotification, unique_identifier="email", phone_number_validator=None
+    ) -> List[Recipient]:
         rec_obj = notification.email_list
         if not rec_obj:
             rec_obj = notification.recipients_list
         if not rec_obj:
             att = ("email", "phone_number", get_pk_name(get_user_model()))
             rec_obj = [
                 {k: v for k, v in profile.__dict__.items() if not k.startswith("_") and k in att}
@@ -126,14 +145,15 @@
             ]
         return [
             Recipient(
                 identifier=u.get("id", "") or "",
                 email=u.get("email", "") or "",
                 phone_number=u.get("phone_number", "") or "",
                 unique_attribute=unique_identifier,
+                phone_number_validator=phone_number_validator,
             )
             for u in rec_obj
         ]
 
     def _make_send(self, notification_obj, rec_obj, message_str, dlr_pk) -> Tuple[Optional[DeliveryReport], bool]:
         do_send = True
         sent = False
@@ -167,20 +187,22 @@
             if sent and do_send:
                 dlr_obj = self.create_delivery_report(notification_obj, rec_obj, dlr_pk)
             return dlr_obj, (sent and do_send)
         except Exception as de:
             logger.exception(de)
             return dlr_obj, (sent and do_send)
 
-    def send(self, notification: DjangoProjectBaseNotification, extra_data, **kwargs) -> int:
+    def send(self, notification: DjangoProjectBaseNotification, extra_data, settings: Settings, **kwargs) -> int:
         logger = logging.getLogger("django")
         try:
             message = self.provider.get_message(notification)
 
-            recipients = self.get_recipients(notification)
+            recipients = self.get_recipients(
+                notification, phone_number_validator=getattr(settings, "IS_PHONE_NUMBER_ALLOWED_FUNCTION", None)
+            )
 
             if not recipients:
                 raise ValueError("No valid recipients")
 
             exclude_providers: List[str] = []
             sent_no = 0
 
@@ -217,15 +239,17 @@
                                 project=notification.project_slug if notification.project_slug else None,
                                 recipients=[
                                     recipient.identifier,
                                 ],
                                 a_sender=notification.sender,
                                 a_extra_data=extra_data,
                                 a_recipients_list=notification.recipients_list,
+                                a_settings=settings,
                                 delay=int(datetime.datetime.now().timestamp()),
+                                user=extra_data["user"],
                             ).send()
                             self.create_delivery_report(
                                 notification, recipient, dlr__uuid, auxiliary_notification=a_notification.pk
                             )
                             continue
                         except Exception as e:
                             logger.exception(e)
@@ -238,15 +262,15 @@
                         if _make_send[1]:
                             dlr__uuid = str(_make_send[0].pk)
                             was_sent = True
                             break
                         else:
                             exclude_providers.append(f"{self.provider.__module__}.{self.provider.__class__.__name__}")
                             if next_provider := self._find_provider(
-                                extra_settings=extra_data,
+                                settings=settings,
                                 setting_name=self.provider_setting_name,
                                 exclude=exclude_providers,
                             ):
                                 self.provider = next_provider
                             else:
                                 break
                     if was_sent:
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/aws_ses.py` & `django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/nexmo_sms.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,79 @@
-from typing import Union
+from typing import Optional, Union
 
-import boto3
-from django.conf import settings
+import requests
+
+from django.conf import Settings
 from rest_framework.status import is_success
 
 from django_project_base.notifications.base.channels.channel import Recipient
 from django_project_base.notifications.base.channels.integrations.provider_integration import ProviderIntegration
-from django_project_base.notifications.models import (
-    DeliveryReport,
-    DjangoProjectBaseMessage,
-    DjangoProjectBaseNotification,
-)
-
+from django_project_base.notifications.base.phone_number_parser import PhoneNumberParser
+from django_project_base.notifications.models import DeliveryReport, DjangoProjectBaseNotification
 
-class AwsSes(ProviderIntegration):
-    key_id: str
-    access_key: str
-    region: str
 
-    is_sms_provider = False
+class NexmoSMS(ProviderIntegration):
+    api_key: str
+    api_secret: str
 
     def __init__(self) -> None:
         super().__init__(settings=object())
 
-    def validate_send(self, response: dict):
-        assert response
-        assert is_success(response.get("ResponseMetadata", {}).get("HTTPStatusCode", 500))
+    def ensure_credentials(self, settings: Optional[Settings] = None):
+        if settings and getattr(settings, "TESTING", False):
+            return
+        self.api_key = getattr(settings, "NOTIFICATIONS_NEXMO_API_KEY", None)
+        self.api_secret = getattr(settings, "NOTIFICATIONS_NEXMO_API_SECRET", None)
+        self.settings = settings
+        assert self.api_key, "NOTIFICATIONS_NEXMO_API_KEY required"
+        assert self.api_secret, "NOTIFICATIONS_NEXMO_API_SECRET required"
 
     def _get_sms_message(self, notification: DjangoProjectBaseNotification) -> Union[dict, str]:
         return super()._get_sms_message(notification)
 
-    def ensure_credentials(self, extra_data):
-        if settings and getattr(settings, "TESTING", False):
+    def validate_send(self, response: object):
+        assert response
+        assert is_success(response.status_code)
+
+    def client_send(self, sender: str, recipient: Recipient, msg: str, dlr_id: str):
+        # TODO: SLOVENIA????????
+        rec = PhoneNumberParser.ensure_country_code_slovenia([recipient.phone_number])
+        if not rec:
             return
-        self.key_id = getattr(settings, "AWS_SES_ACCESS_KEY_ID", None)
-        self.access_key = getattr(settings, "AWS_SES_SECRET_ACCESS_KEY", None)
-        self.region = getattr(settings, "AWS_SES_REGION_NAME", None)
-        self.settings = settings
-        if extra_data and (stgs := extra_data.get("SETTINGS")):
-            self.settings = stgs
-            self.key_id = getattr(stgs, "AWS_SES_ACCESS_KEY_ID", None)
-            self.access_key = getattr(stgs, "AWS_SES_SECRET_ACCESS_KEY", None)
-            self.region = getattr(stgs, "AWS_SES_REGION_NAME", None)
-        assert self.key_id, "AWS SES key id required"
-        assert self.access_key, "AWS SES key id access key required"
-        assert self.region, "AWS SES region required"
-
-    def get_message(self, notification: DjangoProjectBaseNotification) -> dict:
-        msg = {
-            "Body": {},
-            "Subject": {
-                "Charset": "UTF-8",
-                "Data": str(notification.message.subject),
-            },
-        }
-        msg["Body"][
-            "Html" if notification.message.content_type.lower() == DjangoProjectBaseMessage.HTML else "Text"
-        ] = {
-            "Charset": "UTF-8",
-            "Data": str(notification.message.body),
+
+        if not rec[0]:
+            return
+
+        params: dict = {
+            "api_key": self.api_key,
+            "api_secret": self.api_secret,
+            "from": sender,
+            "to": rec[0],
+            "text": msg,
         }
-        return msg
+        response = requests.get(
+            "https://rest.nexmo.com/sms/json",
+            params=params,
+            verify=False,
+            timeout=4,
+        )
+        self.validate_send(response)
+
+    def get_message(self, notification: DjangoProjectBaseNotification) -> Union[dict, str]:
+        return self._get_sms_message(notification)
 
     def parse_delivery_report(self, dlr: DeliveryReport):
         pass
 
     @property
     def delivery_report_username_setting_name(self) -> str:
-        return "aws-ses-email-dlr-user"
+        return "nexmo-sms-dlr-user"
 
     @property
     def delivery_report_password_setting_name(self) -> str:
-        return "aws-ses-email-dlr-password"
+        return "nexmo-sms-dlr-password"
 
     def ensure_dlr_user(self, project_slug: str):
         pass
 
     def enqueue_dlr_request(self, pk: str):
-        DeliveryReport.objects.filter(pk=pk).update(status=DeliveryReport.Status.DELIVERED)
-
-    def client_send(self, sender: str, recipient: Recipient, msg: dict, dlr_id: str):
-        if not recipient.email:
-            return
-        res = (
-            boto3.Session(
-                aws_access_key_id=self.key_id,
-                aws_secret_access_key=self.access_key,
-                region_name=self.region,
-            )
-            .client("ses")
-            .send_email(
-                Destination={
-                    "ToAddresses": [recipient.email],
-                    "CcAddresses": [],
-                    "BccAddresses": [],
-                },
-                Message=msg,
-                Source=sender,
-            )
-        )
-        self.validate_send(res)
+        pass
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py` & `django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/aws_sns_single_sms.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-from typing import Union
+from typing import Optional, Union
 
 import boto3
-from django.conf import settings
+
+from django.conf import Settings
 from rest_framework.status import is_success
 
 from django_project_base.notifications.base.channels.channel import Recipient
 from django_project_base.notifications.base.channels.integrations.provider_integration import ProviderIntegration
 from django_project_base.notifications.models import DeliveryReport, DjangoProjectBaseNotification
 
 
@@ -13,26 +14,21 @@
     key_id: str
     access_key: str
     region: str
 
     def __init__(self) -> None:
         super().__init__(settings=object())
 
-    def ensure_credentials(self, extra_data):
+    def ensure_credentials(self, settings: Optional[Settings] = None):
         if settings and getattr(settings, "TESTING", False):
             return
-        self.key_id = getattr(settings, "AWS_SES_ACCESS_KEY_ID", None)
-        self.access_key = getattr(settings, "AWS_SES_SECRET_ACCESS_KEY", None)
-        self.region = getattr(settings, "AWS_SES_REGION_NAME", None)
+        self.key_id = getattr(settings, "NOTIFICATIONS_AWS_SES_ACCESS_KEY_ID", None)
+        self.access_key = getattr(settings, "NOTIFICATIONS_AWS_SES_SECRET_ACCESS_KEY", None)
+        self.region = getattr(settings, "NOTIFICATIONS_AWS_SES_REGION_NAME", None)
         self.settings = settings
-        if extra_data and (stgs := extra_data.get("SETTINGS")):
-            self.settings = stgs
-            self.key_id = getattr(stgs, "AWS_SES_ACCESS_KEY_ID", None)
-            self.access_key = getattr(stgs, "AWS_SES_SECRET_ACCESS_KEY", None)
-            self.region = getattr(stgs, "AWS_SES_REGION_NAME", None)
         assert self.key_id, "AWS SES key id required"
         assert self.access_key, "AWS SES key id access key required"
         assert self.region, "AWS SES region required"
 
     def _get_sms_message(self, notification: DjangoProjectBaseNotification) -> Union[dict, str]:
         return super()._get_sms_message(notification)
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/provider_integration.py` & `django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/provider_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import re
+
 from abc import ABC, abstractmethod
 from html import unescape
-from typing import Union
+from typing import Optional, Union
 
 import swapper
+
+from django.conf import Settings
 from django.urls import reverse
 from django.utils.html import strip_tags
 
 from django_project_base.constants import SEND_NOTIFICATION_SMS
 from django_project_base.notifications.models import DeliveryReport, DjangoProjectBaseNotification
 
 
 class ProviderIntegration(ABC):
-    settings: object
+    settings: Settings
 
     is_sms_provider = True
 
     def __init__(self, settings: object) -> None:
         super().__init__()
         self.settings = settings
 
     @abstractmethod
     def validate_send(self, response: dict):
         pass
 
     @abstractmethod
-    def ensure_credentials(self, extra_data: dict):
+    def ensure_credentials(self, settings: Optional[Settings] = None):
         pass
 
     @abstractmethod
     def client_send(self, sender: str, recipient: "Recipient", msg: str, dlr_id: str):  # noqa: F821
         pass
 
     @property
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/base/channels/integrations/t2.py` & `django-project-base-0.75.30/django_project_base/notifications/base/channels/integrations/t2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 import json
-from typing import Union
+
+from math import ceil
+from typing import Optional, Union
 
 import requests
 import swapper
-from django.conf import settings
+
+from django.conf import Settings
 from django.contrib.auth import get_user_model
 from requests.auth import HTTPBasicAuth
 from rest_framework.status import is_success
 
 from django_project_base.celery.settings import NOTIFICATION_QUEABLE_HARD_TIME_LIMIT
 from django_project_base.notifications.base.channels.channel import Recipient
 from django_project_base.notifications.base.channels.integrations.provider_integration import ProviderIntegration
 from django_project_base.notifications.models import DeliveryReport, DjangoProjectBaseNotification
 
 # -*- coding: utf8 -*-
 """
 Created on Jul 10, 2016
 @author: Dayo
 """
-from math import ceil
 
 
 class SMSCounter(object):
     # https: // raw.githubusercontent.com / dedayoa / sms - counter - python / master / sms_counter / main.py
     GSM_7BIT = "GSM_7BIT"
     GSM_7BIT_EX = "GSM_7BIT_EX"
     UTF16 = "UTF16"
@@ -273,29 +275,24 @@
     settings: object
 
     url = ""
 
     def __init__(self) -> None:
         super().__init__(settings=object())
 
-    def ensure_credentials(self, extra_data):
+    def ensure_credentials(self, settings: Optional[Settings] = None):
         if settings and getattr(settings, "TESTING", False):
             return
-        self.username = getattr(settings, "T2_USERNAME", None)
-        self.password = getattr(settings, "T2_PASSWORD", None)
-        self.url = getattr(settings, "SMS_API_URL", None)
+        self.username = getattr(settings, "NOTIFICATIONS_T2_USERNAME", None)
+        self.password = getattr(settings, "NOTIFICATIONS_T2_PASSWORD", None)
+        self.url = getattr(settings, "NOTIFICATIONS_SMS_API_URL", None)
         self.settings = settings
-        if extra_data and (stgs := extra_data.get("SETTINGS")):
-            self.settings = stgs
-            self.username = getattr(stgs, "T2_USERNAME", None)
-            self.password = getattr(stgs, "T2_PASSWORD", None)
-            self.url = getattr(stgs, "SMS_API_URL", None)
-        assert self.username, "T2_USERNAME is required"
-        assert self.password, "T2_PASSWORD is required"
-        assert len(self.url) > 0, "T2_PASSWORD is required"
+        assert self.username, "NOTIFICATIONS_T2_USERNAME is required"
+        assert self.password, "NOTIFICATIONS_T2_PASSWORD is required"
+        assert len(self.url) > 0, "NOTIFICATIONS_T2_PASSWORD is required"
 
     def client_send(self, sender: str, recipient: Recipient, msg: str, dlr_id: str):
         if not recipient.phone_number:
             return
         basic_auth = HTTPBasicAuth(self.username, self.password)
         response = requests.post(
             f"{self.url}{self.endpoint_one}",
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/base/channels/mail_channel.py` & `django-project-base-0.75.30/django_project_base/notifications/base/channels/sms_channel.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,36 @@
-import uuid
 from typing import List
 
-from django.conf import settings
-from django.core.exceptions import ValidationError
-from django.core.validators import validate_email
+from django.conf import Settings
 
 from django_project_base.notifications.base.channels.channel import Channel, Recipient
 from django_project_base.notifications.base.enums import ChannelIdentifier
 from django_project_base.notifications.models import DjangoProjectBaseNotification
 
 
-class MailChannel(Channel):
-    id = ChannelIdentifier.MAIL.value
+class SmsChannel(Channel):
+    id = ChannelIdentifier.SMS.value
 
-    name = "EMail"
+    name = "SMS"
 
-    notification_price = 0.0002  # TODO get from settings
+    notification_price = 0.1  # TODO get from settings
 
-    provider_setting_name = "EMAIL_PROVIDER"
+    provider_setting_name = "NOTIFICATIONS_SMS_PROVIDER"
 
-    def send(self, notification: DjangoProjectBaseNotification, extra_data, **kwargs) -> int:
-        if getattr(settings, "TESTING", False):
-            return super().send(notification=notification, extra_data=extra_data)
-        message = self.provider.get_message(notification)
-        sender = self.sender(notification)
-        self.provider.client_send(
-            self.sender(notification),
-            Recipient(identifier=str(uuid.uuid4()), phone_number="", email=sender),
-            message,
-            str(uuid.uuid4()),
+    def get_recipients(
+        self, notification: DjangoProjectBaseNotification, unique_identifier="", phone_number_validator=None
+    ):
+        return list(
+            set(
+                super().get_recipients(
+                    notification, unique_identifier="phone_number", phone_number_validator=phone_number_validator
+                )
+            )
         )
-        return super().send(notification=notification, extra_data=extra_data)
 
-    def get_recipients(self, notification: DjangoProjectBaseNotification, unique_identifier=""):
-        return list(set(super().get_recipients(notification, unique_identifier="email")))
+    def send(
+        self, notification: DjangoProjectBaseNotification, extra_data: dict, settings: Settings, **kwargs
+    ) -> int:  # noqa: F821
+        return super().send(notification=notification, extra_data=extra_data, settings=settings)
 
-    def clean_email_recipients(self, recipients: List[Recipient]) -> List[Recipient]:
-        valid = []
-        for email in self.clean_recipients(recipients):
-            try:
-                validate_email(email.email)
-                valid.append(email)
-            except ValidationError:
-                pass
-        return valid
+    def clean_sms_recipients(self, recipients: List[Recipient]) -> List[Recipient]:
+        return list(filter(lambda r: r.phone_number and len(r.phone_number), self.clean_recipients(recipients)))
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/base/channels/sms_channel.py` & `django-project-base-0.75.30/django_project_base/notifications/maintenance_notification.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-from typing import List
+import uuid
 
-from django_project_base.notifications.base.channels.channel import Channel, Recipient
-from django_project_base.notifications.base.enums import ChannelIdentifier
-from django_project_base.notifications.models import DjangoProjectBaseNotification
+from typing import List, Optional, Type
 
-
-class SmsChannel(Channel):
-    id = ChannelIdentifier.SMS.value
-
-    name = "SMS"
-
-    notification_price = 0.1  # TODO get from settings
-
-    provider_setting_name = "SMS_PROVIDER"
-
-    def get_recipients(self, notification: DjangoProjectBaseNotification, unique_identifier=""):
-        return list(set(super().get_recipients(notification, unique_identifier="phone_number")))
-
-    def send(self, notification: DjangoProjectBaseNotification, extra_data, **kwargs) -> int:  # noqa: F821
-        return super().send(notification=notification, extra_data=extra_data)
-
-    def clean_sms_recipients(self, recipients: List[Recipient]) -> List[Recipient]:
-        return list(filter(lambda r: r.phone_number and len(r.phone_number), self.clean_recipients(recipients)))
+from django_project_base.notifications.base.channels.channel import Channel
+from django_project_base.notifications.base.enums import NotificationLevel, NotificationType
+from django_project_base.notifications.base.notification import Notification
+from django_project_base.notifications.models import DjangoProjectBaseMessage
+
+
+class MaintenanceNotification(Notification):
+    def __init__(self, delay: int, message: DjangoProjectBaseMessage, locale: Optional[str] = None) -> None:
+        super().__init__(
+            message=message,
+            raw_recipents=[],
+            project=None,
+            persist=True,
+            level=NotificationLevel.WARNING.value,
+            locale=locale,
+            delay=delay,
+            type=NotificationType.MAINTENANCE.value,
+            content_entity_context=str(uuid.uuid4()),
+        )
+
+    @property
+    def via_channels(self) -> List[Type[Channel]]:
+        return []
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/base/duplicate_notification_mixin.py` & `django-project-base-0.75.30/django_project_base/notifications/base/duplicate_notification_mixin.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/base/enums.py` & `django-project-base-0.75.30/django_project_base/notifications/base/enums.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from enum import Enum
 from typing import Optional, Union
 
+from django.conf import Settings
+
 
 class NotificationType(Enum):
     MAINTENANCE = "maintenance"
     STANDARD = "standard"
 
 
 class NotificationLevel(Enum):
@@ -25,24 +27,22 @@
         from django_project_base.notifications.base.channels.sms_channel import SmsChannel
 
         return MailChannel(), SmsChannel()
 
     @staticmethod
     def channel(
         identifier: Union[int, str],
-        extra_data: Optional[dict] = None,
+        settings: Optional[Settings] = None,
         project_slug: Optional[str] = None,
         ensure_dlr_user=True,
     ) -> Optional["Channel"]:  # noqa: F821
         channel = next(
             iter(filter(lambda c: c.name == identifier or c.id == identifier, ChannelIdentifier.supported_channels())),
             None,
         )
         if channel:
-            channel.provider = channel._find_provider(
-                extra_settings=extra_data, setting_name=channel.provider_setting_name
-            )
-            channel.provider.ensure_credentials(extra_data=extra_data)
+            channel.provider = channel._find_provider(settings=settings, setting_name=channel.provider_setting_name)
+            channel.provider.ensure_credentials(settings=settings)
             channel.provider.ensure_dlr_user(project_slug) if ensure_dlr_user else False
 
             return channel
         return None
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/base/notification.py` & `django-project-base-0.75.30/django_project_base/notifications/base/notification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 import datetime
 import json
 import uuid
+
 from typing import List, Optional, Type
 
 import swapper
-from django.conf import settings
+
+from django.conf import Settings, settings
 from django.contrib.auth import get_user_model
 
 from django_project_base.constants import (
     EMAIL_SENDER_ID_SETTING_NAME,
     SMS_SENDER_ID_SETTING_NAME,
     USE_EMAIL_IF_RECIPIENT_HAS_NO_PHONE_NUMBER,
 )
 from django_project_base.notifications.base.channels.channel import Channel
 from django_project_base.notifications.base.duplicate_notification_mixin import DuplicateNotificationMixin
 from django_project_base.notifications.base.enums import ChannelIdentifier, NotificationLevel, NotificationType
 from django_project_base.notifications.base.queable_notification_mixin import QueableNotificationMixin
-from django_project_base.notifications.base.send_notification_mixin import SendNotificationMixin
+from django_project_base.notifications.base.send_notification_service import SendNotificationService
 from django_project_base.notifications.models import DjangoProjectBaseMessage, DjangoProjectBaseNotification
 
 
-class Notification(QueableNotificationMixin, DuplicateNotificationMixin, SendNotificationMixin):
+class Notification(QueableNotificationMixin, DuplicateNotificationMixin):
     _persist = False
     _delay = None
     _recipients = []
     _extra_data = {}
     type = NotificationType.STANDARD.value
     level = None
     locale = None
@@ -75,27 +77,29 @@
             self._delay = delay
         if type is not None:
             typ = type.value if isinstance(type, NotificationType) else type
             assert typ in [t.value for t in NotificationType], "Invalid notification type value"
             self.type = type if isinstance(type, NotificationType) else NotificationType(typ)
         assert isinstance(recipients, list), "Recipients must be a list"
         self._recipients = recipients
-        self._extra_data = kwargs
+        self._extra_data = kwargs or {}
         assert isinstance(message, DjangoProjectBaseMessage), "Invalid value for message"
         self.message = message
         self.content_entity_context = content_entity_context
         if channels:
             # TODO: check for supported channels
             self.via_channels = channels
         self._project = project
         self._user = user
 
     @staticmethod
-    def resend(notification: DjangoProjectBaseNotification, user_pk: str):
-        notification.user = user_pk
+    def resend(notification: DjangoProjectBaseNotification, user_pk: Optional[str] = None):
+        if user_pk == "None":
+            user_pk = None
+        notification.user = user_pk or (notification.extra_data or {}).get("user")
         from django_project_base.notifications.rest.notification import MessageToListField
 
         recipients: List[str] = MessageToListField.parse(json.loads(notification.recipients_original_payload))
         notification.recipients = ",".join(map(str, recipients)) if recipients else None
         notification.recipients_original_payload_search = None
         notification.sender = Notification._get_sender_config(notification.project_slug)
         mail_fallback: bool = (
@@ -103,15 +107,17 @@
             .objects.get(name=USE_EMAIL_IF_RECIPIENT_HAS_NO_PHONE_NUMBER, project__slug=notification.project_slug)
             .python_value
             if notification.project_slug
             else False
         )
         notification.email_fallback = mail_fallback
         notification.save(update_fields=["recipients", "recipients_original_payload_search"])
-        SendNotificationMixin().make_send(notification, {}, resend=True)
+        SendNotificationService(settings=settings, use_default_db_connection=True).make_send(
+            notification, {}, resend=True
+        )
 
     def __set_via_channels(self, val):
         self._via_channels = val
 
     def __get_via_channels(self):
         return self._via_channels
 
@@ -149,15 +155,15 @@
             SmsChannel.name: "",
         }
 
     def send(self) -> DjangoProjectBaseNotification:
         required_channels: list = list(
             map(lambda f: str(f), filter(lambda d: d is not None, map(lambda c: c.name, self.via_channels)))
         )
-
+        self._extra_data["user"] = self._user
         notification: DjangoProjectBaseNotification = DjangoProjectBaseNotification(
             locale=self.locale,
             level=self.level.value,
             delayed_to=self.delay,
             required_channels=",".join(required_channels) if required_channels else None,
             type=self.type.value,
             message=self.message,
@@ -165,17 +171,18 @@
             if self.content_entity_context
             else str(uuid.uuid4()),
             recipients=",".join(map(str, self._recipients)) if self._recipients else None,
             recipients_original_payload=self._raw_recipents,
             project_slug=self._project,
             send_notification_sms=self.send_notification_sms,
             send_notification_sms_text=None,
+            extra_data=self._extra_data,
         )
 
-        notification = self._ensure_channels(required_channels, notification)
+        notification = self._ensure_channels(channels=required_channels, notification=notification, settings=settings)
 
         required_channels.sort()
         if self.persist:
             if self.handle_similar_notifications(notification=notification):
                 return notification
             if not self.message.pk or not DjangoProjectBaseMessage.objects.filter(pk=self.message.pk).exists():
                 self.message.save()
@@ -183,65 +190,75 @@
             notification.save()
         else:
             notification.created_at = None
 
         if self.delay:
             if not self.persist:
                 raise Exception("Delayed notification must be persisted")
-            self._set_db()
 
             rec_list = self._extra_data.get("a_recipients_list") or []
             if len(rec_list) == 0:
                 for usr in self._recipients:
                     rec_list.append(
                         {
                             k: v
                             for k, v in get_user_model().objects.get(pk=usr).userprofile.__dict__.items()
                             if not k.startswith("_")
                         }
                     )
             notification.recipients_list = rec_list
-            self.enqueue_notification(notification, self._extra_data.get("a_extra_data") or self._extra_data)
+            ext_data = self._extra_data.get("a_extra_data") or self._extra_data
+            notification.extra_data = ext_data
+            notification.save(update_fields=["extra_data"])
+            self.enqueue_notification(notification, extra_data=ext_data)
             return notification
 
-        notification = self.make_send(notification, self._extra_data)
+        if not self.delay:
+            SendNotificationService(settings=settings, use_default_db_connection=True).make_send(
+                notification, self._extra_data, resend=False
+            )
+        else:
+            if not self.persist:
+                raise Exception("Delayed notification must be persisted")
+            mail_fallback: bool = (
+                swapper.load_model("django_project_base", "ProjectSettings")
+                .objects.get(name=USE_EMAIL_IF_RECIPIENT_HAS_NO_PHONE_NUMBER, project__slug=notification.project_slug)
+                .python_value
+                if notification.project_slug
+                else False
+            )
+            rec_list = []
+            for usr in self._recipients:
+                rec_list.append(
+                    {
+                        k: v
+                        for k, v in get_user_model().objects.get(pk=usr).userprofile.__dict__.items()
+                        if not k.startswith("_") and isinstance(v, (str, list, tuple, int, float))
+                    }
+                )
+            notification.extra_data["recipients-list"] = rec_list
+            notification.extra_data["sender"] = notification.sender
+            notification.extra_data["mail-fallback"] = mail_fallback
+            notification.save(update_fields=["extra_data"])
 
         return notification
 
-    def _set_db(self):
-        from django.db import connection
-
-        sttgs = connection.settings_dict
-
-        sttgs["TIME_ZONE"] = None
-        self._extra_data["DATABASE"] = {
-            "PARAMS": connection.get_connection_params(),
-            "SETTINGS": sttgs,
-        }
-        self._extra_data["SETTINGS"] = settings
-        from dill import dumps as ddumps
-
-        setattr(
-            self._extra_data["SETTINGS"],
-            "IS_PHONE_NUMBER_ALLOWED_FUNCTION",
-            ddumps(
-                getattr(self._extra_data["SETTINGS"], "IS_PHONE_NUMBER_ALLOWED_FUNCTION", ""), fmode=True, recurse=True
-            ),
-        )
-
     def _ensure_channels(
-        self, channels: List[str], notification: DjangoProjectBaseNotification
+        self,
+        channels: List[str],
+        notification: DjangoProjectBaseNotification,
+        settings: Optional[Settings] = None,
     ) -> DjangoProjectBaseNotification:
         from django_project_base.notifications.base.channels.mail_channel import MailChannel
 
         extra_data = self._extra_data.get("a_extra_data") or self._extra_data
-
+        settings = self._extra_data.get("a_settings") or settings
         for channel_name in channels:
             # ensure dlr user and check providers
-            channel = ChannelIdentifier.channel(channel_name, extra_data=extra_data, project_slug=self._project)
+            channel = ChannelIdentifier.channel(channel_name, settings=settings, project_slug=self._project)
 
             if not channel and extra_data.get("is_system_notification"):
                 continue
 
             assert channel
 
             if self.send_notification_sms and channel.name == MailChannel.name:
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/base/phone_number_parser.py` & `django-project-base-0.75.30/django_project_base/notifications/base/phone_number_parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from typing import List
 
-from django.core.cache import cache
-
 
 class PhoneNumberParser:
     @staticmethod
-    def is_allowed(phone_number: str) -> bool:
-        if (allowed_function := cache.get("IS_PHONE_NUMBER_ALLOWED_FUNCTION".lower(), "")) and allowed_function:
-            from dill import loads as dloads
-
-            return dloads(allowed_function)(phone_number)
+    def is_allowed(phone_number: str, allowed_validator=None) -> bool:
+        if allowed_validator:
+            return allowed_validator(phone_number)
         return phone_number and len(phone_number) >= 8
 
     @staticmethod
-    def valid_phone_numbers(candidates: List[str]) -> List[str]:
+    def valid_phone_numbers(candidates: List[str], allowed_validator=None) -> List[str]:
         valid: List[str] = []
         for number in candidates:
-            if not PhoneNumberParser.is_allowed(number):
+            if not PhoneNumberParser.is_allowed(number, allowed_validator):
                 continue
             if number.startswith("+"):
                 valid.append(number.lstrip("+"))
                 continue
             if number.startswith("00"):
                 valid.append(number.lstrip("00"))
                 continue
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/base/queable_notification_mixin.py` & `django-project-base-0.75.30/django_project_base/notifications/base/queable_notification_mixin.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/base/send_notification_mixin.py` & `django-project-base-0.75.30/django_project_base/notifications/base/send_notification_service.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,40 @@
 import logging
 
-from django import db
-from django.core.cache import cache
-from django.db import connections
-from django.db.utils import load_backend
+from django.conf import Settings
 from django.utils import timezone
 
+from django_project_base.constants import NOTIFICATION_QUEUE_NAME
 from django_project_base.notifications.base.enums import ChannelIdentifier
 from django_project_base.notifications.models import DjangoProjectBaseNotification
 
 
-class SendNotificationMixin(object):
+class SendNotificationService(object):
+    settings: Settings
+    use_default_db_connection = False
+
+    def __init__(self, settings: Settings, use_default_db_connection=False) -> None:
+        super().__init__()
+        self.settings = settings
+        self.use_default_db_connection = use_default_db_connection
+
     def make_send(
         self, notification: DjangoProjectBaseNotification, extra_data, resend=False
     ) -> DjangoProjectBaseNotification:
+        # TODO: THIS SHOULD BE CALLED ONLY FROM CELERY BACKGROUND TASK
+
         sent_channels: list = []
         failed_channels: list = []
+        db_name = NOTIFICATION_QUEUE_NAME if not self.use_default_db_connection else "default"
 
         exceptions = ""
         from django_project_base.licensing.logic import LogAccessService
 
         if notification.required_channels is None:
             return notification
-
-        db_connection = "default"
-        db_settings = extra_data.get("DATABASE")
-        if db_settings:
-            db_connection = f"notification-{notification.pk}"
-            backend = load_backend(db_settings["SETTINGS"]["ENGINE"])
-            dw = backend.DatabaseWrapper(db_settings["SETTINGS"])
-            dw.connect()
-            connections.databases[db_connection] = dw.settings_dict
-        if (
-            (stgs := extra_data.get("SETTINGS"))
-            and (phn_allowed := getattr(stgs, "IS_PHONE_NUMBER_ALLOWED_FUNCTION", ""))
-            and phn_allowed
-        ):
-            cache.set("IS_PHONE_NUMBER_ALLOWED_FUNCTION".lower(), phn_allowed, timeout=None)
-
         already_sent_channels = set(
             filter(
                 lambda i: i not in (None, "") and i,
                 notification.sent_channels.split(",") if notification.sent_channels else [],
             )
         )
         required_channels = set(
@@ -60,27 +53,30 @@
         from django_project_base.notifications.base.channels.sms_channel import SmsChannel
 
         if notification.send_notification_sms:
             required_channels.add(SmsChannel.name)
 
         for channel_identifier in required_channels:
             channel = ChannelIdentifier.channel(
-                channel_identifier, extra_data=extra_data, project_slug=notification.project_slug, ensure_dlr_user=False
+                channel_identifier,
+                settings=self.settings,
+                project_slug=notification.project_slug,
+                ensure_dlr_user=False,
             )
             try:
                 # check license
-                any_sent = LogAccessService().log(
+                any_sent = LogAccessService(db=db_name).log(
                     user_profile_pk=notification.user,
                     notifications_channels_state=sent_channels,
                     record=notification,
                     item_price=channel.notification_price,
                     comment=str(channel),
-                    on_sucess=lambda: channel.send(notification, extra_data),
-                    db=db_connection,
-                    settings=extra_data.get("SETTINGS", object()),
+                    on_sucess=lambda: channel.send(
+                        notification=notification, extra_data=extra_data, settings=self.settings
+                    ),
                     is_system_notification=extra_data.get("is_system_notification"),
                     sender=channel.sender(notification),
                 )
                 sent_channels.append(channel) if any_sent > 0 else failed_channels.append(channel)
             except Exception as e:
                 logging.getLogger(__name__).error(e)
                 failed_channels.append(channel)
@@ -135,13 +131,10 @@
             notification.save(
                 update_fields=[
                     "sent_at",
                     "sent_channels",
                     "failed_channels",
                     "exceptions",
                 ],
-                using=db_connection,
+                using=db_name,
             )
-
-            if db_settings:
-                db.connections.close_all()
         return notification
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/email_notification.py` & `django-project-base-0.75.30/django_project_base/notifications/email_notification.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import datetime
 import uuid
+
 from typing import List, Optional, Type
 
+from django.conf import settings
 from django.core.cache import cache
 from rest_framework.exceptions import PermissionDenied
 
 from django_project_base.notifications.base.channels.channel import Channel
 from django_project_base.notifications.base.channels.mail_channel import MailChannel
 from django_project_base.notifications.base.enums import NotificationLevel, NotificationType
 from django_project_base.notifications.base.notification import Notification
@@ -68,23 +70,22 @@
             if self.content_entity_context
             else str(uuid.uuid4()),
             recipients=",".join(map(str, self._recipients)) if self._recipients else None,
             recipients_original_payload=self._raw_recipents,
             project_slug=self._project,
         )
 
-        notification = self._ensure_channels([MailChannel.name], notification)
+        notification = self._ensure_channels([MailChannel.name], notification, settings=settings)
 
         if self.handle_similar_notifications(notification=notification):
             return notification
         if not self.message.pk or not DjangoProjectBaseMessage.objects.filter(pk=self.message.pk).exists():
             self.message.save()
         notification.created_at = int(datetime.datetime.now().timestamp())
         notification.save()
-        self._set_db()
         uuid_val = str(uuid.uuid4())
         notification.email_list = [
             dict(
                 id=uuid_val,
                 email=u,
                 phone_number="",
             )
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/management/commands/resend_notification.py` & `django-project-base-0.75.30/django_project_base/notifications/management/commands/resend_notification.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,14 @@
 
 
 class Command(BaseCommand):
     help = 'Resends notification. Example:  python manage.py resend_notification "178a46c2-2aa3-4a33-bad6-9af2d76f6891" 2'  # noqa: E501
 
     def add_arguments(self, parser) -> None:
         parser.add_argument("notification", type=str, help="Notification identifier (uuid string).")
-        parser.add_argument("user", type=str, help="User identifier (user sending notification).")
+        parser.add_argument("user", type=str, help="User identifier (user sending notification).", nargs="?")
 
     def handle(self, *args, **options):
         Notification.resend(
             get_object_or_404(DjangoProjectBaseNotification, pk=str(options["notification"])), str(options["user"])
         )
         return "ok"
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/migrations/0001_initial.py` & `django-project-base-0.75.30/django_project_base/notifications/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py` & `django-project-base-0.75.30/django_project_base/notifications/migrations/0002_remove_djangoprojectbasenotification_project_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py` & `django-project-base-0.75.30/django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/migrations/0005_merge_20230906_1213.py` & `django-project-base-0.75.30/django_project_base/notifications/migrations/0005_merge_20230906_1213.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py` & `django-project-base-0.75.30/django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/migrations/0007_auto_20231026_0555.py` & `django-project-base-0.75.30/django_project_base/notifications/migrations/0007_auto_20231026_0555.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/migrations/0009_auto_20231108_0658.py` & `django-project-base-0.75.30/django_project_base/notifications/migrations/0009_auto_20231108_0658.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/models.py` & `django-project-base-0.75.30/django_project_base/notifications/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import datetime
 import uuid
 
 import swapper
+
 from django.contrib.auth import get_user_model
 from django.contrib.contenttypes.models import ContentType
 from django.core.validators import int_list_validator
 from django.db import models, OperationalError, ProgrammingError
 from django.db.models import SET_NULL, Value
 from django.db.models.functions import Concat
 from django.utils.translation import gettext_lazy as _
@@ -75,14 +76,15 @@
     content_entity_context = models.TextField()
     counter = models.SmallIntegerField(default=1)
     recipients_original_payload = models.CharField(blank=False, null=False, max_length=2048)
     recipients_original_payload_search = models.TextField(blank=False, null=True, db_index=True)
     project_slug = models.CharField(null=True, blank=True, max_length=1024)
     send_notification_sms = models.BooleanField(null=False, blank=False, default=False)
     send_notification_sms_text = models.TextField(blank=False, null=True)
+    extra_data = models.JSONField(null=True, blank=False)
 
     class Meta:
         abstract = True
         verbose_name = "Notification"
 
 
 class DjangoProjectBaseNotification(AbstractDjangoProjectBaseNotification):
@@ -130,14 +132,19 @@
 
     sender = property(_get_sender, _set_sender)
 
     email_list = property(_get_email_list, _set_email_list)
 
     email_fallback = property(_get_email_fallback, _set_email_fallback)
 
+    @property
+    def recipients_raw(self):
+        ids = [int(recipients_id) for recipients_id in self.recipients.split(",")] if self.recipients else []
+        return swapper.load_model("django_project_base", "Profile").objects.filter(id__in=ids)
+
 
 class SearchItemObject:
     label = ""
 
     def __init__(self, dict_val):
         for key, value in dict_val.items():
             setattr(self, key, value)
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/notification_queryset.py` & `django-project-base-0.75.30/django_project_base/notifications/notification_queryset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+
 from typing import Optional
 
 from django.conf import settings
 from django.core.cache import cache
 
 from django_project_base.base.queryset_with_cache import QuerySetWithCache
 from django_project_base.notifications.base.enums import NotificationType
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/rest/delivery_report.py` & `django-project-base-0.75.30/django_project_base/notifications/rest/delivery_report.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
 import logging
 import uuid
+
 from gettext import gettext
 from typing import Optional
 
 from django.utils.module_loading import import_string
 from rest_framework import viewsets
 from rest_framework.authentication import BasicAuthentication, TokenAuthentication
 from rest_framework.exceptions import ErrorDetail, ValidationError
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/rest/maintenance_notification.py` & `django-project-base-0.75.30/django_project_base/notifications/rest/maintenance_notification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import datetime
+
 from typing import Optional
 
 from django.conf import settings
 from django.db import transaction
 from django.utils.translation import gettext_lazy as _
 from drf_spectacular.utils import extend_schema, extend_schema_view, OpenApiParameter
 from dynamicforms.serializers import ModelSerializer as DFSerializer
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/rest/notification.py` & `django-project-base-0.75.30/django_project_base/notifications/rest/notification.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import datetime
 import json
 import time
+
 from typing import List, Optional
 
 import pytz
 import swapper
+
+from django.conf import settings
 from django.contrib.auth import get_user_model
 from django.contrib.contenttypes.models import ContentType
 from django.core.cache import cache
 from django.db.models import ForeignKey, QuerySet
 from django.http import Http404, HttpResponse
 from django.shortcuts import render
 from django.urls import reverse
@@ -44,15 +47,15 @@
 from django_project_base.utils import get_host_url, get_pk_name
 
 
 class MessageBodyField(fields.RTFField):
     def __init__(self, *args, **kw):
         kw["write_only"] = True
         kw["label"] = _("Body")
-        kw["display_table"] = DisplayMode.HIDDEN
+        kw["display_table"] = DisplayMode.SUPPRESS
         super().__init__(*args, **kw)
         # TODO: if field is write only and not present in model serializer table, field is not rendered
         self.render_params["form_component_name"] = "DCKEditor"
 
 
 class OrginalRecipientsField(fields.CharField):
     def to_representation(self, value, row_data=None):
@@ -116,47 +119,54 @@
 
     id = fields.UUIDField(display=DisplayMode.HIDDEN)
 
     subject = fields.SerializerMethodField(display_form=DisplayMode.HIDDEN)
     recipients = fields.CharField(display_form=DisplayMode.HIDDEN, display_table=DisplayMode.HIDDEN)
 
     recipients_original_payload = OrginalRecipientsField(
-        display_form=DisplayMode.HIDDEN, label=_("Recipients"), read_only=True
+        display_form=DisplayMode.HIDDEN, label=_("Recipients"), read_only=True, render_params={"max_width": "20em"}
     )
 
-    required_channels = fields.CharField(display_form=DisplayMode.HIDDEN)
-    sent_channels = fields.CharField(display_form=DisplayMode.HIDDEN)
-    failed_channels = fields.CharField(display_form=DisplayMode.HIDDEN)
-
-    counter = fields.IntegerField(display_form=DisplayMode.HIDDEN)
+    delivery = fields.SerializerMethodField(label=_("Delivery"))
 
     level = fields.CharField(display=DisplayMode.SUPPRESS)
     type = fields.CharField(display=DisplayMode.SUPPRESS)
 
     message = fields.PrimaryKeyRelatedField(
         display_form=DisplayMode.SUPPRESS,
         display_table=DisplayMode.SUPPRESS,
         read_only=True,
     )
 
     actions = Actions(
         TableAction(
             TablePosition.HEADER,
-            _("Add"),
-            title=_("Add new record"),
+            label=_("Add"),
+            title=_("Add new notification"),
             name="add-notification",
             icon="add-circle-outline",
         ),
         TableAction(
             TablePosition.HEADER,
-            _("View license"),
+            label=_("View license"),
             title=_("View license"),
             name="view-license",
             icon="card-outline",
         ),
+        TableAction(TablePosition.ROW_CLICK, _("Edit"), title=_("Edit record"), name="edit", icon="pencil-outline"),
+        FormButtonAction(
+            btn_type=FormButtonTypes.CANCEL,
+            name="cancel",
+        ),
+        FormButtonAction(
+            btn_type=FormButtonTypes.SUBMIT,
+            label=_("Send"),
+            name="submit",
+        ),
+        add_form_buttons=False,
     )
 
     message_to = fields.ManyRelatedField(
         child_relation=fields.PrimaryKeyRelatedField(
             queryset=SearchItems.objects.get_queryset(),
             required=True,
         ),
@@ -188,15 +198,35 @@
                 ),
             ),
         ),
         label=_("Send notification SMS"),
         display_table=DisplayMode.HIDDEN,
     )
 
-    sent_at = ReadOnlyDateTimeFieldFromTs(display_form=DisplayMode.HIDDEN, read_only=True, allow_null=True)
+    created_at = ReadOnlyDateTimeFieldFromTs(
+        label=_("Sent"),
+        display_form=DisplayMode.HIDDEN,
+        read_only=True,
+        allow_null=True,
+    )
+
+    def get_delivery(self, rec: DjangoProjectBaseNotification):
+        req_channels = rec.required_channels.split(",") if rec.required_channels else []
+        sent_channels = set(rec.sent_channels.split(",")) if rec.sent_channels else set()
+        failed_channels = set(rec.failed_channels.split(",")) if rec.failed_channels else set()
+        res = []
+        for channel in req_channels:
+            if channel in sent_channels:
+                res.append(f'{channel} <span style="color: green">\u2714</span>')
+            elif channel in failed_channels:
+                title_attr = f"title=\"{rec.exceptions if rec.exceptions else ''}\""
+                res.append(f'{channel} <span style="color: red" {title_attr}>\u2717</span>')
+            else:
+                res.append(f"{channel}")
+        return ",".join(res)
 
     def to_representation(self, instance, row_data=None):
         repr = super().to_representation(instance, row_data)
         kw = getattr(self.context.get("view", object()), "kwargs", dict())
         if kw.get("pk") == "new" and kw.get("format") == "componentdef":
             # enable conditional field render in DF
             repr["send_on_channels"] = []
@@ -208,42 +238,44 @@
         return obj.message.subject
 
     class Meta:
         model = DjangoProjectBaseNotification
         exclude = (
             "content_entity_context",
             "locale",
-            "created_at",
+            "sent_at",
             "delayed_to",
             "recipients_original_payload_search",
             "exceptions",
+            "extra_data",
+            "counter",
+            "required_channels",
+            "sent_channels",
+            "failed_channels",
         )
         layout = Layout(
             Row(Column("message_to")),
-            Row(
-                Column("message_subject"),
-            ),
+            Row(Column("message_subject")),
             Row(Column("message_body")),
             Row(Column("send_on_channels")),
             size="large",
         )
         responsive_columns = ResponsiveTableLayouts(
+            auto_generate_single_row_layout=True,
+            auto_generate_single_column_layout=False,
             layouts=[
-                ResponsiveTableLayout(),
                 ResponsiveTableLayout(
-                    "recipients_original_payload",
-                    "subject",
-                    "required_channels",
-                    "sent_channels",
-                    "failed_channels",
-                    "counter",
-                    "sent_at",
-                    auto_add_non_listed_columns=False,
+                    "subject", "recipients_original_payload", "created_at", auto_add_non_listed_columns=False
                 ),
-            ]
+                ResponsiveTableLayout(
+                    [["subject", "created_at"], "recipients_original_payload"], auto_add_non_listed_columns=False
+                ),
+                ResponsiveTableLayout("subject", "created_at", auto_add_non_listed_columns=False),
+                ResponsiveTableLayout(["subject", "created_at"], auto_add_non_listed_columns=False),
+            ],
         )
 
 
 class MessageToListField(fields.ListField):
     def __init__(self, **kw):
         super().__init__(
             child=fields.CharField(),
@@ -329,21 +361,26 @@
     authentication_classes = [
         SessionAuthentication,
         BasicAuthentication,
         TokenAuthentication,
     ]
     permission_classes = [IsAuthenticated]
 
+    def get_permissions(self):
+        if self.action in ("notification_login", "notification_view"):
+            return []
+        else:
+            return super().get_permissions()
+
     @extend_schema(exclude=True)
     @action(
         detail=True,
         methods=["GET"],
         url_name="notification-login",
         url_path="info",
-        permission_classes=[],
         authentication_classes=[],
     )
     def notification_login(self, request, pk=None) -> HttpResponse:
         if not pk:
             raise PermissionDenied
         return render(
             request,
@@ -358,15 +395,14 @@
         )
 
     @extend_schema(exclude=True)
     @action(
         methods=["POST"],
         detail=False,
         url_name="notification-view",
-        permission_classes=[],
         authentication_classes=[],
         url_path="info-view",
     )
     def notification_view(self, request: Request, *args, **kwargs) -> HttpResponse:
         number: Optional[str] = request.data.get("number")
         identifier: Optional[str] = request.data.get("identifier")
         guest_accesses: List[float] = cache.get(identifier, [])
@@ -395,15 +431,15 @@
         return render(
             request,
             "notification.html",
             dict(message=notification.message.subject + "</br></br></br>" + notification.message.body),
         )
 
     def filter_queryset_field(self, queryset, field, value):
-        if field == "sent_at" and value and not value.isnumeric():
+        if field == "created_at" and value and not value.isnumeric():
             # TODO: search by user defined time range
             value = int(datetime.datetime.strptime(value, "%Y-%m-%dT%H:%M:%S.%fZ").timestamp())
             return queryset.filter(**{f"{field}__gte": value - 1800, f"{field}__lte": value + 1800})
 
         if field == "recipients_original_payload" and value:
             return queryset.filter(**{"recipients_original_payload_search__icontains": value})
         return super().filter_queryset_field(queryset, field, value)
@@ -426,15 +462,15 @@
             return NewMessageSerializer
         return NotificationSerializer
 
     def get_queryset(self):
         try:
             return DjangoProjectBaseNotification.objects.filter(
                 project_slug=self.request.selected_project_slug
-            ).order_by("-sent_at")
+            ).order_by("-created_at")
         except ProjectNotSelectedError as e:
             raise NotFound(e.message)
 
     def _create_notification(self, serializer):
         host_url = get_host_url(self.request)
         notification = Notification(
             message=DjangoProjectBaseMessage(
@@ -446,15 +482,15 @@
             raw_recipents=self.request.data["message_to"],
             project=swapper.load_model("django_project_base", "Project")
             .objects.get(slug=self.request.selected_project_slug)
             .slug,
             recipients=serializer.validated_data["message_to"],
             delay=int(datetime.datetime.now().timestamp()),
             channels=[
-                ChannelIdentifier.channel(c, extra_data=None, project_slug=None).__class__
+                ChannelIdentifier.channel(c, settings=settings, project_slug=None).__class__
                 for c in serializer.validated_data["send_on_channels"]
             ],
             persist=True,
             user=self.request.user.pk,
             send_notification_sms=serializer.validated_data["send_notification_sms"],
             host_url=host_url,
         )
@@ -468,45 +504,38 @@
         kwargs.pop("pk", None)
         return super().create(request, *args, **kwargs)
 
     def perform_create(self, serializer):
         return self._create_notification(serializer)
 
 
-class ChannelSerializer(Serializer):
-    available = fields.FloatField(read_only=True, display_table=DisplayMode.HIDDEN)
-
-
-class ChannelsSerializer(Serializer):
-    def __init__(self, *args, is_filter: bool = False, **kwds):
-        super().__init__(*args, is_filter=is_filter, **kwds)
-        for channel in ChannelIdentifier.supported_channels():
-            self.fields[channel.name] = ChannelSerializer()
-
-
 class NotificationsLicenseSerializer(LicenseReportSerializer):
     template_context = dict(url_reverse="notification-license")
 
     def __init__(self, *args, is_filter: bool = False, **kwds):
         super().__init__(*args, is_filter=is_filter, **kwds)
         if (request := self.context.get("request")) and not fields.BooleanField().to_internal_value(
             request.query_params.get("decorate-max-price", "0")
         ):
             self.fields.pop("max_notification_price", None)
+        for channel in ChannelIdentifier.supported_channels():
+            self.fields[channel.name] = fields.IntegerField(read_only=True, label=_(channel.name))
 
     usage_report = None
-    channels = ChannelsSerializer()
     max_notification_price = fields.FloatField(read_only=True, display_table=DisplayMode.HIDDEN)
     actions = Actions(
         FormButtonAction(btn_type=FormButtonTypes.CANCEL, name="cancel"),
         add_default_crud=False,
         add_default_filter=False,
         add_form_buttons=False,
     )
 
+    class Meta:
+        layout = Layout(Row("credit", "used_credit", "remaining_credit"), Row("EMail", "SMS"))
+
 
 class NotificationsLicenseViewSet(SingleRecordViewSet):
     serializer_class = NotificationsLicenseSerializer
 
     permission_classes = (IsAuthenticated,)
 
     def new_object(self):
@@ -524,16 +553,15 @@
 
         license["channels"] = {}
         max_price = 0
         for channel in ChannelIdentifier.supported_channels():
             price = channel.notification_price
             if price > max_price:
                 max_price = price
-            license["channels"][channel.name] = {}
-            license["channels"][channel.name]["available"] = int(max([license["remaining_credit"] / price, 0]))
+            license[channel.name] = int(max([license["remaining_credit"] / price, 0]))
         if fields.BooleanField().to_internal_value(self.request.query_params.get("decorate-max-price", "0")):
             license["max_notification_price"] = max_price
 
         return NotificationsLicenseSerializer(license).data
 
     def create(self, request, *args, **kwargs) -> Response:
         return Response(status=status.HTTP_501_NOT_IMPLEMENTED)
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/rest/router.py` & `django-project-base-0.75.30/django_project_base/notifications/rest/router.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,28 +8,12 @@
 class NotificationsRouter(DefaultRouter):
     pass
 
 
 notifications_router: NotificationsRouter = DefaultRouter()
 
 notifications_router.register(
-    r"maintenance-notification",
-    UsersMaintenanceNotificationViewset,
-    basename="maintenance-notification",
-)
-notifications_router.register(
-    r"notification",
-    NotificationViewset,
-    basename="notification",
-)
-
-notifications_router.register(
-    r"notification-license",
-    NotificationsLicenseViewSet,
-    basename="notification-license",
-)
-
-notifications_router.register(
-    r"notification-dlr",
-    DeliveryReportViewSet,
-    basename="notification-dlr",
+    r"maintenance-notification", UsersMaintenanceNotificationViewset, basename="maintenance-notification"
 )
+notifications_router.register(r"notification", NotificationViewset, basename="notification")
+notifications_router.register(r"notification-license", NotificationsLicenseViewSet, basename="notification-license")
+notifications_router.register(r"notification-dlr", DeliveryReportViewSet, basename="notification-dlr", )
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/settings.py` & `django-project-base-0.75.30/django_project_base/notifications/settings.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/templates/notification.html` & `django-project-base-0.75.30/django_project_base/notifications/templates/notification.html`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/templates/notification_login.html` & `django-project-base-0.75.30/django_project_base/notifications/templates/notification_login.html`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/tests/api/test_create_mail.py` & `django-project-base-0.75.30/django_project_base/notifications/tests/api/test_create_mail.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/tests/api/test_list_mail.py` & `django-project-base-0.75.30/django_project_base/notifications/tests/api/test_list_mail.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/tests/api/test_remainig_license.py` & `django-project-base-0.75.30/django_project_base/notifications/tests/api/test_remainig_license.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+from django.conf import settings
+
 from django_project_base.licensing.logic import LogAccessService
 from django_project_base.notifications.base.enums import ChannelIdentifier
 from django_project_base.notifications.tests.notifications_transaction_test_case import NotificationsTransactionTestCase
 
 
 class TestRemainingLicense(NotificationsTransactionTestCase):
     def test_remaining_license(self):
         mail = self.create_notification_email_object().send()
         log_service = LogAccessService()
         usage = log_service.report(user=self.test_user)
         credit = log_service._user_access_user_inflow(self.test_user.pk)
-        channel = ChannelIdentifier.channel(mail.required_channels.split(",")[0], ensure_dlr_user=False)
+        channel = ChannelIdentifier.channel(
+            mail.required_channels.split(",")[0], ensure_dlr_user=False, settings=settings
+        )
         self.assertEqual(credit - channel.notification_price, usage["remaining_credit"])
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/tests/api/test_retrieve_mail.py` & `django-project-base-0.75.30/django_project_base/notifications/tests/api/test_retrieve_mail.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/tests/notifications_transaction_test_case.py` & `django-project-base-0.75.30/django_project_base/notifications/tests/notifications_transaction_test_case.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/notifications/tests/unit/test_is_mail_sent.py` & `django-project-base-0.75.30/django_project_base/notifications/tests/unit/test_is_mail_sent.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import uuid
 
+from django.conf import settings
+
 from django_project_base.licensing.logic import LogAccessService
 from django_project_base.notifications.base.channels.channel import Recipient
 from django_project_base.notifications.base.enums import ChannelIdentifier
 from django_project_base.notifications.base.notification import Notification
 from django_project_base.notifications.models import DeliveryReport, DjangoProjectBaseNotification
 from django_project_base.notifications.tests.notifications_transaction_test_case import (
     NotificationsTransactionTestCase,
@@ -23,15 +25,17 @@
     def test_resend_email(self):
         lic_start = LogAccessService().report(self.test_user)
         notification: DjangoProjectBaseNotification = self.create_notification_email_object().send()
         lic_first_sent = LogAccessService().report(self.test_user)
         self.assertIsNotNone(notification.sent_at)
         self.assertFalse(bool(notification.failed_channels))
         self.assertEqual(notification.required_channels, notification.sent_channels)
-        channel = ChannelIdentifier.channel(notification.required_channels.split(",")[0], ensure_dlr_user=False)
+        channel = ChannelIdentifier.channel(
+            notification.required_channels.split(",")[0], ensure_dlr_user=False, settings=settings
+        )
         dlr_pk = str(uuid.uuid4())
         dlr_count = DeliveryReport.objects.all().count()
         resend_data = channel._make_send(
             notification_obj=notification,
             rec_obj=Recipient(identifier=str(self.test_user.pk), phone_number="+38634000000", email="xyz@xyz.xyz"),
             message_str="message",
             dlr_pk=dlr_pk,
```

### Comparing `django-project-base-0.4.9/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py` & `django-project-base-0.75.30/django_project_base/notifications/tests/unit/test_is_phone_number_valid.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/profiling/middleware.py` & `django-project-base-0.75.30/django_project_base/profiling/middleware.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import importlib
 import json
 import os
 import re
 import socket
 import threading
 import time
+
 from typing import Optional
 
 from django.conf import settings
 from django.core.cache import cache
 from django.db import connections
 
 DEFAULT_MAX_LOG_FILE_SIZE = 10000000
@@ -76,18 +77,18 @@
         # # Code to be executed for each request/response after
         # # the view is called.
         tms = os.times()
         self._end_time = (int(time.time() * 1000), int(tms.user * 1000), int(tms.system * 1000))
         self._do_profile(self.response, self._start_time, self._end_time)
 
     def _set_profiling_path(self, path_info, query_string):
-        threading.currentThread().profiling_path = (path_info, query_string)
+        threading.current_thread().profiling_path = (path_info, query_string)
 
     def _get_profiling_path(self) -> tuple:
-        return threading.currentThread().profiling_path
+        return threading.current_thread().profiling_path
 
     def _get_path_info(self, path: str, params: Optional[str] = None):
         original_path = path
         path = path.strip("/")
         if "robots.txt" in path:
             return "other"
         if any(x in path for x in (".php", ".map")):
```

### Comparing `django-project-base-0.4.9/django_project_base/profiling/performance_base_command.py` & `django-project-base-0.75.30/django_project_base/profiling/performance_base_command.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/profiling/views.py` & `django-project-base-0.75.30/django_project_base/profiling/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import random
+
 from datetime import datetime
 
 from django.core.cache import cache
 from django.shortcuts import render
 from dynamicforms.struct import Struct
 
 from django_project_base.settings import PROFILER_LOG_LONG_REQUESTS_COUNT
```

### Comparing `django-project-base-0.4.9/django_project_base/rest/project.py` & `django-project-base-0.75.30/django_project_base/rest/project.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import copy
+
 from gettext import gettext
 from typing import Union
 
 import swapper
+
 from django.conf import settings
 from django.core.management import call_command
 from django.db import transaction
 from django.http import Http404
 from django.shortcuts import get_object_or_404
 from drf_spectacular.utils import extend_schema, OpenApiResponse
 from dynamicforms import fields
@@ -25,14 +27,15 @@
 from django_project_base.account.middleware import ProjectNotSelectedError
 from django_project_base.base.event import (
     ProjectSettingConfirmedEvent,
     ProjectSettingPendingResetEvent,
     SmsSenderChangedEvent,
 )
 from django_project_base.base.models import BaseProjectSettings
+from django_project_base.base.permissions import CreateAny, IsProjectOwnerOrReadOnly
 from django_project_base.constants import EMAIL_SENDER_ID_SETTING_NAME, SMS_SENDER_ID_SETTING_NAME
 from django_project_base.utils import get_pk_name
 
 
 class ProjectSerializer(ModelSerializer):
     template_context = dict(url_reverse="project-base-project")
 
@@ -52,14 +55,15 @@
         model = swapper.load_model("django_project_base", "Project")
         exclude = ("logo",)  # TODO we currently don't support logos well. see DPB #3
         layout = Layout(Row("name"), Row("slug"), Row("description"))
 
 
 class ProjectViewSet(ModelViewSet):
     serializer_class = ProjectSerializer
+    permission_classes = (IsProjectOwnerOrReadOnly | CreateAny,)
 
     def new_object(self: ModelViewSet):
         new_object = super().new_object()
         if self.request and self.request.user and self.request.user.is_authenticated:
             new_object.owner = getattr(
                 self.request.user, swapper.load_model("django_project_base", "Profile")._meta.model_name
             )
@@ -82,27 +86,32 @@
 
     def get_queryset(self):
         return ProjectViewSet._get_queryset_for_request(self.request)
 
     def get_serializer(self, *args, **kwargs):
         return super().get_serializer(*args, **kwargs)
 
+    def get_permissions(self):
+        if self.action == "get_current_project":
+            return [IsAuthenticated()]
+        else:
+            return super().get_permissions()
+
     @extend_schema(
         description="Get currently selected project",
         responses={
             status.HTTP_200_OK: OpenApiResponse(description="OK"),
             status.HTTP_403_FORBIDDEN: OpenApiResponse(description="Not allowed"),
         },
     )
     @action(
         methods=["GET"],
         detail=False,
         url_path="current",
         url_name="project-current",
-        permission_classes=[IsAuthenticated],
     )
     def get_current_project(self, request: Request, **kwargs) -> Response:
         try:
             request.selected_project.get_deferred_fields()  # force immediate LazyObject evaluation
             serializer = self.get_serializer(request.selected_project)
         except ProjectNotSelectedError as e:
             raise NotFound(e.message)
@@ -256,17 +265,17 @@
         if obj and obj.action_required:
             return "background-color:red;"
         return ""
 
     def to_representation(self, instance, row_data=None):
         representation = super().to_representation(instance, row_data)
         if instance and instance.pending_value is not None:
-            representation[
-                "table_value"
-            ] = f"{representation['value']} ({gettext('Pending')}: {instance.python_pending_value})"
+            representation["table_value"] = (
+                f"{representation['value']} ({gettext('Pending')}: {instance.python_pending_value})"
+            )
         return representation
 
     class Meta:
         model = swapper.load_model("django_project_base", "ProjectSettings")
         fields = (
             get_pk_name(model),
             "name",
```

### Comparing `django-project-base-0.4.9/django_project_base/rest/project_role.py` & `django-project-base-0.75.30/django_project_base/rest/project_role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Optional
 
 import swapper
+
 from django.db.models import Model
 from django.shortcuts import get_object_or_404
 from django.utils.translation import gettext_lazy as _
 from dynamicforms import fields
 from dynamicforms.fields import AutoGeneratedField
 from dynamicforms.mixins import DisplayMode
 from dynamicforms.serializers import ModelSerializer
```

### Comparing `django-project-base-0.4.9/django_project_base/router.py` & `django-project-base-0.75.30/django_project_base/router.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/settings.py` & `django-project-base-0.75.30/django_project_base/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -37,20 +37,22 @@
             "RESET_PASSWORD_SERIALIZER_PASSWORD_CONFIRM": True,
             "SEND_RESET_PASSWORD_LINK_USER_FINDER": "django_project_base.account.service.reset_password_email_service.find_user_by_send_reset_password_link_data",  # noqa: E501
             "REGISTER_VERIFICATION_ENABLED": True,
             "REGISTER_VERIFICATION_EMAIL_SENDER": "django_project_base.account.service.register_user_service.send_register_verification_email_notification",  # noqa: E501
         },
     },
     {"name": "NOTIFICATION_SENDERS", "default": {}},
+    {"name": "SYSTEM_EMAIL_SENDER_ID", "default": ""},
+    {"name": "SYSTEM_SMS_SENDER_ID", "default": ""},
     {
-        "name": "EMAIL_PROVIDER",
+        "name": "NOTIFICATIONS_EMAIL_PROVIDER",
         "default": "django_project_base.notifications.base.channels.integrations.aws_ses.AwsSes",
     },
     {
-        "name": "SMS_PROVIDER",
+        "name": "NOTIFICATIONS_SMS_PROVIDER",
         "default": [
             "django_project_base.notifications.base.channels.integrations.t2.T2",
             "django_project_base.notifications.base.channels.integrations.aws_sns_single_sms.AwsSnsSingleSMS",
             "django_project_base.notifications.base.channels.integrations.nexmo_sms.NexmoSMS",
         ],
     },
     # this settings silences (rest_registration.E013) SEND_RESET_PASSWORD_LINK_SERIALIZER_USE_EMAIL
```

### Comparing `django-project-base-0.4.9/django_project_base/settings_parser.py` & `django-project-base-0.75.30/django_project_base/settings_parser.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/static/browser-update/update.min.js` & `django-project-base-0.75.30/django_project_base/static/browser-update/update.min.js`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/templates/app-debug/main.html` & `django-project-base-0.75.30/django_project_base/templates/app-debug/main.html`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/urls.py` & `django-project-base-0.75.30/django_project_base/urls.py`

 * *Files identical despite different names*

### Comparing `django-project-base-0.4.9/django_project_base/utils.py` & `django-project-base-0.75.30/django_project_base/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from enum import IntEnum
-from typing import Dict, Union
+from typing import Dict, TYPE_CHECKING, Union
 
 from django.db.models import Model, QuerySet
 from django.http import HttpRequest
-from dynamicforms.serializers import Serializer
 from rest_framework.utils.model_meta import get_field_info
 
+if TYPE_CHECKING:
+    from dynamicforms.serializers import Serializer
+
 
 def set_django_security(django_settings, deploy=True, swagger_version=None):
     """
     Sets django web security settings.
     Call this from settings.py
 
     :param django_settings: globals() of your application
@@ -49,15 +51,15 @@
     django_settings["CSRF_COOKIE_SAMESITE"] = "Strict"
     django_settings["SESSION_COOKIE_SAMESITE"] = "Strict"
 
     # CSP can be changed per request... with decorator:
     #  https://django-csp.readthedocs.io/en/latest/decorators.html#decorator-chapter
     # Content Security Policy
     django_settings["CSP_DEFAULT_SRC"] = [
-        "'none'",
+        "'none'" if deploy else "'self'",
     ]
     # stackpath.bootstrapcdn.com - because of (old) login
     django_settings["CSP_STYLE_SRC"] = [
         "'self'",
         "'unsafe-inline'",
         "cdnjs.cloudflare.com",
         "stackpath.bootstrapcdn.com",
@@ -86,17 +88,18 @@
     ]
     django_settings["CSP_OBJECT_SRC"] = [
         "'none'",
     ]
     django_settings["CSP_BASE_URI"] = [
         "'self'",
     ]
-    django_settings["CSP_FRAME_ANCESTORS"] = [
-        "'none'",
-    ]
+    # TODO temp removed because we're rendering all legacy pages as iframes when everything is moved to vue, reenable
+    # django_settings["CSP_FRAME_ANCESTORS"] = [
+    #     "'none'",
+    # ]
     django_settings["CSP_FORM_ACTION"] = [
         "'self'",
     ]
 
     django_settings["PERMISSIONS_POLICY"] = {
         "accelerometer": [],
         "ambient-light-sensor": [],
@@ -145,15 +148,15 @@
         return tuple((item, item.description) for item in cls)
 
     @classmethod
     def has_value(cls, value):
         return value in cls.__members__.values()
 
 
-def get_pk_name(obj: Union[Model, QuerySet, Dict, Serializer], model: Model = None):
+def get_pk_name(obj: Union[Model, QuerySet, Dict, "Serializer"], model: Model = None):
     if isinstance(obj, QuerySet):
         return obj.model._meta.pk.name
     if isinstance(obj, Model):
         return obj._meta.pk.name
     return get_field_info(model if model else obj).pk.name
```

### Comparing `django-project-base-0.4.9/django_project_base/views.py` & `django-project-base-0.75.30/django_project_base/views.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import requests
+
 from django.http import FileResponse, HttpResponse
 from django.views import static
 
 
 def documentation_view(request: object, path="", document_root=None) -> FileResponse:
     if not path:
         path = "index.html"
```

### Comparing `django-project-base-0.4.9/django_project_base.egg-info/PKG-INFO` & `django-project-base-0.75.30/django_project_base.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: django-project-base
-Version: 0.4.9
+Version: 0.75.30
 Summary: Everything revolves around it: users, roles, permissions, tags, etc.
 Home-page: https://github.com/velis74/django-project-base
 Author: Jure Erznožnik
 Author-email: jure@velis.si
 License: BSD-3-Clause
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: Django
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -53,9 +52,7 @@
 To generate pdf file. Run:
 
 ```bash 
 $ npm run export-pdf  
 ```
 
 Pdf file is located in docs/pdf folder.
-
-
```

### Comparing `django-project-base-0.4.9/django_project_base.egg-info/SOURCES.txt` & `django-project-base-0.75.30/django_project_base.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.txt
 setup.py
 django_project_base/__init__.py
 django_project_base/apps.py
 django_project_base/constants.py
 django_project_base/country_holidays.py
 django_project_base/models.py
@@ -66,14 +67,15 @@
 django_project_base/base/queryset_with_cache.py
 django_project_base/base/signals.py
 django_project_base/celery/__init__.py
 django_project_base/celery/apps.py
 django_project_base/celery/celery.py
 django_project_base/celery/settings.py
 django_project_base/celery/background_tasks/__init__.py
+django_project_base/celery/background_tasks/base_task.py
 django_project_base/celery/background_tasks/notification_tasks.py
 django_project_base/licensing/__init__.py
 django_project_base/licensing/apps.py
 django_project_base/licensing/logic.py
 django_project_base/licensing/models.py
 django_project_base/licensing/urls.py
 django_project_base/licensing/migrations/0001_initial.py
@@ -106,15 +108,15 @@
 django_project_base/notifications/utils.py
 django_project_base/notifications/base/__init__.py
 django_project_base/notifications/base/duplicate_notification_mixin.py
 django_project_base/notifications/base/enums.py
 django_project_base/notifications/base/notification.py
 django_project_base/notifications/base/phone_number_parser.py
 django_project_base/notifications/base/queable_notification_mixin.py
-django_project_base/notifications/base/send_notification_mixin.py
+django_project_base/notifications/base/send_notification_service.py
 django_project_base/notifications/base/channels/__init__.py
 django_project_base/notifications/base/channels/channel.py
 django_project_base/notifications/base/channels/mail_channel.py
 django_project_base/notifications/base/channels/sms_channel.py
 django_project_base/notifications/base/channels/websocket_channel.py
 django_project_base/notifications/base/channels/integrations/__init__.py
 django_project_base/notifications/base/channels/integrations/aws_ses.py
@@ -132,14 +134,15 @@
 django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options.py
 django_project_base/notifications/migrations/0004_alter_djangoprojectbasenotification_options_and_more.py
 django_project_base/notifications/migrations/0005_merge_20230906_1213.py
 django_project_base/notifications/migrations/0006_djangoprojectbasenotification_send_notification_sms.py
 django_project_base/notifications/migrations/0007_auto_20231026_0555.py
 django_project_base/notifications/migrations/0008_deliveryreport_auxiliary_notification.py
 django_project_base/notifications/migrations/0009_auto_20231108_0658.py
+django_project_base/notifications/migrations/0010_djangoprojectbasenotification_extra_data.py
 django_project_base/notifications/migrations/__init__.py
 django_project_base/notifications/rest/__init__.py
 django_project_base/notifications/rest/delivery_report.py
 django_project_base/notifications/rest/maintenance_notification.py
 django_project_base/notifications/rest/notification.py
 django_project_base/notifications/rest/router.py
 django_project_base/notifications/templates/account_created.html
```

### Comparing `django-project-base-0.4.9/setup.py` & `django-project-base-0.75.30/setup.py`

 * *Files identical despite different names*

