# Comparing `tmp/weni_rp_apps-2.8.3a0.tar.gz` & `tmp/weni-rp-apps-2.8.4a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "weni_rp_apps-2.8.3a0.tar", max compression
+gzip compressed data, was "weni-rp-apps-2.8.4a0.tar", max compression
```

## Comparing `weni_rp_apps-2.8.3a0.tar` & `weni-rp-apps-2.8.4a0.tar`

### file list

```diff
@@ -1,180 +1,180 @@
--rw-r--r--   0        0        0      646 2024-04-12 21:43:35.647312 weni_rp_apps-2.8.3a0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.505211 weni_rp_apps-2.8.3a0/weni/activities/__init__.py
--rw-r--r--   0        0        0      315 2024-04-12 21:42:55.465247 weni_rp_apps-2.8.3a0/weni/activities/apps.py
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.505211 weni_rp_apps-2.8.3a0/weni/activities/migrations/__init__.py
--rw-r--r--   0        0        0     1480 2024-04-12 21:42:55.465247 weni_rp_apps-2.8.3a0/weni/activities/recent_activities.py
--rw-r--r--   0        0        0     1601 2024-04-12 21:42:55.465247 weni_rp_apps-2.8.3a0/weni/activities/signals.py
--rw-r--r--   0        0        0      325 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/analytics_api/README.md
--rw-r--r--   0        0        0       66 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/analytics_api/__init__.py
--rw-r--r--   0        0        0      264 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/analytics_api/apps.py
--rw-r--r--   0        0        0    13526 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.3a0/weni/analytics_api/tests.py
--rw-r--r--   0        0        0      371 2024-03-12 23:31:07.018460 weni_rp_apps-2.8.3a0/weni/analytics_api/urls.py
--rw-r--r--   0        0        0     9067 2024-03-12 23:31:07.018460 weni_rp_apps-2.8.3a0/weni/analytics_api/views.py
--rw-r--r--   0        0        0       49 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/auth/__init__.py
--rw-r--r--   0        0        0      285 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/auth/apps.py
--rw-r--r--   0        0        0     1327 2024-03-13 14:14:33.907599 weni_rp_apps-2.8.3a0/weni/auth/backends.py
--rw-r--r--   0        0        0      430 2024-02-02 22:05:28.147811 weni_rp_apps-2.8.3a0/weni/auth/decorators.py
--rw-r--r--   0        0        0      810 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/auth/urls.py
--rw-r--r--   0        0        0     2645 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.3a0/weni/auth/views.py
--rw-r--r--   0        0        0      309 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/channel_stats/README.md
--rw-r--r--   0        0        0       66 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/channel_stats/__init__.py
--rw-r--r--   0        0        0      264 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/channel_stats/apps.py
--rw-r--r--   0        0        0     6157 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.3a0/weni/channel_stats/serializers.py
--rw-r--r--   0        0        0      347 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/channel_stats/urls.py
--rw-r--r--   0        0        0     3575 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/channel_stats/views.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/billing/__init__.py
--rw-r--r--   0        0        0      102 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/billing/apps.py
--rw-r--r--   0        0        0     3508 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.3a0/weni/grpc/billing/queries.py
--rw-r--r--   0        0        0     3194 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.3a0/weni/grpc/billing/serializers.py
--rw-r--r--   0        0        0     2063 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/billing/services.py
--rw-r--r--   0        0        0    11364 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/billing/tests.py
--rw-r--r--   0        0        0      231 2023-09-08 15:21:13.737273 weni_rp_apps-2.8.3a0/weni/grpc/billing/urls.py
--rw-r--r--   0        0        0       64 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/channel/__init__.py
--rw-r--r--   0        0        0      103 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/channel/apps.py
--rw-r--r--   0        0        0      352 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/channel/fields.py
--rw-r--r--   0        0        0     4070 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/channel/serializers.py
--rw-r--r--   0        0        0     4081 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/channel/services.py
--rw-r--r--   0        0        0     7987 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/channel/tests.py
--rw-r--r--   0        0        0      341 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.3a0/weni/grpc/channel/urls.py
--rw-r--r--   0        0        0       70 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/classifier/__init__.py
--rw-r--r--   0        0        0      109 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/classifier/apps.py
--rw-r--r--   0        0        0     1356 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/classifier/serializers.py
--rw-r--r--   0        0        0     1174 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/classifier/services.py
--rw-r--r--   0        0        0     6493 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/classifier/tests.py
--rw-r--r--   0        0        0      249 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.3a0/weni/grpc/classifier/urls.py
--rw-r--r--   0        0        0       61 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/core/__init__.py
--rw-r--r--   0        0        0      100 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/core/apps.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/core/management/__init__.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/core/management/commands/__init__.py
--rw-r--r--   0        0        0     1588 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/core/management/commands/grpc.py
--rw-r--r--   0        0        0     1213 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/core/serializers.py
--rw-r--r--   0        0        0      965 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/core/services.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/core/tests.py
--rw-r--r--   0        0        0      700 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/core/urls.py
--rw-r--r--   0        0        0       58 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/flow/__init__.py
--rw-r--r--   0        0        0       97 2023-03-03 20:32:14.180792 weni_rp_apps-2.8.3a0/weni/grpc/flow/apps.py
--rw-r--r--   0        0        0      307 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/grpc/flow/serializers.py
--rw-r--r--   0        0        0      680 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/flow/services.py
--rw-r--r--   0        0        0     2764 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/flow/tests.py
--rw-r--r--   0        0        0      213 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.3a0/weni/grpc/flow/urls.py
--rw-r--r--   0        0        0       56 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/grpc/org/__init__.py
--rw-r--r--   0        0        0       95 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/grpc/org/apps.py
--rw-r--r--   0        0        0     2836 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/org/serializers.py
--rw-r--r--   0        0        0     4020 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/org/services.py
--rw-r--r--   0        0        0     9821 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/org/tests.py
--rw-r--r--   0        0        0      207 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/grpc/org/urls.py
--rw-r--r--   0        0        0       68 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/grpc/statistic/__init__.py
--rw-r--r--   0        0        0      107 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/grpc/statistic/apps.py
--rw-r--r--   0        0        0      672 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.3a0/weni/grpc/statistic/services.py
--rw-r--r--   0        0        0     3132 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/statistic/tests.py
--rw-r--r--   0        0        0      252 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.3a0/weni/grpc/statistic/urls.py
--rw-r--r--   0        0        0       58 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/grpc/user/__init__.py
--rw-r--r--   0        0        0       97 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/grpc/user/apps.py
--rw-r--r--   0        0        0      843 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.3a0/weni/grpc/user/serializers.py
--rw-r--r--   0        0        0     3916 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/user/services.py
--rw-r--r--   0        0        0    10076 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/grpc/user/tests.py
--rw-r--r--   0        0        0      347 2023-09-08 15:21:13.747273 weni_rp_apps-2.8.3a0/weni/grpc/user/urls.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/internal/__init__.py
--rw-r--r--   0        0        0      328 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/internal/apps.py
--rw-r--r--   0        0        0      300 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/internal/authenticators.py
--rw-r--r--   0        0        0     1374 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/internal/backends.py
--rw-r--r--   0        0        0     5484 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/internal/channel/serializers.py
--rw-r--r--   0        0        0    16305 2023-09-25 22:05:33.515211 weni_rp_apps-2.8.3a0/weni/internal/channel/tests.py
--rw-r--r--   0        0        0      394 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/channel/urls.py
--rw-r--r--   0        0        0     8711 2023-11-09 13:18:30.163158 weni_rp_apps-2.8.3a0/weni/internal/channel/views.py
--rw-r--r--   0        0        0     1527 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/classifier/serializers.py
--rw-r--r--   0        0        0     8626 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/classifier/tests.py
--rw-r--r--   0        0        0      318 2023-09-25 18:26:36.872113 weni_rp_apps-2.8.3a0/weni/internal/classifier/urls.py
--rw-r--r--   0        0        0     2803 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/classifier/views.py
--rw-r--r--   0        0        0      113 2024-03-08 15:16:47.101420 weni_rp_apps-2.8.3a0/weni/internal/clients/__init__.py
--rw-r--r--   0        0        0      692 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/clients/authenticators.py
--rw-r--r--   0        0        0      486 2024-01-16 13:08:31.627802 weni_rp_apps-2.8.3a0/weni/internal/clients/base.py
--rw-r--r--   0        0        0     1108 2024-03-08 15:16:51.401431 weni_rp_apps-2.8.3a0/weni/internal/clients/connect.py
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/externals/__init__.py
--rw-r--r--   0        0        0     2476 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/externals/serializers.py
--rw-r--r--   0        0        0      546 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/externals/urls.py
--rw-r--r--   0        0        0     4243 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/externals/views.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/internal/flows/__init__.py
--rw-r--r--   0        0        0     1460 2024-04-12 21:42:35.404863 weni_rp_apps-2.8.3a0/weni/internal/flows/serializers.py
--rw-r--r--   0        0        0     4436 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/flows/tests.py
--rw-r--r--   0        0        0      308 2023-08-25 21:34:08.985544 weni_rp_apps-2.8.3a0/weni/internal/flows/urls.py
--rw-r--r--   0        0        0     1838 2024-04-12 21:42:35.404863 weni_rp_apps-2.8.3a0/weni/internal/flows/views.py
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/globals/__init__.py
--rw-r--r--   0        0        0     2286 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/globals/serializers.py
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/globals/tests/__init__.py
--rw-r--r--   0        0        0     2183 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/globals/tests/test_serializers.py
--rw-r--r--   0        0        0      220 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/globals/urls.py
--rw-r--r--   0        0        0     1484 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/globals/views.py
--rw-r--r--   0        0        0     1247 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/migrations/0001_initial.py
--rw-r--r--   0        0        0     1032 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/migrations/0002_project.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/internal/migrations/__init__.py
--rw-r--r--   0        0        0     1100 2024-04-12 21:42:55.465247 weni_rp_apps-2.8.3a0/weni/internal/models.py
--rw-r--r--   0        0        0     4281 2023-11-22 18:45:11.406539 weni_rp_apps-2.8.3a0/weni/internal/msgs/## Índice.md
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/msgs/__init__.py
--rw-r--r--   0        0        0     4814 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/msgs/tasks.py
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/msgs/tests/tests.py
--rw-r--r--   0        0        0      259 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/msgs/urls.py
--rw-r--r--   0        0        0     2995 2023-09-25 22:05:33.525211 weni_rp_apps-2.8.3a0/weni/internal/msgs/views.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/internal/orgs/__init__.py
--rw-r--r--   0        0        0     4275 2024-02-02 22:05:40.147858 weni_rp_apps-2.8.3a0/weni/internal/orgs/serializers.py
--rw-r--r--   0        0        0    16862 2024-02-02 22:05:40.147858 weni_rp_apps-2.8.3a0/weni/internal/orgs/tests.py
--rw-r--r--   0        0        0      300 2023-08-25 21:34:08.985544 weni_rp_apps-2.8.3a0/weni/internal/orgs/urls.py
--rw-r--r--   0        0        0     5863 2024-02-02 22:05:40.147858 weni_rp_apps-2.8.3a0/weni/internal/orgs/views.py
--rw-r--r--   0        0        0      246 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.3a0/weni/internal/permissions.py
--rw-r--r--   0        0        0     2164 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/internal/statistic/tests.py
--rw-r--r--   0        0        0      205 2023-08-25 21:34:08.985544 weni_rp_apps-2.8.3a0/weni/internal/statistic/urls.py
--rw-r--r--   0        0        0     1007 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/internal/statistic/views.py
--rw-r--r--   0        0        0       67 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/internal/tasks.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/internal/tests/__init__.py
--rw-r--r--   0        0        0     1249 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.3a0/weni/internal/tests/test_models.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/internal/tickets/__init__.py
--rw-r--r--   0        0        0     1150 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/internal/tickets/serializers.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.190792 weni_rp_apps-2.8.3a0/weni/internal/tickets/tests/__init__.py
--rw-r--r--   0        0        0     3360 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/internal/tickets/tests/test_views.py
--rw-r--r--   0        0        0      521 2024-03-27 21:28:24.596619 weni_rp_apps-2.8.3a0/weni/internal/tickets/urls.py
--rw-r--r--   0        0        0     2385 2024-03-27 21:28:24.596619 weni_rp_apps-2.8.3a0/weni/internal/tickets/views.py
--rw-r--r--   0        0        0     1417 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/internal/urls.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/internal/users/__init__.py
--rw-r--r--   0        0        0      845 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/internal/users/serializers.py
--rw-r--r--   0        0        0    12563 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/internal/users/tests.py
--rw-r--r--   0        0        0      711 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.3a0/weni/internal/users/urls.py
--rw-r--r--   0        0        0     5849 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/internal/users/views.py
--rw-r--r--   0        0        0      555 2023-08-25 21:34:08.985544 weni_rp_apps-2.8.3a0/weni/internal/views.py
--rw-r--r--   0        0        0       55 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/orgs_api/__init__.py
--rw-r--r--   0        0        0      253 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/orgs_api/apps.py
--rw-r--r--   0        0        0      906 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.3a0/weni/orgs_api/serializers.py
--rw-r--r--   0        0        0     4030 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.3a0/weni/orgs_api/tests.py
--rw-r--r--   0        0        0      178 2023-04-13 12:17:16.348555 weni_rp_apps-2.8.3a0/weni/orgs_api/urls.py
--rw-r--r--   0        0        0     1444 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/orgs_api/views.py
--rw-r--r--   0        0        0       45 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/s3/__init__.py
--rw-r--r--   0        0        0      243 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/s3/apps.py
--rw-r--r--   0        0        0      219 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/s3/urls.py
--rw-r--r--   0        0        0      550 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/s3/views.py
--rw-r--r--   0        0        0       93 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/serializers/__init__.py
--rw-r--r--   0        0        0      725 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/serializers/fields.py
--rw-r--r--   0        0        0      281 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/success_orgs/apps.py
--rw-r--r--   0        0        0     2791 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/success_orgs/business.py
--rw-r--r--   0        0        0      619 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/success_orgs/serializers.py
--rw-r--r--   0        0        0        0 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/success_orgs/tests/__init__.py
--rw-r--r--   0        0        0     3354 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/success_orgs/tests/test_business.py
--rw-r--r--   0        0        0      494 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/success_orgs/urls.py
--rw-r--r--   0        0        0     2770 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/success_orgs/views.py
--rw-r--r--   0        0        0      318 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/template_message/README.md
--rw-r--r--   0        0        0       72 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/template_message/__init__.py
--rw-r--r--   0        0        0      294 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/template_message/apps.py
--rw-r--r--   0        0        0     2040 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/template_message/serializers.py
--rw-r--r--   0        0        0     5292 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/template_message/tests.py
--rw-r--r--   0        0        0      344 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.3a0/weni/template_message/urls.py
--rw-r--r--   0        0        0     1651 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/template_message/views.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/templates/__init__.py
--rw-r--r--   0        0        0      545 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/templates/context_processors.py
--rw-r--r--   0        0        0      315 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/ticketer_queues/README.md
--rw-r--r--   0        0        0       70 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/ticketer_queues/__init__.py
--rw-r--r--   0        0        0      291 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/ticketer_queues/apps.py
--rw-r--r--   0        0        0      242 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/ticketer_queues/serializers.py
--rw-r--r--   0        0        0     1584 2023-09-08 15:21:13.757273 weni_rp_apps-2.8.3a0/weni/ticketer_queues/tests.py
--rw-r--r--   0        0        0      378 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/ticketer_queues/urls.py
--rw-r--r--   0        0        0      849 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/ticketer_queues/views.py
--rw-r--r--   0        0        0        0 2023-03-03 20:32:14.200792 weni_rp_apps-2.8.3a0/weni/utils/__init__.py
--rw-r--r--   0        0        0     1091 2023-09-25 22:05:33.535211 weni_rp_apps-2.8.3a0/weni/utils/app_config.py
--rw-r--r--   0        0        0     1003 1970-01-01 00:00:00.000000 weni_rp_apps-2.8.3a0/PKG-INFO
+-rw-r--r--   0        0        0      646 2024-05-21 19:16:16.500521 weni-rp-apps-2.8.4a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/activities/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-21 17:24:07.870487 weni-rp-apps-2.8.4a0/weni/activities/apps.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/activities/migrations/__init__.py
+-rw-r--r--   0        0        0     1480 2024-05-21 17:24:07.870487 weni-rp-apps-2.8.4a0/weni/activities/recent_activities.py
+-rw-r--r--   0        0        0     1601 2024-05-21 17:24:07.870487 weni-rp-apps-2.8.4a0/weni/activities/signals.py
+-rw-r--r--   0        0        0      325 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/analytics_api/README.md
+-rw-r--r--   0        0        0       66 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/analytics_api/__init__.py
+-rw-r--r--   0        0        0      264 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/analytics_api/apps.py
+-rw-r--r--   0        0        0    13526 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/analytics_api/tests.py
+-rw-r--r--   0        0        0      371 2024-05-21 17:24:07.870487 weni-rp-apps-2.8.4a0/weni/analytics_api/urls.py
+-rw-r--r--   0        0        0     9067 2024-05-21 17:24:07.870487 weni-rp-apps-2.8.4a0/weni/analytics_api/views.py
+-rw-r--r--   0        0        0       49 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/auth/__init__.py
+-rw-r--r--   0        0        0      285 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/auth/apps.py
+-rw-r--r--   0        0        0     1327 2024-05-21 17:24:07.870487 weni-rp-apps-2.8.4a0/weni/auth/backends.py
+-rw-r--r--   0        0        0      430 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/auth/decorators.py
+-rw-r--r--   0        0        0      810 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/auth/urls.py
+-rw-r--r--   0        0        0     2645 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/auth/views.py
+-rw-r--r--   0        0        0      309 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/channel_stats/README.md
+-rw-r--r--   0        0        0       66 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/channel_stats/__init__.py
+-rw-r--r--   0        0        0      264 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/channel_stats/apps.py
+-rw-r--r--   0        0        0     6157 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/channel_stats/serializers.py
+-rw-r--r--   0        0        0      347 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/channel_stats/urls.py
+-rw-r--r--   0        0        0     3575 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/channel_stats/views.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/billing/__init__.py
+-rw-r--r--   0        0        0      102 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/billing/apps.py
+-rw-r--r--   0        0        0     3508 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/billing/queries.py
+-rw-r--r--   0        0        0     3194 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/billing/serializers.py
+-rw-r--r--   0        0        0     2063 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/billing/services.py
+-rw-r--r--   0        0        0    11364 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/billing/tests.py
+-rw-r--r--   0        0        0      231 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/billing/urls.py
+-rw-r--r--   0        0        0       64 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/channel/__init__.py
+-rw-r--r--   0        0        0      103 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/channel/apps.py
+-rw-r--r--   0        0        0      352 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/channel/fields.py
+-rw-r--r--   0        0        0     4070 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/channel/serializers.py
+-rw-r--r--   0        0        0     4081 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/channel/services.py
+-rw-r--r--   0        0        0     7987 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/channel/tests.py
+-rw-r--r--   0        0        0      341 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/channel/urls.py
+-rw-r--r--   0        0        0       70 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/classifier/__init__.py
+-rw-r--r--   0        0        0      109 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/classifier/apps.py
+-rw-r--r--   0        0        0     1356 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/classifier/serializers.py
+-rw-r--r--   0        0        0     1174 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/classifier/services.py
+-rw-r--r--   0        0        0     6493 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/classifier/tests.py
+-rw-r--r--   0        0        0      249 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/classifier/urls.py
+-rw-r--r--   0        0        0       61 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/core/__init__.py
+-rw-r--r--   0        0        0      100 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/core/apps.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/core/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/core/management/commands/__init__.py
+-rw-r--r--   0        0        0     1588 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/core/management/commands/grpc.py
+-rw-r--r--   0        0        0     1213 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/core/serializers.py
+-rw-r--r--   0        0        0      965 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/core/services.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/core/tests.py
+-rw-r--r--   0        0        0      700 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/core/urls.py
+-rw-r--r--   0        0        0       58 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/flow/__init__.py
+-rw-r--r--   0        0        0       97 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/flow/apps.py
+-rw-r--r--   0        0        0      307 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/flow/serializers.py
+-rw-r--r--   0        0        0      680 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/flow/services.py
+-rw-r--r--   0        0        0     2764 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/flow/tests.py
+-rw-r--r--   0        0        0      213 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/flow/urls.py
+-rw-r--r--   0        0        0       56 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/org/__init__.py
+-rw-r--r--   0        0        0       95 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/org/apps.py
+-rw-r--r--   0        0        0     2836 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/org/serializers.py
+-rw-r--r--   0        0        0     4020 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/org/services.py
+-rw-r--r--   0        0        0     9821 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/org/tests.py
+-rw-r--r--   0        0        0      207 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/org/urls.py
+-rw-r--r--   0        0        0       68 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/statistic/__init__.py
+-rw-r--r--   0        0        0      107 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/statistic/apps.py
+-rw-r--r--   0        0        0      672 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/statistic/services.py
+-rw-r--r--   0        0        0     3132 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/statistic/tests.py
+-rw-r--r--   0        0        0      252 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/statistic/urls.py
+-rw-r--r--   0        0        0       58 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/user/__init__.py
+-rw-r--r--   0        0        0       97 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/user/apps.py
+-rw-r--r--   0        0        0      843 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/user/serializers.py
+-rw-r--r--   0        0        0     3916 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/user/services.py
+-rw-r--r--   0        0        0    10076 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/user/tests.py
+-rw-r--r--   0        0        0      347 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/grpc/user/urls.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/__init__.py
+-rw-r--r--   0        0        0      328 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/apps.py
+-rw-r--r--   0        0        0      300 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/authenticators.py
+-rw-r--r--   0        0        0     1374 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/backends.py
+-rw-r--r--   0        0        0     5484 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/channel/serializers.py
+-rw-r--r--   0        0        0    16305 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/channel/tests.py
+-rw-r--r--   0        0        0      394 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/channel/urls.py
+-rw-r--r--   0        0        0     8711 2024-05-21 17:24:37.500487 weni-rp-apps-2.8.4a0/weni/internal/channel/views.py
+-rw-r--r--   0        0        0     1527 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/classifier/serializers.py
+-rw-r--r--   0        0        0     8626 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/classifier/tests.py
+-rw-r--r--   0        0        0      318 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/classifier/urls.py
+-rw-r--r--   0        0        0     2803 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/classifier/views.py
+-rw-r--r--   0        0        0      113 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/clients/__init__.py
+-rw-r--r--   0        0        0      692 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/clients/authenticators.py
+-rw-r--r--   0        0        0      486 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/clients/base.py
+-rw-r--r--   0        0        0     1108 2023-12-01 21:28:21.799538 weni-rp-apps-2.8.4a0/weni/internal/clients/connect.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/externals/__init__.py
+-rw-r--r--   0        0        0     2476 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/externals/serializers.py
+-rw-r--r--   0        0        0      546 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/externals/urls.py
+-rw-r--r--   0        0        0     4243 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/externals/views.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/flows/__init__.py
+-rw-r--r--   0        0        0     1460 2024-05-21 18:19:47.320504 weni-rp-apps-2.8.4a0/weni/internal/flows/serializers.py
+-rw-r--r--   0        0        0     4436 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/flows/tests.py
+-rw-r--r--   0        0        0      308 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/flows/urls.py
+-rw-r--r--   0        0        0     1838 2024-05-21 18:19:47.320504 weni-rp-apps-2.8.4a0/weni/internal/flows/views.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/globals/__init__.py
+-rw-r--r--   0        0        0     2286 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/globals/serializers.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/globals/tests/__init__.py
+-rw-r--r--   0        0        0     2183 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/globals/tests/test_serializers.py
+-rw-r--r--   0        0        0      220 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/globals/urls.py
+-rw-r--r--   0        0        0     1484 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/globals/views.py
+-rw-r--r--   0        0        0     1247 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1032 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/migrations/0002_project.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/migrations/__init__.py
+-rw-r--r--   0        0        0     1100 2024-05-21 18:20:23.880504 weni-rp-apps-2.8.4a0/weni/internal/models.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/msgs/__init__.py
+-rw-r--r--   0        0        0     4814 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/msgs/tasks.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/msgs/tests/tests.py
+-rw-r--r--   0        0        0      259 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/msgs/urls.py
+-rw-r--r--   0        0        0     2995 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/msgs/views.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/orgs/__init__.py
+-rw-r--r--   0        0        0     4275 2024-02-22 14:01:53.626509 weni-rp-apps-2.8.4a0/weni/internal/orgs/serializers.py
+-rw-r--r--   0        0        0    16862 2024-02-22 14:01:53.636509 weni-rp-apps-2.8.4a0/weni/internal/orgs/tests.py
+-rw-r--r--   0        0        0      300 2024-02-01 15:07:26.442650 weni-rp-apps-2.8.4a0/weni/internal/orgs/urls.py
+-rw-r--r--   0        0        0     5863 2024-02-22 14:01:53.636509 weni-rp-apps-2.8.4a0/weni/internal/orgs/views.py
+-rw-r--r--   0        0        0      246 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/permissions.py
+-rw-r--r--   0        0        0     2164 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/statistic/tests.py
+-rw-r--r--   0        0        0      205 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/statistic/urls.py
+-rw-r--r--   0        0        0     1007 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/statistic/views.py
+-rw-r--r--   0        0        0       67 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/tasks.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/tests/__init__.py
+-rw-r--r--   0        0        0     1249 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/tests/test_models.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/tickets/__init__.py
+-rw-r--r--   0        0        0     1150 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/tickets/serializers.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.535649 weni-rp-apps-2.8.4a0/weni/internal/tickets/tests/__init__.py
+-rw-r--r--   0        0        0     3360 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/internal/tickets/tests/test_views.py
+-rw-r--r--   0        0        0      521 2024-05-21 17:24:07.870487 weni-rp-apps-2.8.4a0/weni/internal/tickets/urls.py
+-rw-r--r--   0        0        0     2385 2024-05-21 17:24:07.870487 weni-rp-apps-2.8.4a0/weni/internal/tickets/views.py
+-rw-r--r--   0        0        0     1417 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/internal/urls.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/internal/users/__init__.py
+-rw-r--r--   0        0        0      845 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/internal/users/serializers.py
+-rw-r--r--   0        0        0    12563 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/internal/users/tests.py
+-rw-r--r--   0        0        0      711 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/internal/users/urls.py
+-rw-r--r--   0        0        0     6416 2024-05-21 18:20:23.880504 weni-rp-apps-2.8.4a0/weni/internal/users/views.py
+-rw-r--r--   0        0        0      555 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/internal/views.py
+-rw-r--r--   0        0        0       55 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/orgs_api/__init__.py
+-rw-r--r--   0        0        0      253 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/orgs_api/apps.py
+-rw-r--r--   0        0        0      906 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/orgs_api/serializers.py
+-rw-r--r--   0        0        0     4030 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/orgs_api/tests.py
+-rw-r--r--   0        0        0      178 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/orgs_api/urls.py
+-rw-r--r--   0        0        0     1444 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/orgs_api/views.py
+-rw-r--r--   0        0        0       45 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/s3/__init__.py
+-rw-r--r--   0        0        0      243 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/s3/apps.py
+-rw-r--r--   0        0        0      219 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/s3/urls.py
+-rw-r--r--   0        0        0      550 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/s3/views.py
+-rw-r--r--   0        0        0       93 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/serializers/__init__.py
+-rw-r--r--   0        0        0      725 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/serializers/fields.py
+-rw-r--r--   0        0        0      281 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/success_orgs/apps.py
+-rw-r--r--   0        0        0     2791 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/success_orgs/business.py
+-rw-r--r--   0        0        0      619 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/success_orgs/serializers.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/success_orgs/tests/__init__.py
+-rw-r--r--   0        0        0     3354 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/success_orgs/tests/test_business.py
+-rw-r--r--   0        0        0      494 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/success_orgs/urls.py
+-rw-r--r--   0        0        0     2770 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/success_orgs/views.py
+-rw-r--r--   0        0        0      318 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/template_message/README.md
+-rw-r--r--   0        0        0       72 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/template_message/__init__.py
+-rw-r--r--   0        0        0      294 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/template_message/apps.py
+-rw-r--r--   0        0        0     2040 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/template_message/serializers.py
+-rw-r--r--   0        0        0     5292 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/template_message/tests.py
+-rw-r--r--   0        0        0      344 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/template_message/urls.py
+-rw-r--r--   0        0        0     1651 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/template_message/views.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/templates/__init__.py
+-rw-r--r--   0        0        0      545 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/templates/context_processors.py
+-rw-r--r--   0        0        0      315 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/ticketer_queues/README.md
+-rw-r--r--   0        0        0       70 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/ticketer_queues/__init__.py
+-rw-r--r--   0        0        0      291 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/ticketer_queues/apps.py
+-rw-r--r--   0        0        0      242 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/ticketer_queues/serializers.py
+-rw-r--r--   0        0        0     1584 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/ticketer_queues/tests.py
+-rw-r--r--   0        0        0      378 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/ticketer_queues/urls.py
+-rw-r--r--   0        0        0      849 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/ticketer_queues/views.py
+-rw-r--r--   0        0        0        0 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/utils/__init__.py
+-rw-r--r--   0        0        0     1091 2023-10-28 15:26:01.545649 weni-rp-apps-2.8.4a0/weni/utils/app_config.py
+-rw-r--r--   0        0        0     1878 2024-05-21 19:16:36.475294 weni-rp-apps-2.8.4a0/setup.py
+-rw-r--r--   0        0        0      952 2024-05-21 19:16:36.475691 weni-rp-apps-2.8.4a0/PKG-INFO
```

### Comparing `weni_rp_apps-2.8.3a0/pyproject.toml` & `weni-rp-apps-2.8.4a0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "weni-rp-apps"
-version = "2.8.3a0"
+version = "2.8.4a0"
 description = "Weni apps for Rapidpro Platform"
 authors = ["jcbalmeida"]
 license = "AGPL-3.0"
 packages = [
     { include = "weni" }
 ]
