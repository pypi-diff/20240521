# Comparing `tmp/piccolo-1.5.0.tar.gz` & `tmp/piccolo-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "piccolo-1.5.0.tar", last modified: Fri Mar 22 17:02:54 2024, max compression
+gzip compressed data, was "piccolo-1.5.1.tar", last modified: Tue May 21 11:18:46 2024, max compression
```

## Comparing `piccolo-1.5.0.tar` & `piccolo-1.5.1.tar`

### file list

```diff
@@ -1,454 +1,456 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.344185 piccolo-1.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-03-22 17:02:30.000000 piccolo-1.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-03-22 17:02:54.344185 piccolo-1.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-03-22 17:02:30.000000 piccolo-1.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.276185 piccolo-1.5.0/piccolo/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.276185 piccolo-1.5.0/piccolo/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.276185 piccolo-1.5.0/piccolo/apps/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.280185 piccolo-1.5.0/piccolo/apps/app/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/app/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/app/commands/new.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/app/commands/show_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.280185 piccolo-1.5.0/piccolo/apps/app/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/app/commands/templates/piccolo_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/app/commands/templates/tables.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/app/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.280185 piccolo-1.5.0/piccolo/apps/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.280185 piccolo-1.5.0/piccolo/apps/asgi/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.264185 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.280185 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/README.md.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/_esmerald_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/app.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/conftest.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.284185 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/__init__.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/_blacksheep_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/_esmerald_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/_starlette_endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/endpoints.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_app.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.284185 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/tables.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.284185 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/templates/base.html.jinja_raw
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/main.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/piccolo_conf_test.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/requirements.txt.jinja
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.284185 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/static/
--rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/static/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/asgi/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.284185 piccolo-1.5.0/piccolo/apps/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.284185 piccolo-1.5.0/piccolo/apps/fixtures/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/fixtures/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/fixtures/commands/dump.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/fixtures/commands/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/fixtures/commands/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/fixtures/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.284185 piccolo-1.5.0/piccolo/apps/meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.284185 piccolo-1.5.0/piccolo/apps/meta/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/meta/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/meta/commands/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/meta/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.284185 piccolo-1.5.0/piccolo/apps/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.288185 piccolo-1.5.0/piccolo/apps/migrations/auto/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/auto/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/auto/diffable_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    35096 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/auto/migration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/auto/operations.py
--rw-r--r--   0 runner    (1001) docker     (127)    26266 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/auto/schema_differ.py
--rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/auto/schema_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    23927 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/auto/serialisation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/auto/serialisation_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.288185 piccolo-1.5.0/piccolo/apps/migrations/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/commands/backwards.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/commands/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/commands/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/commands/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/commands/forwards.py
--rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.288185 piccolo-1.5.0/piccolo/apps/migrations/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/commands/templates/migration.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/piccolo_app.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/migrations/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.288185 piccolo-1.5.0/piccolo/apps/playground/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/playground/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.288185 piccolo-1.5.0/piccolo/apps/playground/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/playground/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/playground/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/playground/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.288185 piccolo-1.5.0/piccolo/apps/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.292185 piccolo-1.5.0/piccolo/apps/project/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/project/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/project/commands/new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.292185 piccolo-1.5.0/piccolo/apps/project/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/project/commands/templates/piccolo_conf.py.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/project/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.292185 piccolo-1.5.0/piccolo/apps/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.292185 piccolo-1.5.0/piccolo/apps/schema/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/schema/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/schema/commands/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30638 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/schema/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/schema/commands/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.292185 piccolo-1.5.0/piccolo/apps/schema/commands/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/schema/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.292185 piccolo-1.5.0/piccolo/apps/shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.292185 piccolo-1.5.0/piccolo/apps/shell/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/shell/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/shell/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.292185 piccolo-1.5.0/piccolo/apps/sql_shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/sql_shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.292185 piccolo-1.5.0/piccolo/apps/sql_shell/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/sql_shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/sql_shell/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/sql_shell/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.292185 piccolo-1.5.0/piccolo/apps/tester/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/tester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.292185 piccolo-1.5.0/piccolo/apps/tester/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/tester/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/tester/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/tester/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.296185 piccolo-1.5.0/piccolo/apps/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.296185 piccolo-1.5.0/piccolo/apps/user/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/user/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/user/commands/change_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/user/commands/change_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/user/commands/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/user/commands/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/user/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.296185 piccolo-1.5.0/piccolo/apps/user/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/user/piccolo_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/apps/user/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.296185 piccolo-1.5.0/piccolo/columns/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31620 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)    81013 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/column_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/combination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.300185 piccolo-1.5.0/piccolo/columns/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/defaults/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/defaults/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/defaults/date.py
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/defaults/interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/defaults/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/defaults/timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/defaults/timestamptz.py
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/defaults/uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/m2m.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.300185 piccolo-1.5.0/piccolo/columns/operators/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/operators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/operators/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/operators/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/operators/math.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/operators/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/readable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/columns/reference.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.300185 piccolo-1.5.0/piccolo/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/conf/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)      604 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/custom_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.300185 piccolo-1.5.0/piccolo/engine/
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/engine/cockroach.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/engine/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/engine/finder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18276 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/engine/postgres.py
--rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/engine/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/main.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.304185 piccolo-1.5.0/piccolo/query/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15397 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.304185 piccolo-1.5.0/piccolo/query/methods/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/alter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/create_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/drop_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/exists.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/insert.py
--rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/raw.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)    26883 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/table_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/methods/update.py
--rw-r--r--   0 runner    (1001) docker     (127)    21639 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/query/proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/querystring.py
--rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    50001 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/table_reflection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.308185 piccolo-1.5.0/piccolo/testing/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/testing/model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/testing/random_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.308185 piccolo-1.5.0/piccolo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/encoding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.308185 piccolo-1.5.0/piccolo/utils/graphlib/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/graphlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/graphlib/_graphlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/lazy_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/naming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/printing.py
--rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/sql_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-22 17:02:30.000000 piccolo-1.5.0/piccolo/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.340185 piccolo-1.5.0/piccolo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5093 2024-03-22 17:02:54.000000 piccolo-1.5.0/piccolo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13148 2024-03-22 17:02:54.000000 piccolo-1.5.0/piccolo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 17:02:54.000000 piccolo-1.5.0/piccolo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-22 17:02:54.000000 piccolo-1.5.0/piccolo.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-22 17:02:54.000000 piccolo-1.5.0/piccolo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-22 17:02:54.000000 piccolo-1.5.0/piccolo.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.308185 piccolo-1.5.0/profiling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/profiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-22 17:02:30.000000 piccolo-1.5.0/profiling/run_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-03-22 17:02:30.000000 piccolo-1.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 17:02:54.344185 piccolo-1.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-03-22 17:02:30.000000 piccolo-1.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.308185 piccolo-1.5.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.308185 piccolo-1.5.0/tests/apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.312185 piccolo-1.5.0/tests/apps/app/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.312185 piccolo-1.5.0/tests/apps/app/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/app/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/app/commands/test_new.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/app/commands/test_show_all.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.312185 piccolo-1.5.0/tests/apps/asgi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/asgi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.312185 piccolo-1.5.0/tests/apps/asgi/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/asgi/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/asgi/commands/test_new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.312185 piccolo-1.5.0/tests/apps/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.312185 piccolo-1.5.0/tests/apps/fixtures/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/fixtures/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/fixtures/commands/test_dump_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/fixtures/commands/test_shared.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.312185 piccolo-1.5.0/tests/apps/meta/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/meta/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.312185 piccolo-1.5.0/tests/apps/meta/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/meta/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/meta/commands/test_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.312185 piccolo-1.5.0/tests/apps/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.312185 piccolo-1.5.0/tests/apps/migrations/auto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/auto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.316185 piccolo-1.5.0/tests/apps/migrations/auto/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/auto/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46131 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/auto/integration/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/auto/test_diffable_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    34741 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/auto/test_migration_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/auto/test_schema_differ.py
--rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/auto/test_schema_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/auto/test_serialisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.316185 piccolo-1.5.0/tests/apps/migrations/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/commands/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/commands/test_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/commands/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/commands/test_forwards_backwards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.316185 piccolo-1.5.0/tests/apps/migrations/commands/test_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/commands/test_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/commands/test_new.py
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/migrations/test_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.316185 piccolo-1.5.0/tests/apps/project/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.316185 piccolo-1.5.0/tests/apps/project/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/project/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/project/commands/test_new.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.316185 piccolo-1.5.0/tests/apps/schema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.316185 piccolo-1.5.0/tests/apps/shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.316185 piccolo-1.5.0/tests/apps/shell/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/shell/commands/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.316185 piccolo-1.5.0/tests/apps/sql_shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/sql_shell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.316185 piccolo-1.5.0/tests/apps/sql_shell/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/sql_shell/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/sql_shell/commands/test_run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.316185 piccolo-1.5.0/tests/apps/tester/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/tester/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.316185 piccolo-1.5.0/tests/apps/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/user/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.320186 piccolo-1.5.0/tests/apps/user/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/user/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/user/commands/test_change_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/user/commands/test_change_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/user/commands/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/user/commands/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/apps/user/test_tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.324185 piccolo-1.5.0/tests/columns/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.324185 piccolo-1.5.0/tests/columns/m2m/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/m2m/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/m2m/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/m2m/test_m2m.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/m2m/test_m2m_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_bigint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_boolean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_bytea.py
--rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_combination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_db_column_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_double_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_jsonb.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_numeric.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_primary_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_real.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_reference.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_reserved_column_names.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_smallint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_timestamptz.py
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_uuid.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/columns/test_varchar.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.324185 piccolo-1.5.0/tests/conf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/conf/example.py
--rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/conf/test_apps.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.328185 piccolo-1.5.0/tests/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/engine/test_extra_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/engine/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/engine/test_nested_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/engine/test_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/engine/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/engine/test_version_parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.328185 piccolo-1.5.0/tests/example_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/example_apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.328185 piccolo-1.5.0/tests/example_apps/mega/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/example_apps/mega/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/example_apps/mega/piccolo_app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.328185 piccolo-1.5.0/tests/example_apps/mega/piccolo_migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/example_apps/mega/piccolo_migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/example_apps/mega/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.328185 piccolo-1.5.0/tests/example_apps/music/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/example_apps/music/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/example_apps/music/piccolo_app.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/example_apps/music/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/example_apps/music/tables_detailed.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.328185 piccolo-1.5.0/tests/query/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/query/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.328185 piccolo-1.5.0/tests/query/mixins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/query/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/query/mixins/test_columns_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/query/mixins/test_order_by_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/query/test_await.py
--rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/query/test_camelcase.py
--rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/query/test_freeze.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/query/test_gather.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/query/test_querystring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/query/test_slots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.336186 piccolo-1.5.0/tests/table/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.336186 piccolo-1.5.0/tests/table/instance/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/instance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/instance/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/instance/test_get_related.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/instance/test_get_related_readable.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/instance/test_instantiate.py
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/instance/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/instance/test_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/instance/test_to_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_all_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_constructor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_count.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_create_db_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_create_table_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_drop_db_tables.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_from_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_indexes.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_insert.py
--rw-r--r--   0 runner    (1001) docker     (127)    15910 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_join.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_join_on.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_metaclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_raw.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_refresh.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)    40607 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_str.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_table_exists.py
--rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/table/test_update.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/test_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.336186 piccolo-1.5.0/tests/testing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/testing/test_model_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/testing/test_random_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:54.340185 piccolo-1.5.0/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/utils/test_dictionary.py
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/utils/test_encoding.py
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/utils/test_lazy_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/utils/test_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/utils/test_naming.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/utils/test_printing.py
--rw-r--r--   0 runner    (1001) docker     (127)    26623 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/utils/test_pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/utils/test_sql_values.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/utils/test_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/utils/test_table_reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-03-22 17:02:30.000000 piccolo-1.5.0/tests/utils/test_warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.548570 piccolo-1.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-21 11:18:26.000000 piccolo-1.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-21 11:18:46.548570 piccolo-1.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-21 11:18:26.000000 piccolo-1.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.484570 piccolo-1.5.1/piccolo/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.484570 piccolo-1.5.1/piccolo/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.484570 piccolo-1.5.1/piccolo/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.484570 piccolo-1.5.1/piccolo/apps/app/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/app/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/app/commands/new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/app/commands/show_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.484570 piccolo-1.5.1/piccolo/apps/app/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/app/commands/templates/piccolo_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/app/commands/templates/tables.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/app/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.484570 piccolo-1.5.1/piccolo/apps/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.484570 piccolo-1.5.1/piccolo/apps/asgi/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.472570 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.488570 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/README.md.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2670 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/_esmerald_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/_lilya_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/app.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/conftest.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.488570 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/__init__.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/_blacksheep_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/_esmerald_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/_lilya_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/_starlette_endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/endpoints.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/piccolo_app.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.492570 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/tables.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.492570 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/templates/base.html.jinja_raw
+-rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/main.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/piccolo_conf.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/piccolo_conf_test.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/requirements.txt.jinja
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.492570 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     7406 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/static/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/asgi/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.492570 piccolo-1.5.1/piccolo/apps/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.492570 piccolo-1.5.1/piccolo/apps/fixtures/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/fixtures/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/fixtures/commands/dump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/fixtures/commands/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/fixtures/commands/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/fixtures/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.492570 piccolo-1.5.1/piccolo/apps/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.492570 piccolo-1.5.1/piccolo/apps/meta/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/meta/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/meta/commands/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/meta/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.492570 piccolo-1.5.1/piccolo/apps/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.496570 piccolo-1.5.1/piccolo/apps/migrations/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/auto/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7058 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/auto/diffable_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35096 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/auto/migration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/auto/operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26266 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/auto/schema_differ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/auto/schema_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23927 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/auto/serialisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/auto/serialisation_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.496570 piccolo-1.5.1/piccolo/apps/migrations/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/commands/backwards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/commands/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/commands/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/commands/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5374 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/commands/forwards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7892 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.496570 piccolo-1.5.1/piccolo/apps/migrations/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/commands/templates/migration.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/piccolo_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/migrations/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.496570 piccolo-1.5.1/piccolo/apps/playground/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/playground/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.496570 piccolo-1.5.1/piccolo/apps/playground/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/playground/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7351 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/playground/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/playground/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.496570 piccolo-1.5.1/piccolo/apps/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.496570 piccolo-1.5.1/piccolo/apps/project/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/project/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/project/commands/new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.496570 piccolo-1.5.1/piccolo/apps/project/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/project/commands/templates/piccolo_conf.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/project/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.500570 piccolo-1.5.1/piccolo/apps/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.500570 piccolo-1.5.1/piccolo/apps/schema/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/schema/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/schema/commands/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30638 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/schema/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/schema/commands/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.500570 piccolo-1.5.1/piccolo/apps/schema/commands/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/schema/commands/templates/graphviz.dot.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/schema/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.500570 piccolo-1.5.1/piccolo/apps/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.500570 piccolo-1.5.1/piccolo/apps/shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/shell/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/shell/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.500570 piccolo-1.5.1/piccolo/apps/sql_shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/sql_shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.500570 piccolo-1.5.1/piccolo/apps/sql_shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/sql_shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2060 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/sql_shell/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/sql_shell/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.500570 piccolo-1.5.1/piccolo/apps/tester/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.500570 piccolo-1.5.1/piccolo/apps/tester/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/tester/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/tester/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/tester/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.500570 piccolo-1.5.1/piccolo/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.504570 piccolo-1.5.1/piccolo/apps/user/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/user/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/user/commands/change_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/user/commands/change_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/user/commands/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/user/commands/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/user/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.504570 piccolo-1.5.1/piccolo/apps/user/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     2139 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/user/piccolo_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8954 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/apps/user/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.504570 piccolo-1.5.1/piccolo/columns/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31620 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81013 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/column_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6900 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/combination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.508570 piccolo-1.5.1/piccolo/columns/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/defaults/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/defaults/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/defaults/date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/defaults/interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/defaults/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/defaults/timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/defaults/timestamptz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/defaults/uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14365 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/m2m.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.508570 piccolo-1.5.1/piccolo/columns/operators/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/operators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/operators/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/operators/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/operators/math.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/operators/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3574 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/columns/reference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.508570 piccolo-1.5.1/piccolo/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18904 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/conf/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/custom_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.508570 piccolo-1.5.1/piccolo/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4881 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/engine/cockroach.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/engine/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/engine/finder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18276 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/engine/postgres.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/engine/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.508570 piccolo-1.5.1/piccolo/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15397 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.512570 piccolo-1.5.1/piccolo/query/methods/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16728 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2216 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/create_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/drop_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11705 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26883 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1259 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/table_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/methods/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21639 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/query/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5863 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/querystring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7731 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50001 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7094 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/table_reflection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.512570 piccolo-1.5.1/piccolo/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/testing/model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/testing/random_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.516570 piccolo-1.5.1/piccolo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/encoding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.516570 piccolo-1.5.1/piccolo/utils/graphlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/graphlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9677 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/graphlib/_graphlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/lazy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12328 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/sql_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-21 11:18:26.000000 piccolo-1.5.1/piccolo/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.548570 piccolo-1.5.1/piccolo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-05-21 11:18:46.000000 piccolo-1.5.1/piccolo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13281 2024-05-21 11:18:46.000000 piccolo-1.5.1/piccolo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:18:46.000000 piccolo-1.5.1/piccolo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 11:18:46.000000 piccolo-1.5.1/piccolo.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-21 11:18:46.000000 piccolo-1.5.1/piccolo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-21 11:18:46.000000 piccolo-1.5.1/piccolo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.516570 piccolo-1.5.1/profiling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/profiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-21 11:18:26.000000 piccolo-1.5.1/profiling/run_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-21 11:18:26.000000 piccolo-1.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:18:46.548570 piccolo-1.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-05-21 11:18:26.000000 piccolo-1.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.516570 piccolo-1.5.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.516570 piccolo-1.5.1/tests/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.516570 piccolo-1.5.1/tests/apps/app/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.516570 piccolo-1.5.1/tests/apps/app/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/app/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/app/commands/test_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/app/commands/test_show_all.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.520570 piccolo-1.5.1/tests/apps/asgi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/asgi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.520570 piccolo-1.5.1/tests/apps/asgi/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/asgi/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3097 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/asgi/commands/test_new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.520570 piccolo-1.5.1/tests/apps/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.520570 piccolo-1.5.1/tests/apps/fixtures/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/fixtures/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9205 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/fixtures/commands/test_dump_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/fixtures/commands/test_shared.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.520570 piccolo-1.5.1/tests/apps/meta/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/meta/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.520570 piccolo-1.5.1/tests/apps/meta/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/meta/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/meta/commands/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.520570 piccolo-1.5.1/tests/apps/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.520570 piccolo-1.5.1/tests/apps/migrations/auto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/auto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.520570 piccolo-1.5.1/tests/apps/migrations/auto/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/auto/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46131 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/auto/integration/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2932 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/auto/test_diffable_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34741 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/auto/test_migration_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19391 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/auto/test_schema_differ.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6196 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/auto/test_schema_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13548 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/auto/test_serialisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.524570 piccolo-1.5.1/tests/apps/migrations/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1829 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/commands/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/commands/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/commands/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7029 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/commands/test_forwards_backwards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.524570 piccolo-1.5.1/tests/apps/migrations/commands/test_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/commands/test_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4249 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/commands/test_new.py
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/migrations/test_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.524570 piccolo-1.5.1/tests/apps/project/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.524570 piccolo-1.5.1/tests/apps/project/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/project/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/project/commands/test_new.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.524570 piccolo-1.5.1/tests/apps/schema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.524570 piccolo-1.5.1/tests/apps/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.524570 piccolo-1.5.1/tests/apps/shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/shell/commands/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.524570 piccolo-1.5.1/tests/apps/sql_shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/sql_shell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.524570 piccolo-1.5.1/tests/apps/sql_shell/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/sql_shell/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/sql_shell/commands/test_run.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.524570 piccolo-1.5.1/tests/apps/tester/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/tester/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.524570 piccolo-1.5.1/tests/apps/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/user/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.528570 piccolo-1.5.1/tests/apps/user/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/user/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/user/commands/test_change_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/user/commands/test_change_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/user/commands/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2840 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/user/commands/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/apps/user/test_tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.532570 piccolo-1.5.1/tests/columns/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.532570 piccolo-1.5.1/tests/columns/m2m/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/m2m/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14563 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/m2m/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12647 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/m2m/test_m2m.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/m2m/test_m2m_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6660 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_bigint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1720 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_boolean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_bytea.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_combination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7670 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_db_column_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_double_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2993 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3920 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6914 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_jsonb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_primary_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_real.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_reserved_column_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_smallint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_timestamptz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/columns/test_varchar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.532570 piccolo-1.5.1/tests/conf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/conf/example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/conf/test_apps.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.532570 piccolo-1.5.1/tests/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/engine/test_extra_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/engine/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/engine/test_nested_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/engine/test_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9944 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/engine/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/engine/test_version_parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.536570 piccolo-1.5.1/tests/example_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/example_apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.536570 piccolo-1.5.1/tests/example_apps/mega/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/example_apps/mega/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/example_apps/mega/piccolo_app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.536570 piccolo-1.5.1/tests/example_apps/mega/piccolo_migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/example_apps/mega/piccolo_migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/example_apps/mega/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.536570 piccolo-1.5.1/tests/example_apps/music/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/example_apps/music/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/example_apps/music/piccolo_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/example_apps/music/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/example_apps/music/tables_detailed.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.536570 piccolo-1.5.1/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/query/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.536570 piccolo-1.5.1/tests/query/mixins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/query/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/query/mixins/test_columns_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/query/mixins/test_order_by_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/query/test_await.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/query/test_camelcase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3887 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/query/test_freeze.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/query/test_gather.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/query/test_querystring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/query/test_slots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.544571 piccolo-1.5.1/tests/table/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.544571 piccolo-1.5.1/tests/table/instance/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/instance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/instance/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/instance/test_get_related.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/instance/test_get_related_readable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/instance/test_instantiate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/instance/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4388 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/instance/test_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3442 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/instance/test_to_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_all_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3795 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_create_db_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_create_table_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_drop_db_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_from_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_indexes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13695 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15910 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_join.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_join_on.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_metaclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_raw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_refresh.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40607 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_str.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_table_exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20505 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/table/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5212 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.544571 piccolo-1.5.1/tests/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6206 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/testing/test_model_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/testing/test_random_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:46.548570 piccolo-1.5.1/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/utils/test_dictionary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/utils/test_encoding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/utils/test_lazy_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/utils/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/utils/test_naming.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/utils/test_printing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26623 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/utils/test_pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2535 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/utils/test_sql_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/utils/test_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/utils/test_table_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-21 11:18:26.000000 piccolo-1.5.1/tests/utils/test_warnings.py
```

### Comparing `piccolo-1.5.0/LICENSE` & `piccolo-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/PKG-INFO` & `piccolo-1.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piccolo
-Version: 1.5.0
+Version: 1.5.1
 Summary: A fast, user friendly ORM and query builder which supports asyncio.
 Home-page: https://github.com/piccolo-orm/piccolo
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Project-URL: Documentation, https://piccolo-orm.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/piccolo-orm/piccolo
@@ -140,15 +140,15 @@
 
 Let Piccolo scaffold you an ASGI web app, using Piccolo as the ORM:
 
 ```bash
 piccolo asgi new
 ```
 
