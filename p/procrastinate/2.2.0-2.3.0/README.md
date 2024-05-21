# Comparing `tmp/procrastinate-2.2.0.tar.gz` & `tmp/procrastinate-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "procrastinate-2.2.0.tar", max compression
+gzip compressed data, was "procrastinate-2.3.0.tar", max compression
```

## Comparing `procrastinate-2.2.0.tar` & `procrastinate-2.3.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0     1122 2024-04-17 21:42:41.056214 procrastinate-2.2.0/LICENSE.md
--rw-r--r--   0        0        0     5140 2024-04-17 21:42:41.056214 procrastinate-2.2.0/README.md
--rw-r--r--   0        0        0     1196 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/__init__.py
--rw-r--r--   0        0        0      180 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/__main__.py
--rw-r--r--   0        0        0    11994 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/app.py
--rw-r--r--   0        0        0    10104 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/blueprints.py
--rw-r--r--   0        0        0     1090 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/builtin_tasks.py
--rw-r--r--   0        0        0    19466 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/cli.py
--rw-r--r--   0        0        0     3197 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/connector.py
--rw-r--r--   0        0        0      181 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/README.md
--rw-r--r--   0        0        0        0 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/__init__.py
--rw-r--r--   0        0        0      110 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/aiopg/__init__.py
--rw-r--r--   0        0        0    12731 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/aiopg/aiopg_connector.py
--rw-r--r--   0        0        0     6148 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/README.md
--rw-r--r--   0        0        0      234 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/__init__.py
--rw-r--r--   0        0        0      733 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/admin.py
--rw-r--r--   0        0        0     1649 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/apps.py
--rw-r--r--   0        0        0     5662 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/django_connector.py
--rw-r--r--   0        0        0      208 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/exceptions.py
--rw-r--r--   0        0        0     1558 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/healthchecks.py
--rw-r--r--   0        0        0        0 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/management/__init__.py
--rw-r--r--   0        0        0        0 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/management/commands/__init__.py
--rw-r--r--   0        0        0      899 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/management/commands/procrastinate.py
--rw-r--r--   0        0        0     4788 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/migrations_magic.py
--rw-r--r--   0        0        0     3450 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/models.py
--rw-r--r--   0        0        0     2424 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/procrastinate_app.py
--rw-r--r--   0        0        0      736 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/settings.py
--rw-r--r--   0        0        0     3450 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/static_migrations.py
--rw-r--r--   0        0        0     1139 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/django/utils.py
--rw-r--r--   0        0        0      119 2024-04-17 21:42:41.060214 procrastinate-2.2.0/procrastinate/contrib/psycopg2/__init__.py
--rw-r--r--   0        0        0     7864 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/contrib/psycopg2/psycopg2_connector.py
--rw-r--r--   0        0        0      428 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/contrib/sqlalchemy/README.md
--rw-r--r--   0        0        0      187 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     6050 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/contrib/sqlalchemy/psycopg2_connector.py
--rw-r--r--   0        0        0     3406 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/exceptions.py
--rw-r--r--   0        0        0     3172 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/job_context.py
--rw-r--r--   0        0        0     4948 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/jobs.py
--rw-r--r--   0        0        0    20361 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/manager.py
--rw-r--r--   0        0        0      477 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/metadata.py
--rw-r--r--   0        0        0     8874 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/periodic.py
--rw-r--r--   0        0        0     9703 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/psycopg_connector.py
--rw-r--r--   0        0        0        0 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/py.typed
--rw-r--r--   0        0        0     3762 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/retry.py
--rw-r--r--   0        0        0     1555 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/schema.py
--rw-r--r--   0        0        0     5662 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/shell.py
--rw-r--r--   0        0        0     2947 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/signals.py
--rw-r--r--   0        0        0     1325 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/__init__.py
--rw-r--r--   0        0        0      120 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/future_migrations/02.00.00_01_drop_old_procrastinate_finish_job.sql
--rw-r--r--   0        0        0     6554 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.00.00_01_initial.sql
--rw-r--r--   0        0        0     1212 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.05.00_01_drop_started_at_column.sql
--rw-r--r--   0        0        0      121 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.05.00_02_drop_started_at_column.sql
--rw-r--r--   0        0        0       84 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.05.00_03_drop_procrastinate_version_table.sql
--rw-r--r--   0        0        0     1188 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.06.00_01_fix_procrastinate_fetch_job.sql
--rw-r--r--   0        0        0      394 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.07.01_01_fix_trigger_status_events_insert.sql
--rw-r--r--   0        0        0      242 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.08.01_01_add_queueing_lock_column.sql
--rw-r--r--   0        0        0     1742 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.10.00_01_close_fetch_job_race_condition.sql
--rw-r--r--   0        0        0      502 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.10.00_02_add_defer_job_function.sql
--rw-r--r--   0        0        0     2081 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.11.00_03_add_procrastinate_periodic_defers.sql
--rw-r--r--   0        0        0       97 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.12.00_01_add_foreign_key_index.sql
--rw-r--r--   0        0        0     1791 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.14.00_01_add_locks_to_periodic_defer.sql
--rw-r--r--   0        0        0     1553 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.15.02_01_fix_procrastinate_defer_periodic_job.sql
--rw-r--r--   0        0        0      561 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.16.00_01_add_finish_job_and_retry_job_functions.sql
--rw-r--r--   0        0        0      384 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.17.00_01_add_trigger_on_job_deletion.sql
--rw-r--r--   0        0        0      401 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.17.00_02_delete_finished_jobs.sql
--rw-r--r--   0        0        0      987 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.17.00_03_add_checks_to_finish_job.sql
--rw-r--r--   0        0        0      499 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.17.00_04_add_checks_to_retry_job.sql
--rw-r--r--   0        0        0     1115 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.18.01_01_fix_finish_job_compat_issue.sql
--rw-r--r--   0        0        0      188 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.19.00_01_add_index_on_procrastinate_jobs.sql
--rw-r--r--   0        0        0     2068 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.22.00_01_add_kwargs_to_defer_periodic_job.sql
--rw-r--r--   0        0        0     1361 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/00.23.00_01_null_locks_excluded.sql
--rw-r--r--   0        0        0     1699 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/01.00.00_01_remove_old_finish_job_function.sql
--rw-r--r--   0        0        0     1736 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/01.01.01_01_job_id_bigint.sql
--rw-r--r--   0        0        0        0 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/migrations/__init__.py
--rw-r--r--   0        0        0     5802 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/queries.sql
--rw-r--r--   0        0        0    12318 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sql/schema.sql
--rw-r--r--   0        0        0     5996 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/sync_psycopg_connector.py
--rw-r--r--   0        0        0     7235 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/tasks.py
--rw-r--r--   0        0        0    10224 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/testing.py
--rw-r--r--   0        0        0      174 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/types.py
--rw-r--r--   0        0        0    13732 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/utils.py
--rw-r--r--   0        0        0    11926 2024-04-17 21:42:41.064214 procrastinate-2.2.0/procrastinate/worker.py
--rw-r--r--   0        0        0     4104 2024-04-17 21:42:41.920210 procrastinate-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     6752 1970-01-01 00:00:00.000000 procrastinate-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1122 2024-05-21 08:36:12.530564 procrastinate-2.3.0/LICENSE.md
+-rw-r--r--   0        0        0     5140 2024-05-21 08:36:12.530564 procrastinate-2.3.0/README.md
+-rw-r--r--   0        0        0     1196 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/__init__.py
+-rw-r--r--   0        0        0      180 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/__main__.py
+-rw-r--r--   0        0        0    11994 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/app.py
+-rw-r--r--   0        0        0    12043 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/blueprints.py
+-rw-r--r--   0        0        0     1090 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/builtin_tasks.py
+-rw-r--r--   0        0        0    19466 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/cli.py
+-rw-r--r--   0        0        0     3197 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/connector.py
+-rw-r--r--   0        0        0      181 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/__init__.py
+-rw-r--r--   0        0        0      110 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/aiopg/__init__.py
+-rw-r--r--   0        0        0    12731 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/aiopg/aiopg_connector.py
+-rw-r--r--   0        0        0     6148 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/django/README.md
+-rw-r--r--   0        0        0      234 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/django/__init__.py
+-rw-r--r--   0        0        0      733 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/django/admin.py
+-rw-r--r--   0        0        0     1649 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/django/apps.py
+-rw-r--r--   0        0        0     5662 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/django/django_connector.py
+-rw-r--r--   0        0        0      208 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/django/exceptions.py
+-rw-r--r--   0        0        0     1558 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/django/healthchecks.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/django/management/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/django/management/commands/__init__.py
+-rw-r--r--   0        0        0      899 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/django/management/commands/procrastinate.py
+-rw-r--r--   0        0        0     4788 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/django/migrations_magic.py
+-rw-r--r--   0        0        0     3450 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/django/models.py
+-rw-r--r--   0        0        0     2424 2024-05-21 08:36:12.534564 procrastinate-2.3.0/procrastinate/contrib/django/procrastinate_app.py
+-rw-r--r--   0        0        0      736 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/contrib/django/settings.py
+-rw-r--r--   0        0        0     3450 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/contrib/django/static_migrations.py
+-rw-r--r--   0        0        0     1139 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/contrib/django/utils.py
+-rw-r--r--   0        0        0      119 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/contrib/psycopg2/__init__.py
+-rw-r--r--   0        0        0     7864 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/contrib/psycopg2/psycopg2_connector.py
+-rw-r--r--   0        0        0      428 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/contrib/sqlalchemy/README.md
+-rw-r--r--   0        0        0      187 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     6050 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/contrib/sqlalchemy/psycopg2_connector.py
+-rw-r--r--   0        0        0     3406 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/exceptions.py
+-rw-r--r--   0        0        0     3172 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/job_context.py
+-rw-r--r--   0        0        0     4948 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/jobs.py
+-rw-r--r--   0        0        0    20361 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/manager.py
+-rw-r--r--   0        0        0      477 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/metadata.py
+-rw-r--r--   0        0        0     9559 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/periodic.py
+-rw-r--r--   0        0        0     9703 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/psycopg_connector.py
+-rw-r--r--   0        0        0        0 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/py.typed
+-rw-r--r--   0        0        0     3762 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/retry.py
+-rw-r--r--   0        0        0     1555 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/schema.py
+-rw-r--r--   0        0        0     5662 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/shell.py
+-rw-r--r--   0        0        0     2947 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/signals.py
+-rw-r--r--   0        0        0     1325 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/__init__.py
+-rw-r--r--   0        0        0      120 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/future_migrations/02.00.00_01_drop_old_procrastinate_finish_job.sql
+-rw-r--r--   0        0        0     6554 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.00.00_01_initial.sql
+-rw-r--r--   0        0        0     1212 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.05.00_01_drop_started_at_column.sql
+-rw-r--r--   0        0        0      121 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.05.00_02_drop_started_at_column.sql
+-rw-r--r--   0        0        0       84 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.05.00_03_drop_procrastinate_version_table.sql
+-rw-r--r--   0        0        0     1188 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.06.00_01_fix_procrastinate_fetch_job.sql
+-rw-r--r--   0        0        0      394 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.07.01_01_fix_trigger_status_events_insert.sql
+-rw-r--r--   0        0        0      242 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.08.01_01_add_queueing_lock_column.sql
+-rw-r--r--   0        0        0     1742 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.10.00_01_close_fetch_job_race_condition.sql
+-rw-r--r--   0        0        0      502 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.10.00_02_add_defer_job_function.sql
+-rw-r--r--   0        0        0     2081 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.11.00_03_add_procrastinate_periodic_defers.sql
+-rw-r--r--   0        0        0       97 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.12.00_01_add_foreign_key_index.sql
+-rw-r--r--   0        0        0     1791 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.14.00_01_add_locks_to_periodic_defer.sql
+-rw-r--r--   0        0        0     1553 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.15.02_01_fix_procrastinate_defer_periodic_job.sql
+-rw-r--r--   0        0        0      561 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.16.00_01_add_finish_job_and_retry_job_functions.sql
+-rw-r--r--   0        0        0      384 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.17.00_01_add_trigger_on_job_deletion.sql
+-rw-r--r--   0        0        0      401 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.17.00_02_delete_finished_jobs.sql
+-rw-r--r--   0        0        0      987 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.17.00_03_add_checks_to_finish_job.sql
+-rw-r--r--   0        0        0      499 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.17.00_04_add_checks_to_retry_job.sql
+-rw-r--r--   0        0        0     1115 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.18.01_01_fix_finish_job_compat_issue.sql
+-rw-r--r--   0        0        0      188 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.19.00_01_add_index_on_procrastinate_jobs.sql
+-rw-r--r--   0        0        0     2068 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.22.00_01_add_kwargs_to_defer_periodic_job.sql
+-rw-r--r--   0        0        0     1361 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/00.23.00_01_null_locks_excluded.sql
+-rw-r--r--   0        0        0     1699 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/01.00.00_01_remove_old_finish_job_function.sql
+-rw-r--r--   0        0        0     1736 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/01.01.01_01_job_id_bigint.sql
+-rw-r--r--   0        0        0        0 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/migrations/__init__.py
+-rw-r--r--   0        0        0     5802 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/queries.sql
+-rw-r--r--   0        0        0    12318 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sql/schema.sql
+-rw-r--r--   0        0        0     5996 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/sync_psycopg_connector.py
+-rw-r--r--   0        0        0     7964 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/tasks.py
+-rw-r--r--   0        0        0    10224 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/testing.py
+-rw-r--r--   0        0        0      174 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/types.py
+-rw-r--r--   0        0        0    13732 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/utils.py
+-rw-r--r--   0        0        0    11926 2024-05-21 08:36:12.538564 procrastinate-2.3.0/procrastinate/worker.py
+-rw-r--r--   0        0        0     4104 2024-05-21 08:36:13.426564 procrastinate-2.3.0/pyproject.toml
+-rw-r--r--   0        0        0     6752 1970-01-01 00:00:00.000000 procrastinate-2.3.0/PKG-INFO
```

### Comparing `procrastinate-2.2.0/LICENSE.md` & `procrastinate-2.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/README.md` & `procrastinate-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/__init__.py` & `procrastinate-2.3.0/procrastinate/__init__.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/app.py` & `procrastinate-2.3.0/procrastinate/app.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/blueprints.py` & `procrastinate-2.3.0/procrastinate/blueprints.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,27 @@
 from __future__ import annotations
 
 import functools
 import logging
 import sys