```

### Comparing `weni_rp_apps-2.8.3a0/weni/activities/recent_activities.py` & `weni-rp-apps-2.8.4a0/weni/activities/recent_activities.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/activities/signals.py` & `weni-rp-apps-2.8.4a0/weni/activities/signals.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/analytics_api/tests.py` & `weni-rp-apps-2.8.4a0/weni/analytics_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/analytics_api/views.py` & `weni-rp-apps-2.8.4a0/weni/analytics_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/auth/backends.py` & `weni-rp-apps-2.8.4a0/weni/auth/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/auth/urls.py` & `weni-rp-apps-2.8.4a0/weni/auth/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/auth/views.py` & `weni-rp-apps-2.8.4a0/weni/auth/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/channel_stats/serializers.py` & `weni-rp-apps-2.8.4a0/weni/channel_stats/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/channel_stats/views.py` & `weni-rp-apps-2.8.4a0/weni/channel_stats/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/billing/queries.py` & `weni-rp-apps-2.8.4a0/weni/grpc/billing/queries.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/billing/serializers.py` & `weni-rp-apps-2.8.4a0/weni/grpc/billing/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/billing/services.py` & `weni-rp-apps-2.8.4a0/weni/grpc/billing/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/billing/tests.py` & `weni-rp-apps-2.8.4a0/weni/grpc/billing/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/channel/serializers.py` & `weni-rp-apps-2.8.4a0/weni/grpc/channel/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/channel/services.py` & `weni-rp-apps-2.8.4a0/weni/grpc/channel/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/channel/tests.py` & `weni-rp-apps-2.8.4a0/weni/grpc/channel/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/classifier/serializers.py` & `weni-rp-apps-2.8.4a0/weni/grpc/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/classifier/services.py` & `weni-rp-apps-2.8.4a0/weni/grpc/classifier/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/classifier/tests.py` & `weni-rp-apps-2.8.4a0/weni/grpc/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/core/management/commands/grpc.py` & `weni-rp-apps-2.8.4a0/weni/grpc/core/management/commands/grpc.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/core/serializers.py` & `weni-rp-apps-2.8.4a0/weni/grpc/core/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/core/services.py` & `weni-rp-apps-2.8.4a0/weni/grpc/core/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/core/urls.py` & `weni-rp-apps-2.8.4a0/weni/grpc/core/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/flow/services.py` & `weni-rp-apps-2.8.4a0/weni/grpc/flow/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/flow/tests.py` & `weni-rp-apps-2.8.4a0/weni/grpc/flow/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/org/serializers.py` & `weni-rp-apps-2.8.4a0/weni/grpc/org/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/org/services.py` & `weni-rp-apps-2.8.4a0/weni/grpc/org/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/org/tests.py` & `weni-rp-apps-2.8.4a0/weni/grpc/org/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/statistic/services.py` & `weni-rp-apps-2.8.4a0/weni/grpc/statistic/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/statistic/tests.py` & `weni-rp-apps-2.8.4a0/weni/grpc/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/user/serializers.py` & `weni-rp-apps-2.8.4a0/weni/grpc/user/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/user/services.py` & `weni-rp-apps-2.8.4a0/weni/grpc/user/services.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/grpc/user/tests.py` & `weni-rp-apps-2.8.4a0/weni/grpc/user/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/backends.py` & `weni-rp-apps-2.8.4a0/weni/internal/backends.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/channel/serializers.py` & `weni-rp-apps-2.8.4a0/weni/internal/channel/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/channel/tests.py` & `weni-rp-apps-2.8.4a0/weni/internal/channel/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/channel/views.py` & `weni-rp-apps-2.8.4a0/weni/internal/channel/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/classifier/serializers.py` & `weni-rp-apps-2.8.4a0/weni/internal/classifier/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/classifier/tests.py` & `weni-rp-apps-2.8.4a0/weni/internal/classifier/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/classifier/views.py` & `weni-rp-apps-2.8.4a0/weni/internal/classifier/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/clients/authenticators.py` & `weni-rp-apps-2.8.4a0/weni/internal/clients/authenticators.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/clients/connect.py` & `weni-rp-apps-2.8.4a0/weni/internal/clients/connect.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/externals/serializers.py` & `weni-rp-apps-2.8.4a0/weni/internal/externals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/externals/urls.py` & `weni-rp-apps-2.8.4a0/weni/internal/externals/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/externals/views.py` & `weni-rp-apps-2.8.4a0/weni/internal/externals/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/flows/serializers.py` & `weni-rp-apps-2.8.4a0/weni/internal/flows/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/flows/tests.py` & `weni-rp-apps-2.8.4a0/weni/internal/flows/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/flows/views.py` & `weni-rp-apps-2.8.4a0/weni/internal/flows/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/globals/serializers.py` & `weni-rp-apps-2.8.4a0/weni/internal/globals/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/globals/tests/test_serializers.py` & `weni-rp-apps-2.8.4a0/weni/internal/globals/tests/test_serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/globals/views.py` & `weni-rp-apps-2.8.4a0/weni/internal/globals/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/migrations/0001_initial.py` & `weni-rp-apps-2.8.4a0/weni/internal/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/migrations/0002_project.py` & `weni-rp-apps-2.8.4a0/weni/internal/migrations/0002_project.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/models.py` & `weni-rp-apps-2.8.4a0/weni/internal/models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/msgs/tasks.py` & `weni-rp-apps-2.8.4a0/weni/internal/msgs/tasks.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/msgs/views.py` & `weni-rp-apps-2.8.4a0/weni/internal/msgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/orgs/serializers.py` & `weni-rp-apps-2.8.4a0/weni/internal/orgs/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/orgs/tests.py` & `weni-rp-apps-2.8.4a0/weni/internal/orgs/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/orgs/views.py` & `weni-rp-apps-2.8.4a0/weni/internal/orgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/statistic/tests.py` & `weni-rp-apps-2.8.4a0/weni/internal/statistic/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/statistic/views.py` & `weni-rp-apps-2.8.4a0/weni/internal/statistic/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/tests/test_models.py` & `weni-rp-apps-2.8.4a0/weni/internal/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/tickets/serializers.py` & `weni-rp-apps-2.8.4a0/weni/internal/tickets/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/tickets/tests/test_views.py` & `weni-rp-apps-2.8.4a0/weni/internal/tickets/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/tickets/urls.py` & `weni-rp-apps-2.8.4a0/weni/internal/tickets/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/tickets/views.py` & `weni-rp-apps-2.8.4a0/weni/internal/tickets/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/urls.py` & `weni-rp-apps-2.8.4a0/weni/internal/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/users/serializers.py` & `weni-rp-apps-2.8.4a0/weni/internal/users/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/users/tests.py` & `weni-rp-apps-2.8.4a0/weni/internal/users/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/users/urls.py` & `weni-rp-apps-2.8.4a0/weni/internal/users/urls.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/users/views.py` & `weni-rp-apps-2.8.4a0/weni/internal/users/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import TYPE_CHECKING
 
 from django.conf import settings
 from django.shortcuts import get_object_or_404
 from django.contrib.auth import get_user_model