-[Starlette](https://www.starlette.io/), [FastAPI](https://fastapi.tiangolo.com/), [BlackSheep](https://www.neoteroi.dev/blacksheep/), [Litestar](https://litestar.dev/) and [Esmerald](https://esmerald.dev/) are currently supported.
+[Starlette](https://www.starlette.io/), [FastAPI](https://fastapi.tiangolo.com/), [BlackSheep](https://www.neoteroi.dev/blacksheep/), [Litestar](https://litestar.dev/), [Esmerald](https://esmerald.dev/) and [Lilya](https://lilya.dev) are currently supported.
 
 ## Are you a Django user?
 
 We have a handy page which shows the equivalent of [common Django queries in Piccolo](https://piccolo-orm.readthedocs.io/en/latest/piccolo/query_types/django_comparison.html).
 
 ## Documentation
```

### Comparing `piccolo-1.5.0/README.md` & `piccolo-1.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
 Let Piccolo scaffold you an ASGI web app, using Piccolo as the ORM:
 
 ```bash
 piccolo asgi new
 ```
 
-[Starlette](https://www.starlette.io/), [FastAPI](https://fastapi.tiangolo.com/), [BlackSheep](https://www.neoteroi.dev/blacksheep/), [Litestar](https://litestar.dev/) and [Esmerald](https://esmerald.dev/) are currently supported.
+[Starlette](https://www.starlette.io/), [FastAPI](https://fastapi.tiangolo.com/), [BlackSheep](https://www.neoteroi.dev/blacksheep/), [Litestar](https://litestar.dev/), [Esmerald](https://esmerald.dev/) and [Lilya](https://lilya.dev) are currently supported.
 
 ## Are you a Django user?
 
 We have a handy page which shows the equivalent of [common Django queries in Piccolo](https://piccolo-orm.readthedocs.io/en/latest/piccolo/query_types/django_comparison.html).
 
 ## Documentation
```

### Comparing `piccolo-1.5.0/piccolo/apps/app/commands/new.py` & `piccolo-1.5.1/piccolo/apps/app/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/app/commands/templates/piccolo_app.py.jinja` & `piccolo-1.5.1/piccolo/apps/app/commands/templates/piccolo_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/asgi/commands/new.py` & `piccolo-1.5.1/piccolo/apps/asgi/commands/new.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 SERVERS = ["uvicorn", "Hypercorn"]
 ROUTER_DEPENDENCIES = {
     "starlette": ["starlette"],
     "fastapi": ["fastapi>=0.100.0"],
     "blacksheep": ["blacksheep"],
     "litestar": ["litestar"],
     "esmerald": ["esmerald"],
+    "lilya": ["lilya"],
 }
 ROUTERS = list(ROUTER_DEPENDENCIES.keys())
 
 
 def print_instruction(message: str):
     print(f"{colorama.Fore.CYAN}{message}{colorama.Fore.RESET}")
```

### Comparing `piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja` & `piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/_esmerald_app.py.jinja` & `piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/_esmerald_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja` & `piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja` & `piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja` & `piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja` & `piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw` & `piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/home/templates/home.html.jinja_raw`

 * *Files 6% similar despite different names*

```diff
@@ -57,10 +57,15 @@
                 <li><a href="/schema/swagger">Swagger API</a></li>
             </ul>
             <h3>Esmerald</h3>
             <ul>
                 <li><a href="/admin/">Admin</a></li>
                 <li><a href="/docs/swagger">Swagger API</a></li>
             </ul>
+            <h3>Lilya</h3>
+            <ul>
+                <li><a href="/admin/">Admin</a></li>
+                <li><a href="/tasks/">JSON endpoint</a></li>
+            </ul>
         </section>
     </div>
 {% endblock content %}
```

#### html2text {}

```diff
@@ -26,8 +26,11 @@
     * _S_w_a_g_g_e_r_ _A_P_I
 ******** LLiitteessttaarr ********
     * _A_d_m_i_n
     * _S_w_a_g_g_e_r_ _A_P_I
 ******** EEssmmeerraalldd ********
     * _A_d_m_i_n
     * _S_w_a_g_g_e_r_ _A_P_I
+******** LLiillyyaa ********
+    * _A_d_m_i_n
+    * _J_S_O_N_ _e_n_d_p_o_i_n_t
 {% endblock content %}
```

### Comparing `piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/static/favicon.ico` & `piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/asgi/commands/templates/app/static/main.css` & `piccolo-1.5.1/piccolo/apps/asgi/commands/templates/app/static/main.css`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/fixtures/commands/dump.py` & `piccolo-1.5.1/piccolo/apps/fixtures/commands/dump.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/fixtures/commands/load.py` & `piccolo-1.5.1/piccolo/apps/fixtures/commands/load.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/fixtures/commands/shared.py` & `piccolo-1.5.1/piccolo/apps/fixtures/commands/shared.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/auto/diffable_table.py` & `piccolo-1.5.1/piccolo/apps/migrations/auto/diffable_table.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/auto/migration_manager.py` & `piccolo-1.5.1/piccolo/apps/migrations/auto/migration_manager.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/auto/operations.py` & `piccolo-1.5.1/piccolo/apps/migrations/auto/operations.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/auto/schema_differ.py` & `piccolo-1.5.1/piccolo/apps/migrations/auto/schema_differ.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/auto/schema_snapshot.py` & `piccolo-1.5.1/piccolo/apps/migrations/auto/schema_snapshot.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/auto/serialisation.py` & `piccolo-1.5.1/piccolo/apps/migrations/auto/serialisation.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/auto/serialisation_legacy.py` & `piccolo-1.5.1/piccolo/apps/migrations/auto/serialisation_legacy.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/commands/backwards.py` & `piccolo-1.5.1/piccolo/apps/migrations/commands/backwards.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,17 +74,19 @@
 
         #######################################################################
 
         n = len(reversed_migration_ids)
         _continue = (
             "y"
             if self.auto_agree
-            else input(f"Reverse {n} migration{'s' if n != 1 else ''}? [y/N] ")
+            else input(
+                f"Reverse {n} migration{'s' if n != 1 else ''}? [y/N] "
+            ).lower()
         )
-        if _continue in "yY":
+        if _continue == "y":
             for migration_id in reversed_migration_ids:
                 migration_module = migration_modules[migration_id]
                 response = await migration_module.forwards()
 
                 if isinstance(response, MigrationManager):
                     if self.preview:
                         response.preview = True
@@ -127,18 +129,18 @@
             "y"
             if auto_agree
             else input(
                 "You are about to undo the migrations for the following "
                 "apps:\n"
                 f"{', '.join(names)}\n"
                 "Are you sure you want to continue? [y/N] "
-            )
+            ).lower()
         )
 
-        if _continue not in "yY":
+        if _continue != "y":
             return MigrationResult(success=False, message="user cancelled")
         for _app_name in sorted_app_names:
             print_heading(_app_name)
             manager = BackwardsMigrationManager(
                 app_name=_app_name,
                 migration_id="all",
                 auto_agree=auto_agree,
```

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/commands/base.py` & `piccolo-1.5.1/piccolo/apps/migrations/commands/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/commands/check.py` & `piccolo-1.5.1/piccolo/apps/migrations/commands/check.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/commands/clean.py` & `piccolo-1.5.1/piccolo/apps/migrations/commands/clean.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/commands/forwards.py` & `piccolo-1.5.1/piccolo/apps/migrations/commands/forwards.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/commands/new.py` & `piccolo-1.5.1/piccolo/apps/migrations/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/commands/templates/migration.py.jinja` & `piccolo-1.5.1/piccolo/apps/migrations/commands/templates/migration.py.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/piccolo_app.py` & `piccolo-1.5.1/piccolo/apps/migrations/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/migrations/tables.py` & `piccolo-1.5.1/piccolo/apps/migrations/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/playground/commands/run.py` & `piccolo-1.5.1/piccolo/apps/playground/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/project/commands/new.py` & `piccolo-1.5.1/piccolo/apps/project/commands/new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/schema/commands/generate.py` & `piccolo-1.5.1/piccolo/apps/schema/commands/generate.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/schema/commands/graph.py` & `piccolo-1.5.1/piccolo/apps/schema/commands/graph.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/schema/commands/templates/graphviz.dot.jinja` & `piccolo-1.5.1/piccolo/apps/schema/commands/templates/graphviz.dot.jinja`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/shell/commands/run.py` & `piccolo-1.5.1/piccolo/apps/shell/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/sql_shell/commands/run.py` & `piccolo-1.5.1/piccolo/apps/sql_shell/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/tester/commands/run.py` & `piccolo-1.5.1/piccolo/apps/tester/commands/run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/user/commands/change_password.py` & `piccolo-1.5.1/piccolo/apps/user/commands/change_password.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/user/commands/change_permissions.py` & `piccolo-1.5.1/piccolo/apps/user/commands/change_permissions.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/user/commands/create.py` & `piccolo-1.5.1/piccolo/apps/user/commands/create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/user/commands/list.py` & `piccolo-1.5.1/piccolo/apps/user/commands/list.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/user/piccolo_app.py` & `piccolo-1.5.1/piccolo/apps/user/piccolo_app.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py` & `piccolo-1.5.1/piccolo/apps/user/piccolo_migrations/2019-11-14T21-52-21.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py` & `piccolo-1.5.1/piccolo/apps/user/piccolo_migrations/2020-06-11T21-38-55.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py` & `piccolo-1.5.1/piccolo/apps/user/piccolo_migrations/2021-04-30T16-14-15.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/apps/user/tables.py` & `piccolo-1.5.1/piccolo/apps/user/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/__init__.py` & `piccolo-1.5.1/piccolo/columns/__init__.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/base.py` & `piccolo-1.5.1/piccolo/columns/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/choices.py` & `piccolo-1.5.1/piccolo/columns/choices.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/column_types.py` & `piccolo-1.5.1/piccolo/columns/column_types.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/combination.py` & `piccolo-1.5.1/piccolo/columns/combination.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/defaults/base.py` & `piccolo-1.5.1/piccolo/columns/defaults/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/defaults/date.py` & `piccolo-1.5.1/piccolo/columns/defaults/date.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/defaults/interval.py` & `piccolo-1.5.1/piccolo/columns/defaults/interval.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/defaults/time.py` & `piccolo-1.5.1/piccolo/columns/defaults/time.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/defaults/timestamp.py` & `piccolo-1.5.1/piccolo/columns/defaults/timestamp.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/defaults/timestamptz.py` & `piccolo-1.5.1/piccolo/columns/defaults/timestamptz.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/m2m.py` & `piccolo-1.5.1/piccolo/columns/m2m.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/operators/comparison.py` & `piccolo-1.5.1/piccolo/columns/operators/comparison.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/readable.py` & `piccolo-1.5.1/piccolo/columns/readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/columns/reference.py` & `piccolo-1.5.1/piccolo/columns/reference.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/conf/apps.py` & `piccolo-1.5.1/piccolo/conf/apps.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/custom_types.py` & `piccolo-1.5.1/piccolo/custom_types.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/engine/base.py` & `piccolo-1.5.1/piccolo/engine/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/engine/cockroach.py` & `piccolo-1.5.1/piccolo/engine/cockroach.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/engine/postgres.py` & `piccolo-1.5.1/piccolo/engine/postgres.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/engine/sqlite.py` & `piccolo-1.5.1/piccolo/engine/sqlite.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/main.py` & `piccolo-1.5.1/piccolo/main.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/__init__.py` & `piccolo-1.5.1/piccolo/query/__init__.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/base.py` & `piccolo-1.5.1/piccolo/query/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/alter.py` & `piccolo-1.5.1/piccolo/query/methods/alter.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/count.py` & `piccolo-1.5.1/piccolo/query/methods/count.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/create.py` & `piccolo-1.5.1/piccolo/query/methods/create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/create_index.py` & `piccolo-1.5.1/piccolo/query/methods/create_index.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/delete.py` & `piccolo-1.5.1/piccolo/query/methods/delete.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/drop_index.py` & `piccolo-1.5.1/piccolo/query/methods/drop_index.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/exists.py` & `piccolo-1.5.1/piccolo/query/methods/exists.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/indexes.py` & `piccolo-1.5.1/piccolo/query/methods/indexes.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/insert.py` & `piccolo-1.5.1/piccolo/query/methods/insert.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/objects.py` & `piccolo-1.5.1/piccolo/query/methods/objects.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/raw.py` & `piccolo-1.5.1/piccolo/query/methods/raw.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/refresh.py` & `piccolo-1.5.1/piccolo/query/methods/refresh.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/select.py` & `piccolo-1.5.1/piccolo/query/methods/select.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/table_exists.py` & `piccolo-1.5.1/piccolo/query/methods/table_exists.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/methods/update.py` & `piccolo-1.5.1/piccolo/query/methods/update.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/mixins.py` & `piccolo-1.5.1/piccolo/query/mixins.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/query/proxy.py` & `piccolo-1.5.1/piccolo/query/proxy.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/querystring.py` & `piccolo-1.5.1/piccolo/querystring.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/schema.py` & `piccolo-1.5.1/piccolo/schema.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/table.py` & `piccolo-1.5.1/piccolo/table.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/table_reflection.py` & `piccolo-1.5.1/piccolo/table_reflection.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/testing/model_builder.py` & `piccolo-1.5.1/piccolo/testing/model_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/testing/random_builder.py` & `piccolo-1.5.1/piccolo/testing/random_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/utils/dictionary.py` & `piccolo-1.5.1/piccolo/utils/dictionary.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/utils/encoding.py` & `piccolo-1.5.1/piccolo/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/utils/graphlib/_graphlib.py` & `piccolo-1.5.1/piccolo/utils/graphlib/_graphlib.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/utils/lazy_loader.py` & `piccolo-1.5.1/piccolo/utils/lazy_loader.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/utils/list.py` & `piccolo-1.5.1/piccolo/utils/list.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/utils/objects.py` & `piccolo-1.5.1/piccolo/utils/objects.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/utils/printing.py` & `piccolo-1.5.1/piccolo/utils/printing.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/utils/pydantic.py` & `piccolo-1.5.1/piccolo/utils/pydantic.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/utils/repr.py` & `piccolo-1.5.1/piccolo/utils/repr.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/utils/sql_values.py` & `piccolo-1.5.1/piccolo/utils/sql_values.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/utils/sync.py` & `piccolo-1.5.1/piccolo/utils/sync.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo/utils/warnings.py` & `piccolo-1.5.1/piccolo/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/piccolo.egg-info/PKG-INFO` & `piccolo-1.5.1/piccolo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: piccolo
-Version: 1.5.0
+Version: 1.5.1
 Summary: A fast, user friendly ORM and query builder which supports asyncio.
 Home-page: https://github.com/piccolo-orm/piccolo
 Author: Daniel Townsend
 Author-email: dan@dantownsend.co.uk
 License: MIT
 Project-URL: Documentation, https://piccolo-orm.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://github.com/piccolo-orm/piccolo
@@ -140,15 +140,15 @@
 
 Let Piccolo scaffold you an ASGI web app, using Piccolo as the ORM:
 
 ```bash
 piccolo asgi new
 ```
 
-[Starlette](https://www.starlette.io/), [FastAPI](https://fastapi.tiangolo.com/), [BlackSheep](https://www.neoteroi.dev/blacksheep/), [Litestar](https://litestar.dev/) and [Esmerald](https://esmerald.dev/) are currently supported.
+[Starlette](https://www.starlette.io/), [FastAPI](https://fastapi.tiangolo.com/), [BlackSheep](https://www.neoteroi.dev/blacksheep/), [Litestar](https://litestar.dev/), [Esmerald](https://esmerald.dev/) and [Lilya](https://lilya.dev) are currently supported.
 
 ## Are you a Django user?
 
 We have a handy page which shows the equivalent of [common Django queries in Piccolo](https://piccolo-orm.readthedocs.io/en/latest/piccolo/query_types/django_comparison.html).
 
 ## Documentation
```

### Comparing `piccolo-1.5.0/piccolo.egg-info/SOURCES.txt` & `piccolo-1.5.1/piccolo.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,25 +28,27 @@
 piccolo/apps/asgi/piccolo_app.py
 piccolo/apps/asgi/commands/__init__.py
 piccolo/apps/asgi/commands/new.py
 piccolo/apps/asgi/commands/templates/app/README.md.jinja
 piccolo/apps/asgi/commands/templates/app/_blacksheep_app.py.jinja
 piccolo/apps/asgi/commands/templates/app/_esmerald_app.py.jinja
 piccolo/apps/asgi/commands/templates/app/_fastapi_app.py.jinja
+piccolo/apps/asgi/commands/templates/app/_lilya_app.py.jinja
 piccolo/apps/asgi/commands/templates/app/_litestar_app.py.jinja
 piccolo/apps/asgi/commands/templates/app/_starlette_app.py.jinja
 piccolo/apps/asgi/commands/templates/app/app.py.jinja
 piccolo/apps/asgi/commands/templates/app/conftest.py.jinja
 piccolo/apps/asgi/commands/templates/app/main.py.jinja
 piccolo/apps/asgi/commands/templates/app/piccolo_conf.py.jinja
 piccolo/apps/asgi/commands/templates/app/piccolo_conf_test.py.jinja
 piccolo/apps/asgi/commands/templates/app/requirements.txt.jinja
 piccolo/apps/asgi/commands/templates/app/home/__init__.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/_blacksheep_endpoints.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/_esmerald_endpoints.py.jinja
+piccolo/apps/asgi/commands/templates/app/home/_lilya_endpoints.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/_litestar_endpoints.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/_starlette_endpoints.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/endpoints.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/piccolo_app.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/tables.py.jinja
 piccolo/apps/asgi/commands/templates/app/home/piccolo_migrations/README.md
 piccolo/apps/asgi/commands/templates/app/home/templates/base.html.jinja_raw
```

### Comparing `piccolo-1.5.0/profiling/run_profile.py` & `piccolo-1.5.1/profiling/run_profile.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/pyproject.toml` & `piccolo-1.5.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/setup.py` & `piccolo-1.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/app/commands/test_new.py` & `piccolo-1.5.1/tests/apps/app/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/app/commands/test_show_all.py` & `piccolo-1.5.1/tests/apps/app/commands/test_show_all.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/asgi/commands/test_new.py` & `piccolo-1.5.1/tests/apps/asgi/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/fixtures/commands/test_dump_load.py` & `piccolo-1.5.1/tests/apps/fixtures/commands/test_dump_load.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/fixtures/commands/test_shared.py` & `piccolo-1.5.1/tests/apps/fixtures/commands/test_shared.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/migrations/auto/integration/test_migrations.py` & `piccolo-1.5.1/tests/apps/migrations/auto/integration/test_migrations.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/migrations/auto/test_diffable_table.py` & `piccolo-1.5.1/tests/apps/migrations/auto/test_diffable_table.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/migrations/auto/test_migration_manager.py` & `piccolo-1.5.1/tests/apps/migrations/auto/test_migration_manager.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/migrations/auto/test_schema_differ.py` & `piccolo-1.5.1/tests/apps/migrations/auto/test_schema_differ.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/migrations/auto/test_schema_snapshot.py` & `piccolo-1.5.1/tests/apps/migrations/auto/test_schema_snapshot.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/migrations/auto/test_serialisation.py` & `piccolo-1.5.1/tests/apps/migrations/auto/test_serialisation.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/migrations/commands/test_base.py` & `piccolo-1.5.1/tests/apps/migrations/commands/test_base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/migrations/commands/test_check.py` & `piccolo-1.5.1/tests/apps/migrations/commands/test_check.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/migrations/commands/test_clean.py` & `piccolo-1.5.1/tests/apps/migrations/commands/test_clean.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/migrations/commands/test_forwards_backwards.py` & `piccolo-1.5.1/tests/apps/migrations/commands/test_forwards_backwards.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py` & `piccolo-1.5.1/tests/apps/migrations/commands/test_migrations/2020-03-31T20-38-22.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/migrations/commands/test_new.py` & `piccolo-1.5.1/tests/apps/migrations/commands/test_new.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/shell/commands/test_run.py` & `piccolo-1.5.1/tests/apps/shell/commands/test_run.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/user/commands/test_change_password.py` & `piccolo-1.5.1/tests/apps/user/commands/test_change_password.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/user/commands/test_change_permissions.py` & `piccolo-1.5.1/tests/apps/user/commands/test_change_permissions.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/user/commands/test_create.py` & `piccolo-1.5.1/tests/apps/user/commands/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/user/commands/test_list.py` & `piccolo-1.5.1/tests/apps/user/commands/test_list.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/apps/user/test_tables.py` & `piccolo-1.5.1/tests/apps/user/test_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/m2m/base.py` & `piccolo-1.5.1/tests/columns/m2m/base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/m2m/test_m2m.py` & `piccolo-1.5.1/tests/columns/m2m/test_m2m.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_array.py` & `piccolo-1.5.1/tests/columns/test_array.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,14 @@
         """
         self.assertEqual(Array(Integer())._get_dimensions(), 1)
         self.assertEqual(Array(Array(Integer()))._get_dimensions(), 2)
         self.assertEqual(Array(Array(Array(Integer())))._get_dimensions(), 3)
 
 
 class TestGetInnerValueType(TestCase):
-
     def test_get_inner_value_type(self):
         """
         Make sure that `_get_inner_value_type` returns the correct base type.
         """
         self.assertEqual(Array(Integer())._get_inner_value_type(), int)
         self.assertEqual(Array(Array(Integer()))._get_inner_value_type(), int)
         self.assertEqual(
```

### Comparing `piccolo-1.5.0/tests/columns/test_base.py` & `piccolo-1.5.1/tests/columns/test_base.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_bigint.py` & `piccolo-1.5.1/tests/columns/test_bigint.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_boolean.py` & `piccolo-1.5.1/tests/columns/test_boolean.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_bytea.py` & `piccolo-1.5.1/tests/columns/test_bytea.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_choices.py` & `piccolo-1.5.1/tests/columns/test_choices.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_combination.py` & `piccolo-1.5.1/tests/columns/test_combination.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_date.py` & `piccolo-1.5.1/tests/columns/test_date.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_db_column_name.py` & `piccolo-1.5.1/tests/columns/test_db_column_name.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_defaults.py` & `piccolo-1.5.1/tests/columns/test_defaults.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_double_precision.py` & `piccolo-1.5.1/tests/columns/test_double_precision.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_interval.py` & `piccolo-1.5.1/tests/columns/test_interval.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_json.py` & `piccolo-1.5.1/tests/columns/test_json.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_jsonb.py` & `piccolo-1.5.1/tests/columns/test_jsonb.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_numeric.py` & `piccolo-1.5.1/tests/columns/test_numeric.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_primary_key.py` & `piccolo-1.5.1/tests/columns/test_primary_key.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_readable.py` & `piccolo-1.5.1/tests/columns/test_readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_real.py` & `piccolo-1.5.1/tests/columns/test_real.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_reference.py` & `piccolo-1.5.1/tests/columns/test_reference.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_reserved_column_names.py` & `piccolo-1.5.1/tests/columns/test_reserved_column_names.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_smallint.py` & `piccolo-1.5.1/tests/columns/test_smallint.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_time.py` & `piccolo-1.5.1/tests/columns/test_time.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_timestamp.py` & `piccolo-1.5.1/tests/columns/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_timestamptz.py` & `piccolo-1.5.1/tests/columns/test_timestamptz.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/columns/test_varchar.py` & `piccolo-1.5.1/tests/columns/test_varchar.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/conf/test_apps.py` & `piccolo-1.5.1/tests/conf/test_apps.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/engine/test_extra_nodes.py` & `piccolo-1.5.1/tests/engine/test_extra_nodes.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/engine/test_logging.py` & `piccolo-1.5.1/tests/engine/test_logging.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/engine/test_nested_transaction.py` & `piccolo-1.5.1/tests/engine/test_nested_transaction.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/engine/test_pool.py` & `piccolo-1.5.1/tests/engine/test_pool.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/engine/test_transaction.py` & `piccolo-1.5.1/tests/engine/test_transaction.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/engine/test_version_parsing.py` & `piccolo-1.5.1/tests/engine/test_version_parsing.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py` & `piccolo-1.5.1/tests/example_apps/mega/piccolo_migrations/2021-09-20T21-23-25-698988.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/example_apps/mega/tables.py` & `piccolo-1.5.1/tests/example_apps/mega/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/example_apps/music/tables.py` & `piccolo-1.5.1/tests/example_apps/music/tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/example_apps/music/tables_detailed.py` & `piccolo-1.5.1/tests/example_apps/music/tables_detailed.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/query/mixins/test_columns_delegate.py` & `piccolo-1.5.1/tests/query/mixins/test_columns_delegate.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/query/test_camelcase.py` & `piccolo-1.5.1/tests/query/test_camelcase.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/query/test_freeze.py` & `piccolo-1.5.1/tests/query/test_freeze.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/query/test_gather.py` & `piccolo-1.5.1/tests/query/test_gather.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/query/test_querystring.py` & `piccolo-1.5.1/tests/query/test_querystring.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/query/test_slots.py` & `piccolo-1.5.1/tests/query/test_slots.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/instance/test_create.py` & `piccolo-1.5.1/tests/table/instance/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/instance/test_get_related.py` & `piccolo-1.5.1/tests/table/instance/test_get_related.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/instance/test_get_related_readable.py` & `piccolo-1.5.1/tests/table/instance/test_get_related_readable.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/instance/test_instantiate.py` & `piccolo-1.5.1/tests/table/instance/test_instantiate.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/instance/test_remove.py` & `piccolo-1.5.1/tests/table/instance/test_remove.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/instance/test_save.py` & `piccolo-1.5.1/tests/table/instance/test_save.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/instance/test_to_dict.py` & `piccolo-1.5.1/tests/table/instance/test_to_dict.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_all_columns.py` & `piccolo-1.5.1/tests/table/test_all_columns.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_alter.py` & `piccolo-1.5.1/tests/table/test_alter.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_batch.py` & `piccolo-1.5.1/tests/table/test_batch.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_callback.py` & `piccolo-1.5.1/tests/table/test_callback.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_constructor.py` & `piccolo-1.5.1/tests/table/test_constructor.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_count.py` & `piccolo-1.5.1/tests/table/test_count.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_create.py` & `piccolo-1.5.1/tests/table/test_create.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_create_db_tables.py` & `piccolo-1.5.1/tests/table/test_create_db_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_create_table_class.py` & `piccolo-1.5.1/tests/table/test_create_table_class.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_delete.py` & `piccolo-1.5.1/tests/table/test_delete.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_drop_db_tables.py` & `piccolo-1.5.1/tests/table/test_drop_db_tables.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_from_dict.py` & `piccolo-1.5.1/tests/table/test_from_dict.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_indexes.py` & `piccolo-1.5.1/tests/table/test_indexes.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_inheritance.py` & `piccolo-1.5.1/tests/table/test_inheritance.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_insert.py` & `piccolo-1.5.1/tests/table/test_insert.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_join.py` & `piccolo-1.5.1/tests/table/test_join.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_join_on.py` & `piccolo-1.5.1/tests/table/test_join_on.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_metaclass.py` & `piccolo-1.5.1/tests/table/test_metaclass.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_objects.py` & `piccolo-1.5.1/tests/table/test_objects.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_output.py` & `piccolo-1.5.1/tests/table/test_output.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_raw.py` & `piccolo-1.5.1/tests/table/test_raw.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_refresh.py` & `piccolo-1.5.1/tests/table/test_refresh.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_select.py` & `piccolo-1.5.1/tests/table/test_select.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_str.py` & `piccolo-1.5.1/tests/table/test_str.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_table_exists.py` & `piccolo-1.5.1/tests/table/test_table_exists.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/table/test_update.py` & `piccolo-1.5.1/tests/table/test_update.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/test_schema.py` & `piccolo-1.5.1/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/testing/test_model_builder.py` & `piccolo-1.5.1/tests/testing/test_model_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/testing/test_random_builder.py` & `piccolo-1.5.1/tests/testing/test_random_builder.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/utils/test_dictionary.py` & `piccolo-1.5.1/tests/utils/test_dictionary.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/utils/test_lazy_loader.py` & `piccolo-1.5.1/tests/utils/test_lazy_loader.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/utils/test_list.py` & `piccolo-1.5.1/tests/utils/test_list.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/utils/test_naming.py` & `piccolo-1.5.1/tests/utils/test_naming.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/utils/test_printing.py` & `piccolo-1.5.1/tests/utils/test_printing.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/utils/test_pydantic.py` & `piccolo-1.5.1/tests/utils/test_pydantic.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/utils/test_sql_values.py` & `piccolo-1.5.1/tests/utils/test_sql_values.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/utils/test_sync.py` & `piccolo-1.5.1/tests/utils/test_sync.py`

 * *Files identical despite different names*

### Comparing `piccolo-1.5.0/tests/utils/test_table_reflection.py` & `piccolo-1.5.1/tests/utils/test_table_reflection.py`

 * *Files identical despite different names*