-from typing import TYPE_CHECKING, Any, Callable
+from typing import TYPE_CHECKING, Any, Callable, Literal, Union, cast, overload
+
+from typing_extensions import Concatenate, ParamSpec, Unpack
 
 from procrastinate import exceptions, jobs, periodic, retry, utils
+from procrastinate.job_context import JobContext
 
 if TYPE_CHECKING:
-    from procrastinate import tasks
+    from procrastinate.tasks import ConfigureTaskOptions, Task
+
 
 logger = logging.getLogger(__name__)
 
+P = ParamSpec("P")
+
 
 class Blueprint:
     """
     A Blueprint provides a way to declare tasks that can be registered on an
     `App` later::
 
         # Create blueprint for all tasks related to the cat
@@ -59,15 +65,15 @@
 
             Traceback (most recent call last):
                 File "..."
             `UnboundTaskError`: ...
     """
 
     def __init__(self) -> None:
-        self.tasks: dict[str, tasks.Task] = {}
+        self.tasks: dict[str, Task] = {}
         self.periodic_registry = periodic.PeriodicRegistry()
         self._check_stack()
 
     def _check_stack(self):
         # Emit a warning if the app is defined in the __main__ module
         name = None
         try:
@@ -84,47 +90,47 @@
             logger.warning(
                 f"{type(self).__name__} is instantiated in the main Python module "
                 f"({sys.argv[0]}). "
                 "See https://procrastinate.readthedocs.io/en/stable/discussions.html#top-level-app",
                 extra={"action": "app_defined_in___main__"},
             )
 
