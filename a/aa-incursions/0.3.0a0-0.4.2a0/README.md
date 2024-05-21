# Comparing `tmp/aa_incursions-0.3.0a0.tar.gz` & `tmp/aa_incursions-0.4.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aa_incursions-0.3.0a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aa_incursions-0.4.2a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aa_incursions-0.3.0a0.tar` & `aa_incursions-0.4.2a0.tar`

### file list

```diff
@@ -1,77 +1,52 @@
--rw-r--r--   0        0        0     1069 2023-08-02 06:03:24.928765 aa_incursions-0.3.0a0/LICENSE
--rw-r--r--   0        0        0     2529 2023-10-11 09:23:15.287264 aa_incursions-0.3.0a0/README.md
--rw-r--r--   0        0        0       85 2023-10-08 07:07:41.571529 aa_incursions-0.3.0a0/incursions/__init__.py
--rw-r--r--   0        0        0      923 2023-08-07 02:39:06.173527 aa_incursions-0.3.0a0/incursions/admin.py
--rw-r--r--   0        0        0      289 2023-08-02 06:26:44.468347 aa_incursions-0.3.0a0/incursions/app_settings.py
--rw-r--r--   0        0        0      299 2023-06-19 05:41:16.429155 aa_incursions-0.3.0a0/incursions/apps.py
--rw-r--r--   0        0        0      133 2023-06-19 05:41:28.569151 aa_incursions-0.3.0a0/incursions/auth_hooks.py
--rw-r--r--   0        0        0     4775 2023-08-07 02:41:20.223467 aa_incursions-0.3.0a0/incursions/cogs/incursions.py
--rw-r--r--   0        0        0      417 2023-10-11 04:08:15.465302 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_11-30-01.json.bz2
--rw-r--r--   0        0        0      415 2023-10-11 04:08:16.545302 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_11-35-01.json.bz2
--rw-r--r--   0        0        0      405 2023-10-11 04:08:18.015302 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_11-40-01.json.bz2
--rw-r--r--   0        0        0      402 2023-10-11 04:08:18.865302 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_11-45-01.json.bz2
--rw-r--r--   0        0        0      402 2023-10-11 04:08:19.895301 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_11-50-01.json.bz2
--rw-r--r--   0        0        0      400 2023-10-11 04:08:20.895301 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_11-55-01.json.bz2
--rw-r--r--   0        0        0      402 2023-10-11 04:08:21.585301 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_12-00-01.json.bz2
--rw-r--r--   0        0        0      403 2023-10-11 04:08:22.535301 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_12-05-01.json.bz2
--rw-r--r--   0        0        0      404 2023-10-11 04:08:23.535301 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_12-10-01.json.bz2
--rw-r--r--   0        0        0      397 2023-10-11 04:08:24.445301 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_12-15-01.json.bz2
--rw-r--r--   0        0        0      404 2023-10-11 04:08:25.415301 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_12-20-01.json.bz2
--rw-r--r--   0        0        0      395 2023-10-11 04:08:26.375301 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_12-25-01.json.bz2
--rw-r--r--   0        0        0      403 2023-10-11 04:08:27.335299 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_12-30-01.json.bz2
--rw-r--r--   0        0        0      410 2023-10-11 04:08:28.525295 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_12-35-01.json.bz2
--rw-r--r--   0        0        0      407 2023-10-11 04:08:29.455292 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_12-40-01.json.bz2
--rw-r--r--   0        0        0      403 2023-10-11 04:08:30.545288 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_12-45-01.json.bz2
--rw-r--r--   0        0        0      404 2023-10-11 04:08:31.455287 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_12-50-01.json.bz2
--rw-r--r--   0        0        0      397 2023-10-11 04:08:32.535286 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_12-55-01.json.bz2
--rw-r--r--   0        0        0      405 2023-10-11 04:08:33.545286 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_13-00-01.json.bz2
--rw-r--r--   0        0        0      407 2023-10-11 04:08:35.045286 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_13-05-01.json.bz2
--rw-r--r--   0        0        0      403 2023-10-11 04:08:36.145286 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_13-10-01.json.bz2
--rw-r--r--   0        0        0      406 2023-10-11 04:08:36.925286 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_13-15-01.json.bz2
--rw-r--r--   0        0        0      404 2023-10-11 04:08:37.975287 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_13-20-01.json.bz2
--rw-r--r--   0        0        0      402 2023-10-11 04:08:39.835287 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_13-25-01.json.bz2
--rw-r--r--   0        0        0      410 2023-10-11 04:08:41.195287 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_13-30-01.json.bz2
--rw-r--r--   0        0        0      404 2023-10-11 04:08:42.335287 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_13-35-01.json.bz2
--rw-r--r--   0        0        0      408 2023-10-11 04:08:43.255287 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_13-40-01.json.bz2
--rw-r--r--   0        0        0      406 2023-10-11 04:08:44.435287 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_13-45-01.json.bz2
--rw-r--r--   0        0        0      406 2023-10-11 04:08:45.355287 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_13-50-01.json.bz2
--rw-r--r--   0        0        0      404 2023-10-11 04:08:46.405287 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_13-55-01.json.bz2
--rw-r--r--   0        0        0      409 2023-10-11 04:08:47.585287 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_14-00-01.json.bz2
--rw-r--r--   0        0        0      403 2023-10-11 04:08:48.485287 aa_incursions-0.3.0a0/incursions/data.everef.net/incursions/history/2022/2022-12-20/incursions-2022-12-20_14-05-01.json.bz2
--rw-r--r--   0        0        0     9219 2023-10-08 07:32:06.781351 aa_incursions-0.3.0a0/incursions/helpers.py
--rw-r--r--   0        0        0      400 2023-10-08 04:49:53.732533 aa_incursions-0.3.0a0/incursions/locale/da_DK/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2596 2023-10-08 04:49:40.392534 aa_incursions-0.3.0a0/incursions/locale/da_DK/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      384 2023-10-08 04:49:53.722533 aa_incursions-0.3.0a0/incursions/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2580 2023-10-08 04:49:40.402534 aa_incursions-0.3.0a0/incursions/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      380 2023-10-08 04:49:53.722533 aa_incursions-0.3.0a0/incursions/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2579 2023-10-11 09:23:15.287264 aa_incursions-0.3.0a0/incursions/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      424 2023-10-08 04:49:53.732533 aa_incursions-0.3.0a0/incursions/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2620 2023-10-08 04:49:40.682534 aa_incursions-0.3.0a0/incursions/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      450 2023-10-08 04:49:53.732533 aa_incursions-0.3.0a0/incursions/locale/fr_FR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2646 2023-10-08 04:49:40.682534 aa_incursions-0.3.0a0/incursions/locale/fr_FR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      438 2023-10-08 04:49:53.722533 aa_incursions-0.3.0a0/incursions/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2634 2023-10-08 04:49:40.392534 aa_incursions-0.3.0a0/incursions/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-10-08 04:49:53.722533 aa_incursions-0.3.0a0/incursions/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2575 2023-10-08 04:49:42.552534 aa_incursions-0.3.0a0/incursions/locale/ja/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      391 2023-10-08 04:49:53.722533 aa_incursions-0.3.0a0/incursions/locale/ko_KR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2587 2023-10-08 04:49:42.542534 aa_incursions-0.3.0a0/incursions/locale/ko_KR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      523 2023-10-08 04:49:53.732533 aa_incursions-0.3.0a0/incursions/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2719 2023-10-08 04:49:42.552534 aa_incursions-0.3.0a0/incursions/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      609 2023-10-08 04:49:53.732533 aa_incursions-0.3.0a0/incursions/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2805 2023-10-08 04:49:42.872534 aa_incursions-0.3.0a0/incursions/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      399 2023-10-08 04:49:53.732533 aa_incursions-0.3.0a0/incursions/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     2595 2023-10-08 04:49:42.862534 aa_incursions-0.3.0a0/incursions/locale/zh_Hans/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     4033 2023-08-02 05:43:13.069130 aa_incursions-0.3.0a0/incursions/migrations/0001_initial.py
--rw-r--r--   0        0        0     1944 2023-08-02 05:43:13.049130 aa_incursions-0.3.0a0/incursions/migrations/0002_remove_incursion_influence_and_more.py
--rw-r--r--   0        0        0      831 2023-08-07 02:39:33.343519 aa_incursions-0.3.0a0/incursions/migrations/0003_focus.py
--rw-r--r--   0        0        0      523 2023-08-07 02:39:33.353519 aa_incursions-0.3.0a0/incursions/migrations/0004_alter_focus_incursion.py
--rw-r--r--   0        0        0        0 2023-06-19 03:16:44.542558 aa_incursions-0.3.0a0/incursions/migrations/__init__.py
--rw-r--r--   0        0        0     6376 2023-08-07 02:40:44.343498 aa_incursions-0.3.0a0/incursions/models.py
--rw-r--r--   0        0        0      652 2023-10-11 08:58:56.647438 aa_incursions-0.3.0a0/incursions/providers.py
--rw-r--r--   0        0        0     1249 2023-10-08 06:46:01.991686 aa_incursions-0.3.0a0/incursions/signals.py
--rw-r--r--   0        0        0    84246 2023-06-22 05:52:48.702921 aa_incursions-0.3.0a0/incursions/static_data.py
--rw-r--r--   0        0        0   881823 2023-06-19 04:34:55.670712 aa_incursions-0.3.0a0/incursions/swagger.json
--rw-r--r--   0        0        0     5231 2023-10-11 09:23:15.287264 aa_incursions-0.3.0a0/incursions/tasks.py
--rw-r--r--   0        0        0    38212 2023-10-11 04:08:48.485287 aa_incursions-0.3.0a0/incursions/wget-log
--rw-r--r--   0        0        0     1912 2023-10-08 06:04:14.251991 aa_incursions-0.3.0a0/pyproject.toml
--rw-r--r--   0        0        0     3917 1970-01-01 00:00:00.000000 aa_incursions-0.3.0a0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-21 04:49:40.779788 aa_incursions-0.4.2a0/LICENSE
+-rw-r--r--   0        0        0     2530 2024-05-21 04:49:40.780788 aa_incursions-0.4.2a0/README.md
+-rw-r--r--   0        0        0       85 2024-05-21 04:49:40.780788 aa_incursions-0.4.2a0/incursions/__init__.py
+-rw-r--r--   0        0        0     1200 2024-05-21 04:49:40.780788 aa_incursions-0.4.2a0/incursions/admin.py
+-rw-r--r--   0        0        0      382 2024-05-21 04:49:40.780788 aa_incursions-0.4.2a0/incursions/app_settings.py
+-rw-r--r--   0        0        0      299 2024-05-21 04:49:40.780788 aa_incursions-0.4.2a0/incursions/apps.py
+-rw-r--r--   0        0        0      133 2024-05-21 04:49:40.780788 aa_incursions-0.4.2a0/incursions/auth_hooks.py
+-rw-r--r--   0        0        0     4775 2024-05-21 04:49:40.780788 aa_incursions-0.4.2a0/incursions/cogs/incursions.py
+-rw-r--r--   0        0        0  1705544 2024-05-21 04:49:40.784788 aa_incursions-0.4.2a0/incursions/data.everef.net/incursions/history/backfills/eve-incursions-de-2023-10-12.json.xz
+-rw-r--r--   0        0        0      914 2024-05-21 04:49:40.784788 aa_incursions-0.4.2a0/incursions/data.everef.net/readme.md
+-rw-r--r--   0        0        0     5677 2024-05-21 04:49:40.784788 aa_incursions-0.4.2a0/incursions/everef.py
+-rw-r--r--   0        0        0    59780 2024-05-21 04:49:40.784788 aa_incursions-0.4.2a0/incursions/fixtures/Incursion.json.xz
+-rw-r--r--   0        0        0  1444644 2024-05-21 04:49:40.787788 aa_incursions-0.4.2a0/incursions/fixtures/IncursionInfluence.json.xz
+-rw-r--r--   0        0        0     9653 2024-05-21 04:49:40.787788 aa_incursions-0.4.2a0/incursions/helpers.py
+-rw-r--r--   0        0        0      400 2024-05-21 04:49:40.787788 aa_incursions-0.4.2a0/incursions/locale/da_DK/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2596 2024-05-21 04:49:40.787788 aa_incursions-0.4.2a0/incursions/locale/da_DK/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      384 2024-05-21 04:49:40.788788 aa_incursions-0.4.2a0/incursions/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2580 2024-05-21 04:49:40.788788 aa_incursions-0.4.2a0/incursions/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      380 2024-05-21 04:49:40.788788 aa_incursions-0.4.2a0/incursions/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2884 2024-05-21 04:49:40.788788 aa_incursions-0.4.2a0/incursions/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      424 2024-05-21 04:49:40.788788 aa_incursions-0.4.2a0/incursions/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2620 2024-05-21 04:49:40.788788 aa_incursions-0.4.2a0/incursions/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      450 2024-05-21 04:49:40.788788 aa_incursions-0.4.2a0/incursions/locale/fr_FR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2646 2024-05-21 04:49:40.788788 aa_incursions-0.4.2a0/incursions/locale/fr_FR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      438 2024-05-21 04:49:40.788788 aa_incursions-0.4.2a0/incursions/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2634 2024-05-21 04:49:40.789788 aa_incursions-0.4.2a0/incursions/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2024-05-21 04:49:40.789788 aa_incursions-0.4.2a0/incursions/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2575 2024-05-21 04:49:40.789788 aa_incursions-0.4.2a0/incursions/locale/ja/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      391 2024-05-21 04:49:40.789788 aa_incursions-0.4.2a0/incursions/locale/ko_KR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2587 2024-05-21 04:49:40.789788 aa_incursions-0.4.2a0/incursions/locale/ko_KR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      523 2024-05-21 04:49:40.789788 aa_incursions-0.4.2a0/incursions/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2719 2024-05-21 04:49:40.789788 aa_incursions-0.4.2a0/incursions/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      609 2024-05-21 04:49:40.789788 aa_incursions-0.4.2a0/incursions/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2805 2024-05-21 04:49:40.789788 aa_incursions-0.4.2a0/incursions/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      399 2024-05-21 04:49:40.790788 aa_incursions-0.4.2a0/incursions/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     2595 2024-05-21 04:49:40.790788 aa_incursions-0.4.2a0/incursions/locale/zh_Hans/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     4033 2024-05-21 04:49:40.790788 aa_incursions-0.4.2a0/incursions/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1944 2024-05-21 04:49:40.790788 aa_incursions-0.4.2a0/incursions/migrations/0002_remove_incursion_influence_and_more.py
+-rw-r--r--   0        0        0      831 2024-05-21 04:49:40.790788 aa_incursions-0.4.2a0/incursions/migrations/0003_focus.py
+-rw-r--r--   0        0        0      523 2024-05-21 04:49:40.790788 aa_incursions-0.4.2a0/incursions/migrations/0004_alter_focus_incursion.py
+-rw-r--r--   0        0        0      458 2024-05-21 04:49:40.790788 aa_incursions-0.4.2a0/incursions/migrations/0005_incursioninfluence_uniqueincursioninfluencelogtimestamp.py
+-rw-r--r--   0        0        0      902 2024-05-21 04:49:40.790788 aa_incursions-0.4.2a0/incursions/migrations/0006_alter_incursion_infested_solar_systems_and_more.py
+-rw-r--r--   0        0        0      455 2024-05-21 04:49:40.790788 aa_incursions-0.4.2a0/incursions/migrations/0007_alter_focus_options.py
+-rw-r--r--   0        0        0        0 2024-05-21 04:49:40.828788 aa_incursions-0.4.2a0/incursions/migrations/__init__.py
+-rw-r--r--   0        0        0     6589 2024-05-21 04:49:40.790788 aa_incursions-0.4.2a0/incursions/models.py
+-rw-r--r--   0        0        0      652 2024-05-21 04:49:40.791788 aa_incursions-0.4.2a0/incursions/providers.py
+-rw-r--r--   0        0        0     1462 2024-05-21 04:49:40.791788 aa_incursions-0.4.2a0/incursions/signals.py
+-rw-r--r--   0        0        0    87001 2024-05-21 04:49:40.791788 aa_incursions-0.4.2a0/incursions/static_data.py
+-rw-r--r--   0        0        0   881823 2024-05-21 04:49:40.794788 aa_incursions-0.4.2a0/incursions/swagger.json
+-rw-r--r--   0        0        0     5492 2024-05-21 04:49:40.794788 aa_incursions-0.4.2a0/incursions/tasks.py
+-rw-r--r--   0        0        0     2195 2024-05-21 04:49:40.794788 aa_incursions-0.4.2a0/pyproject.toml
+-rw-r--r--   0        0        0     4018 1970-01-01 00:00:00.000000 aa_incursions-0.4.2a0/PKG-INFO
```

### Comparing `aa_incursions-0.3.0a0/LICENSE` & `aa_incursions-0.4.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/README.md` & `aa_incursions-0.4.2a0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 Incursions is an App for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth/), Please make sure you have this installed. incursions is not a standalone Django Application
 
 Incursions needs the App [django-eveuniverse](https://gitlab.com/ErikKalkoken/django-eveuniverse) to function. Please make sure it is installed before continuing.
 
 ### Step 2 - Install app
 
-```bash
+```shell
 pip install aa-incursions
 ```
 
 ### Step 3 - Configure Auth settings
 
 Configure your Auth settings (`local.py`) as follows:
```

### Comparing `aa_incursions-0.3.0a0/incursions/cogs/incursions.py` & `aa_incursions-0.4.2a0/incursions/cogs/incursions.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/helpers.py` & `aa_incursions-0.4.2a0/incursions/helpers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 import logging
 from datetime import datetime, timedelta
 
 from discord import Colour, Embed
 from eveuniverse.models import EveSolarSystem
+from routing.routing import (
+    route_check_edencom, route_check_triglavian, route_length,
+)
 
 from incursions import __version__
-from incursions.models import Incursion
+from incursions.models import Focus, Incursion
 from incursions.static_data import incursion_constellations
 
 from .app_settings import get_site_url
 
 logger = logging.getLogger(__name__)
 
 
@@ -31,33 +34,34 @@
     embed.description = "PSA: Create and use an Insta-Dock Bookmark when warping to the new dockup. Scout the route ahead including the dockup station."
     embed.add_field(
         name="Region",
         value=f"[{incursion.constellation.eve_region.name}]({incursion.constellation.eve_region.profile_url})",
         inline=True)
     embed.add_field(
         name="Constellation",
-        value=f"[{incursion.constellation.name}]({incursion.constellation.profile_url})")
+        value=f"{incursion.constellation.name}")
     # newline
     embed.add_field(
         name="Headquarters",
         value=incursion_constellations[incursion.constellation.name]["Headquarter"])
     embed.add_field(
         name="Assault",
-        value=incursion_constellations[incursion.constellation.name]["Assaults"],
+        value="".join(incursion_constellations[incursion.constellation.name]["Assaults"]),
         inline=True)
     embed.add_field(
         name="Vanguard",
-        value=incursion_constellations[incursion.constellation.name]["Vanguards"],
+        value="".join(incursion_constellations[incursion.constellation.name]["Vanguards"]),
         inline=True)
     # newline
     embed.add_field(name="Stations in HQ",
                     value=f"{ EveSolarSystem.objects.get(name=incursion_constellations[incursion.constellation.name]['Headquarter']).eve_stations.count() }", inline=True)
     embed.add_field(name="HS Island?",
                     value=f"{incursion.is_island}", inline=True)
-    embed.add_field(name="Jumps from last HQ", value="69420lmao", inline=True)
+    embed.add_field(name="Jumps from last HQ",
+                    value=f"{route_length(incursion.staging_solar_system.id, Focus.get_solo().incursion.staging_solar_system.id)}", inline=True)
     # newline
     embed.add_field(name="Suggested Dockup",
                     value="Not Implemented", inline=True)
     embed.add_field(name="Edencom In Spawn",
                     value="Not Implemented", inline=True)
     embed.add_field(name="Trigs In Spawn",
                     value="Not Implemented", inline=True)
@@ -74,47 +78,56 @@
                     value=f"<t:{ int((incursion.established_timestamp + timedelta(days=4)).timestamp()) }:R>", inline=True)
     embed.add_field(name="Despawn Window Ends",
                     value=f"<t:{ int((incursion.established_timestamp + timedelta(days=8)).timestamp()) }:R>", inline=True)
     # newline
     embed.add_field(name="Max Established Time",
                     value=f"<t:{ int((incursion.established_timestamp + timedelta(days=5)).timestamp()) }:R>")
     embed.add_field(name="HQ to Hek",
-                    value=f"{incursion.staging_solar_system.jumps_to(destination=EveSolarSystem.objects.get(id=30002053)) }", inline=True)
+                    value=f"{route_length(incursion.staging_solar_system.id, 30002053)}", inline=True)
     embed.add_field(name="HQ to Dodixie",
-                    value=f"{incursion.staging_solar_system.jumps_to(destination=EveSolarSystem.objects.get(id=30002659)) }", inline=True)
+                    value=f"{route_length(incursion.staging_solar_system.id, 30002659)}", inline=True)
     # newline
     embed.add_field(name="HQ to Rens",
-                    value=f"{incursion.staging_solar_system.jumps_to(destination=EveSolarSystem.objects.get(id=30002510)) }")
+                    value=f"{route_length(incursion.staging_solar_system.id, 30002510)}")
     embed.add_field(name="HQ to Jita",
-                    value=f"{incursion.staging_solar_system.jumps_to(destination=EveSolarSystem.objects.get(id=30000142)) }", inline=True)
+                    value=f"{route_length(incursion.staging_solar_system.id, 30000142)}", inline=True)
     embed.add_field(name="HQ to Amarr",
-                    value=f"{incursion.staging_solar_system.jumps_to(destination=EveSolarSystem.objects.get(id=30002187)) }", inline=True)
+                    value=f"{route_length(incursion.staging_solar_system.id, 30002187)}", inline=True)
     # newline
     embed.add_field(name="Gank Pipes In Route", value="Not Implemented")