+from django.contrib.auth.models import Group
 
 from rest_framework import status
 from rest_framework.decorators import action
 from rest_framework.response import Response
 from rest_framework import exceptions
 from rest_framework import mixins
 from rest_framework.exceptions import ValidationError
@@ -37,17 +38,30 @@
     def api_token(self, request: "Request", **kwargs):
         serializer = self.get_serializer(data=request.query_params)
         serializer.is_valid(raise_exception=True)
         user = serializer.validated_data.get("user")
         project = serializer.validated_data.get("project")
 
         try:
-            api_token = APIToken.objects.get(user=user, org=project.org)
-        except APIToken.DoesNotExist:
-            raise exceptions.PermissionDenied()
+            group_prometheus = Group.objects.get(name="Prometheus")
+        except Group.DoesNotExist:
+            raise exceptions.PermissionDenied("Group 'Prometheus' does not exist.")
+
+        api_tokens = APIToken.objects.filter(
+            is_active=True, user=user, org=project.org
+        ).exclude(role=group_prometheus)
+
+        if api_tokens.count() == 0:
+            raise exceptions.PermissionDenied("No active API token found for the user.")
+        elif api_tokens.count() > 1:
+            raise exceptions.PermissionDenied(
+                "Multiple active API tokens found for the user."
+            )
+
+        api_token = api_tokens.first()
 
         return Response(
             dict(
                 user=api_token.user.email,
                 project=project.project_uuid,
                 api_token=api_token.key,
             )
@@ -144,15 +158,17 @@
     serializer_class = UserSerializer
     queryset = User.objects.all()
     lookup_field = "uuid"
 
     def partial_update(self, request):
         instance = get_object_or_404(User, email=request.query_params.get("email"))
 
-        if request.data.get("language") not in [language[0] for language in settings.LANGUAGES]:
+        if request.data.get("language") not in [
+            language[0] for language in settings.LANGUAGES
+        ]:
             raise ValidationError("Invalid argument: language")
 
         user_settings = instance.get_settings()
         user_settings.language = request.data.get("language")
         user_settings.save()
 
         return Response(status=status.HTTP_200_OK)
```

### Comparing `weni_rp_apps-2.8.3a0/weni/internal/views.py` & `weni-rp-apps-2.8.4a0/weni/internal/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/orgs_api/serializers.py` & `weni-rp-apps-2.8.4a0/weni/orgs_api/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/orgs_api/tests.py` & `weni-rp-apps-2.8.4a0/weni/orgs_api/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/orgs_api/views.py` & `weni-rp-apps-2.8.4a0/weni/orgs_api/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/s3/views.py` & `weni-rp-apps-2.8.4a0/weni/s3/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/serializers/fields.py` & `weni-rp-apps-2.8.4a0/weni/serializers/fields.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/success_orgs/business.py` & `weni-rp-apps-2.8.4a0/weni/success_orgs/business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/success_orgs/serializers.py` & `weni-rp-apps-2.8.4a0/weni/success_orgs/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/success_orgs/tests/test_business.py` & `weni-rp-apps-2.8.4a0/weni/success_orgs/tests/test_business.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/success_orgs/views.py` & `weni-rp-apps-2.8.4a0/weni/success_orgs/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/template_message/serializers.py` & `weni-rp-apps-2.8.4a0/weni/template_message/serializers.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/template_message/tests.py` & `weni-rp-apps-2.8.4a0/weni/template_message/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/template_message/views.py` & `weni-rp-apps-2.8.4a0/weni/template_message/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/templates/context_processors.py` & `weni-rp-apps-2.8.4a0/weni/templates/context_processors.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/ticketer_queues/tests.py` & `weni-rp-apps-2.8.4a0/weni/ticketer_queues/tests.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/ticketer_queues/views.py` & `weni-rp-apps-2.8.4a0/weni/ticketer_queues/views.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/weni/utils/app_config.py` & `weni-rp-apps-2.8.4a0/weni/utils/app_config.py`

 * *Files identical despite different names*

### Comparing `weni_rp_apps-2.8.3a0/PKG-INFO` & `weni-rp-apps-2.8.4a0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: weni-rp-apps
-Version: 2.8.3a0
+Version: 2.8.4a0
 Summary: Weni apps for Rapidpro Platform
 License: AGPL-3.0
 Author: jcbalmeida
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: django-csp (>=3.7,<4.0)
 Requires-Dist: django-environ (>=0.7.0,<0.8.0)
 Requires-Dist: django-templates-macros (>=0.2,<0.3)
 Requires-Dist: djangogrpcframework (>=0.2.1,<0.3.0)
 Requires-Dist: drf-nested-routers (>=0.93.4,<0.94.0)
 Requires-Dist: elastic-apm (>=6.4.0,<7.0.0)
 Requires-Dist: flower (>=0.9,<0.10)
```