-    def _register_task(self, task: tasks.Task) -> None:
+    def _register_task(self, task: Task) -> None:
         """
         Register the task into the blueprint task registry.
         Raises exceptions.TaskAlreadyRegistered if the task name
         or an alias already exists in the registry
         """
 
         # Each call to _add_task may raise TaskAlreadyRegistered.
         # We're using an intermediary dict to make sure that if the registration
         # is interrupted midway though, self.tasks is left unmodified.
-        to_add: dict[str, tasks.Task] = {}
+        to_add: dict[str, Task] = {}
         self._add_task(task=task, name=task.name, to=to_add)
 
         for alias in task.aliases:
             self._add_task(task=task, name=alias, to=to_add)
 
         self.tasks.update(to_add)
 
-    def _add_task(self, task: tasks.Task, name: str, to: dict | None = None) -> None:
+    def _add_task(self, task: Task, name: str, to: dict | None = None) -> None:
         # Add a task to a dict of task while making
         # sure a task of the same name was not already in self.tasks.
         # This lets us prepare a dict of tasks we might add while not adding
         # them until we're 100% sure there's no clash.
 
         if name in self.tasks:
             raise exceptions.TaskAlreadyRegistered(
                 f"A task named {name} was already registered"
             )
 
         result_dict = self.tasks if to is None else to
         result_dict[name] = task
 