-    embed.add_field(name="Edencom In Route",
-                    value="Not Implemented", inline=True)
-    embed.add_field(name="Edencom In Route",
-                    value="Not Implemented", inline=True)
+    try:
+        embed.add_field(name="Triglavian In Route",
+                        value=str(route_check_triglavian(incursion.staging_solar_system.id, Focus.get_solo().incursion.staging_solar_system.id)), inline=True)
+    except Exception:
+        pass
+    try:
+        embed.add_field(name="Edencom In Route",
+                        value=str(route_check_edencom(incursion.staging_solar_system.id, Focus.get_solo().incursion.staging_solar_system.id)), inline=True)
+    except Exception:
+        pass
     return embed
 
 
 def embed_mobilizing(incursion: Incursion) -> Embed:
     embed = embed_base()
     embed.colour = Colour.yellow()
     embed.title = f"Mobilizing {incursion.security_string}: {incursion.constellation.name}"
     embed.add_field(name="Estimated Withdrawing Time",
                     value=f"<t:{ int((incursion.mobilizing_timestamp + timedelta(days=2)).timestamp()) }:R>", inline=False)
     embed.add_field(name="Estimated Despawn Time",
                     value=f"<t:{ int((incursion.mobilizing_timestamp + timedelta(days=3)).timestamp()) }:R>", inline=False)
-    embed.add_field(name="Max Spawn Stats",
-                    value=f'''
-                        {incursion.mobilizing_timestamp - incursion.established_timestamp} Uptime
-                        {(incursion.mobilizing_timestamp - incursion.established_timestamp) - timedelta(days=5)} Unused
-                        {(incursion.mobilizing_timestamp - incursion.established_timestamp).microseconds / timedelta(days=5).microseconds - 100:.3f}% total possible `established` time used")
-                    ''')
+    try:
+        embed.add_field(name="Max Spawn Stats",
+                        value=f'''
+                            {incursion.mobilizing_timestamp - incursion.established_timestamp} Uptime
+                            {(incursion.mobilizing_timestamp - incursion.established_timestamp) - timedelta(days=5)} Unused
+                            {(incursion.mobilizing_timestamp - incursion.established_timestamp).microseconds / timedelta(days=5).microseconds - 100:.3f}% total possible `established` time used")
+                        ''')
+    except Exception:
+        pass
     embed.add_field(name="Estimated Respawn Window Opens",
                     value=f"<t:{ int((incursion.mobilizing_timestamp + timedelta(days=3, hours=12)).timestamp()) }:R>", inline=False)
     embed.add_field(name="Estimated Respawn Window Closes",
                     value=f"<t:{ int((incursion.mobilizing_timestamp + timedelta(days=3, hours=36)).timestamp()) }:R>", inline=False)
     return embed
 
     # Spawn Mobilizing!
@@ -157,23 +170,26 @@
 
 def embed_ended(incursion: Incursion) -> Embed:
     embed = embed_base()
     embed.colour = Colour.red()
     embed.description = "The next spawn will occur in 12-36 hours."
     embed.title = f"Ended {incursion.security_string}: {incursion.constellation.name}"
     embed.add_field(name="Spawn Window Opens",
-                    value=f"<t:{ int((incursion.established_timestamp + timedelta(days=1)).timestamp()) }:R>", inline=False)
+                    value=f"<t:{ int((incursion.ended_timestamp + timedelta(days=1)).timestamp()) }:R>", inline=False)
     embed.add_field(name="Spawn Window Closes",
-                    value=f"<t:{ int((incursion.established_timestamp + timedelta(days=1, hours=12)).timestamp()) }:R>", inline=False)
-    embed.add_field(name="Max Spawn Stats",
-                    value=f'''
-                        {incursion.ended_timestamp - incursion.withdrawing_timestamp} Withdrawing
-                        {(incursion.ended_timestamp - incursion.withdrawing_timestamp) + timedelta(days=1)} Unused
-                        {(incursion.ended_timestamp - incursion.withdrawing_timestamp) / timedelta(days=1):.2f}% total possible `withdrawing` time used")
-                    ''')
+                    value=f"<t:{ int((incursion.ended_timestamp + timedelta(days=1, hours=12)).timestamp()) }:R>", inline=False)
+    try:
+        embed.add_field(name="Max Spawn Stats",
+                        value=f'''
+                            {incursion.ended_timestamp - incursion.withdrawing_timestamp} Withdrawing
+                            {(incursion.ended_timestamp - incursion.withdrawing_timestamp) + timedelta(days=1)} Unused
+                            {(incursion.ended_timestamp - incursion.withdrawing_timestamp) / timedelta(days=1):.2f}% total possible `withdrawing` time used")
+                        ''')
+    except Exception:
+        pass
     return embed
 
     # Max Spawn Stats
     # 23 hours 50 minutes withdrawing
     # 10 minutes unused
     # 99.31% total possible "withdrawing" time used
```

### Comparing `aa_incursions-0.3.0a0/incursions/locale/da_DK/LC_MESSAGES/django.po` & `aa_incursions-0.4.2a0/incursions/locale/da_DK/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/locale/de/LC_MESSAGES/django.po` & `aa_incursions-0.4.2a0/incursions/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/locale/en/LC_MESSAGES/django.po` & `aa_incursions-0.4.2a0/incursions/locale/en/LC_MESSAGES/django.po`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-10-08 23:29+1000\n"
+"POT-Creation-Date: 2024-05-21 14:37+1000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -98,26 +98,38 @@
 msgid "IncursionInfluence"
 msgstr ""
 
 #: incursions/models.py:116
 msgid "IncursionInfluences"
 msgstr ""
 
-#: incursions/models.py:141
+#: incursions/models.py:134
+msgid "Destination Webhook"
+msgstr ""
+
+#: incursions/models.py:135
+msgid "Destination Webhooks"
+msgstr ""
+
+#: incursions/models.py:144
 msgid "Destination Webhook for Incursion Updates"
 msgstr ""
 
-#: incursions/models.py:143
+#: incursions/models.py:146
 msgid "Notify on High Security Incursions"
 msgstr ""
 
-#: incursions/models.py:144
+#: incursions/models.py:147
 msgid "Notify on Low Security Incursions"
 msgstr ""
 
-#: incursions/models.py:145
+#: incursions/models.py:148
 msgid "Notify on Null Security Incursions"
 msgstr ""
 
-#: incursions/models.py:160
+#: incursions/models.py:151 incursions/models.py:158 incursions/models.py:159
+msgid "AA Incursions Settings"
+msgstr ""
+
+#: incursions/models.py:165 incursions/models.py:179 incursions/models.py:180
 msgid "Current Focus"
 msgstr ""
```

### Comparing `aa_incursions-0.3.0a0/incursions/locale/es/LC_MESSAGES/django.po` & `aa_incursions-0.4.2a0/incursions/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/locale/fr_FR/LC_MESSAGES/django.po` & `aa_incursions-0.4.2a0/incursions/locale/fr_FR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/locale/it_IT/LC_MESSAGES/django.po` & `aa_incursions-0.4.2a0/incursions/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/locale/ja/LC_MESSAGES/django.po` & `aa_incursions-0.4.2a0/incursions/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/locale/ko_KR/LC_MESSAGES/django.po` & `aa_incursions-0.4.2a0/incursions/locale/ko_KR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/locale/ru/LC_MESSAGES/django.mo` & `aa_incursions-0.4.2a0/incursions/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/locale/ru/LC_MESSAGES/django.po` & `aa_incursions-0.4.2a0/incursions/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/locale/uk/LC_MESSAGES/django.mo` & `aa_incursions-0.4.2a0/incursions/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/locale/uk/LC_MESSAGES/django.po` & `aa_incursions-0.4.2a0/incursions/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/locale/zh_Hans/LC_MESSAGES/django.po` & `aa_incursions-0.4.2a0/incursions/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/migrations/0001_initial.py` & `aa_incursions-0.4.2a0/incursions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/migrations/0002_remove_incursion_influence_and_more.py` & `aa_incursions-0.4.2a0/incursions/migrations/0002_remove_incursion_influence_and_more.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/migrations/0003_focus.py` & `aa_incursions-0.4.2a0/incursions/migrations/0003_focus.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/migrations/0004_alter_focus_incursion.py` & `aa_incursions-0.4.2a0/incursions/migrations/0004_alter_focus_incursion.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/models.py` & `aa_incursions-0.4.2a0/incursions/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -110,30 +110,33 @@
     timestamp = models.DateTimeField(_("Timestamp"), auto_now=False, auto_now_add=False)
     influence = models.FloatField(
         _("Influence of this incursion as a float from 0 to 1"), default=float(0))
 
     class Meta:
         verbose_name = _("IncursionInfluence")
         verbose_name_plural = _("IncursionInfluences")
+        constraints = [
+            models.UniqueConstraint(fields=['incursion', 'timestamp'], name="UniqueIncursionInfluenceLogTimestamp"),
+        ]
 
     def __str__(self):
         return f"{self.incursion} @ {self.timestamp}"
 
 
 class Webhook(models.Model):
     """Destinations for Relays"""
     url = models.CharField(max_length=200)
     name = models.CharField(max_length=50)
 
     def __str__(self):
         return f'"{self.name}"'
 
     class Meta:
-        verbose_name = 'Destination Webhook'
-        verbose_name_plural = 'Destination Webhooks'
+        verbose_name = _('Destination Webhook')
+        verbose_name_plural = _('Destination Webhooks')
 
     def send_embed(self, embed):
         webhook = SyncWebhook.from_url(self.url)
         webhook.send(embed=embed, username="AA Incursions")
 
 
 class IncursionsConfig(SingletonModel):
@@ -141,34 +144,37 @@
         Webhook, verbose_name=_("Destination Webhook for Incursion Updates"))
 
     security_high = models.BooleanField(_("Notify on High Security Incursions"))
     security_low = models.BooleanField(_("Notify on Low Security Incursions"))
     security_null = models.BooleanField(_("Notify on Null Security Incursions"))
 
     def __str__(self):
-        return "AA Incursions Settings"
+        return _("AA Incursions Settings")
 
     class Meta:
         """
         Meta definitions
         """
         default_permissions = ()
-        verbose_name = "AA Incursions Settings"
-        verbose_name_plural = "AA Incursions Settings"
+        verbose_name = _("AA Incursions Settings")
+        verbose_name_plural = _("AA Incursions Settings")
 
 
 class Focus(SingletonModel):
-    incursion = models.ForeignKey(Incursion, verbose_name=_("Current Focus"), on_delete=models.CASCADE, blank=True, null=True)
+    incursion = models.ForeignKey(
+        Incursion,
+        verbose_name=_("Current Focus"),
+        on_delete=models.CASCADE, blank=True, null=True)
 
     def __str__(self):
         try:
             return f"Current Focus: {self.incursion}"
         except Exception:
             return "No Focus Set"
 
     class Meta:
         """
         Meta definitions
         """
         default_permissions = ()
-        verbose_name = "Focus"
-        verbose_name_plural = "Focus"
+        verbose_name = _("Current Focus")
+        verbose_name_plural = _("Current Focus")
```

### Comparing `aa_incursions-0.3.0a0/incursions/providers.py` & `aa_incursions-0.4.2a0/incursions/providers.py`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/signals.py` & `aa_incursions-0.4.2a0/incursions/signals.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 import logging
 
 from django.db.models.signals import post_save
 from django.dispatch import receiver
 
-from incursions.models import Incursion
+from incursions.app_settings import INCURSIONS_AUTO_HIGHSEC_STATIC
+from incursions.models import Focus, Incursion
 from incursions.tasks import (
     incursion_boss_spawned, incursion_ended, incursion_established,
     incursion_mobilizing, incursion_withdrawing,
 )
 
 logger = logging.getLogger(__name__)
 
 
 @receiver(post_save, sender=Incursion)
 def incursion(sender, instance: Incursion, created: bool, *args, **kwargs):
     update_fields = kwargs.pop('update_fields', []) or []
 
     if created is True:
         incursion_established.apply_async(args=[instance.pk])
+        if INCURSIONS_AUTO_HIGHSEC_STATIC and instance.staging_solar_system.is_high_sec:
+            Focus.get_solo().incursion = instance
 
     if 'state' in update_fields:
         if instance.state == Incursion.States.ESTABLISHED:
             # This should have been handled above?
             pass
         elif instance.state == Incursion.States.MOBILIZING:
             incursion_mobilizing.apply_async(args=[instance.pk])
```