-    def add_task_alias(self, task: tasks.Task, alias: str) -> None:
+    def add_task_alias(self, task: Task, alias: str) -> None:
         """
         Add an alias to a task. This can be useful if a task was in a given
         Blueprint and moves to a different blueprint.
 
         Parameters
         ----------
         task :
@@ -185,45 +191,30 @@
             self.periodic_registry.register_task(
                 task=periodic_task.task,
                 cron=periodic_task.cron,
                 periodic_id=periodic_task.periodic_id,
                 configure_kwargs=periodic_task.configure_kwargs,
             )
 
+    @overload
     def task(
         self,
-        _func: Callable[..., Any] | None = None,
         *,
+        _func: None = None,
         name: str | None = None,
         aliases: list[str] | None = None,
         retry: retry.RetryValue = False,
-        pass_context: bool = False,
+        pass_context: Literal[False] = False,
         queue: str = jobs.DEFAULT_QUEUE,
         lock: str | None = None,
         queueing_lock: str | None = None,
-    ) -> Any:
-        """
-        Declare a function as a task. This method is meant to be used as a decorator::
-
-            @app.task(...)
-            def my_task(args):
-                ...
-
-        or::
-
-            @app.task
-            def my_task(args):
-                ...
-
-        The second form will use the default value for all parameters.
-
+    ) -> Callable[[Callable[P]], Task[P, P]]:
+        """Declare a function as a task. This method is meant to be used as a decorator
         Parameters
         ----------
-        _func :
-            The decorated function
         queue :
             The name of the queue in which jobs from this task will be launched, if
             the queue is not overridden at launch.
             Default is ``"default"``.
             When a worker is launched, it can listen to specific queues, or to all
             queues.
         lock :
@@ -247,19 +238,81 @@
             - An ``int``: the number of retries before it gives up
             - A `procrastinate.RetryStrategy` instance for complex cases
 
             Default is no retry.
         pass_context :
             Passes the task execution context in the task as first
         """
+        ...
+
+    @overload
+    def task(
+        self,
+        *,
+        _func: None = None,
+        name: str | None = None,
+        aliases: list[str] | None = None,
+        retry: retry.RetryValue = False,
+        pass_context: Literal[True],
+        queue: str = jobs.DEFAULT_QUEUE,
+        lock: str | None = None,
+        queueing_lock: str | None = None,
+    ) -> Callable[
+        [Callable[Concatenate[JobContext, P]]],
+        Task[Concatenate[JobContext, P], P],
+    ]:
+        """Declare a function as a task. This method is meant to be used as a decorator
+        Parameters
+        ----------
+        _func :
+            The decorated function
+        """
+        ...
 