### Comparing `aa_incursions-0.3.0a0/incursions/static_data.py` & `aa_incursions-0.4.2a0/incursions/static_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,66 +1,77 @@
 incursion_constellations = {
     "Agiesseson": {"Staging": "Claysson", "Vanguards": ["Adiere", "Oirtlair", "Olelon", "Stetille"], "Assaults": ["Auberulle", "Doussivitte"], "Headquarter": "Unel"},
     "Ahrnot": {"Staging": "Kasi", "Vanguards": ["Hilmar", "Jeshideh", "Shura"], "Assaults": ["Yooh"], "Headquarter": "Hostakoh"},
     "Ajah": {"Staging": "Sizamod", "Vanguards": ["Assiad", "Iswa", "Rand", "Rumida"], "Assaults": ["Kerepa", "Marthia", "Nosodnis"], "Headquarter": "Safilbab"},
     "Algintal": {"Staging": "Barmalie", "Vanguards": ["Audaerne", "Augnais", "Fluekele", "Jolia"], "Assaults": ["Alsottobier", "Deltole", "Parchanier"], "Headquarter": "Colelie"},
     "Amdimmah": {"Staging": "Moniyyuku", "Vanguards": ["Palas", "Reteka", "Safshela"], "Assaults": ["Gidali"], "Headquarter": "Molea"},
+    "Ananah": {"Staging": "Mifrata", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Ancbeu": {"Staging": "Chesiette", "Vanguards": ["Annelle", "Claulenne", "Masalle"], "Assaults": ["Sortet"], "Headquarter": "Scolluzer"},
     "Ankard": {"Staging": "Vilur", "Vanguards": ["Altrinur", "Eygfe", "Reset"], "Assaults": ["Fildar", "Olbra"], "Headquarter": "Jondik"},
     "Aokinen": {"Staging": "Astoh", "Vanguards": ["Onnamon", "Tsuruma", "Uuhulanen"], "Assaults": ["Rohamaa", "Samanuni"], "Headquarter": "Uchomida"},
     "Aptetter": {"Staging": "Libold", "Vanguards": ["Aldrat", "Erstur", "Urnhard"], "Assaults": ["Fredagod"], "Headquarter": "Hardbako"},
     "Araz": {"Staging": "Koona", "Vanguards": ["Jakri", "Munory", "Nidupad", "Zimse"], "Assaults": ["Aphi", "Garisas"], "Headquarter": "Chanoun"},
     "Arekin": {"Staging": "Kaimon", "Vanguards": ["Alikara", "Kausaaja", "Oiniken"], "Assaults": ["Aikoro"], "Headquarter": "Ahynada"},
     "Argeir": {"Staging": "Klaevik", "Vanguards": ["Atonder", "Hotrardik", "Ridoner"], "Assaults": ["Engosi"], "Headquarter": "Orduin"},
+    "Arvachah": {"Staging": "Tash-Murkon Prime", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Asalola": {"Staging": "Torrinos", "Vanguards": ["Ibura", "Isinokka", "Yoma"], "Assaults": ["Oipo"], "Headquarter": "Haajinen"},
     "Avib": {"Staging": "Adia", "Vanguards": ["Azizora", "Hadonoo", "Shabura"], "Assaults": ["Jarshitsan"], "Headquarter": "Ahmak"},
     "Brazinget": {"Staging": "Lumegen", "Vanguards": ["Gedugaud", "Oppold", "Tratokard"], "Assaults": ["Geffur"], "Headquarter": "Hilfhurmur"},
-    "Caldari" "Border" "Zone": {"Staging": "Sivala", "Vanguards": ["Hatakani", "Iivinen", "Tennen"], "Assaults": ["Yashunen"], "Headquarter": "Kassigainen"},
+    "Caldari Border Zone": {"Staging": "Sivala", "Vanguards": ["Hatakani", "Iivinen", "Tennen"], "Assaults": ["Yashunen"], "Headquarter": "Kassigainen"},
     "Charak": {"Staging": "Abhan", "Vanguards": ["Anyed", "Chiga", "Habu"], "Assaults": ["Anzalaisio"], "Headquarter": "Asanot"},
     "Chardu": {"Staging": "Lahnina", "Vanguards": ["Etav", "Pedel", "Saheri"], "Assaults": ["Anila", "Yeeramoun"], "Headquarter": "Ides"},
+    "Comadu": {"Staging": "Atarli", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Damadil": {"Staging": "Perdan", "Vanguards": ["Kibursha", "Hostni", "Mimime"], "Assaults": ["Onazel", "Asesamy"], "Headquarter": "Lossa"},
     "Daredan": {"Staging": "Akes", "Vanguards": ["Hati", "Riavayed", "Uadelah"], "Assaults": ["Hakshma", "Laddiaha"], "Headquarter": "Nakatre"},
+    "Disier": {"Staging": "Aufay", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Elalan": {"Staging": "Aydoteaux", "Vanguards": ["Averon", "Carirgnottin", "Muer", "Odixie", "Scuelazyns", "Tolle"], "Assaults": ["Antollare", "Enedore", "Laic"], "Headquarter": "Avele"},
     "Enka": {"Staging": "Palpis", "Vanguards": ["Arveyil", "Nidebora", "Ulerah", "Uktiad"], "Assaults": ["Faktun", "Halenan"], "Headquarter": "Mili"},
     "Erada": {"Staging": "Loguttur", "Vanguards": ["Krilmokenur", "Magiko", "Onga", "Vullat"], "Assaults": ["Larkugei", "Oremmulf", "Osaumuni"], "Headquarter": "Hurjafren"},
     "Eustron": {"Staging": "Andole", "Vanguards": ["Cat", "Derririntel", "Ommare"], "Assaults": ["Atlangeins"], "Headquarter": "Hecarrin"},
     "Fabas": {"Staging": "Heorah", "Vanguards": ["Agal", "Doza", "Ebasez"], "Assaults": ["Bania", "Nasreri"], "Headquarter": "Girani-Fa"},
-    "Febihkin": {"Staging": "Dantan", "Vanguards": ["Kador" "Prime", "Khafis", "Nordar"], "Assaults": ["Askonak", "Murini"], "Headquarter": "Uanim"},
+    "Febihkin": {"Staging": "Dantan", "Vanguards": ["Kador Prime", "Khafis", "Nordar"], "Assaults": ["Askonak", "Murini"], "Headquarter": "Uanim"},
     "Fekhoya": {"Staging": "Balanaz", "Vanguards": ["Afnakat", "Bashyam", "Parses"], "Assaults": ["Firbha"], "Headquarter": "Col"},
     "Finaka": {"Staging": "Geztic", "Vanguards": ["Hishai", "Osis", "Sehsasez", "Yezara"], "Assaults": ["Ervekam", "Kahah", "Mashtarmem"], "Headquarter": "Saloti"},
     "Frar": {"Staging": "Aderkan", "Vanguards": ["Earled", "Ogoten", "Tollus"], "Assaults": ["Hebisa", "Polstodur"], "Headquarter": "Ansher"},
+    "Fribrodi": {"Staging": "Ansen", "Vanguards": ["Arwa", "Krirald", "Arifsdald"], "Assaults": ["Hakisalki"], "Headquarter": "Dudreda"},  # Lost to Pochven
     "Gedur": {"Staging": "Abrat", "Vanguards": ["Alf", "Arlulf", "Brundakur", "Illuin"], "Assaults": ["Aldilur", "Orgron", "Nedegulf"], "Headquarter": "Stirht"},
     "Goins": {"Staging": "Stoure", "Vanguards": ["Arasare", "Lazer", "Yvelet"], "Assaults": ["Vecodie"], "Headquarter": "Yvaeroure"},
+    "Haurala": {"Staging": "Kino", "Vanguards": ["Erenta", "Ouranienen", "Uemisaisen"], "Assaults": ["Sotrentaira"], "Headquarter": "Raussinen"},  # Lost to Pochven
     "Hoosa": {"Staging": "Horir", "Vanguards": ["Abaim", "Somouh", "Sorzielang"], "Assaults": ["Sayartchen", "Teshi"], "Headquarter": "Gosalav"},
     "Ichida": {"Staging": "Malpara", "Vanguards": ["Hakodan", "Hatori", "Ronne"], "Assaults": ["Jarkkolen"], "Headquarter": "Junsen"},
     "Ihilakken": {"Staging": "Sakenta", "Vanguards": ["Ansila", "Aokannitoh", "Hirtamon", "Ikuchi"], "Assaults": ["Hykkota", "Ohmahailen", "Outuni"], "Headquarter": "Eskunen"},
+    "Jayai": {"Staging": "Tararan", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Jonar": {"Staging": "Anbald", "Vanguards": ["Bongveber", "Freatlidur", "Maturat"], "Assaults": ["Roleinn", "Vorsk"], "Headquarter": "Eiluvodi"},
     "Jonenor": {"Staging": "Gallareue", "Vanguards": ["Ansone", "Dunraelare", "Nausschie", "Trosquesere"], "Assaults": ["Estene", "Stayme"], "Headquarter": "Inghenges"},
+    "Kabo": {"Staging": "Rahadalon", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Kakol": {"Staging": "Neburab", "Vanguards": ["Aband", "Ghesis", "Gonan"], "Assaults": ["Gamdis", "Joamma"], "Headquarter": "Joramok"},
+    "Kainokai": {"Staging": "Ajanen", "Vanguards": ["Autama", "Kuoka", "Tsukuras"], "Assaults": ["Kirras"], "Headquarter": "Nani"},  # Lost to Pochven
     "Kalangin": {"Staging": "Lachailes", "Vanguards": ["Eshtah", "Kasrasi", "Ordize", "Rashy"], "Assaults": ["Fovihi", "Psasa"], "Headquarter": "Kiereend"},
     "Kehina": {"Staging": "Nalu", "Vanguards": ["Esteban", "Luromooh", "Sahdil"], "Assaults": ["Nadohman"], "Headquarter": "Moussou"},
+    "Kekah": {"Staging": "Harva", "Vanguards": ["Aghesi", "Charra", "Patzcha"], "Assaults": ["Airshaz"], "Headquarter": "Fabin"},  # Lost to Pochven
     "Kiartanne": {"Staging": "Theruesse", "Vanguards": ["Ansalle", "Ellmay", "Gisleres"], "Assaults": ["Amygnon", "Jufvitte"], "Headquarter": "Scheenins"},
     "Kisana": {"Staging": "Eredan", "Vanguards": ["Gheth", "Lisudeh", "Mehatoor"], "Assaults": ["Sasoutikh"], "Headquarter": "Ohide"},
     "Lorundio": {"Staging": "Asgeir", "Vanguards": ["Evuldgenzo", "Flost", "Ongund"], "Assaults": ["Eust"], "Headquarter": "Todrir"},
-    "Maddam": {"Staging": "Chesoh", "Vanguards": ["Hama", "Hanan", "Irnal", "Sarum" "Prime"], "Assaults": ["Alkabsi", "Bagodan", "Mahrokht"], "Headquarter": "Murzi"},
+    "Maddam": {"Staging": "Chesoh", "Vanguards": ["Hama", "Hanan", "Irnal", "Sarum Prime"], "Assaults": ["Alkabsi", "Bagodan", "Mahrokht"], "Headquarter": "Murzi"},
     "Maseend": {"Staging": "Ana", "Vanguards": ["Hamse", "Jaswelu", "Lashkai", "Zhilshinou"], "Assaults": ["Maiah", "Yuhelia"], "Headquarter": "Barira"},
     "Mayonhen": {"Staging": "Mishi", "Vanguards": ["Avada", "Haimeh", "Pahineh"], "Assaults": ["Bazadod"], "Headquarter": "Chibi"},
+    "Mamouna": {"Staging": "Podion", "Vanguards": ["Futzchag", "Jayneleb", "Kuharah"], "Assaults": ["Lilmad"], "Headquarter": "Kazna"},  # Lost to Pochven
     "Mazake": {"Staging": "Sakhti", "Vanguards": ["Hiramu", "Hutian", "Mazitah", "Pelkia"], "Assaults": ["Joppaya", "Raren"], "Headquarter": "Noli"},
     "Megeh": {"Staging": "Dresi", "Vanguards": ["Aharalel", "Gensela", "Zororzih"], "Assaults": ["Aphend", "Romi"], "Headquarter": "Hiroudeh"},
     "Mekashtad": {"Staging": "Pirohdim", "Vanguards": ["Iosantin", "Janus", "Orva", "Salashayama", "Thiarer", "Zet"], "Assaults": ["Amphar", "Nikh", "Usroh"], "Headquarter": "Agha"},
     "Mimishia": {"Staging": "Unkah", "Vanguards": ["Atoosh", "Hoona", "Mimen"], "Assaults": ["Thashkarai"], "Headquarter": "Sacalan"},
     "Mobit": {"Staging": "Narai", "Vanguards": ["Bashakru", "Shuria", "Sukirah"], "Assaults": ["Mikhir", "Ziona"], "Headquarter": "Akhragan"},
     "Moghiz": {"Staging": "Yehnifi", "Vanguards": ["Kooreng", "Shaggoth", "Ustnia"], "Assaults": ["Elmed", "Minin"], "Headquarter": "Jennim"},
     "Mossas": {"Staging": "Shala", "Vanguards": ["Ibaria", "Maspah", "Zemalu"], "Assaults": ["Juddi"], "Headquarter": "Khankenirdia"},
     "Mulata": {"Staging": "Hizhara", "Vanguards": ["Ahala", "Arera", "Knophtikoo"], "Assaults": ["Hai", "Seiradih"], "Headquarter": "Mamenkhanar"},
     "Nagaslaiken": {"Staging": "Saikanen", "Vanguards": ["Jeras", "Kakki", "Oijamon"], "Assaults": ["Auviken"], "Headquarter": "Ohvosamon"},
     "Naloran": {"Staging": "Akhmoh", "Vanguards": ["Hapala", "Salah", "Yebouz"], "Assaults": ["Syrikos"], "Headquarter": "Hikansog"},
     "Nasorin": {"Staging": "Azhgabid", "Vanguards": ["Arkoz", "Jinizu", "Taru", "Yanuel"], "Assaults": ["Nafrivik", "Remoriu"], "Headquarter": "Phoren"},
     "Nimedaz": {"Staging": "Chaktaren", "Vanguards": ["Danyana", "Jinkah", "Nibainkier", "Polfaly"], "Assaults": ["Annad", "Nahyeen"], "Headquarter": "Andrub"},
-    "Nohshayess": {"Staging": "Sazre", "Vanguards": ["Ipref", "Jachanu", "Khanid" "Prime", "Kihtaled"], "Assaults": ["Agil", "Gousoviba", "Neyi"], "Headquarter": "Bukah"},
+    "Nohshayess": {"Staging": "Sazre", "Vanguards": ["Ipref", "Jachanu", "Khanid Prime", "Kihtaled"], "Assaults": ["Agil", "Gousoviba", "Neyi"], "Headquarter": "Bukah"},
     "Norgoh": {"Staging": "Fora", "Vanguards": ["Bhizheba", "Eba", "Safizon", "Zatsyaki"], "Assaults": ["Artoun", "Ebtesham"], "Headquarter": "Isamm"},
     "Odengsolf": {"Staging": "Balginia", "Vanguards": ["Avesber", "Frarn", "Gyng", "Illinfrik"], "Assaults": ["Ivar", "Meirakulf"], "Headquarter": "Usteli"},
     "Odilis": {"Staging": "Quier", "Vanguards": ["Frarolle", "Gicodel", "Mattere"], "Assaults": ["Ethernity", "Meves"], "Headquarter": "Athinard"},
     "Oraron": {"Staging": "Akeva", "Vanguards": ["Ejahi", "Gelhan", "Jarizza"], "Assaults": ["Asghatil", "Bar"], "Headquarter": "Sucha"},
     "Orshed": {"Staging": "Buftiar", "Vanguards": ["Jofan", "Odlib", "Yadi"], "Assaults": ["Tidacha"], "Headquarter": "Milu"},
     "Orvanne": {"Staging": "Gererique", "Vanguards": ["Niballe", "Odinesyn", "Postouvin"], "Assaults": ["Larryn"], "Headquarter": "Weraroix"},
     "Osnins": {"Staging": "Aice", "Vanguards": ["Amattens", "Bereye", "Junsoraert", "Jurlesel"], "Assaults": ["Arnatele", "Halle"], "Headquarter": "Mormoen"},
@@ -73,20 +84,20 @@
     "Peges": {"Staging": "Ahteer", "Vanguards": ["Hath", "Judra", "Sharios", "Uhodoh"], "Assaults": ["Esa", "Kari"], "Headquarter": "Arakor"},
     "Pietanen": {"Staging": "Jotenen", "Vanguards": ["Atai", "Otalieto", "Rauntaka"], "Assaults": ["Liukikka"], "Headquarter": "Aikantoh"},
     "Qermi": {"Staging": "Lazara", "Vanguards": ["Asrios", "Ithar", "Shemah"], "Assaults": ["Zorrabed"], "Headquarter": "Telang"},
     "Reya": {"Staging": "Imya", "Vanguards": ["Gergish", "Kobam", "Tahli"], "Assaults": ["Madomi"], "Headquarter": "Hirizan"},
     "Rifenda": {"Staging": "Ahkour", "Vanguards": ["Gaknem", "Nehkiah", "Siyi"], "Assaults": ["Iro"], "Headquarter": "Abai"},
     "Ryra": {"Staging": "Thasinaz", "Vanguards": ["Choonka", "Dihra", "Dital"], "Assaults": ["Esescama"], "Headquarter": "Odin"},
     "Ruomo": {"Staging": "Itamo", "Vanguards": ["Ahtulaima", "Kylmabe", "Vaankalen"], "Assaults": ["Jatate", "Mitsolen"], "Headquarter": "Mahtista"},
-    "San" "Matar": {"Staging": "Zaid", "Vanguards": ["Akpivem", "Nirbhi", "Tanoo", "Yuzier"], "Assaults": ["Jark", "Sasta"], "Headquarter": "Lashesih"},
+    "San Matar": {"Staging": "Zaid", "Vanguards": ["Akpivem", "Nirbhi", "Tanoo", "Yuzier"], "Assaults": ["Jark", "Sasta"], "Headquarter": "Lashesih"},
     "Sanair": {"Staging": "Ahrosseas", "Vanguards": ["Adahum", "Goram", "Tendhyes"], "Assaults": ["Tividu"], "Headquarter": "Anjedin"},
     "Santenpaa": {"Staging": "Motsu", "Vanguards": ["Aramachi", "Laah", "Oichiya"], "Assaults": ["Saila", "Isenairos"], "Headquarter": "Uotila"},
     "Sib": {"Staging": "Moro", "Vanguards": ["Ainsan", "Badivefi", "Talidal"], "Assaults": ["Ashi", "Tzashrah"], "Headquarter": "Sabusi"},
     "Somi": {"Staging": "Matyas", "Vanguards": ["Imeshasa", "Jarzalad", "Pimsu"], "Assaults": ["Nafomeh"], "Headquarter": "Riramia"},
-    "Sosarir": {"Staging": "Shumam", "Vanguards": ["Ardishapur" "Prime", "Gid", "Nererut", "Nifshed", "Vashkah"], "Assaults": ["Rasile", "Sitanan", "Thebeka"], "Headquarter": "Dakba"},
+    "Sosarir": {"Staging": "Shumam", "Vanguards": ["Ardishapur Prime", "Gid", "Nererut", "Nifshed", "Vashkah"], "Assaults": ["Rasile", "Sitanan", "Thebeka"], "Headquarter": "Dakba"},
     "Subhatoub": {"Staging": "Seitam", "Vanguards": ["Tew", "Zehru", "Zith"], "Assaults": ["Alra", "Ilas"], "Headquarter": "Sinid"},
     "Suon": {"Staging": "Inari", "Vanguards": ["Inaro", "Irjunen", "Waskisen"], "Assaults": ["Sirppala"], "Headquarter": "Kaaputenen"},
     "Stadakorn": {"Staging": "Situner", "Vanguards": ["Agtver", "Datulen", "Erego", "Meimungen", "Totkubad"], "Assaults": ["Evettullur", "Hjortur", "Tamekamur"], "Headquarter": "Egbonbet"},
     "Trigentia": {"Staging": "Akhwa", "Vanguards": ["Inis-Ilix", "Sonama", "Suner"], "Assaults": ["Halibai", "Turba"], "Headquarter": "Kothe"},
     "Tsemshatel": {"Staging": "Yasud", "Vanguards": ["Azerakish", "Ghishul", "Lari", "Moutid"], "Assaults": ["Asezai", "Yeder"], "Headquarter": "Ferira"},
     "Unour": {"Staging": "Vilinnon", "Vanguards": ["Iffrue", "Mollin", "Ommaerrer"], "Assaults": ["Ivorider"], "Headquarter": "Osmallanais"},
     "Urtfer": {"Staging": "Jorus", "Vanguards": ["Appen", "Javrendei", "Klir"], "Assaults": ["Trer"], "Headquarter": "Egmur"},
@@ -109,15 +120,15 @@
     "Aven": {"Staging": "Olin", "Vanguards": ["Galnafsad", "Otakod", "Shalne"], "Assaults": ["Shapisin"], "Headquarter": "Gonditsa"},
     "Braille": {"Staging": "Vevelonel", "Vanguards": ["Anckee", "Elore", "Meunvon", "Yveve"], "Assaults": ["Aimoguier", "Conomette"], "Headquarter": "Cadelanne"},
     "Budar": {"Staging": "Ibani", "Vanguards": ["Cabeki", "Irmalin", "Timudan"], "Assaults": ["Sassecho"], "Headquarter": "Goudiyah"},
     "Elerelle": {"Staging": "Agaullores", "Vanguards": ["Babirmoult", "Faurulle", "Hare", "Ogaria"], "Assaults": ["Heluene", "Oruse"], "Headquarter": "Arittant"},
     "Elfrard": {"Staging": "Kadlina", "Vanguards": ["Aeditide", "Hegfunden", "Egbinger"], "Assaults": ["Weld"], "Headquarter": "Klingt"},
     "Essin": {"Staging": "Hofjaldgund", "Vanguards": ["Ebolfer", "Gebuladi", "Eszur"], "Assaults": ["Frerstorn", "Sirekur"], "Headquarter": "Ontorn"},
     "Eugidi": {"Staging": "Vimeini", "Vanguards": ["Aset", "Avenod", "Isbrabata", "Turnur"], "Assaults": ["Eytjangard", "Uisper"], "Headquarter": "Floseswin"},
-    "EVE": {"Staging": "New" "Eden", "Vanguards": ["Canard", "Central" "Point", "Promised" "Land"], "Assaults": ["Dead" "End", "Gateway"], "Headquarter": "Exit"},
+    "EVE": {"Staging": "New Eden", "Vanguards": ["Canard", "Central Point", "Promised Land"], "Assaults": ["Dead End", "Gateway"], "Headquarter": "Exit"},
     "Fabai": {"Staging": "Sakht", "Vanguards": ["Anath", "Naga", "Tisot"], "Assaults": ["Omigiav"], "Headquarter": "Efu"},
     "Fua": {"Staging": "Amod", "Vanguards": ["Akila", "Basan", "Shajarleg"], "Assaults": ["Sahda"], "Headquarter": "Naguton"},
     "Ganoure": {"Staging": "Kenninck", "Vanguards": ["Ausmaert", "Barleguet"], "Assaults": ["Aulbres", "Vestouve"], "Headquarter": "Espigoure"},
     "Hed": {"Staging": "Lantorn", "Vanguards": ["Dal", "Siseide", "Vard"], "Assaults": ["Auga"], "Headquarter": "Amamake"},
     "Helab": {"Staging": "Sheri", "Vanguards": ["Ahraghen", "Ajna", "Tukanas"], "Assaults": ["Nielez", "Soliara"], "Headquarter": "Fageras"},
     "Homroon": {"Staging": "Neda", "Vanguards": ["Chitiamem", "Zahefeus", "Zephan"], "Assaults": ["Kuhri", "Nandeza"], "Headquarter": "Dimoohan"},
     "Inolari": {"Staging": "Pavanakka", "Vanguards": ["Eha", "Innia", "Martoh"], "Assaults": ["Iralaja", "Kinakka"], "Headquarter": "Raihbaka"},
@@ -133,72 +144,78 @@
     "Makh": {"Staging": "Korridi", "Vanguards": ["Bantish", "Lela", "Saphthar"], "Assaults": ["Itrin"], "Headquarter": "Keri"},
     "Mallugier": {"Staging": "Amasiree", "Vanguards": ["Amoen", "Aubonnie", "Hedoubel"], "Assaults": ["Gallusiene", "Ruerrotta"], "Headquarter": "Avaux"},
     "Mareerieh": {"Staging": "Vehan", "Vanguards": ["Udianoor", "Onanam", "Sadana"], "Assaults": ["Isid"], "Headquarter": "Marmeha"},
     "Meli": {"Staging": "Naka", "Vanguards": ["Aring", "Chej", "Gayar"], "Assaults": ["Noranim", "Petidu"], "Headquarter": "Menai"},
     "Mivora": {"Staging": "Fuskunen", "Vanguards": ["Otosela", "Paala", "Uemon"], "Assaults": ["Akkio"], "Headquarter": "Tasti"},
     "Monalaz": {"Staging": "Access", "Vanguards": ["Angur", "Djimame", "Hangond"], "Assaults": ["Mozzidit"], "Headquarter": "Antem"},
     "Nadire": {"Staging": "Esmes", "Vanguards": ["Goinard", "Allipes", "Aetree"], "Assaults": ["Raeghoscon"], "Headquarter": "Lermireve"},
+    "Nashar": {"Staging": "Bika", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Okakuola": {"Staging": "Notoras", "Vanguards": ["Hirri", "Kedama", "Nisuwa", "Oinasiken", "Reitsato"], "Assaults": ["Pynekastoh", "Rakapas", "Teimo"], "Headquarter": "Iwisoda"},
+    "Okomon": {"Staging": "Uoyonen", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Ombil": {"Staging": "Yekh", "Vanguards": ["Balas", "Edilkam", "Ertoo", "Feshur", "Hoseen", "Hoseen", "Pemsah"], "Assaults": ["Fihrneh", "Gesh", "Hakatiz", "Khnar"], "Headquarter": "Parouz"},
     "Pezarba": {"Staging": "Hiremir", "Vanguards": ["Omam", "Sechmaren", "Zinoo"], "Assaults": ["Bersyrim"], "Headquarter": "Mod"},
     "Ravin": {"Staging": "Kerying", "Vanguards": ["Arzi", "Oguser", "Zorenyen"], "Assaults": ["Mafra", "Schmaeel"], "Headquarter": "Abath"},
+    "Sanctum": {"Staging": "Yulai", "Vanguards": ["Esmar", "Kemerk", "Manarq", "Ourapheh"], "Assaults": ["Pakhshi", "Tar", "Tekaima"], "Headquarter": "Tarta"},
     "Seevadin": {"Staging": "Upt", "Vanguards": ["Gehi", "Ham", "Vezila"], "Assaults": ["Claini", "Seshala"], "Headquarter": "Hemouner"},
     "Selonat": {"Staging": "Ned", "Vanguards": ["Fobiner", "Karan", "Nouta"], "Assaults": ["Esaeel", "Huna"], "Headquarter": "Hophib"},
     "Semou": {"Staging": "Arzad", "Vanguards": ["Ezzara", "Oyeman", "Sifilar"], "Assaults": ["Raa"], "Headquarter": "Tzvi"},
     "Serthoulde": {"Staging": "Athounon", "Vanguards": ["Alparena", "Arderonne", "Mercomesier", "Reschard"], "Assaults": ["Alamel", "Odamia"], "Headquarter": "Mantenault"},
     "Sukanan": {"Staging": "Tirbam", "Vanguards": ["Nasesharafa", "Keshirou", "Rethan"], "Assaults": ["Ordat"], "Headquarter": "Teshkat"},
     "Tandoiras": {"Staging": "Haras", "Vanguards": ["Sahtogas", "Tannakan", "Oyonata"], "Assaults": ["Kurniainen"], "Headquarter": "Saidusairos"},
     "Tartatven": {"Staging": "Muttokon", "Vanguards": ["Aedald", "Audesder", "Heild"], "Assaults": ["Hrokkur"], "Headquarter": "Hrober"},
     "Tendrara": {"Staging": "Arza", "Vanguards": ["Liparer", "Miroona", "Ranni"], "Assaults": ["Jedandan"], "Headquarter": "Enal"},
     "Umamon": {"Staging": "Saranen", "Vanguards": ["Anin", "Karjataimon", "Tartoken"], "Assaults": ["Nannaras"], "Headquarter": "Tamo"},
     "Urpiken": {"Staging": "Kehjari", "Vanguards": ["Ashitsu", "Ienakkamon", "Villasen", "Korasen"], "Assaults": ["Hykanima", "Okagaiken"], "Headquarter": "Sarenemi"},
+    "Vaarma": {"Staging": "Sosala", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Viriette": {"Staging": "Brarel", "Vanguards": ["Annancale", "Intaki", "Vey"], "Assaults": ["Agoze", "Ostingele"], "Headquarter": "Harroule"},
     "Woenckee": {"Staging": "Muetralle", "Vanguards": ["Costolle", "Costolle", "Ouelletta"], "Assaults": ["Murethand"], "Headquarter": "Loes"},
+    "Zemont": {"Staging": "Zaimeth", "Vanguards": ["Ekid", "Raravoss", "Sharhelund"], "Assaults": ["Youl"], "Headquarter": "Nakri"},  # Lost to pochven
     "0-8MWQ": {"Staging": "LS9B-9", "Vanguards": ["RVCZ-C", "VI2K-J", "ZLZ-1Z"], "Assaults": ["6Y-WRK"], "Headquarter": "5T-KM3"},
     "0-YMZM": {"Staging": "MOCW-2", "Vanguards": ["3AE-CP", "9OLQ-6", "Q-3HS5"], "Assaults": ["0-VG7A"], "Headquarter": "EUU-4N"},
     "02QH-A": {"Staging": "JLO-Z3", "Vanguards": ["03-OR2", "5-MQQ7", "6-EQYE"], "Assaults": ["U2-28D"], "Headquarter": "LQ-OAI"},
     "03C-SU": {"Staging": "C8VC-S", "Vanguards": ["GIH-ZG", "K-6SNI", "L-VXTK", "XD-TOV"], "Assaults": ["V7-FB4", "W-UQA5"], "Headquarter": "S8-NSQ"},
     "04-H4M": {"Staging": "8B-VLX", "Vanguards": ["G-B22J", "R3-K7K", "X-R3NM", "X6AB-Y"], "Assaults": ["1-1I53", "N8XA-L"], "Headquarter": "18-GZM"},
     "04-LOF": {"Staging": "GK3-RX", "Vanguards": ["1P-QWR", "3-JG3X", "FJ-GUR"], "Assaults": ["BQ0-UU"], "Headquarter": "RF-X7V"},
     "05M-I1": {"Staging": "UK-SHL", "Vanguards": ["01TG-J", "U3SQ-X", "A1BK-A"], "Assaults": ["L6BY-P", "NUG-OF"], "Headquarter": "E7VE-V"},
     "09-4XW": {"Staging": "ZXA-V6", "Vanguards": ["I1-BE8", "ZH3-BS", "ZJ-QOO"], "Assaults": ["1QH-0K"], "Headquarter": "W8O-19"},
     "0A-73B": {"Staging": "UI-8ZE", "Vanguards": ["7D-0SQ", "OGV-AS", "Y-C3EQ"], "Assaults": ["H1-J33"], "Headquarter": "KU5R-W"},
-    "0C-PZ4": {"Staging": "BKG-Q2", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "0C-PZ4": {"Staging": "BKG-Q2", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "0EA3-8": {"Staging": "4CJ-AC", "Vanguards": ["67Y-NR", "A24L-V", "QTME-D"], "Assaults": ["GDHN-K", "RQN-OO"], "Headquarter": "GK5Z-T"},
     "0FC-ZX": {"Staging": "J7-BDX", "Vanguards": ["30-YOU", "384-IN", "4F89-U", "MKIG-5", "YHEN-G"], "Assaults": ["E-JCUS", "LP1M-Q", "W-QN5X"], "Headquarter": "G063-U"},
     "0HD-6C": {"Staging": "42XJ-N", "Vanguards": ["G9D-XW", "GVZ-1W", "Z3U-GI"], "Assaults": ["B3QP-K"], "Headquarter": "FHB-QA"},
     "0KTC-R": {"Staging": "ZD4-G9", "Vanguards": ["YJ3-UT", "C2-DDA", "VG-QW1"], "Assaults": ["L-IE41"], "Headquarter": "2IBE-N"},
     "0PS-L5": {"Staging": "GGMF-J", "Vanguards": ["GGMF-J", "IG-4OF", "M-NWLB"], "Assaults": ["0-QP56", "ORB4-J"], "Headquarter": "MTGF-2"},
     "0YMH-Q": {"Staging": "EFM-C4", "Vanguards": ["74-VZA", "I-1QKL", "L5-UWT"], "Assaults": ["Q7-FZ8"], "Headquarter": "YPW-M4"},
     "1-A81R": {"Staging": "7UTB-F", "Vanguards": ["31X-RE", "5-6QW7", "Q-02UL"], "Assaults": ["Y5C-YD"], "Headquarter": "F-9PXR"},
     "17K-QM": {"Staging": "9T-APQ", "Vanguards": ["33-JRO", "ARBX-9", "O-MCZR"], "Assaults": ["5-CSE3"], "Headquarter": "JI-K5H"},
     "1A-WYQ": {"Staging": "LJK-T0", "Vanguards": ["M-9V5D", "M-VEJZ", "O2-39S"], "Assaults": ["XWY-YM"], "Headquarter": "DY-40Z"},
     "1ANT-J": {"Staging": "9-ZFCG", "Vanguards": ["3-YX2D", "CFLF-P", "V-TN6Q"], "Assaults": ["UD-VZW"], "Headquarter": "QBH5-F"},
     "1D-65L": {"Staging": "2-3Q2G", "Vanguards": ["M-UC0S", "SY0W-2", "V7-MID"], "Assaults": ["JSI-LL"], "Headquarter": "Q1U-IU"},
     "1G-8KY": {"Staging": "9-R6GU", "Vanguards": ["KK-L97", "R-KZK7", "Z-GY5S"], "Assaults": ["N-Q5PW", "Y6-HPG"], "Headquarter": "Y-W1Q3"},
     "1M4-FN": {"Staging": "O8W-5O", "Vanguards": ["0-TRV1", "F-TQWO", "NBO-O0"], "Assaults": ["6UT-1K"], "Headquarter": "13-49W"},
-    "1P-VL2": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "1P-VL2": {"Staging": "MJI3-8", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "1RG-GU": {"Staging": "RZ-PIY", "Vanguards": ["A-C5TC", "FR46-E", "QLPX-J"], "Assaults": ["2-X0PF", "OFVH-Y"], "Headquarter": "1-PGSG"},
     "1VN-XC": {"Staging": "CT8K-0", "Vanguards": ["C-4D0W", "IL-H0A", "M9-LAN"], "Assaults": ["L4X-1V", "WPV-JN"], "Headquarter": "PX-IHN"},
     "2-M6DE": {"Staging": "M2-CF1", "Vanguards": ["8-JYPM", "JH-M2W", "PVH8-0"], "Assaults": ["EZA-FM"], "Headquarter": "6-CZ49"},
     "2-ZRM0": {"Staging": "AR-5SY", "Vanguards": ["A1RR-M", "GW7P-8", "OE-4HB", "SF-XJS"], "Assaults": ["Y-YHZQ", "Z-SR1I"], "Headquarter": "A-1IJ9"},
-    "309452": {"Staging": "UW-6MW", "Vanguards": ["0-N1BJ", "FO9-FZ", "T-8GWA"], "Assaults": ["4QY-NT"], "Headquarter": "T-8GWA"},
+    "2747-4": {"Staging": "UW-6MW", "Vanguards": [""], "Assaults": [""], "Headquarter": "A-"},
     "29V-1R": {"Staging": "QPO-WI", "Vanguards": ["FO8M-2", "R8S-1K", "T-945F"], "Assaults": ["4U90-Z"], "Headquarter": "AD-CBT"},
     "2FYX-H": {"Staging": "ZJ-5IS", "Vanguards": ["ZZK-VF", "SN-Q1T", "L1YK-V"], "Assaults": ["R3P0-Z"], "Headquarter": "8RL-OG"},
     "2O-VY7": {"Staging": "SG-3HY", "Vanguards": ["A-YB15", "D-6PKO", "QZX-L9"], "Assaults": ["SY-0AM"], "Headquarter": "AU2V-J"},
     "2Q-8WA": {"Staging": "S-LHPJ", "Vanguards": ["5-VFC6", "J-OAH2"], "Assaults": ["86L-9F", "BZ-BCK", "IUU3-L", "O5-YNW"], "Headquarter": "FB5U-I"},
+    "309452": {"Staging": "UW-6MW", "Vanguards": ["0-N1BJ", "FO9-FZ", "T-8GWA"], "Assaults": ["4QY-NT"], "Headquarter": "T-8GWA"},
     "3-PC31": {"Staging": "K-9UG4", "Vanguards": ["2-RSC7", "D4-2XN", "ZID-LE"], "Assaults": ["KJ-V0P"], "Headquarter": "OBK-K8"},
     "3-U491": {"Staging": "CL-J9W", "Vanguards": ["5-LCI7", "VNGJ-U", "VVO-R6", "Y2-I3W"], "Assaults": ["AZN-D2", "E-PR0S", "TR07-S"], "Headquarter": "2-F3OE"},
     "304-QS": {"Staging": "B-GC1T", "Vanguards": ["AH-B84", "HB7R-F", "O-JPKH"], "Assaults": ["JTAU-5"], "Headquarter": "F-9F6Q"},
     "304Z-R": {"Staging": "RZC-16", "Vanguards": ["F-NMX6", "FWA-4V", "ZKYV-W"], "Assaults": ["7RM-N0", "S-MDYI"], "Headquarter": "GA-P6C"},
     "38G6-L": {"Staging": "ROIR-Y", "Vanguards": ["G95-VZ", "J-CIJV", "KLY-C0"], "Assaults": ["CL6-ZG", "CXN1-Z"], "Headquarter": "X-7OMU"},
     "3B-IWE": {"Staging": "K4-RFZ", "Vanguards": ["DG-L7S", "L-FVHR", "RKM-GE"], "Assaults": ["4-2UXV"], "Headquarter": "F2OY-X"},
     "3D-ROC": {"Staging": "3ET-G8", "Vanguards": ["0J-MQW", "K-BBYU", "XT-1E0"], "Assaults": ["N-PS2Y"], "Headquarter": "T6T-BQ"},
     "3GK-WS": {"Staging": "5Q65-4", "Vanguards": ["5DE-QS", "R0-DMM", "UZ-QXW"], "Assaults": ["F-3FOY", "OAIG-0"], "Headquarter": "UM-SCG"},
-    "3NA-Z1": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "3NA-Z1": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "3R-BJL": {"Staging": "XW2H-V", "Vanguards": ["F2W-C6", "KZ9T-C", "X40H-9"], "Assaults": ["FIDY-8"], "Headquarter": "8FN-GP"},
     "3RU-10": {"Staging": "IO-R2S", "Vanguards": ["Q-ITV5", "QE2-FS", "R-ZESX"], "Assaults": ["7-UVMT", "HF-K3O"], "Headquarter": "WVMS-X"},
     "3TS-12": {"Staging": "A0M-R8", "Vanguards": ["1NZV-7", "B-VFDD", "LY-WRW", "QCGG-Q"], "Assaults": ["7-2Z93", "NIM-FY"], "Headquarter": "9F-ERQ"},
     "3WN-1T": {"Staging": "BY-MSY", "Vanguards": ["6EK-BV", "D-PNP9", "E1UU-3"], "Assaults": ["G-YZUX", "P-3XVV"], "Headquarter": "CZ6U-1"},
     "4-0VL9": {"Staging": "Y8K-5B", "Vanguards": ["4HF-4R", "B6-XE8", "JLH-FN"], "Assaults": ["DFTK-D", "MOSA-I"], "Headquarter": "L7-BLT"},
     "4-QV2L": {"Staging": "XEN7-0", "Vanguards": ["F5M-CC", "LKZ-CY", "TZE-UB"], "Assaults": ["WRL4-2"], "Headquarter": "V7G-RL"},
     "4QZ-2M": {"Staging": "B-7DFU", "Vanguards": ["8-YNBE"], "Assaults": ["BX-VEX", "QY1E-N", "YQX-7U"], "Headquarter": "E-VKJV"},
@@ -206,32 +223,32 @@
     "48R-PS": {"Staging": "9-8BL8", "Vanguards": ["6W-HRH", "MQFX-Q", "N5Y-4N"], "Assaults": ["CSOA-B"], "Headquarter": "K3JR-J"},
     "49A-BZ": {"Staging": "A-SJ8X", "Vanguards": ["0LTQ-C", "2P-4LS", "31-MLU", "LSC4-P"], "Assaults": ["A9D-R0", "BMNV-P", "RF-GGF"], "Headquarter": "BY-S36"},
     "4BZ-R3": {"Staging": "I7S-1S", "Vanguards": ["FSW-3C", "FX-7EM", "G7AQ-7", "QBL-BV"], "Assaults": ["D-GTMI", "T-RPFU"], "Headquarter": "MH9C-S"},
     "4LEZ-6": {"Staging": "6Q4-X6", "Vanguards": ["B9N2-2", "D-QJR9", "U4-V3J"], "Assaults": ["H-29TM"], "Headquarter": "KOI8-Z"},
     "4M6-GJ": {"Staging": "J7M-3W", "Vanguards": ["2G-VDP", "9P-870", "KRPF-A"], "Assaults": ["9F-3CR"], "Headquarter": "QNXJ-M"},
     "4MY-AB": {"Staging": "F76-8Q", "Vanguards": ["D-BAMJ", "DW-N2S", "JKWP-U", "RHE7-W"], "Assaults": ["W-FHWJ", "X-6WC7"], "Headquarter": "PH-NFR"},
     "4R-HUN": {"Staging": "IF-KD1", "Vanguards": ["IBOX-2", "TD-4XL", "VW-PXL"], "Assaults": ["8AB-Q4"], "Headquarter": "JA-G0T"},
-    "4SRW-B": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "4SRW-B": {"Staging": "62O-UE", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "4YFT-F": {"Staging": "SG-75T", "Vanguards": ["N3-JBX", "GN-PDU", "9PX2-F"], "Assaults": ["F-5FDA"], "Headquarter": "S1-XTL"},
     "4ZXC-8": {"Staging": "5-IH57", "Vanguards": ["JXQJ-B", "QYT-X8", "Y-BIPM"], "Assaults": ["PND-SI", "XKM-DE"], "Headquarter": "H-MHWF"},
     "5-88B9": {"Staging": "YQB-22", "Vanguards": ["8P9-BM"], "Assaults": ["3GXF-U", "H-GKI6", "VKI-T7"], "Headquarter": "F-YH5B"},
     "50-5UD": {"Staging": "BB-EKF", "Vanguards": ["16AM-3", "B8HU-Z", "BB-EKF", "Q5KZ-W"], "Assaults": ["Q0G-L8", "WE-KK2"], "Headquarter": "A-REKV"},
     "51ZT-6": {"Staging": "U-IVGH", "Vanguards": ["ARG-3R", "K212-A", "K7-LDX", "P-N5N9", "R-3FBU", "S-E6ES"], "Assaults": ["EIN-QG", "JMH-PT", "X9V-15"], "Headquarter": "DE-A7P"},
-    "52-JKU": {"Staging": "Q-CAB2", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "52-JKU": {"Staging": "Q-CAB2", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "59H-0G": {"Staging": "5-VKCN", "Vanguards": ["5KS-AB", "KLYN-8", "Y-W6GF"], "Assaults": ["KFR-ZE", "U0V6-T"], "Headquarter": "D85-VD"},
     "5F8-PZ": {"Staging": "GR-X26", "Vanguards": ["6OU9-U", "9N-0HF", "U-OVFR"], "Assaults": ["9-OUGJ"], "Headquarter": "4NDT-W"},
     "5HN-S5": {"Staging": "U-QMOA", "Vanguards": ["I6-SYN", "O-5TN1", "VK-A5G"], "Assaults": ["B-T6BT"], "Headquarter": "8-SPNN"},
     "5J-SSP": {"Staging": "AFJ-NB", "Vanguards": ["4OIV-X", "TM-0P2", "Y-JKJ8"], "Assaults": ["3-UCBF", "N-CREL"], "Headquarter": "1-7KWU"},
-    "5P4-QA": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "5P4-QA": {"Staging": "M-XUZZ", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "5Y1E-3": {"Staging": "M-MBRT", "Vanguards": ["HPBE-D", "R4N-LD", "TP7-KE"], "Assaults": ["A-4JOO"], "Headquarter": "3Q-VZA"},
     "5YHF-H": {"Staging": "0J3L-V", "Vanguards": ["AZBR-2", "T-GCGL", "Z-8Q65"], "Assaults": ["0MV-4W", "T-GCGL"], "Headquarter": "V-NL3K"},
-    "5Z0Y-S": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "5Z0Y-S": {"Staging": "DJK-67", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "5ZAB-N": {"Staging": "SBEN-Q", "Vanguards": ["4GSZ-1", "E-EFAM", "VEQ-3V"], "Assaults": ["9-7SRQ", "J-QOKQ"], "Headquarter": "4T-VDE"},
     "5ZR-29": {"Staging": "C-LTXS", "Vanguards": ["C0O6-K", "G9NE-B", "HD-AJ7", "SJJ-4F"], "Assaults": ["0RI-OV", "G9NE-B"], "Headquarter": "SR-4EK"},
-    "6-CBBM": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "6-CBBM": {"Staging": "UJXC-B", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "6-UCYU": {"Staging": "I3Q-II", "Vanguards": ["0N-3RO", "319-3D", "YZ9-F6"], "Assaults": ["FWST-8"], "Headquarter": "G-TT5V"},
     "6-V49K": {"Staging": "EF-F36", "Vanguards": ["3-IN0V", "DUV-5Y", "GRNJ-3"], "Assaults": ["D-B7YK"], "Headquarter": "Z-QENW"},
     "6GU-AT": {"Staging": "YC-ANK", "Vanguards": ["G-HE0N", "J7X-VN", "LTT-AP", "UAJ5-K"], "Assaults": ["2WU-XT", "9S-GPT", "XJ-AG7"], "Headquarter": "F-WCLC"},
     "6I-3VX": {"Staging": "T-AKQZ", "Vanguards": ["0P-U0Q", "G-D0N3", "XGH-SH"], "Assaults": ["B-6STA"], "Headquarter": "7KIK-H"},
     "6JCS-4": {"Staging": "BUZ-DB", "Vanguards": ["JGW-OT", "KB-U56", "KH0Z-0", "UCG4-B"], "Assaults": ["5-N2EY", "NH-1X6"], "Headquarter": "K717-8"},
     "6KFH-X": {"Staging": "E2-RDQ", "Vanguards": ["HIX4-H", "OY0-2T", "TN25-J"], "Assaults": ["GR-J8B"], "Headquarter": "ZU-MS3"},
     "6TT8-Z": {"Staging": "1H5-3W", "Vanguards": ["GTY-FW", "QZV-X3", "RV-GA8", "TP-RTO"], "Assaults": ["JTA2-2", "R-6KYM"], "Headquarter": "3H58-R"},
@@ -241,25 +258,25 @@
     "760-9C": {"Staging": "Z-A8FS", "Vanguards": ["07-SLO", "DUO-51", "J-RXYN"], "Assaults": ["GPD5-0"], "Headquarter": "GRHS-B"},
     "78-6RI": {"Staging": "6V-D0E", "Vanguards": ["BVRQ-O", "LS3-HP", "QX-4HO"], "Assaults": ["FBH-JN"], "Headquarter": "SH6X-F"},
     "7UNX-J": {"Staging": "5-A0PX", "Vanguards": ["CLW-SI", "O7-RFZ", "R-RMDH"], "Assaults": ["SH-YZY"], "Headquarter": "Z-EKCY"},
     "7VJ-7M": {"Staging": "A-80UA", "Vanguards": ["4E-EZS", "C8-7AS", "ZNF-OK"], "Assaults": ["8Q-T7B"], "Headquarter": "WV0D-1"},
     "7X-X1Y": {"Staging": "WQY-IQ", "Vanguards": ["8W-OSE", "E9KD-N", "FIO1-8"], "Assaults": ["C-OK0R", "YKSC-A"], "Headquarter": "0-ARFO"},
     "7ZRW-G": {"Staging": "Q1-R7K", "Vanguards": ["6-TYRX", "IR-FDV", "NIZJ-0", "V1ZC-S"], "Assaults": ["111-F1", "J-RVGD"], "Headquarter": "H-T40Z"},
     "8-4EFQ": {"Staging": "M4-GJ6", "Vanguards": ["2JT-3Q", "2JT-3Q", "I3CR-F", "SN9-3Z"], "Assaults": ["2-Q4YG", "7-JT09"], "Headquarter": "AGCP-I"},
-    "8-IL7S": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "8-IL7S": {"Staging": "0P9Z-I", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "88G-M4": {"Staging": "JZV-F4", "Vanguards": ["MGAM-4", "Q3-BAY", "VORM-W"], "Assaults": ["7G-H7D"], "Headquarter": "R-RSZZ"},
     "8AO-5V": {"Staging": "8KE-YS", "Vanguards": ["LXQ2-T", "O-LJOO", "ZS-PNI"], "Assaults": ["TZ-74M"], "Headquarter": "43-1TL"},
     "8BO-IH": {"Staging": "K-L690", "Vanguards": ["9CG6-H", "NDII-Q", "W6V-VM"], "Assaults": ["UYU-VV"], "Headquarter": "P-ZMZV"},
-    "8ET-D1": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "8ET-D1": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "8G-JN6": {"Staging": "FKR-SR", "Vanguards": ["5U-3PW", "89JS-J", "C9R-NO"], "Assaults": ["CYB-BZ"], "Headquarter": "KMH-J1"},
     "8K-CHA": {"Staging": "9-KWXC", "Vanguards": ["3USX-F", "K42-IE", "VSJ-PP"], "Assaults": ["39-DGG", "6RQ9-A"], "Headquarter": "SV-K8J"},
     "8MJO-4": {"Staging": "L-AS00", "Vanguards": ["6T3I-L", "AXDX-F", "QSF-EJ"], "Assaults": ["PEM-LC", "X-EHHD"], "Headquarter": "J-4FNO"},
     "8T-OLH": {"Staging": "5-9UXZ", "Vanguards": ["Q0OH-V", "X-7BIX", "C9N-CC", "DTX8-M"], "Assaults": ["JAUD-V", "4-OUKF"], "Headquarter": "HAJ-DQ"},
     "8UD2-J": {"Staging": "ND-GL4", "Vanguards": ["1S-SU1", "HD-HOZ", "LEM-I1"], "Assaults": ["42G-OB", "V2-GZS"], "Headquarter": "G4-QU6"},
-    "9BGY-6": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "9BGY-6": {"Staging": "G-GRSZ", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "9D1V-O": {"Staging": "IPX-H5", "Vanguards": ["QS-530", "VR-YRV", "X-HISR"], "Assaults": ["29YH-V", "DL-CDY"], "Headquarter": "LG-RO2"},
     "9HXQ-G": {"Staging": "MY-W1V", "Vanguards": ["3-OKDA", "4M-HGL", "3GD6-8"], "Assaults": ["YHN-3K", "GE-8JV"], "Headquarter": "AX-DOT"},
     "9KX-M0": {"Staging": "9-GBPD", "Vanguards": ["A3-RQ3", "LS-JEP", "PX5-LR"], "Assaults": ["WMBZ-U"], "Headquarter": "A-QRQT"},
     "9NP-KR": {"Staging": "A-5F4A", "Vanguards": ["Q2-N6W", "LNVW-K", "P4-3TJ", "K-Z0V4", "8B-SAJ"], "Assaults": ["W-IX39", "K-B8DK", "L-6W1J"], "Headquarter": "C-9RRR"},
     "9P57-V": {"Staging": "S-1LIO", "Vanguards": ["1BWK-S", "NV-3KA", "RKE-CP"], "Assaults": ["KMV-CQ"], "Headquarter": "U1TX-A"},
     "A-JI5E": {"Staging": "JA-O6J", "Vanguards": ["CX65-5", "SNFV-I", "V2-VC2"], "Assaults": ["8B-2YA", "HP-64T"], "Headquarter": "L-B55M"},
     "A-Z7C9": {"Staging": "A-BO4V", "Vanguards": ["T8T-RA", "V-3U8T", "SKR-SP"], "Assaults": ["GOP-GE"], "Headquarter": "MKD-O8"},
@@ -277,306 +294,306 @@
     "B-MQ0Y": {"Staging": "EF-QZK", "Vanguards": ["0FG-KS", "E-WMT7", "F-5WYK"], "Assaults": ["RZ3O-K"], "Headquarter": "FLK-LJ"},
     "B4H-9W": {"Staging": "AJI-MA", "Vanguards": ["HM-XR2", "NOL-M9", "O-IOAI"], "Assaults": ["QX-LIJ"], "Headquarter": "4K-TRB"},
     "Balenne": {"Staging": "O-IVNH", "Vanguards": ["1-NW2G", "F7C-H0", "O-ZXUV"], "Assaults": ["77-KDQ", "FD53-H"], "Headquarter": "TN-T7T"},
     "Basilisk": {"Staging": "Y-2ANO", "Vanguards": ["G1CA-Y", "LBGI-2", "WMH-SO"], "Assaults": ["4HS-CR"], "Headquarter": "Z-YN5Y"},
     "BB-48X": {"Staging": "B-U299", "Vanguards": ["5ED-4E", "DN58-U", "JE-VLG"], "Assaults": ["C2-1B5"], "Headquarter": "87-1PM"},
     "BB8E-G": {"Staging": "AI-EVH", "Vanguards": ["F-MKH3", "V-2GYS", "W-RFUO", "ZM-DNR"], "Assaults": ["0NV-YU", "168-6H", "WPR-EI"], "Headquarter": "VKU-BG"},
     "Belt": {"Staging": "J1H-R4", "Vanguards": ["0-9UHT", "0-WVQS", "5WAE-M"], "Assaults": ["H-M1BY"], "Headquarter": "M-NKZM"},
-    "BI-NFW": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "BI-NFW": {"Staging": "SVB-RE", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "BRP2-K": {"Staging": "4-07MU", "Vanguards": ["25S-6P", "6BPS-T", "RR-D05"], "Assaults": ["FAT-6P", "Y-PNRL"], "Headquarter": "CNC-4V"},
     "BUG6-X": {"Staging": "5ZO-NZ", "Vanguards": ["7-UH4Z", "X97D-W", "Y0-BVN"], "Assaults": ["FS-RFL", "N-HSK0"], "Headquarter": "05R-7A"},
     "BVA-YH": {"Staging": "E1W-TB", "Vanguards": ["2-2EWC", "995-3G", "LMM7-L"], "Assaults": ["D-6H64"], "Headquarter": "8-BIE3"},
     "BXT7-V": {"Staging": "W-KXEX", "Vanguards": ["M-SG47", "SR-10Z", "TAL1-3"], "Assaults": ["2-YO2K"], "Headquarter": "QHY-RU"},
     "BZ-10K": {"Staging": "X7R-JW", "Vanguards": ["LRWD-B", "M-HU4V", "QXQ-BA"], "Assaults": ["T-Q2DD"], "Headquarter": "8-4GQM"},
-    "BZZ-1U": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "BZZ-1U": {"Staging": "T6GY-Y", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "C-ULS4": {"Staging": "P7Z-R3", "Vanguards": ["4-BE0M", "A-G1FM", "ZIU-EP"], "Assaults": ["3-N3OO", "I-7RIS"], "Headquarter": "CS-ZGD"},
     "C45-9Y": {"Staging": "C-0ND2", "Vanguards": ["5XR-KZ", "75C-WN", "JI-LGM", "PO-3QW", "VF-FN6", "Y-YGMW"], "Assaults": ["BG-W90", "I5Q2-S", "OCU4-R"], "Headquarter": "Z-PNIA"},
     "C73-U5": {"Staging": "Q-HJ97", "Vanguards": ["GM-0K7", "RF6T-8", "Z4-QLD", "ZJA-6U"], "Assaults": ["94FR-S", "E1F-LK", "I-NGI8"], "Headquarter": "R-ZUOL"},
-    "C9XB-L": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "C9XB-L": {"Staging": "P-8PDJ", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Centaur": {"Staging": "D2AH-Z", "Vanguards": ["7X-02R", "EI-O0O", "J5A-IX"], "Assaults": ["Z9PP-H"], "Headquarter": "7-8S5X"},
     "Chimera": {"Staging": "AV-VB6", "Vanguards": ["6VDT-H", "7BX-6F", "NDH-NV", "XJP-Y7"], "Assaults": ["15U-JY", "NY6-FH", "QV28-G"], "Headquarter": "HMF-9D"},
     "CL-QB2": {"Staging": "M-4KDB", "Vanguards": ["FE-6YQ", "W-16DY", "ZMV9-A"], "Assaults": ["S-9RCJ", "C-FD0D"], "Headquarter": "ZD1-Z2"},
-    "CN5-F2": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
-    "Crown": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "CN5-F2": {"Staging": "OX-S7P", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
+    "Crown": {"Staging": "UO9-YG", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "CZ-06R": {"Staging": "R8WV-7", "Vanguards": ["LQQH-J", "X-Z4JW", "W5-VBR"], "Assaults": ["Y-770C"], "Headquarter": "J-D5U7"},
     "D-95MV": {"Staging": "U-MFTL", "Vanguards": ["A-7XFN", "DX-TAR", "O3-4MN", "T-0JWP"], "Assaults": ["7-P1JO", "EDQG-L", "TYB-69"], "Headquarter": "J-L9MA"},
     "D-AWFI": {"Staging": "RG9-7U", "Vanguards": ["A4L-A2", "CZDJ-1", "UJY-HE"], "Assaults": ["UEJX-G"], "Headquarter": "U-TJ7Y"},
     "D-GU3R": {"Staging": "5J-62N", "Vanguards": ["8-MXHA", "LPVL-5", "Z-DRIY"], "Assaults": ["AID-9T", "PXE-RG"], "Headquarter": "D3S-EA"},
     "D-YKXH": {"Staging": "QZ1-OH", "Vanguards": ["5B-YDD", "PWPY-4", "Y-XZA7"], "Assaults": ["W-XY4J"], "Headquarter": "2XI8-Y"},
     "D4J-PP": {"Staging": "P-ZWKH", "Vanguards": ["QY2Y-N", "X-9ZZR", "VZEG-B"], "Assaults": ["HO4E-Q", "RO-AIQ"], "Headquarter": "E6Q-LE"},
     "D5-SOW": {"Staging": "4O-239", "Vanguards": ["Q-JQSG", "T-IPZB", "T-M0FA"], "Assaults": ["QC-YX6"], "Headquarter": "LUA5-L"},
     "D61-WV": {"Staging": "OZ-DS5", "Vanguards": ["91-KD8", "0PU2-R", "XM-RMD"], "Assaults": ["B-ETDW"], "Headquarter": "9G5J-1"},
     "D9DM-O": {"Staging": "ZDYA-G", "Vanguards": ["LX5K-W", "MP5-KR", "O-N589"], "Assaults": ["ZBY-0I"], "Headquarter": "LD-2VL"},
     "DA0V-R": {"Staging": "T-67F8", "Vanguards": ["58Z-IH", "CHP-76", "M-VACR"], "Assaults": ["E0DR-G", "KI2-S3"], "Headquarter": "0B-VOJ"},
     "DILJ-7": {"Staging": "1N-FJ8", "Vanguards": ["0R-F2F", "2DWM-2", "R-P7KL"], "Assaults": ["XF-PWO"], "Headquarter": "669-IX"},
     "DITJ-X": {"Staging": "1QZ-Y9", "Vanguards": ["4-CM8I", "B-1UJC", "ZDB-HT"], "Assaults": ["Q4C-S5"], "Headquarter": "Q-NA5H"},
     "DJ-XCW": {"Staging": "M3-KAQ", "Vanguards": ["6-L4YC", "GPLB-C", "U104-3"], "Assaults": ["5E-CMA"], "Headquarter": "GGE-5Q"},
-    "DMXN-3": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
-    "DOCS-O": {"Staging": "XXZ-3W", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "DMXN-3": {"Staging": "N-5QPW", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
+    "DOCS-O": {"Staging": "XXZ-3W", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "DS-M4Q": {"Staging": "0EK-NJ", "Vanguards": ["PFP-GU", "T-LIWS", "UM-Q7F", "V4-L0X"], "Assaults": ["1-NKVT", "AAS-8R", "KTHT-O"], "Headquarter": "QWF-6P"},
     "DYK-G8": {"Staging": "4M-P1I", "Vanguards": ["H7O-JZ", "O-RXCZ", "WE3-BX"], "Assaults": ["H-8F5Q"], "Headquarter": "LXTC-S"},
     "E-312G": {"Staging": "YG-82V", "Vanguards": ["5LJ-MD", "B8O-KJ", "QCWA-Z", "UB-UQZ", "XM-4L0"], "Assaults": ["52G-NZ", "KV-8SN", "Z-K495"], "Headquarter": "6-O5GY"},
     "E-72A3": {"Staging": "3-QYVE", "Vanguards": ["P-UCRP", "T-K10W", "V-LDEJ"], "Assaults": ["7D-PAT"], "Headquarter": "C-XNUA"},
     "E-8CSQ": {"Staging": "BR-6XP", "Vanguards": ["8-TFDX", "G5ED-Y", "UL-4ZW"], "Assaults": ["O-LR1H", "Y5J-EU"], "Headquarter": "B-E3KQ"},
     "E-95ID": {"Staging": "S0U-MO", "Vanguards": ["V-QXXK", "W-6GBI", "XKH-6O"], "Assaults": ["XQP-9C"], "Headquarter": "F39H-1"},
-    "E-I1JW": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "E-I1JW": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "E-IFSA": {"Staging": "2PG-KN", "Vanguards": ["9-MJVQ", "PDF-3Z", "PEK-8Z"], "Assaults": ["4-IT9G", "C3-0YD"], "Headquarter": "L2GN-K"},
     "E-ILCH": {"Staging": "MS2-V8", "Vanguards": ["02V-BK", "JD-TYH", "R-ARKN"], "Assaults": ["SN9S-N"], "Headquarter": "A5MT-B"},
-    "E-UBWI": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "E-UBWI": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "E1L-UY": {"Staging": "GTB-O4", "Vanguards": ["EU-WFW", "K-YL9T", "Y4B-BQ"], "Assaults": ["G-VFVB"], "Headquarter": "P65-TA"},
     "E3-NLE": {"Staging": "3G-LHB", "Vanguards": ["9GI-FB", "DBT-GB", "U-W3WS"], "Assaults": ["L-1HKR"], "Headquarter": "PBD-0G"},
     "E65-47": {"Staging": "ZWM-BB", "Vanguards": ["7-QOYS", "KS8G-M", "LH-LY1"], "Assaults": ["OTJ9-E"], "Headquarter": "S-CUEA"},
     "E6EO-H": {"Staging": "XU-BF8", "Vanguards": ["DAI-SH", "RIU-GC", "S-R9J2", "V3P-AZ"], "Assaults": ["F-WZYG", "X1W-AL"], "Headquarter": "C-KW6X"},
     "EIX-HK": {"Staging": "WSK-1A", "Vanguards": ["5-NZNW", "8-BEW8", "NZW-ZO"], "Assaults": ["MS1-KJ", "Y-EQ0C"], "Headquarter": "7M4C-F"},
     "EK-NQ2": {"Staging": "Z-N9IP", "Vanguards": ["442-CS", "9ZFH-Z", "TWJ-AW"], "Assaults": ["4-MPSJ", "PZMA-E"], "Headquarter": "N-7ECY"},
     "EL8Z-M": {"Staging": "U79-JF", "Vanguards": ["9-XN3F", "AC-7LZ", "Y-FZ5N"], "Assaults": ["E8-YS9"], "Headquarter": "LBA-SO"},
-    "Elysium": {"Staging": "8G-MQV", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "Elysium": {"Staging": "8G-MQV", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "EM-L3K": {"Staging": "L7XS-5", "Vanguards": ["1P-WGB", "K0CN-3", "VA6-DR"], "Assaults": ["F4R2-Q"], "Headquarter": "WLAR-J"},
     "ENP-SH": {"Staging": "2-KPW6", "Vanguards": ["LBC-AW", "Q-K2T7", "XV-MWG"], "Assaults": ["1V-LI2", "OAQY-M"], "Headquarter": "M9-MLR"},
-    "F-I56R": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "F-I56R": {"Staging": "M-SRKS", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "F-RA63": {"Staging": "RF-CN3", "Vanguards": ["C-7SBM", "DS-LO3", "Z-UZZN"], "Assaults": ["BX2-ZX"], "Headquarter": "YW-SYT"},
     "F-V9QW": {"Staging": "Y-ZXIO", "Vanguards": ["G96R-F", "C-FP70", "ZA0L-U"], "Assaults": ["1-GBBP"], "Headquarter": "T-ZWA1"},
     "F-W6B4": {"Staging": "1-HDQ4", "Vanguards": ["1EO-OE", "5-9L3H", "YQTK-R"], "Assaults": ["6U-MFQ"], "Headquarter": "FZCR-3"},
     "F-ZNNG": {"Staging": "E-91FV", "Vanguards": ["54-MF6", "AD-5B8", "G-73MR", "QP0K-B"], "Assaults": ["EOA-ZC", "TJM-JJ"], "Headquarter": "UBX-CC"},
     "F5-O9O": {"Staging": "OQTY-Z", "Vanguards": ["G1-0UI", "QLU-P0", "XUDX-A"], "Assaults": ["DZ6-I5", "QCDG-H"], "Headquarter": "R-XDKM"},
     "FD-7Y4": {"Staging": "38NZ-1", "Vanguards": ["74L2-U", "HL-VZX", "W-MF6J"], "Assaults": ["D-P1EH", "HZ-O18"], "Headquarter": "N-O53U"},
     "FDR-EQ": {"Staging": "X3FQ-W", "Vanguards": ["3-SFWG", "A-VILQ", "CB4-Q2", "N-8BZ6"], "Assaults": ["CBL-XP", "WJ-9YO"], "Headquarter": "UQ-PWD"},
     "FQ-COP": {"Staging": "LJ-RJK", "Vanguards": ["4YO-QK", "8-VC6H", "U93O-A"], "Assaults": ["BTLH-I"], "Headquarter": "0LY-W1"},
     "FY6-NK": {"Staging": "B1D-KU", "Vanguards": ["2R-KLH", "6SB-BN", "QFIU-K"], "Assaults": ["KSM-1T"], "Headquarter": "YRV-MZ"},
     "G-HISF": {"Staging": "APES-G", "Vanguards": ["2Z-HPQ", "6-WMKE", "I8-AJY", "J-Z8C2"], "Assaults": ["1-EVAX", "B2J-5N"], "Headquarter": "XTVZ-E"},
-    "G2E-RJ": {"Staging": "49GC-R", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "G2E-RJ": {"Staging": "49GC-R", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "G3-MU3": {"Staging": "1M7-RK", "Vanguards": ["5HN-D6", "MK-YNM", "P-H5IY"], "Assaults": ["2-9Z6V", "4A-6NI"], "Headquarter": "E-B957"},
-    "G3IP-E": {"Staging": "TY2X-C", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "G3IP-E": {"Staging": "TY2X-C", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "G8-D09": {"Staging": "R-LW2I", "Vanguards": ["3V8-LJ", "4-ABS8", "DP-1YE"], "Assaults": ["B8EN-S"], "Headquarter": "R6XN-9"},
     "GDBW-2": {"Staging": "UYG-YX", "Vanguards": ["06-70G", "GL6S-2", "LO5-LN", "LO5-LN"], "Assaults": ["C-NMG9", "NBW-GD", "YM-SRU"], "Headquarter": "P3X-TN"},
     "GEP-XF": {"Staging": "G-M4GK", "Vanguards": ["0SUF-3", "GQ2S-8", "KU3-BB", "O1Q-P1"], "Assaults": ["2I-520", "G1D0-G"], "Headquarter": "O-97ZG"},
     "GFE-SS": {"Staging": "HE5T-A", "Vanguards": ["0M-103", "6OYQ-Z", "Z-LO6I"], "Assaults": ["O36A-P"], "Headquarter": "DCJ-ZT"},
     "GJH-1C": {"Staging": "OEG-K9", "Vanguards": ["B-5UFY", "PQRE-W", "V-4DBR"], "Assaults": ["SK42-F", "WU-FHQ"], "Headquarter": "EU9-J3"},
-    "GORV-P": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "GORV-P": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "GP-GIU": {"Staging": "KL3O-J", "Vanguards": ["3-TD6L", "Q-NJZ4", "R4O-I6"], "Assaults": ["NLPB-0"], "Headquarter": "CX-1XF"},
     "GN-ACS": {"Staging": "VLGD-R", "Vanguards": ["10UZ-P", "9GYL-O", "S-GKKR"], "Assaults": ["9U-TTJ"], "Headquarter": "EN-VOD"},
     "Griffin": {"Staging": "TU-Y2A", "Vanguards": ["38IA-E", "7BIX-A", "M-KXEH"], "Assaults": ["G-UTHL"], "Headquarter": "LIWW-P"},
     "GU-JZ1": {"Staging": "JEQG-7", "Vanguards": ["5NQI-E", "B-WQDP", "OR-7N5"], "Assaults": ["7K-NSE"], "Headquarter": "L-Z9KJ"},
     "H-6HGD": {"Staging": "0-WT2D", "Vanguards": ["7V-KHW", "O3L-95", "T8H-66"], "Assaults": ["A3-LOG"], "Headquarter": "A2-V27"},
     "H-KW4A": {"Staging": "TXJ-II", "Vanguards": ["7YWV-S", "C1-HAB", "GA9P-0"], "Assaults": ["H9-J8N", "HP-6Z6"], "Headquarter": "2V-CS5"},
     "H7Q-DG": {"Staging": "C-V6DQ", "Vanguards": ["1PF-BC", "EX-GBT", "Z-FET0"], "Assaults": ["D-OJEZ"], "Headquarter": "QHJR-E"},
     "Hale": {"Staging": "J4UD-J", "Vanguards": ["BPK-XK", "CL-1JE", "G-0Q86", "LJ-YSW"], "Assaults": ["K88X-J", "Y-K50G"], "Headquarter": "G-R4W1"},
     "Heart": {"Staging": "F5FO-U", "Vanguards": ["4C-B7X", "BF-SDP", "LGUZ-1"], "Assaults": ["D5IW-F", "F-XWIN"], "Headquarter": "1L-BHT"},
     "Heaven": {"Staging": "Jamunda", "Vanguards": ["Doril", "Litom", "Utopia"], "Assaults": ["Hemin", "Jorund"], "Headquarter": "Farit"},
-    "HNZF-Z": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "HNZF-Z": {"Staging": "KIG9-K", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "HOV-VI": {"Staging": "I-9GI1", "Vanguards": ["DVWV-3", "DX-DFJ", "KE-0FB"], "Assaults": ["SY-UWN", "U0W-DR"], "Headquarter": "X-31TE"},
     "HRJG-D": {"Staging": "V-IH6B", "Vanguards": ["BRT-OP", "JUK0-1", "66U-1P"], "Assaults": ["V89M-R"], "Headquarter": "OJOS-T"},
-    "HS7W-T": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "HS7W-T": {"Staging": "ZT-LPU", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Hydra": {"Staging": "87XQ-0", "Vanguards": ["KVN-36", "LJ-TZW", "TEG-SD"], "Assaults": ["14YI-D", "J-RQMF"], "Headquarter": "I-CUVX"},
     "I-3ODK": {"Staging": "TSG-NO", "Vanguards": ["BJD4-E", "BLC-X0", "K-X5AX"], "Assaults": ["3L-Y9M", "O9V-R7"], "Headquarter": "DUU1-K"},
     "I-CCEI": {"Staging": "JK-GLL", "Vanguards": ["8Q-UYU", "LUL-WX"], "Assaults": ["3PPT-9", "S-KU8B", "UAAU-C"], "Headquarter": "YV-FDG"},
     "I-WRVM": {"Staging": "9-WEMC", "Vanguards": ["CUT-0V", "O-F4SN", "QT-EBC"], "Assaults": ["FV1-RQ"], "Headquarter": "VAF1-P"},
     "I3-2J0": {"Staging": "M9U-75", "Vanguards": ["K-IYNW", "N-RAEL", "UD-AOK"], "Assaults": ["28-QWU"], "Headquarter": "0-3VW8"},
     "I89-EP": {"Staging": "YMJG-4", "Vanguards": ["4-HWWF", "8TPX-N", "PM-DWE"], "Assaults": ["4GYV-Q"], "Headquarter": "WBR5-R"},
-    "I9B-8X": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "I9B-8X": {"Staging": "SI-I89", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "ICH-B6": {"Staging": "I64-XB", "Vanguards": ["2B-UUQ", "N-SFZK", "NWX-LI"], "Assaults": ["9QS5-C", "ALC-JM"], "Headquarter": "Z0G-XG"},
     "IJE6-J": {"Staging": "QN-6J2", "Vanguards": ["DR-427", "FRTC-5", "M-ZJWJ", "O7-VJ5"], "Assaults": ["KCDX-7", "NI-J0B", "R-ORB7"], "Headquarter": "RU-PT9"},
-    "IM-8S5": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "IM-8S5": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "IPS-QB": {"Staging": "RLSI-V", "Vanguards": ["4-CUM5", "8MG-J6", "BWF-ZZ"], "Assaults": ["IOO-7O"], "Headquarter": "BND-16"},
     "IV-LWJ": {"Staging": "PT-21C", "Vanguards": ["5M2-KP", "EKPB-3", "TK-DLH"], "Assaults": ["KD-KPR", "Z182-R"], "Headquarter": "KDG-TA"},
     "IYOO-M": {"Staging": "GF-3FL", "Vanguards": ["0R-GZQ", "9-34L5", "QM-20X"], "Assaults": ["ZJ-GOU"], "Headquarter": "QQ3-YI"},
     "IZ-FBT": {"Staging": "LG-WA9", "Vanguards": ["AA-GWF", "O4T-Z5", "ZWV-GD"], "Assaults": ["1DDR-X"], "Headquarter": "HHJD-5"},
     "J-78ZG": {"Staging": "CL-IRS", "Vanguards": ["MO-I1W", "O-EUHA", "QBZO-R", "ZZ5X-M"], "Assaults": ["3IK-7O", "HV-EAP"], "Headquarter": "UAV-1E"},
     "J-9M7D": {"Staging": "EIH-IU", "Vanguards": ["4-EFLU", "F-QQ5N", "U-HVIX"], "Assaults": ["1-7B6D"], "Headquarter": "H6-EYX"},
     "J0-59Y": {"Staging": "6U-1RX", "Vanguards": ["FO1U-K", "VX1-HV", "Y4OK-W"], "Assaults": ["JNG7-K", "K-XJJT"], "Headquarter": "P-NI4K"},
     "J33-JR": {"Staging": "TFPT-U", "Vanguards": ["6-GRN7", "D-JVGJ", "YQM-P1"], "Assaults": ["1-10QG", "WIO-OL"], "Headquarter": "WK2F-Y"},
     "J8-G8K": {"Staging": "VQE-CN", "Vanguards": ["8KR9-5", "EIMJ-M", "Y-CWQY"], "Assaults": ["1-NJLK", "L5D-ZL"], "Headquarter": "G-C8QO"},
-    "JE7-F2": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "JE7-F2": {"Staging": "KMC-WI", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "JQA8-6": {"Staging": "H-P4LB", "Vanguards": ["2UK4-N", "5ELE-A", "BJ-ZFD"], "Assaults": ["H65-HE", "M-CMLV"], "Headquarter": "QK-CDG"},
     "JQV5-9": {"Staging": "CY-ZLP", "Vanguards": ["98Q-8O", "U4-Q2V", "ZV-72W"], "Assaults": ["2G38-I"], "Headquarter": "S-U8A4"},
     "JSZ-X6": {"Staging": "CR-0E5", "Vanguards": ["16P-PX", "WX-6UX", "Z-Y9C3"], "Assaults": ["XKZ8-H"], "Headquarter": "BZ-0GW"},
     "JZV-O6": {"Staging": "FZ-6A5", "Vanguards": ["6-MM99", "JBY6-F", "MB-NKE"], "Assaults": ["G-7WUF"], "Headquarter": "RNF-YH"},
     "K-DLD2": {"Staging": "N-6Z8B", "Vanguards": ["504Z-V", "AB-FZE", "F8K-WQ"], "Assaults": ["NE-3GR"], "Headquarter": "YUY-LM"},
     "K-JO26": {"Staging": "UVHO-F", "Vanguards": ["H-4R6Z", "IGE-NE", "Z-XX2J"], "Assaults": ["8-SNUD"], "Headquarter": "OGY-6D"},
     "K-N3MD": {"Staging": "B-KDOZ", "Vanguards": ["LK1K-5", "QE-E1D", "Z-H2MA"], "Assaults": ["4-GB14", "REB-KR"], "Headquarter": "L-5JCJ"},
     "K-QUVW": {"Staging": "J-OK0C", "Vanguards": ["6GWE-A", "KDV-DE", "MT9Q-S"], "Assaults": ["UC3H-Y"], "Headquarter": "RD-G2R"},
     "K-ZKBM": {"Staging": "O7-7UX", "Vanguards": ["B9E-H6", "JDAS-0", "Y19P-1", "Y2-QUV"], "Assaults": ["A4B-V5", "LN-56V"], "Headquarter": "SPBS-6"},
-    "KPU3-3": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
-    "KR-XF4": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "KPU3-3": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
+    "KR-XF4": {"Staging": "u6D-9A", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Kraken": {"Staging": "Z30S-A", "Vanguards": ["671-ST", "A-HZYL", "ESC-RI"], "Assaults": ["H-S80W"], "Headquarter": "UAYL-F"},
     "KUSW-P": {"Staging": "RBW-8G", "Vanguards": ["A-CJGE", "G2-INZ", "WAC-HW"], "Assaults": ["HHQ-M1", "VYJ-DA"], "Headquarter": "HT4K-M"},
     "KWCZ-A": {"Staging": "D4R-H7", "Vanguards": ["EQI2-2", "J9-5MQ", "Q-4DEC"], "Assaults": ["313I-B"], "Headquarter": "4DTQ-K"},
     "L-1T22": {"Staging": "AZ-UWB", "Vanguards": ["H-S5BM", "OJ-CT4", "SHJO-J"], "Assaults": ["430-BE", "LHJ-2G"], "Headquarter": "6UQ-4U"},
     "L-H07K": {"Staging": "U1-C18", "Vanguards": ["6O-XIO", "NX5W-U", "U-JJEW"], "Assaults": ["NW2S-A", "U-BXU9"], "Headquarter": "ZXOG-O"},
     "L-TEVM": {"Staging": "F7A-MR", "Vanguards": ["HB-1NJ", "O-8SOC", "PUZ-IO"], "Assaults": ["P7UZ-T"], "Headquarter": "EOE3-N"},
     "L7-RDZ": {"Staging": "UYOC-1", "Vanguards": ["4-1ECP", "5-U12M", "7AH-SF"], "Assaults": ["7MMJ-3", "9-EXU9"], "Headquarter": "PVF-N9"},
     "LI-BA0": {"Staging": "U-HYZN", "Vanguards": ["3-FKCZ", "I1Y-IU", "LS-V29"], "Assaults": ["9SBB-9"], "Headquarter": "ED-L9T"},
     "LIB-F9": {"Staging": "1IX-C0", "Vanguards": ["PUWL-4", "W-4FA9", "Y-1918"], "Assaults": ["2B7A-3", "3F-JZF"], "Headquarter": "5-0WB9"},
     "LLAP-1": {"Staging": "H-W9TY", "Vanguards": ["15W-GC", "C2X-M5", "MSHD-4"], "Assaults": ["PNDN-V"], "Headquarter": "N-FK87"},
-    "LN-L8L": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "LN-L8L": {"Staging": "E-Z2Zx", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "LSC-4P": {"Staging": "PF-KUQ", "Vanguards": ["8F-TK3", "9O-8W1", "UEXO-Z"], "Assaults": ["GY6A-L"], "Headquarter": "N8D9-Z"},
-    "LWMW-6": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "LWMW-6": {"Staging": "L5Y4-M", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "LY-FY6": {"Staging": "Q-5211", "Vanguards": ["CR-AQH", "M-YCD4", "R-2R0G"], "Assaults": ["XQ-PXU"], "Headquarter": "WW-KGD"},
     "M-J57M": {"Staging": "0-UVHJ", "Vanguards": ["EOY-BG", "IG-ZAM", "NCG-PW", "S-EVIQ"], "Assaults": ["3DR-CR", "PNS7-J", "RLTG-3"], "Headquarter": "H1-ESN"},
     "M9-AN3": {"Staging": "1ACJ-6", "Vanguards": ["F9-FUV", "RO-0PZ", "XB-9U2"], "Assaults": ["BNX-AS"], "Headquarter": "FB-MPY"},
     "Manticore": {"Staging": "SPLE-Y", "Vanguards": ["9R4-EJ", "K8L-X7", "Q-XEB3"], "Assaults": ["Y-1W01"], "Headquarter": "E-BWUU"},
     "MDM8-J": {"Staging": "D7T-C0", "Vanguards": ["2D-0SO", "O-BY0Y", "UR-E6D"], "Assaults": ["X47L-Q"], "Headquarter": "KQK1-2"},
-    "Mermaid": {"Staging": "L7-APB", "Vanguards": [], "Assaults": [], "Headquarter": ""},
-    "Miennue": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
-    "Minotaur": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "Mermaid": {"Staging": "L7-APB", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
+    "Miennue": {"Staging": "X-M9ON", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
+    "Minotaur": {"Staging": "PXF-RF", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "MK7-AO": {"Staging": "A-3ES3", "Vanguards": ["6-U2M8", "617I-I", "DP34-U", "I0AB-R", "MXYS-8", "XS-XAY"], "Assaults": ["35-RK9", "IIRH-G", "VV-VCR"], "Headquarter": "5-75MB"},
     "MPJW-6": {"Staging": "N-M1A3", "Vanguards": ["3-JCJT", "49-U6U", "5V-BJI", "8QT-H4", "M1BZ-2"], "Assaults": ["4-GJT1", "L3-I3K", "W-IIYI"], "Headquarter": "AO-N1P"},
     "MRC-29": {"Staging": "PKN-NJ", "Vanguards": ["LQ-01M", "NG-M8K", "RV5-TT"], "Assaults": ["K85Y-6"], "Headquarter": "8OYE-Z"},
     "MW49-U": {"Staging": "RXTY-4", "Vanguards": ["2FL-5W", "HG-YEQ", "QSCO-D", "RSE-PT"], "Assaults": ["6A-FUY", "863P-X"], "Headquarter": "ZO-YJZ"},
     "MY-HQD": {"Staging": "QRH-BF", "Vanguards": ["M-NP5O", "WIW-X8", "X-KHRZ"], "Assaults": ["L-EUY2"], "Headquarter": "JL-ZUQ"},
-    "MY-QQI": {"Staging": "Z8-81T", "Vanguards": ["DY-P7Q", "H-RXNZ" "XVV-21"], "Assaults": ["ZBP-TP"], "Headquarter": "XD-JW7"},
-    "MZ-PA2": {"Staging": "52CW-6", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "MY-QQI": {"Staging": "Z8-81T", "Vanguards": ["DY-P7Q", "H-RXNZ" ,"XVV-21"], "Assaults": ["ZBP-TP"], "Headquarter": "XD-JW7"},
+    "MZ-PA2": {"Staging": "52CW-6", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "N-39FI": {"Staging": "UR-E46", "Vanguards": ["VYO-68", "TCAG-3", "TPAR-G"], "Assaults": ["CW9-1Y"], "Headquarter": "MG0-RD"},
     "N-APJ8": {"Staging": "4LJ6-Q", "Vanguards": ["G-QTSD", "MF-PGF", "SAH-AD"], "Assaults": ["KGT3-6"], "Headquarter": "L-ZJLN"},
     "N-K4Q0": {"Staging": "OEY-OR", "Vanguards": ["O1-FTD", "2E-ZR5", "SR-KBB"], "Assaults": ["FDZ4-A", "MR4-MY"], "Headquarter": "Roua"},
     "N-LY4R": {"Staging": "LVL-GZ", "Vanguards": ["FN0-QS", "TTP-2B", "X0-6LH"], "Assaults": ["N7-BIY"], "Headquarter": "F3-8X2"},
     "N-OGI1": {"Staging": "2J-WJY", "Vanguards": ["6-K738", "9-8GBA", "ZXIC-7"], "Assaults": ["KDF-GY", "QBQ-RF"], "Headquarter": "QSM-LM"},
     "N-U2LX": {"Staging": "N-TFXK", "Vanguards": ["33RB-O", "3OAT-Q", "DKUK-G"], "Assaults": ["X-Z4DA"], "Headquarter": "C7Y-7Z"},
-    "N32Z-Z": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "N32Z-Z": {"Staging": "AA-YRK", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "N4TD-6": {"Staging": "VY-866", "Vanguards": ["1GT-MA", "D9Z-VY", "HB-5L3", "RGU1-T"], "Assaults": ["MO-YDG", "Q-VTWJ"], "Headquarter": "42SU-L"},
     "N5V-Y0": {"Staging": "KS-1TS", "Vanguards": ["F2A-GX", "RD-FWY", "VBPT-T"], "Assaults": ["ZO-4AR"], "Headquarter": "MJ-LGH"},
     "NJU-QV": {"Staging": "S-6HHN", "Vanguards": ["5-CQDA", "S-6HHN", "ZXB-VC"], "Assaults": ["M2-XFE"], "Headquarter": "KEE-N6"},
     "NK-AOZ": {"Staging": "K25-XD", "Vanguards": ["4VY-Y1", "6L78-1", "6YC-TU", "LU-HQS", "U-L4KS"], "Assaults": ["04-LQM", "LX-ZOJ", "O-VWPB"], "Headquarter": "Y8R-XZ"},
     "NNLX-K": {"Staging": "IS-R7P", "Vanguards": ["BR-N97", "ERVK-P", "S25C-K"], "Assaults": ["UL-7I8"], "Headquarter": "7MD-S1"},
     "NOB-HD": {"Staging": "7F-2FB", "Vanguards": ["4AZV-W", "J-0KB3", "UNV-3J"], "Assaults": ["90-A1P", "GA58-7"], "Headquarter": "UC-8XF"},
-    "NOK-FZ": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "NOK-FZ": {"Staging": "RJ3H-0", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "NPL-WH": {"Staging": "DJ-GBH", "Vanguards": ["0-4VQL", "FVQF-W", "I0N-BM", "SN-DZ6"], "Assaults": ["2ID-87", "8K-QCZ", "XDTW-F"], "Headquarter": "JBUH-H"},
     "NT1-5Q": {"Staging": "DE-IHK", "Vanguards": ["B-B0ME", "OJT-J3", "TDP-T3"], "Assaults": ["H-HGGJ"], "Headquarter": "A9-F18"},
     "NZU8-G": {"Staging": "L-L7PE", "Vanguards": ["7-A6XV", "H-93YV", "QXE-1N", "U69-YC"], "Assaults": ["E51-JE", "W6P-7U"], "Headquarter": "0IF-26"},
     "O-EIMK": {"Staging": "Y-OMTZ", "Vanguards": ["5BTK-M", "8WA-Z6", "8WA-Z6"], "Assaults": ["1DQ1-A", "N-8YET"], "Headquarter": "3-DMQT"},
     "O-EOI9": {"Staging": "U5-XW7", "Vanguards": ["JI-1UQ", "MZPH-W", "W0X-MG"], "Assaults": ["ZK-YQ3"], "Headquarter": "EN-GTB"},
     "O-PQU0": {"Staging": "L-M6JK", "Vanguards": ["P9F-ZG", "PK-PHZ", "QFGB-E"], "Assaults": ["7P-J38", "WT-2J9"], "Headquarter": "C-PEWN"},
     "O5K-Y6": {"Staging": "1B-VKF", "Vanguards": ["E3OI-U", "IP6V-X", "T-J6HT"], "Assaults": ["R5-MM8"], "Headquarter": "RF-K9W"},
     "O5PO-O": {"Staging": "AK-L0Z", "Vanguards": ["2V-ZHM", "V-3K7C", "XU7-CH"], "Assaults": ["R-AG7W"], "Headquarter": "AY9X-Q"},
     "O5QG-M": {"Staging": "ZJG-7D", "Vanguards": ["C-WPWH", "CO-7BI", "LS-QLX"], "Assaults": ["S-XZHU"], "Headquarter": "9MWZ-B"},
     "O6W-QE": {"Staging": "6B-GKA", "Vanguards": ["6E-MOW", "GZ1-A1", "LHGA-W"], "Assaults": ["4RS-L1", "GBT4-J"], "Headquarter": "X-0CKQ"},
     "O9X-CV": {"Staging": "IAMJ-Q", "Vanguards": ["21M1-B", "QZ-DIZ", "U-RELP"], "Assaults": ["UGR-J2", "Y-0HVF"], "Headquarter": "KED-2O"},
     "OC-TTA": {"Staging": "A-J6SN", "Vanguards": ["AG-SYG", "AL-JSG", "C6C-K9", "ETO-OT"], "Assaults": ["1I5-0V", "KPI-OW"], "Headquarter": "OTJ-4W"},
     "OFQ-HG": {"Staging": "MSKR-1", "Vanguards": ["J94-MU"], "Assaults": ["JO-32L", "M2GJ-X", "UB5Z-3"], "Headquarter": "YHP2-D"},
-    "OK-FEM": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
-    "OSJ7-I": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "OK-FEM": {"Staging": "M0O-JG", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
+    "OSJ7-I": {"Staging": "FMBR-8", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "OWT3-6": {"Staging": "XR-ZL7", "Vanguards": ["GF-GR7", "HPMN-V", "Z19-B8"], "Assaults": ["DVN6-0"], "Headquarter": "U1-VHY"},
-    "OY3-DM": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "OY3-DM": {"Staging": "MVUO-F", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "P-B2NE": {"Staging": "O9K-FT", "Vanguards": ["FZX-PU", "GQ-7SP", "I2D3-5"], "Assaults": ["BGMZ-0", "R1O-GN"], "Headquarter": "RQOO-U"},
     "P-FL48": {"Staging": "OSW-0P", "Vanguards": ["4DH-ST", "C-BHDN", "R-RE2B"], "Assaults": ["H4X-0I"], "Headquarter": "6W-6O9"},
     "P-I9PF": {"Staging": "V-KDY2", "Vanguards": ["ER2O-Y", "J2-PZ6", "RNM-Y6"], "Assaults": ["AZ3F-N"], "Headquarter": "FYD-TO"},
-    "P6N8-J": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "P6N8-J": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Paradise": {"Staging": "V7D-JD", "Vanguards": ["5E-VR8", "D87E-A", "K-B2D3", "PO4F-3"], "Assaults": ["0SHT-A", "JWJ-P1", "V-IUEL"], "Headquarter": "J7A-UR"},
     "Pegasus": {"Staging": "IR-WT1", "Vanguards": ["3WE-KY", "9-VO0Q", "A8-XBW"], "Assaults": ["4-EP12", "XF-TQL"], "Headquarter": "YZS5-4"},
     "PFL-QY": {"Staging": "T-4H0B", "Vanguards": ["NRD-5Q", "XCZ5-Y", "Z0H2-4"], "Assaults": ["63-7Q6"], "Headquarter": "W5-205"},
     "PG-RWX": {"Staging": "T-IDGH", "Vanguards": ["F69O-M", "RK-Q51", "V-OL61"], "Assaults": ["DYPL-6"], "Headquarter": "M-V0PQ"},
-    "PGPJ-8": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
-    "Phoenix": {"Staging": "WY-9LL", "Vanguards": ["75FA-Z", "Serpentis" "Prime", "YZ-LQL"], "Assaults": ["A-1CON", "D-Q04X"], "Headquarter": "MN5N-X"},
-    "PR-ACX": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "PGPJ-8": {"Staging": "YX-0KH", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
+    "Phoenix": {"Staging": "WY-9LL", "Vanguards": ["75FA-Z", "Serpentis Prime", "YZ-LQL"], "Assaults": ["A-1CON", "D-Q04X"], "Headquarter": "MN5N-X"},
+    "PR-ACX": {"Staging": "1-GBVE", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Prelle": {"Staging": "O-BDXB", "Vanguards": ["9-4RP2", "MJYW-3", "XZH-4X", "Z-Y7R7"], "Assaults": ["FQ9W-C", "G8AD-C"], "Headquarter": "6Z9-0M"},
     "PUB-0R": {"Staging": "1M4-FK", "Vanguards": ["7GCD-P", "G-3BOG", "L-6BE1"], "Assaults": ["K7D-II"], "Headquarter": "V-LEKM"},
     "PX0-P4": {"Staging": "S5W-1Z", "Vanguards": ["7T-0QS", "IL-OL1", "V-JCJS"], "Assaults": ["8C-VE3", "WVJU-4"], "Headquarter": "RWML-A"},
     "Q-2BI6": {"Staging": "FN-GFQ", "Vanguards": ["0-O6XF", "NH-R5B", "VL7-60"], "Assaults": ["D-FVI7"], "Headquarter": "C-VZAK"},
-    "Q-6LG1": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "Q-6LG1": {"Staging": "18XA-C", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Q-IPAA": {"Staging": "PPFB-U", "Vanguards": ["B-A587", "B-S347", "QI-S9W"], "Assaults": ["AF0-V5"], "Headquarter": "NS2L-4"},
     "Q-PVMK": {"Staging": "U3K-4A", "Vanguards": ["OK-6XN", "SUR-F7"], "Assaults": ["7Q-8Z2", "8YC-AN"], "Headquarter": "Q2FL-T"},
-    "QA-P7J": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "QA-P7J": {"Staging": "8G-2FP", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Q0-4FU": {"Staging": "VWES-Y", "Vanguards": ["NGM-OK", "O-QKSM", "QKQ3-L"], "Assaults": ["IU-E9T"], "Headquarter": "9-ZA4Z"},
     "Q5KW-Z": {"Staging": "WO-AIJ", "Vanguards": ["9F-7PZ", "C-LP3N"], "Assaults": ["1G-MJE", "MA-VDX", "RO90-H"], "Headquarter": "LXWN-W"},
     "QI1M-Q": {"Staging": "SD4A-2", "Vanguards": ["F2-NXA", "NSBE-L", "U6K-RG"], "Assaults": ["V-S9YY"], "Headquarter": "AH8-Q7"},
-    "QJ2-0M": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "QJ2-0M": {"Staging": "4-PCHD", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "QP6B-I": {"Staging": "6-IAFR", "Vanguards": ["3L3N-X", "DT-PXH", "UALX-3", "Y-ORBJ"], "Assaults": ["BW-WJ2", "S4-9DN"], "Headquarter": "WB-AYY"},
     "QS-FVH": {"Staging": "51-5XG", "Vanguards": ["4L-E5P", "RLL-9R", "UFXF-C"], "Assaults": ["57-YRU"], "Headquarter": "0T-AMZ"},
     "QZJ-FL": {"Staging": "FR-B1H", "Vanguards": ["DDI-B7", "FG-1GH", "WFYM-0"], "Assaults": ["GU-9F4"], "Headquarter": "D-L4H0"},
     "R-CL2W": {"Staging": "J-ZYSZ", "Vanguards": ["5C-RPA", "CR2-PQ", "N7-KGJ", "VD-8QY"], "Assaults": ["7EX-14", "GB-6X5"], "Headquarter": "0-6VZ5"},
-    "R-M719": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "R-M719": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "R2-BT6": {"Staging": "450I-W", "Vanguards": ["A1-AUH", "F-UVBV", "V-XANH", "VUAC-Y"], "Assaults": ["R-FM0G", "TEIZ-C"], "Headquarter": "OIOM-Y"},
     "Rapture": {"Staging": "CVY-UC", "Vanguards": ["EQX-AE", "QFEW-K", "Y-DW5K"], "Assaults": ["ES-UWY", "M-N7WD"], "Headquarter": "S1DP-Y"},
     "RDD-E6": {"Staging": "IRD-HU", "Vanguards": ["1GH-48", "B-2VXB", "JAWX-R"], "Assaults": ["FIZU-X"], "Headquarter": "IS-OBW"},
     "Regalia": {"Staging": "2JJ-0E", "Vanguards": ["AN-G54", "CT7-5V", "T-Z6J2"], "Assaults": ["ZXI-K2"], "Headquarter": "L3-XYO"},
     "RF9-ZU": {"Staging": "ZH-GKG", "Vanguards": ["C-62I5", "JQU-KY", "UY5A-D"], "Assaults": ["H-HHTH"], "Headquarter": "MWA-5Q"},
     "RFQ-8Y": {"Staging": "H-FGJO", "Vanguards": ["5J4K-9", "MD-0AW", "0-W778"], "Assaults": ["DG-8VJ"], "Headquarter": "1KAW-T"},
     "RFY-QB": {"Staging": "XCBK-X", "Vanguards": ["43B-O1", "4N-BUI", "9CK-KZ", "GY5-26", "N2IS-B", "VPLL-N", "WUZ-WM"], "Assaults": ["3T7-M8", "5S-KXA", "J1AU-9", "MZ1E-P"], "Headquarter": "X3-PBC"},
     "RHG-4O": {"Staging": "NLO-3Z", "Vanguards": ["GHZ-SJ", "K-J50B", "5P-AIP"], "Assaults": ["R4K-8L", "RIT-A7"], "Headquarter": "P8-BKO"},
-    "RJ-1R7": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "RJ-1R7": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "RL36-K": {"Staging": "7-8EOE", "Vanguards": ["66-PMM", "7L9-ZC", "OKEO-X"], "Assaults": ["UEP0-A", "Z-7OK1"], "Headquarter": "1I6F-9"},
     "RTCU-5": {"Staging": "FYI-49", "Vanguards": ["CJNF-J", "EA-HSA", "WYF8-8"], "Assaults": ["GXK-7F"], "Headquarter": "78TS-Q"},
     "S-B1E4": {"Staging": "E3UY-6", "Vanguards": ["5W3-DG", "7T6P-C", "8S28-3", "LT-DRO", "RO0-AF", "ZOYW-O"], "Assaults": ["3QE-9Q", "E-FIC0", "YZ-UKA"], "Headquarter": "85-B52"},
-    "S-Q02B": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "S-Q02B": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "S0X-O4": {"Staging": "OBV-YC", "Vanguards": ["2AUL-X", "F-A3TR", "F-HQWV"], "Assaults": ["9IZ-HU"], "Headquarter": "PA-ALN"},
-    "S4GH-I": {"Staging": "DT-TCD", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "S4GH-I": {"Staging": "DT-TCD", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "S4S-SD": {"Staging": "0S1-GI", "Vanguards": ["74-DRC", "M3-H2Y", "O31W-6"], "Assaults": ["B1UE-J", "L-GY1B"], "Headquarter": "LE-67X"},
     "Satyr": {"Staging": "CHA2-Q", "Vanguards": ["B32-14", "C-N4OD", "G95F-H"], "Assaults": ["C1XD-X"], "Headquarter": "00GD-D"},
-    "Scepter": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "Scepter": {"Staging": "G-YT55", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "SG-CTQ": {"Staging": "8RQJ-2", "Vanguards": ["39P-1J", "NIDJ-K", "PS-94K"], "Assaults": ["7G-QIG"], "Headquarter": "HZAQ-W"},
     "SI1-CF": {"Staging": "ETXT-F", "Vanguards": ["A-0IIQ", "E-BYOS", "H23-B5"], "Assaults": ["CBY8-J"], "Headquarter": "I-CMZA"},
     "Skaven": {"Staging": "F-88PJ", "Vanguards": ["1-5GBW", "ATQ-QS", "O-PNSN"], "Assaults": ["F2-2C3"], "Headquarter": "C-FER9"},
     "SKX-PL": {"Staging": "G-6SXJ", "Vanguards": ["4-JWWQ", "CIS-7X", "DCHR-L"], "Assaults": ["EU0I-T", "RSS-KA"], "Headquarter": "VSIG-K"},
     "SLYP-5": {"Staging": "D-IZT9", "Vanguards": ["89-JPE", "E8-432", "WU9-ZR"], "Assaults": ["FGJP-J"], "Headquarter": "4-QDIX"},
     "Sole": {"Staging": "A2V6-6", "Vanguards": ["BOE7-P", "E-GCX0"], "Assaults": ["0D-CHA", "E-GCX0", "VBFC-8", "VJ0-81"], "Headquarter": "A-5M31"},
-    "Sound": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "Sound": {"Staging": "YKE4-3", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Sphinx": {"Staging": "IGE-RI", "Vanguards": ["8ESL-G", "9O-ORX", "AL8-V4", "APM-6K", "JGOW-Y", "OW-TPO"], "Assaults": ["5-D82P", "KCT-0A", "RE-C26"], "Headquarter": "N2-OQG"},
     "SPNZ-Z": {"Staging": "PDE-U3", "Vanguards": ["4X0-8B", "FM-JK5", "JP4-AA"], "Assaults": ["23G-XC", "D-W7F0"], "Headquarter": "T5ZI-S"},
     "ST-0EZ": {"Staging": "D-8SI1", "Vanguards": ["1-Y6KI", "9-266Q", "YP-J33"], "Assaults": ["H-PA29"], "Headquarter": "P-FSQE"},
     "Sword": {"Staging": "7-692B", "Vanguards": ["DB-6W4", "GA-2V7", "R-OCBA"], "Assaults": ["3HQC-6"], "Headquarter": "OX-RGN"},
     "T-1WDH": {"Staging": "E3-SDZ", "Vanguards": ["7LHB-Z", "B-XJX4", "E1-4YH"], "Assaults": ["E1-4YH"], "Headquarter": "MUXX-4"},
-    "T-4ACL": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "T-4ACL": {"Staging": "DYS-CG", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "T-HHHT": {"Staging": "J6QB-P", "Vanguards": ["E-YJ8G", "KA6D-K", "TA3T-3"], "Assaults": ["G-AOTH"], "Headquarter": "ZQ-Z3Y"},
     "T-RQ7S": {"Staging": "QYZM-W", "Vanguards": ["BU-IU4", "CH9L-K", "I-7JR4"], "Assaults": ["3KNA-N", "ME-4IU"], "Headquarter": "9-B1DS"},
-    "T-W4L3": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "T-W4L3": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "T875-C": {"Staging": "Q0J-RH", "Vanguards": ["BOZ1-O", "E-ACV6", "QIMO-2", "Z-2Y2Y"], "Assaults": ["F9O-U9", "S-51XG"], "Headquarter": "E-1XVP"},
     "TA-A7V": {"Staging": "I-YGGI", "Vanguards": ["5-T0PZ", "A-ZLHX", "UTKS-5", "Y9G-KS"], "Assaults": ["2Q-I6Q", "97X-CH"], "Headquarter": "6R-PWU"},
     "Taurus": {"Staging": "3ZTV-V", "Vanguards": ["9D6O-M", "L-A5XP", "YRNJ-8"], "Assaults": ["D4KU-5"], "Headquarter": "P5-EFH"},
     "TCC-ZV": {"Staging": "H8-ZTO", "Vanguards": ["0-MX34", "0ZN7-G", "T-ZFID"], "Assaults": ["5AQ-5H"], "Headquarter": "4Y-OBL"},
     "Tinnimerci": {"Staging": "W-4NUU", "Vanguards": ["6-4V20", "O-0HW8", "YI-8ZM"], "Assaults": ["8R-RTB", "OU-X3P"], "Headquarter": "Q-UA3C"},
     "TJ10-O": {"Staging": "HB-FSO", "Vanguards": ["30-D5G", "J1-KJP", "R-YWID"], "Assaults": ["5-O8B1", "S-KSWL"], "Headquarter": "KW-1MV"},
     "TL-FDN": {"Staging": "1ZF-PJ", "Vanguards": ["FX4L-2", "HFC-AQ", "RZ-TI6"], "Assaults": ["27-HP0", "O-9G5Y"], "Headquarter": "X1-IZ0"},
     "TPB-KG": {"Staging": "RZ8A-P", "Vanguards": ["C3I-D5", "MTO2-2", "0-U2M4"], "Assaults": ["F18-AY"], "Headquarter": "01B-88"},
     "Tranquility": {"Staging": "K-MGJ7", "Vanguards": ["G-G78S", "OSY-UD", "UW9B-F"], "Assaults": ["ZZ-ZWC"], "Headquarter": "H-ADOC"},
     "TY0-Q2": {"Staging": "U-3FKL", "Vanguards": ["0XN-SK", "4F9Y-3", "MS-RXH"], "Assaults": ["5V-Q1R"], "Headquarter": "M4-KX5"},
     "U-3HAO": {"Staging": "UMDQ-6", "Vanguards": ["56D-TC", "6EG7-R", "8DL-CP"], "Assaults": ["2X7Z-L"], "Headquarter": "FVXK-D"},
     "U-7RBK": {"Staging": "OE-9UF", "Vanguards": ["5ZXX-K", "JE-D5U", "PFU-LH"], "Assaults": ["2-6TGQ"], "Headquarter": "8S-0E1"},
     "U-EUG7": {"Staging": "8EF-58", "Vanguards": ["4DS-OI", "TZN-2V", "WF4C-8"], "Assaults": ["7L3-JS", "C8H5-X"], "Headquarter": "O-7LAI"},
     "U-HSM3": {"Staging": "H7S-5I", "Vanguards": ["6FS-CZ", "B3ZU-H", "GSO-SR", "WNM-V0"], "Assaults": ["C3J0-O", "HPV-RJ"], "Headquarter": "G-KCFT"},
-    "U-IOR1": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "U-IOR1": {"Staging": "2ULC-J", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "U-JTBT": {"Staging": "CZK-ZQ", "Vanguards": ["4NBN-9", "Q-U96U", "W-MPTH", "X4-WL0"], "Assaults": ["EX6-AO", "WFC-MY"], "Headquarter": "QETZ-W"},
     "U29-0S": {"Staging": "U54-1L", "Vanguards": ["HE-V4V", "MC6O-F", "NCGR-Q"], "Assaults": ["G-LOIT", "LZ-6SU"], "Headquarter": "B-588R"},
     "U7-GIV": {"Staging": "RI-JB1", "Vanguards": ["0DD-MH", "99-0GS", "NQH-MR", "X-3AUU"], "Assaults": ["H90-C9", "K-1OY3", "MMUF-8"], "Headquarter": "NZPK-G"},
     "U8-CWA": {"Staging": "BDV3-T", "Vanguards": ["12YA-2", "5-9WNU", "EL8-4Q", "N-H32Y"], "Assaults": ["JC-YX8", "KI-TL0"], "Headquarter": "XI-VUF"},
     "UBPU-9": {"Staging": "B6-52M", "Vanguards": ["L-HV5C", "L4X-FH", "M-MD31", "NBPH-N", "V-MZW0"], "Assaults": ["D0-F4W", "QKTR-L", "YN3-E3"], "Headquarter": "WH-2EZ"},
     "UD-ZJ3": {"Staging": "BK4-YC", "Vanguards": ["2-TEGJ", "LF-2KP", "MVCJ-E"], "Assaults": ["K1I1-J"], "Headquarter": "AY-24I"},
     "UK-MI6": {"Staging": "C-J7CR", "Vanguards": ["KX-2UI", "MA-XAP", "MO-FIF"], "Assaults": ["97-M96"], "Headquarter": "H-NOU5"},
     "UL8-RD": {"Staging": "Z-DDVJ", "Vanguards": ["8-2JZA", "LH-PLU", "VVB-QH"], "Assaults": ["ZT-L3S"], "Headquarter": "AZA-QE"},
     "Unicorn": {"Staging": "DBRN-Z", "Vanguards": ["H-NPXW", "L-1SW8", "U-SOH2"], "Assaults": ["6F-H3W"], "Headquarter": "B17O-R"},
-    "UR-HG4": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "UR-HG4": {"Staging": "0UBC-R", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "UTQ-BO": {"Staging": "ZZZR-5", "Vanguards": ["JU-OWQ", "MXX5-9", "S-DN5M"], "Assaults": ["2O9G-D", "NC-N3F"], "Headquarter": "I30-3A"},
-    "UTZ-7B": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "UTZ-7B": {"Staging": "Y-4CFK", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "UWRZ-2": {"Staging": "L-C3O7", "Vanguards": ["K4YZ-Y", "O1Y-ED", "X36Y-G"], "Assaults": ["L-SCBU", "VRH-H7"], "Headquarter": "O-CNPR"},
     "UX3-N2": {"Staging": "HY-RWO", "Vanguards": ["36N-HZ", "9KOE-A", "B-3QPD", "U-QVWD", "V-3YG7"], "Assaults": ["HED-GP", "SV5-8N", "WD-VTV"], "Headquarter": "F9E-KX"},
     "V-4QJC": {"Staging": "B-VIP9", "Vanguards": ["0PI4-E", "6WT-BE", "9SNK-O"], "Assaults": ["SL-YBS", "UNJ-GX"], "Headquarter": "L1S-G1"},
     "V-LQBF": {"Staging": "UT-UZB", "Vanguards": ["AZF-GH", "BY5-V8", "M-EKDF", "VXO-OM"], "Assaults": ["7-IDWY", "TET3-B", "Y4-GQV"], "Headquarter": "CRXA-Y"},
     "V1G-63": {"Staging": "9P4O-F", "Vanguards": ["4D9-66", "L-TOFR", "Q-TBHW"], "Assaults": ["P-E9GN"], "Headquarter": "HJO-84"},
-    "V2S-RH": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "V2S-RH": {"Staging": "04-EHC", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Velvet": {"Staging": "O-RIDF", "Vanguards": ["LBV-Q1", "Z-40CG", "ZXC8-1"], "Assaults": ["BMU-V1"], "Headquarter": "W2F-ZH"},
     "VNX-P0": {"Staging": "I-UUI5", "Vanguards": ["8QMO-E", "GME-PQ", "MPPA-A"], "Assaults": ["X5-UME"], "Headquarter": "C4C-Z4"},
     "VS-8P0": {"Staging": "W2T-TR", "Vanguards": ["04EI-U", "IVP-KA", "YE1-9S"], "Assaults": ["BLMX-B", "M-CNUD"], "Headquarter": "Q-UEN6"},
     "VSC-W9": {"Staging": "NIF-JE", "Vanguards": ["JZ-B5Y", "P7-45V", "TPG-DD"], "Assaults": ["M-MCP8"], "Headquarter": "5F-MG1"},
     "VT-LHB": {"Staging": "9WVY-F", "Vanguards": ["7M4-4C", "JZ-UQC", "M5NO-B", "U-W436", "Z-ENUD"], "Assaults": ["972C-1", "JPEZ-R", "MJ-5F9"], "Headquarter": "BEG-RL"},
     "VW7-YN": {"Staging": "CCP-US", "Vanguards": ["2-KF56", "2R-CRW", "VFK-IV"], "Assaults": ["YA0-XJ"], "Headquarter": "II-5O9"},
     "W-3E44": {"Staging": "JV1V-O", "Vanguards": ["9-980U", "EMIG-F", "M-RPN3"], "Assaults": ["46DP-O"], "Headquarter": "ZO-P5K"},
     "W-3Y6D": {"Staging": "SB-23C", "Vanguards": ["52V6-B", "92-B0X", "O-OVOQ"], "Assaults": ["5FCV-A"], "Headquarter": "PUC-JZ"},
     "W-4U1E": {"Staging": "0-HDC8", "Vanguards": ["K-6K16", "PUIG-F", "SVM-3K", "W-KQPI"], "Assaults": ["D-3GIQ", "F-TE1T", "QY6-RK"], "Headquarter": "J-LPX7"},
-    "W-XBGF": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "W-XBGF": {"Staging": "F-G7BO", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "W9MQ-1": {"Staging": "S-1ZXZ", "Vanguards": ["9IPC-E", "EIV-1W", "QHJ-FW", "Z0-TJW"], "Assaults": ["N0C-UN", "V3X-L8", "VG-6CH"], "Headquarter": "4RX-EE"},
-    "WE-WLQ": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
-    "Wield": {"Staging": "NM-OEA", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "WE-WLQ": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
+    "Wield": {"Staging": "NM-OEA", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "WMP-OF": {"Staging": "M-76XI", "Vanguards": ["DK-FXK", "U-INPD", "ZJET-E"], "Assaults": ["A8I-C5", "C-H9X7"], "Headquarter": "ION-FG"},
     "WQZ8-4": {"Staging": "X2-ZA5", "Vanguards": ["IAK-JW", "RYC-19", "WO-GC0"], "Assaults": ["KZFV-4"], "Headquarter": "28Y9-P"},
     "WS5L-X": {"Staging": "H-EBQG", "Vanguards": ["9NI-FW", "N6NK-J", "TP-APY"], "Assaults": ["ZOPZ-6"], "Headquarter": "DOA-YU"},
     "WTE-CK": {"Staging": "7YSF-E", "Vanguards": ["2O-EEW", "J-QA7I", "OP9L-F"], "Assaults": ["Y-N4EF"], "Headquarter": "W4E-IT"},
     "WXB-RY": {"Staging": "8B-A4E", "Vanguards": ["3LL-O0", "4F6-VZ", "J9A-BH", "JM0A-4", "L-POLO"], "Assaults": ["A1F-22", "B-7LYC", "PT-2KR"], "Headquarter": "49V-E4"},
-    "Wyvern": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "Wyvern": {"Staging": "C-C99Z", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "X-FHU3": {"Staging": "33CE-7", "Vanguards": ["6-AOLS", "G06-8Y", "L-P3XM", "U-O2DA"], "Assaults": ["SZ6-TA", "WV-0R2"], "Headquarter": "U-O2DA"},
     "X-VN63": {"Staging": "0-YMBJ", "Vanguards": ["AW1-2I", "B-S42H", "F-749O", "UMI-KK"], "Assaults": ["F-RT6Q", "GKP-YT", "NL6V-7"], "Headquarter": "A-DDGY"},
-    "X5O9-E": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "X5O9-E": {"Staging": "I-HRX3", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "X7-FTR": {"Staging": "4-M1TY", "Vanguards": ["C6CG-W", "K-3PQW", "RY-2FX"], "Assaults": ["1A8-6G", "PE-SAM"], "Headquarter": "H-FOYG"},
     "XFLN-F": {"Staging": "DW-T2I", "Vanguards": ["CR-IFM", "DO6H-Q", "P-33KR"], "Assaults": ["E-9ORY", "HHK-VL"], "Headquarter": "C8-CHY"},
     "XHL-TZ": {"Staging": "DK0-N8", "Vanguards": ["4LNE-M", "HXK-J6", "L-Z9NB"], "Assaults": ["EJ-5X2"], "Headquarter": "U6R-F9"},
     "XHYS-O": {"Staging": "W3KK-R", "Vanguards": ["EK2-ET", "N-5476", "PZOZ-K"], "Assaults": ["SE-SHZ"], "Headquarter": "92D-OI"},
     "XI0-X2": {"Staging": "N-YLOE", "Vanguards": ["7-YHRX", "N-H95C", "X-PQEX"], "Assaults": ["Y6-9LF"], "Headquarter": "NSI-MW"},
     "XLL-Z7": {"Staging": "H74-B0", "Vanguards": ["3D5K-R", "F-NXLQ", "NU4-2G"], "Assaults": ["ES-Q0W"], "Headquarter": "ZXJ-71"},
     "XMNF-7": {"Staging": "4S-PVC", "Vanguards": ["E1F-E5", "H-AJ27", "M2-2V1"], "Assaults": ["2TH-3F"], "Headquarter": "WLF-D3"},
@@ -584,40 +601,42 @@
     "XPBM-F": {"Staging": "O94U-A", "Vanguards": ["C-VGYO", "K-8SQS", "XW-JHT"], "Assaults": ["C-4ZOS"], "Headquarter": "NEH-CS"},
     "XPG-HE": {"Staging": "K76A-3", "Vanguards": ["HVGR-R", "M-75WN", "PNFW-O"], "Assaults": ["K95-9I"], "Headquarter": "9-0QB7"},
     "XPJ1-6": {"Staging": "PR-8CA", "Vanguards": ["1DH-SX", "A-ELE2", "Z3V-1W"], "Assaults": ["KFIE-Z"], "Headquarter": "UHKL-N"},
     "XR9-LP": {"Staging": "I-8D0G", "Vanguards": ["6X7-JO", "A-803L", "GJ0-OJ", "R-K4QY", "WQH-4K"], "Assaults": ["JWZ2-V", "OGL8-Q", "Q-S7ZD"], "Headquarter": "J-ODE7"},
     "XV7L-S": {"Staging": "E-YCML", "Vanguards": ["B-WPLZ", "TU-O0T", "Y9-MDG"], "Assaults": ["KBP7-G"], "Headquarter": "XHQ-7V"},
     "Y-JSM8": {"Staging": "W4C8-Q", "Vanguards": ["E5T-CS", "I-2705", "M53-1V"], "Assaults": ["C-6YHJ", "K-RMI5"], "Headquarter": "4S0-NP"},
     "Y-LRWI": {"Staging": "LOI-L1", "Vanguards": ["G-B3PR", "KR8-27", "VULA-I", "XPUM-L"], "Assaults": ["LQ-AHE", "R2TJ-1"], "Headquarter": "73-JQO"},
-    "Y-M7ML": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
-    "Y46-EN": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "Y-M7ML": {"Staging": "WHI-61", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
+    "Y46-EN": {"Staging": "7-ZT1Y", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "Y4Y7-Q": {"Staging": "5-DSFH", "Vanguards": ["AK-QBU", "X-PYH5", "ZN0-SR"], "Assaults": ["PC9-AY"], "Headquarter": "T22-QI"},
-    "Y8-HHZ": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
-    "Y8HB-U": {"Staging": "HD-JVQ", "Vanguards": [], "Assaults": [], "Headquarter": ""},
-    "YB7B-8": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "Y8-HHZ": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
+    "Y8HB-U": {"Staging": "HD-JVQ", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
+    "YB7B-8": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "YCM-AI": {"Staging": "6-KPAB", "Vanguards": ["9BC-EB", "9M-M0P", "PU-UMM", "QPTT-F"], "Assaults": ["HJ-BCH", "WFFE-4", "Y5-E1U"], "Headquarter": "71-UTX"},
     "YDS0-Y": {"Staging": "C-DHON", "Vanguards": ["F-D49D", "H-1EOH", "IR-DYY"], "Assaults": ["XSQ-TF"], "Headquarter": "Q-EHMJ"},
     "YENX-U": {"Staging": "8X6T-8", "Vanguards": ["08-N7Q", "CKX-RW", "Y-C4AL"], "Assaults": ["6-I162", "U9U-TQ"], "Headquarter": "B2-UQW"},
     "YFN-UN": {"Staging": "XYY-IA", "Vanguards": ["3MOG-V", "NG-C6Y", "TXW-EI"], "Assaults": ["5-FGQI", "8V-SJJ"], "Headquarter": "3KNK-A"},
     "Yrton": {"Staging": "DY-F70", "Vanguards": ["5-MLDT", "B-DBYQ", "QXW-PV"], "Assaults": ["XT-R36"], "Headquarter": "1-3HWZ"},
-    "YS-GOP": {"Staging": "MI6O-6", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "YS-GOP": {"Staging": "MI6O-6", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "YUT3-U": {"Staging": "A8A-JN", "Vanguards": ["47L-J4", "6WW-28", "S-NJBB"], "Assaults": ["E-D0VZ", "IFJ-EL"], "Headquarter": "Q-L07F"},
     "YX-LYK": {"Staging": "MJXW-P", "Vanguards": ["1-SMEB", "6Q-R50", "RCI-VL"], "Assaults": ["M5-CGW", "Q-HESZ"], "Headquarter": "ZA9-PY"},
     "YZKE-Q": {"Staging": "DB1R-4", "Vanguards": ["23M-PX", "UTDH-N", "ZS-2LT"], "Assaults": ["GPUS-A"], "Headquarter": "3-BADZ"},
     "Z-6NQ6": {"Staging": "K5-JRD", "Vanguards": ["F67E-Q", "FD-MLJ", "PF-346", "Poitot", "X-BV98", "X-M2LR"], "Assaults": ["2X-PQG", "6E-578", "ATY-2U", "MHC-R3"], "Headquarter": "ZVN5-H"},
     "Z6T6-B": {"Staging": "L-WG68", "Vanguards": ["5LAJ-8", "GZM-KB", "HIK-MC"], "Assaults": ["E-BFLT", "E4-E8W"], "Headquarter": "B9EA-G"},
     "Z-D6K5": {"Staging": "K5F-Z2", "Vanguards": ["0P-F3K", "FMB-JP", "TXME-A"], "Assaults": ["CU9-T0", "XCF-8N"], "Headquarter": "94-H3F"},
     "Z-DO53": {"Staging": "V-OJEN", "Vanguards": ["49-0LI", "DAYP-G", "EIDI-N", "IPAY-2", "KRUN-N"], "Assaults": ["9OO-LH", "K8X-6B", "P3EN-E"], "Headquarter": "X445-5"},
-    "Z-ONUI": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "Z-ONUI": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "ZPI-2E": {"Staging": "FMH-OV", "Vanguards": ["77S8-E", "HZFJ-M", "SLVP-D"], "Assaults": ["QRFJ-Q"], "Headquarter": "0-G8NO"},
-    "ZQ2-CF": {"Staging": "5KG-PY", "Vanguards": [], "Assaults": [], "Headquarter": ""},
+    "ZQ2-CF": {"Staging": "5KG-PY", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
     "ZQ7-QS": {"Staging": "YF-P4X", "Vanguards": ["EQWO-Y", "JK-Q77", "QI9-42", "U2U5-A"], "Assaults": ["IL-YTR", "KW-OAM"], "Headquarter": "ABE-M2"},
     "ZW-BY5": {"Staging": "EX-0LQ", "Vanguards": ["GE-94X", "KW-I6T", "W9-DID"], "Assaults": ["S-U2VD"], "Headquarter": "GMLH-K"},
-    "ZYL-FT": {"Staging": "", "Vanguards": [], "Assaults": [], "Headquarter": ""},
-    "ZYR-NF": {"Staging": "F-3H2P", "Vanguards": ["68FT-6", "9-IIBL", "9I-SRF", "HOHF-B", "IRE-98", "Y-6B0E"], "Assaults": ["5GQ-S9", "H-64KI", "YALR-F"], "Headquarter": "IV-UNR"}}
+    "ZYL-FT": {"Staging": "", "Vanguards": [""], "Assaults": [""], "Headquarter": ""},
+    "ZYR-NF": {"Staging": "F-3H2P", "Vanguards": ["68FT-6", "9-IIBL", "9I-SRF", "HOHF-B", "IRE-98", "Y-6B0E"], "Assaults": ["5GQ-S9", "H-64KI", "YALR-F"], "Headquarter": "IV-UNR"},
+    "Krai Veles": {"Staging": "Archee", "Vanguards": ["Ala", "Angymonne", "Ichoriya", "Vale"], "Assaults": ["Kaunokka", "Senda", "Wirashoda"], "Headquarter": "Arvasaras"},
+}
 
 
 incursion_payouts_isk = {
     "Scout": {
         "H": {
             5: 3500,
         },
```

### Comparing `aa_incursions-0.3.0a0/incursions/swagger.json` & `aa_incursions-0.4.2a0/incursions/swagger.json`

 * *Files identical despite different names*

### Comparing `aa_incursions-0.3.0a0/incursions/tasks.py` & `aa_incursions-0.4.2a0/incursions/tasks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import datetime
 
 from celery import shared_task
 from eveuniverse.models import EveConstellation, EveSolarSystem
 
+from django.db import IntegrityError
+
 from allianceauth.eveonline.models import EveFactionInfo
 
 from incursions.helpers import (
     embed_boss_spawned, embed_ended, embed_established,
     embed_established_addendum, embed_mobilizing, embed_withdrawing,
 )
 from incursions.models import Incursion, IncursionInfluence, IncursionsConfig
@@ -19,61 +21,63 @@
     actives = []
     for incursion in incursions:
         actives.append(incursion['constellation_id'])
         try:
             # Get, because i need to do more steps than an update_or_create would let me
             # Also incursions have no unique id.... wtf ccp
             i = Incursion.objects.get(
-                constellation=EveConstellation.objects.get_or_create_esi(
-                    id=incursion['constellation_id'])[0],
+                constellation=EveConstellation.objects.get_or_create_esi(id=incursion['constellation_id'])[0],
                 ended_timestamp__isnull=True)
             if incursion['state'] == "established":
                 # This is still just an established incursion, nothing to act on
                 pass
             elif incursion['state'] == "mobilizing" and i.state != Incursion.States.MOBILIZING:
                 i.mobilizing_timestamp = datetime.datetime.strptime(
-                    str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z')
+                    str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc)
                 i.state = Incursion.States.MOBILIZING
                 i.save(update_fields=["mobilizing_timestamp", "state"])
             elif incursion['state'] == "withdrawing " and i.state != Incursion.States.WITHDRAWING:
                 i.withdrawing_timestamp = datetime.datetime.strptime(
-                    str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z')
+                    str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc)
                 i.state = Incursion.States.WITHDRAWING
                 i.save(update_fields=["withdrawing_timestamp", "state"])
             else:
                 # ????
                 pass
             IncursionInfluence.objects.create(
                 incursion=i,
                 influence=incursion['influence'],
                 timestamp=datetime.datetime.strptime(
-                    str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z')
+                    str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc)
             )
         except Incursion.DoesNotExist:
             # Create an Incursion
             i = Incursion.objects.create(
                 constellation=EveConstellation.objects.get_or_create_esi(
                     id=incursion['constellation_id'])[0],
                 faction=EveFactionInfo.objects.get_or_create(
                     faction_id=incursion['faction_id'])[0],
                 has_boss=incursion['has_boss'],
                 staging_solar_system=EveSolarSystem.objects.get_or_create_esi(
                     id=incursion['staging_solar_system_id'])[0],
                 state=incursion['state'],
                 type=incursion['type'],
                 established_timestamp=datetime.datetime.strptime(
-                    str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z')
+                    str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc)
             )
-            IncursionInfluence.objects.create(
-                incursion=i,
-                influence=incursion['influence'],
-                timestamp=datetime.datetime.strptime(
-                    str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z')
+            try:
+                IncursionInfluence.objects.create(
+                    incursion=i,
+                    influence=incursion['influence'],
+                    timestamp=datetime.datetime.strptime(
+                        str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z').replace(tzinfo=datetime.timezone.utc))
+            except IntegrityError:
+                # If we call this task too often cache will return the same influence
+                pass
 
-            )
     for ended in Incursion.objects.filter(ended_timestamp__isnull=True).exclude(constellation_id__in=actives):
         # Cant use update here, need to fire signals
         ended.ended_timestamp = datetime.datetime.strptime(
             str(response.headers['Last-Modified']), '%a, %d %b %Y %H:%M:%S %Z')
         ended.state = Incursion.States.ENDED
         ended.save(update_fields=["ended_timestamp", "state"])
 
@@ -108,13 +112,7 @@
 
 
 @shared_task
 def incursion_boss_spawned(incursion_pk: int):
     incursion = Incursion.objects.get(pk=incursion_pk)
     for webhook in IncursionsConfig.get_solo().status_webhooks.all():
         webhook.send_embed(embed=embed_boss_spawned(incursion))
-
-
-@shared_task
-def recreate_history():
-    # Step through eve-ref data and recreate incursion history.
-    pass
```

### Comparing `aa_incursions-0.3.0a0/pyproject.toml` & `aa_incursions-0.4.2a0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,70 +1,108 @@
 [build-system]
-requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
+requires = [
+    "flit-core>=3.2,<4",
+]
+
 [project]
-name = "aa_incursions"
-dynamic = ["version", "description" ]
+name = "aa-incursions"
 readme = "README.md"
-license = {file = "LICENSE"}
-requires-python = ">=3.8"
-authors = [
-    { name = "Joel Falknau", email = "joel.falknau@gmail.com" },
-]
 keywords = [
     "allianceauth",
     "eveonline",
 ]
+license = { file = "LICENSE" }
+authors = [
+    { name = "Joel Falknau", email = "joel.falknau@gmail.com" },
+]
+requires-python = ">=3.8"
 classifiers = [
     "Environment :: Web Environment",
     "Framework :: Celery",
     "Framework :: Django",
     "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.2",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP",
-    "Topic :: Internet :: WWW/HTTP :: Dynamic Content"
+    "Topic :: Internet :: WWW/HTTP :: Dynamic Content",
+]
+dynamic = [
+    "description",
+    "version",
 ]
 dependencies = [
-    "allianceauth>=3.0.0,<5.0.0",
+    "aa-routing",
+    "allianceauth>=3,<5",
     "django-eveuniverse",
-    "django-solo>=2.0.0,<3.0.0",
-    "py-cord>=2.0.0,<3.0.0"
+    "django-solo>=2,<3",
+    "py-cord>=2,<3",
 ]
 
-[project.urls]
-Homepage = "https://gitlab.com/tactical-supremacy/aa-incursions"
-Source = "https://gitlab.com/tactical-supremacy/aa-incursions"
-Tracker = "https://gitlab.com/tactical-supremacy/aa-incursions/-/issues"
+urls.Homepage = "https://gitlab.com/tactical-supremacy/aa-incursions"
+urls.Source = "https://gitlab.com/tactical-supremacy/aa-incursions"
+urls.Tracker = "https://gitlab.com/tactical-supremacy/aa-incursions/-/issues"
 
 [tool.flit.module]
 name = "incursions"
 
 [tool.isort]
 profile = "django"
 sections = [
     "FUTURE",
     "STDLIB",
     "THIRDPARTY",
     "DJANGO",
     "ALLIANCEAUTH",
     "FIRSTPARTY",
-    "LOCALFOLDER"
+    "LOCALFOLDER",
+]
+known_allianceauth = [
+    "allianceauth",
+    "esi",
+]
+known_django = [
+    "django",
 ]
-known_allianceauth = ["allianceauth", "esi"]
-known_django = ["django"]
 skip_gitignore = true
 
 [tool.flake8]
-exclude = [".git", "*migrations*", ".tox", "dist", "htmlcov"]
+exclude = [
+    ".git",
+    "*migrations*",
+    ".tox",
+    "dist",
+    "htmlcov",
+]
 max-line-length = 119
-select = ["C", "E", "F", "W", "B", "B950"]
-ignore = ['E203', 'E231', 'E501', 'W503', 'W291', 'W293']
+select = [
+    "C",
+    "E",
+    "F",
+    "W",
+    "B",
+    "B950",
+]
+ignore = [
+    'E203',
+    'E231',
+    'E501',
+    'W503',
+    'W291',
+    'W293',
+]
+
+[tool.djlint]
+max_attribute_length = 119
+max_line_length = 119
+max_blank_lines = 1
```

### Comparing `aa_incursions-0.3.0a0/PKG-INFO` & `aa_incursions-0.4.2a0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
-Name: aa_incursions
-Version: 0.3.0a0
+Name: aa-incursions
+Version: 0.4.2a0
 Summary: AllianceAuth Incursion Tools
 Keywords: allianceauth,eveonline
 Author-email: Joel Falknau <joel.falknau@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Celery
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
-Requires-Dist: allianceauth>=3.0.0,<5.0.0
+Requires-Dist: aa-routing
+Requires-Dist: allianceauth>=3,<5
 Requires-Dist: django-eveuniverse
-Requires-Dist: django-solo>=2.0.0,<3.0.0
-Requires-Dist: py-cord>=2.0.0,<3.0.0
+Requires-Dist: django-solo>=2,<3
+Requires-Dist: py-cord>=2,<3
 Project-URL: Homepage, https://gitlab.com/tactical-supremacy/aa-incursions
 Project-URL: Source, https://gitlab.com/tactical-supremacy/aa-incursions
 Project-URL: Tracker, https://gitlab.com/tactical-supremacy/aa-incursions/-/issues
 
 # Incursions for Alliance Auth
 
 Incursion Tools for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth/).
@@ -61,15 +64,15 @@
 
 Incursions is an App for [Alliance Auth](https://gitlab.com/allianceauth/allianceauth/), Please make sure you have this installed. incursions is not a standalone Django Application
 
 Incursions needs the App [django-eveuniverse](https://gitlab.com/ErikKalkoken/django-eveuniverse) to function. Please make sure it is installed before continuing.
 
 ### Step 2 - Install app
 
-```bash
+```shell
 pip install aa-incursions
 ```
 
 ### Step 3 - Configure Auth settings
 
 Configure your Auth settings (`local.py`) as follows:
```