-        def _wrap(func: Callable[..., tasks.Task]):
-            from procrastinate import tasks
+    @overload
+    def task(self, _func: Callable[P]) -> Task[P, P]:
+        """Declare a function as a task. This method is meant to be used as a decorator
+        Parameters
+        ----------
+        _func :
+            The decorated function
+        """
+        ...
+
+    def task(
+        self,
+        _func: Callable[P] | None = None,
+        *,
+        name: str | None = None,
+        aliases: list[str] | None = None,
+        retry: retry.RetryValue = False,
+        pass_context: bool = False,
+        queue: str = jobs.DEFAULT_QUEUE,
+        lock: str | None = None,
+        queueing_lock: str | None = None,
+    ):
+        from procrastinate.tasks import Task
 
-            task = tasks.Task(
+        """
+        Declare a function as a task. This method is meant to be used as a decorator::
+
+            @app.task(...)
+            def my_task(args):
+                ...
+
+        or::
+
+            @app.task
+            def my_task(args):
+                ...
+        The second form will use the default value for all parameters.
+        """
+
+        def _wrap(func: Callable[P]):
+            task = Task(
                 func,
                 blueprint=self,
                 queue=queue,
                 lock=lock,
                 queueing_lock=queueing_lock,
                 name=name,
                 aliases=aliases,
@@ -267,31 +320,46 @@
                 pass_context=pass_context,
             )
             self._register_task(task)
 
             return functools.update_wrapper(task, func, updated=())
 
         if _func is None:  # Called as @app.task(...)
-            return _wrap
+            return cast(
+                Union[
+                    Callable[[Callable[P, Any]], Task[P, P]],
+                    Callable[
+                        [Callable[Concatenate[JobContext, P], Any]],
+                        Task[Concatenate[JobContext, P], P],
+                    ],
+                ],
+                _wrap,
+            )
 
         return _wrap(_func)  # Called as @app.task
 
-    def periodic(self, *, cron: str, periodic_id: str = "", **kwargs: dict[str, Any]):
+    def periodic(
+        self,
+        *,
+        cron: str,
+        periodic_id: str = "",
+        **configure_kwargs: Unpack[ConfigureTaskOptions],
+    ):
         """
         Task decorator, marks task as being scheduled for periodic deferring (see
         `howto/advanced/cron`).
 
         Parameters
         ----------
         cron :
             Cron-like string. Optionally add a 6th column for seconds.
         periodic_id :
             Task name suffix. Used to distinguish periodic tasks with different kwargs.
         **kwargs :
             Additional parameters are passed to `Task.configure`.
         """
         return self.periodic_registry.periodic_decorator(
-            cron=cron, periodic_id=periodic_id, **kwargs
+            cron=cron, periodic_id=periodic_id, **configure_kwargs
         )
 
     def will_configure_task(self) -> None:
         raise exceptions.UnboundTaskError
```

### Comparing `procrastinate-2.2.0/procrastinate/builtin_tasks.py` & `procrastinate-2.3.0/procrastinate/builtin_tasks.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/cli.py` & `procrastinate-2.3.0/procrastinate/cli.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/connector.py` & `procrastinate-2.3.0/procrastinate/connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/aiopg/aiopg_connector.py` & `procrastinate-2.3.0/procrastinate/contrib/aiopg/aiopg_connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/django/README.md` & `procrastinate-2.3.0/procrastinate/contrib/django/README.md`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/django/admin.py` & `procrastinate-2.3.0/procrastinate/contrib/django/admin.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/django/apps.py` & `procrastinate-2.3.0/procrastinate/contrib/django/apps.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/django/django_connector.py` & `procrastinate-2.3.0/procrastinate/contrib/django/django_connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/django/healthchecks.py` & `procrastinate-2.3.0/procrastinate/contrib/django/healthchecks.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/django/management/commands/procrastinate.py` & `procrastinate-2.3.0/procrastinate/contrib/django/management/commands/procrastinate.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/django/migrations_magic.py` & `procrastinate-2.3.0/procrastinate/contrib/django/migrations_magic.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/django/models.py` & `procrastinate-2.3.0/procrastinate/contrib/django/models.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/django/procrastinate_app.py` & `procrastinate-2.3.0/procrastinate/contrib/django/procrastinate_app.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/django/settings.py` & `procrastinate-2.3.0/procrastinate/contrib/django/settings.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/django/static_migrations.py` & `procrastinate-2.3.0/procrastinate/contrib/django/static_migrations.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/django/utils.py` & `procrastinate-2.3.0/procrastinate/contrib/django/utils.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/psycopg2/psycopg2_connector.py` & `procrastinate-2.3.0/procrastinate/contrib/psycopg2/psycopg2_connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/contrib/sqlalchemy/psycopg2_connector.py` & `procrastinate-2.3.0/procrastinate/contrib/sqlalchemy/psycopg2_connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/exceptions.py` & `procrastinate-2.3.0/procrastinate/exceptions.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/job_context.py` & `procrastinate-2.3.0/procrastinate/job_context.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/jobs.py` & `procrastinate-2.3.0/procrastinate/jobs.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/manager.py` & `procrastinate-2.3.0/procrastinate/manager.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/periodic.py` & `procrastinate-2.3.0/procrastinate/periodic.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,73 +1,85 @@
 from __future__ import annotations
 
 import asyncio
 import functools
 import logging
 import time
-from typing import Any, Iterable, Tuple
+from typing import Callable, Generic, Iterable, Tuple, cast
 
 import attr
 import croniter
+from typing_extensions import Concatenate, ParamSpec, Unpack
 
 from procrastinate import exceptions, tasks
 
+P = ParamSpec("P")
+Args = ParamSpec("Args")
+
 # The maximum delay after which tasks will be considered as
 # outdated, and ignored.
 MAX_DELAY = 60 * 10  # 10 minutes
 # We'll always be oversleeping by this amount to avoid waking up too early for our
 # tasks. This is, of course, the most important part of procrastinate ;)
 MARGIN = 0.5  # seconds
 
 logger = logging.getLogger(__name__)
 
 cached_property = functools.cached_property
 
 
 @attr.dataclass(frozen=True)
-class PeriodicTask:
-    task: tasks.Task
+class PeriodicTask(Generic[P, Args]):
+    task: tasks.Task[P, Args]
     cron: str
     periodic_id: str
-    configure_kwargs: dict[str, Any]
+    configure_kwargs: tasks.ConfigureTaskOptions
 
     @cached_property
     def croniter(self) -> croniter.croniter:
         return croniter.croniter(self.cron)
 
 
 TaskAtTime = Tuple[PeriodicTask, int]
 
 
 class PeriodicRegistry:
     def __init__(self):
         self.periodic_tasks: dict[tuple[str, str], PeriodicTask] = {}
 
-    def periodic_decorator(self, cron: str, periodic_id: str, **kwargs):
+    def periodic_decorator(
+        self,
+        cron: str,
+        periodic_id: str,
+        **configure_kwargs: Unpack[tasks.ConfigureTaskOptions],
+    ) -> Callable[[tasks.Task[P, Concatenate[int, Args]]], tasks.Task[P, Args]]:
         """
         Decorator over a task definition that registers that task for periodic
         launch. This decorator should not be used directly, ``@app.periodic()`` is meant
         to be used instead.
         """
 
-        def wrapper(task: tasks.Task):
+        def wrapper(task: tasks.Task[P, Concatenate[int, Args]]) -> tasks.Task[P, Args]:
             self.register_task(
-                task=task, cron=cron, periodic_id=periodic_id, configure_kwargs=kwargs
+                task=task,
+                cron=cron,
+                periodic_id=periodic_id,
+                configure_kwargs=configure_kwargs,
             )
-            return task
+            return cast(tasks.Task[P, Args], task)
 
         return wrapper
 
     def register_task(
         self,
-        task: tasks.Task,
+        task: tasks.Task[P, Concatenate[int, Args]],
         cron: str,
         periodic_id: str,
-        configure_kwargs: dict[str, Any],
-    ) -> PeriodicTask:
+        configure_kwargs: tasks.ConfigureTaskOptions,
+    ) -> PeriodicTask[P, Concatenate[int, Args]]:
         key = (task.name, periodic_id)
         if key in self.periodic_tasks:
             raise exceptions.TaskAlreadyRegistered(
                 "A periodic task was already registed with the same periodic_id "
                 f"({periodic_id!r}). Please use a different periodic_id for multiple "
                 "schedules of the same task."
             )
@@ -186,15 +198,20 @@
         Try deferring all tasks that might need deferring. The database will keep us
         from deferring the same task for the same scheduled time multiple times.
         """
         for periodic_task, timestamp in jobs_to_defer:
             task = periodic_task.task
             periodic_id = periodic_task.periodic_id
             configure_kwargs = periodic_task.configure_kwargs
-            configure_kwargs.setdefault("task_kwargs", {})["timestamp"] = timestamp
+            task_kwargs = configure_kwargs.get("task_kwargs")
+            if task_kwargs is None:
+                task_kwargs = {}
+                configure_kwargs["task_kwargs"] = task_kwargs
+            task_kwargs["timestamp"] = timestamp
+
             description = {
                 "task_name": task.name,
                 "periodic_id": periodic_id,
                 "defer_timestamp": timestamp,
                 "kwargs": configure_kwargs,
             }
             job_deferrer = task.configure(**configure_kwargs)
```

### Comparing `procrastinate-2.2.0/procrastinate/psycopg_connector.py` & `procrastinate-2.3.0/procrastinate/psycopg_connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/retry.py` & `procrastinate-2.3.0/procrastinate/retry.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/schema.py` & `procrastinate-2.3.0/procrastinate/schema.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/shell.py` & `procrastinate-2.3.0/procrastinate/shell.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/signals.py` & `procrastinate-2.3.0/procrastinate/signals.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/__init__.py` & `procrastinate-2.3.0/procrastinate/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/00.00.00_01_initial.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/00.00.00_01_initial.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/00.05.00_01_drop_started_at_column.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/00.05.00_01_drop_started_at_column.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/00.06.00_01_fix_procrastinate_fetch_job.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/00.06.00_01_fix_procrastinate_fetch_job.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/00.10.00_01_close_fetch_job_race_condition.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/00.10.00_01_close_fetch_job_race_condition.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/00.11.00_03_add_procrastinate_periodic_defers.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/00.11.00_03_add_procrastinate_periodic_defers.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/00.14.00_01_add_locks_to_periodic_defer.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/00.14.00_01_add_locks_to_periodic_defer.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/00.15.02_01_fix_procrastinate_defer_periodic_job.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/00.15.02_01_fix_procrastinate_defer_periodic_job.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/00.16.00_01_add_finish_job_and_retry_job_functions.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/00.16.00_01_add_finish_job_and_retry_job_functions.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/00.17.00_03_add_checks_to_finish_job.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/00.17.00_03_add_checks_to_finish_job.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/00.18.01_01_fix_finish_job_compat_issue.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/00.18.01_01_fix_finish_job_compat_issue.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/00.22.00_01_add_kwargs_to_defer_periodic_job.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/00.22.00_01_add_kwargs_to_defer_periodic_job.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/00.23.00_01_null_locks_excluded.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/00.23.00_01_null_locks_excluded.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/01.00.00_01_remove_old_finish_job_function.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/01.00.00_01_remove_old_finish_job_function.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/migrations/01.01.01_01_job_id_bigint.sql` & `procrastinate-2.3.0/procrastinate/sql/migrations/01.01.01_01_job_id_bigint.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/queries.sql` & `procrastinate-2.3.0/procrastinate/sql/queries.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sql/schema.sql` & `procrastinate-2.3.0/procrastinate/sql/schema.sql`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/sync_psycopg_connector.py` & `procrastinate-2.3.0/procrastinate/sync_psycopg_connector.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/tasks.py` & `procrastinate-2.3.0/procrastinate/tasks.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,53 +1,76 @@
 from __future__ import annotations
 
 import datetime
 import logging
-from typing import Any, Callable, cast
+from typing import Any, Callable, Generic, TypedDict, cast
+
+from typing_extensions import NotRequired, ParamSpec, Unpack
 
 from procrastinate import app as app_module
 from procrastinate import blueprints, exceptions, jobs, manager, types, utils
 from procrastinate import retry as retry_module
 
 logger = logging.getLogger(__name__)
 
 
+Args = ParamSpec("Args")
+P = ParamSpec("P")
+
+
+class TimeDeltaParams(TypedDict):
+    weeks: NotRequired[int]
+    days: NotRequired[int]
+    hours: NotRequired[int]
+    minutes: NotRequired[int]
+    seconds: NotRequired[int]
+    milliseconds: NotRequired[int]
+    microseconds: NotRequired[int]
+
+
+class ConfigureTaskOptions(TypedDict):
+    lock: NotRequired[str | None]
+    queueing_lock: NotRequired[str | None]
+    task_kwargs: NotRequired[types.JSONDict | None]
+    schedule_at: NotRequired[datetime.datetime | None]
+    schedule_in: NotRequired[TimeDeltaParams | None]
+    queue: NotRequired[str | None]
+
+
 def configure_task(
     *,
     name: str,
     job_manager: manager.JobManager,
-    lock: str | None = None,
-    queueing_lock: str | None = None,
-    task_kwargs: types.JSONDict | None = None,
-    schedule_at: datetime.datetime | None = None,
-    schedule_in: dict[str, int] | None = None,
-    queue: str = jobs.DEFAULT_QUEUE,
+    **options: Unpack[ConfigureTaskOptions],
 ) -> jobs.JobDeferrer:
+    schedule_at = options.get("schedule_at")
+    schedule_in = options.get("schedule_in")
+
     if schedule_at and schedule_in is not None:
         raise ValueError("Cannot set both schedule_at and schedule_in")
 
     if schedule_in is not None:
         schedule_at = utils.utcnow() + datetime.timedelta(**schedule_in)
 
-    task_kwargs = task_kwargs or {}
+    task_kwargs = options.get("task_kwargs") or {}
     return jobs.JobDeferrer(
         job=jobs.Job(
             id=None,
-            lock=lock,
-            queueing_lock=queueing_lock,
+            lock=options.get("lock"),
+            queueing_lock=options.get("queueing_lock"),
             task_name=name,
-            queue=queue,
+            queue=options.get("queue") or jobs.DEFAULT_QUEUE,
             task_kwargs=task_kwargs,
             scheduled_at=schedule_at,
         ),
         job_manager=job_manager,
     )
 
 
-class Task:
+class Task(Generic[P, Args]):
     """
     A task is a function that should be executed later. It is linked to a
     default queue, and expects keyword arguments.
 
     Attributes
     ----------
     name : ``str``
@@ -68,15 +91,15 @@
     queueing_lock : ``Optional[str]``
         Default queueing lock. The queuing lock can be overridden when a job is
         deferred.
     """
 
     def __init__(
         self,
-        func: Callable,
+        func: Callable[P],
         *,
         blueprint: blueprints.Blueprint,
         # task naming
         name: str | None = None,
         aliases: list[str] | None = None,
         # task specific settings
         retry: retry_module.RetryValue = False,
@@ -84,15 +107,15 @@
         # default defer arguments
         queue: str,
         lock: str | None = None,
         queueing_lock: str | None = None,
     ):
         self.queue = queue
         self.blueprint = blueprint
-        self.func: Callable = func
+        self.func: Callable[P] = func
         self.aliases = aliases if aliases else []
         self.retry_strategy = retry_module.get_retry_strategy(retry)
         self.name: str = name if name else self.full_path
         self.pass_context = pass_context
         self.lock = lock
         self.queueing_lock = queueing_lock
 
@@ -102,47 +125,38 @@
         """
         self.name = utils.add_namespace(name=self.name, namespace=namespace)
         self.aliases = [
             utils.add_namespace(name=alias, namespace=namespace)
             for alias in self.aliases
         ]
 
-    def __call__(self, *args, **kwargs: types.JSONValue) -> Any:
+    def __call__(self, *args: P.args, **kwargs: P.kwargs) -> Any:
         return self.func(*args, **kwargs)
 
     @property
     def full_path(self) -> str:
         return utils.get_full_path(self.func)
 
-    async def defer_async(self, **task_kwargs: types.JSONValue) -> int:
+    async def defer_async(self, *_: Args.args, **task_kwargs: Args.kwargs) -> int:
         """
         Create a job from this task and the given arguments.
         The job will be created with default parameters, if you want to better
         specify when and how to launch this job, see `Task.configure`.
         """
         return await self.configure().defer_async(**task_kwargs)
 
-    def defer(self, **task_kwargs: types.JSONValue) -> int:
+    def defer(self, *_: Args.args, **task_kwargs: Args.kwargs) -> int:
         """
         Create a job from this task and the given arguments.
         The job will be created with default parameters, if you want to better
         specify when and how to launch this job, see `Task.configure`.
         """
         return self.configure().defer(**task_kwargs)
 
-    def configure(
-        self,
-        *,
-        lock: str | None = None,
-        queueing_lock: str | None = None,
-        task_kwargs: types.JSONDict | None = None,
-        schedule_at: datetime.datetime | None = None,
-        schedule_in: dict[str, int] | None = None,
-        queue: str | None = None,
-    ) -> jobs.JobDeferrer:
+    def configure(self, **options: Unpack[ConfigureTaskOptions]) -> jobs.JobDeferrer:
         """
         Configure the job with all the specific settings, defining how the job
         should be launched.
 
         You should call the `defer` method (see `Task.defer`) on the resulting
         object, with the job task parameters.
 
@@ -177,16 +191,22 @@
         Raises
         ------
         ValueError
             If you try to define both schedule_at and schedule_in
         """
         self.blueprint.will_configure_task()
 
-        app = cast(app_module.App, self.blueprint)
+        lock = options.get("lock")
+        queueing_lock = options.get("queueing_lock")
+        task_kwargs = options.get("task_kwargs")
+        schedule_at = options.get("schedule_at")
+        schedule_in = options.get("schedule_in")
+        queue = options.get("queue")
 
+        app = cast(app_module.App, self.blueprint)
         return configure_task(
             name=self.name,
             job_manager=app.job_manager,
             lock=lock if lock is not None else self.lock,
             queueing_lock=(
                 queueing_lock if queueing_lock is not None else self.queueing_lock
             ),
```

### Comparing `procrastinate-2.2.0/procrastinate/testing.py` & `procrastinate-2.3.0/procrastinate/testing.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/utils.py` & `procrastinate-2.3.0/procrastinate/utils.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/procrastinate/worker.py` & `procrastinate-2.3.0/procrastinate/worker.py`

 * *Files identical despite different names*

### Comparing `procrastinate-2.2.0/pyproject.toml` & `procrastinate-2.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "procrastinate"
-version = "2.2.0"
+version = "2.3.0"
 description = "Postgres-based distributed task processing library"
 authors = ["Joachim Jablon", "Eric Lemoine"]
 license = "MIT License"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `procrastinate-2.2.0/PKG-INFO` & `procrastinate-2.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: procrastinate
-Version: 2.2.0
+Version: 2.3.0
 Summary: Postgres-based distributed task processing library
 Home-page: https://procrastinate.readthedocs.io/
 License: MIT
 Keywords: postgres,task-queue
 Author: Joachim Jablon
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

