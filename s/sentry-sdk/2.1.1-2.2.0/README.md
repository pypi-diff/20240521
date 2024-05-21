# Comparing `tmp/sentry_sdk-2.1.1.tar.gz` & `tmp/sentry_sdk-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sentry_sdk-2.1.1.tar", last modified: Mon May  6 11:53:20 2024, max compression
+gzip compressed data, was "sentry_sdk-2.2.0.tar", last modified: Thu May 16 08:34:55 2024, max compression
```

## Comparing `sentry_sdk-2.1.1.tar` & `sentry_sdk-2.2.0.tar`

### file list

```diff
@@ -1,172 +1,173 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.474496 sentry_sdk-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-06 11:53:20.474496 sentry_sdk-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.446497 sentry_sdk-2.1.1/sentry_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     6653 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/_werkzeug.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.450497 sentry_sdk-2.1.1/sentry_sdk/ai/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2742 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/ai/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/ai/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/attachments.py
--rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14185 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.450497 sentry_sdk-2.1.1/sentry_sdk/crons/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/crons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/crons/api.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/crons/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/crons/decorator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.450497 sentry_sdk-2.1.1/sentry_sdk/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/db/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.450497 sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/django.py
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/hub.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/
--rw-r--r--   0 runner    (1001) docker     (127)     7676 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/_asgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/_wsgi_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/argv.py
--rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/ariadne.py
--rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/arq.py
--rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/asyncpg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/atexit.py
--rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/aws_lambda.py
--rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/beam.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/boto3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/bottle.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/celery/
--rw-r--r--   0 runner    (1001) docker     (127)    13542 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/celery/beat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/celery/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/chalice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/clickhouse_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/cloud_resource_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/django/
--rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/asgi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/caching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/middleware.py
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/signals_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/django/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/excepthook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/executing.py
--rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/falcon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/gcp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/gnu_backtrace.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/gql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/graphene.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/aio/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/aio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/aio/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/httpx.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/huey.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/huggingface_hub.py
--rw-r--r--   0 runner    (1001) docker     (127)    17406 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/langchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/loguru.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/openai.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/propagator.py
--rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/span_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/pure_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/pymongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/pyramid.py
--rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/quart.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.462496 sentry_sdk-2.1.1/sentry_sdk/integrations/redis/
--rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/redis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/redis/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/rq.py
--rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/sanic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/serverless.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.466496 sentry_sdk-2.1.1/sentry_sdk/integrations/spark/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/spark/spark_driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/spark/spark_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (127)    23511 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/starlette.py
--rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/starlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/stdlib.py
--rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/strawberry.py
--rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/threading.py
--rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/tornado.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/trytond.py
--rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/integrations/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (127)    29725 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    56641 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    39120 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/tracing.py
--rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/tracing_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21002 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    56591 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/sentry_sdk/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.470496 sentry_sdk-2.1.1/sentry_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-06 11:53:20.000000 sentry_sdk-2.1.1/sentry_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4873 2024-05-06 11:53:20.000000 sentry_sdk-2.1.1/sentry_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:53:20.000000 sentry_sdk-2.1.1/sentry_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 11:53:20.000000 sentry_sdk-2.1.1/sentry_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-06 11:53:20.000000 sentry_sdk-2.1.1/sentry_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-06 11:53:20.000000 sentry_sdk-2.1.1/sentry_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-06 11:53:20.474496 sentry_sdk-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 11:53:20.466496 sentry_sdk-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    23225 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_basics.py
--rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_crons.py
--rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_envelope.py
--rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_exceptiongroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_lru_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    29128 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_new_scopes_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_new_scopes_compat_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_propagationcontext.py
--rw-r--r--   0 runner    (1001) docker     (127)    26432 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_scrubber.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_sessions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_spotlight.py
--rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-05-06 11:53:12.000000 sentry_sdk-2.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:55.001584 sentry_sdk-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-16 08:34:55.001584 sentry_sdk-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5325 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.973584 sentry_sdk-2.2.0/sentry_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5382 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11259 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6701 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3745 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/_werkzeug.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.973584 sentry_sdk-2.2.0/sentry_sdk/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/ai/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/ai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10018 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/attachments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29194 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15717 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.973584 sentry_sdk-2.2.0/sentry_sdk/crons/
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/crons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/crons/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/crons/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/crons/decorator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.977584 sentry_sdk-2.2.0/sentry_sdk/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/db/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.977584 sentry_sdk-2.2.0/sentry_sdk/db/explain_plan/
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/db/explain_plan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/db/explain_plan/django.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/db/explain_plan/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9923 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27085 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/hub.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.985584 sentry_sdk-2.2.0/sentry_sdk/integrations/
+-rw-r--r--   0 runner    (1001) docker     (127)     7794 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/_asgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/_wsgi_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6446 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/argv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/ariadne.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7200 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/arq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11600 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6180 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/asyncpg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/atexit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/aws_lambda.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5192 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/beam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/boto3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/bottle.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.985584 sentry_sdk-2.2.0/sentry_sdk/integrations/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)    15107 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9813 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/celery/beat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1238 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/celery/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4721 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/chalice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5064 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/clickhouse_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6755 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/cloud_resource_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/cohere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.985584 sentry_sdk-2.2.0/sentry_sdk/integrations/django/
+-rw-r--r--   0 runner    (1001) docker     (127)    23519 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7691 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/django/asgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3622 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/django/caching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5770 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/django/middleware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/django/signals_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5683 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/django/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/django/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/django/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/excepthook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/executing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9347 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/falcon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8149 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/gnu_backtrace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/gql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3636 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/graphene.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.989584 sentry_sdk-2.2.0/sentry_sdk/integrations/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)     4979 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/grpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.989584 sentry_sdk-2.2.0/sentry_sdk/integrations/grpc/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/grpc/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/grpc/aio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/grpc/aio/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3249 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/grpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/grpc/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/huey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/huggingface_hub.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17445 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/langchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9592 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/loguru.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/openai.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.989584 sentry_sdk-2.2.0/sentry_sdk/integrations/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/opentelemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/opentelemetry/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/opentelemetry/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3731 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/opentelemetry/propagator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12225 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/opentelemetry/span_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/pure_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/pymongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7151 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/pyramid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/quart.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.989584 sentry_sdk-2.2.0/sentry_sdk/integrations/redis/
+-rw-r--r--   0 runner    (1001) docker     (127)    11834 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/redis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/redis/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5297 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/rq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13164 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/sanic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/serverless.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.989584 sentry_sdk-2.2.0/sentry_sdk/integrations/spark/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8276 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/spark/spark_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3747 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/spark/spark_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23511 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/starlette.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9871 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/starlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14566 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/strawberry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4033 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/threading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7185 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/tornado.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/trytond.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9870 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/integrations/wsgi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29729 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33332 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    57822 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12729 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39492 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21048 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/tracing_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21002 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56591 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/sentry_sdk/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.993584 sentry_sdk-2.2.0/sentry_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10123 2024-05-16 08:34:54.000000 sentry_sdk-2.2.0/sentry_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-16 08:34:54.000000 sentry_sdk-2.2.0/sentry_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:34:54.000000 sentry_sdk-2.2.0/sentry_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 08:34:54.000000 sentry_sdk-2.2.0/sentry_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-16 08:34:54.000000 sentry_sdk-2.2.0/sentry_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 08:34:54.000000 sentry_sdk-2.2.0/sentry_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 08:34:55.001584 sentry_sdk-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 08:34:54.993584 sentry_sdk-2.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4975 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23697 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_basics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36053 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13795 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_crons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8057 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_envelope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8578 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_exceptiongroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_lru_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29128 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8686 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_new_scopes_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17288 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_new_scopes_compat_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23653 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_propagationcontext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26931 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_scrubber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4098 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_spotlight.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18754 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26384 2024-05-16 08:34:45.000000 sentry_sdk-2.2.0/tests/test_utils.py
```

### Comparing `sentry_sdk-2.1.1/LICENSE` & `sentry_sdk-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/PKG-INFO` & `sentry_sdk-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.1.1
+Version: 2.2.0
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

### Comparing `sentry_sdk-2.1.1/README.md` & `sentry_sdk-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/__init__.py` & `sentry_sdk-2.2.0/sentry_sdk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "flush",
     "get_baggage",
     "get_client",
     "get_current_span",
     "get_traceparent",
     "is_initialized",
     "isolation_scope",
+    "last_event_id",
     "new_scope",
     "push_scope",
     "set_context",
     "set_extra",
     "set_level",
     "set_measurement",
     "set_tag",
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk/_compat.py` & `sentry_sdk-2.2.0/sentry_sdk/_compat.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/_lru_cache.py` & `sentry_sdk-2.2.0/sentry_sdk/_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/_queue.py` & `sentry_sdk-2.2.0/sentry_sdk/_queue.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/_types.py` & `sentry_sdk-2.2.0/sentry_sdk/_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 
     from types import TracebackType
     from typing import Any
     from typing import Callable
     from typing import Dict
     from typing import List
     from typing import Mapping
+    from typing import NotRequired
     from typing import Optional
     from typing import Tuple
     from typing import Type
     from typing import Union
     from typing_extensions import Literal, TypedDict
 
     # "critical" is an alias of "fatal" recognized by Relay
@@ -59,15 +60,15 @@
     FractionUnit = Literal["ratio", "percent"]
     MeasurementUnit = Union[DurationUnit, InformationUnit, FractionUnit, str]
 
     MeasurementValue = TypedDict(
         "MeasurementValue",
         {
             "value": float,
-            "unit": Optional[MeasurementUnit],
+            "unit": NotRequired[Optional[MeasurementUnit]],
         },
     )
 
     Event = TypedDict(
         "Event",
         {
             "breadcrumbs": dict[
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk/_werkzeug.py` & `sentry_sdk-2.2.0/sentry_sdk/_werkzeug.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/ai/monitoring.py` & `sentry_sdk-2.2.0/sentry_sdk/ai/monitoring.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,15 +27,20 @@
     def decorator(f):
         # type: (Callable[..., Any]) -> Callable[..., Any]
         @wraps(f)
         def wrapped(*args, **kwargs):
             # type: (Any, Any) -> Any
             curr_pipeline = _ai_pipeline_name.get()
             op = span_kwargs.get("op", "ai.run" if curr_pipeline else "ai.pipeline")
+
             with start_span(description=description, op=op, **span_kwargs) as span:
+                for k, v in kwargs.pop("sentry_tags", {}).items():
+                    span.set_tag(k, v)
+                for k, v in kwargs.pop("sentry_data", {}).items():
+                    span.set_data(k, v)
                 if curr_pipeline:
                     span.set_data("ai.pipeline.name", curr_pipeline)
                     return f(*args, **kwargs)
                 else:
                     _ai_pipeline_name.set(description)
                     try:
                         res = f(*args, **kwargs)
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk/ai/utils.py` & `sentry_sdk-2.2.0/sentry_sdk/ai/utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/api.py` & `sentry_sdk-2.2.0/sentry_sdk/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,15 @@
     "flush",
     "get_baggage",
     "get_client",
     "get_current_span",
     "get_traceparent",
     "is_initialized",
     "isolation_scope",
+    "last_event_id",
     "new_scope",
     "push_scope",
     "set_context",
     "set_extra",
     "set_level",
     "set_measurement",
     "set_tag",
@@ -328,14 +329,24 @@
         available arguments.
     """
     return Scope.get_current_scope().start_transaction(
         transaction, instrumenter, custom_sampling_context, **kwargs
     )
 
 
+@scopemethod
+def last_event_id():
+    # type: () -> Optional[str]
+    """
+    See :py:meth:`sentry_sdk.Scope.last_event_id` documentation regarding
+    this method's limitations.
+    """
+    return Scope.last_event_id()
+
+
 def set_measurement(name, value, unit=""):
     # type: (str, float, MeasurementUnit) -> None
     transaction = Scope.get_current_scope().transaction
     if transaction is not None:
         transaction.set_measurement(name, value, unit)
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk/attachments.py` & `sentry_sdk-2.2.0/sentry_sdk/attachments.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/client.py` & `sentry_sdk-2.2.0/sentry_sdk/client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/consts.py` & `sentry_sdk-2.2.0/sentry_sdk/consts.py`

 * *Files 4% similar despite different names*

```diff
@@ -87,14 +87,26 @@
 
 class SPANDATA:
     """
     Additional information describing the type of the span.
     See: https://develop.sentry.dev/sdk/performance/span-data-conventions/
     """
 
+    AI_FREQUENCY_PENALTY = "ai.frequency_penalty"
+    """
+    Used to reduce repetitiveness of generated tokens.
+    Example: 0.5
+    """
+
+    AI_PRESENCE_PENALTY = "ai.presence_penalty"
+    """
+    Used to reduce repetitiveness of generated tokens.
+    Example: 0.5
+    """
+
     AI_INPUT_MESSAGES = "ai.input_messages"
     """
     The input messages to an LLM call.
     Example: [{"role": "user", "message": "hello"}]
     """
 
     AI_MODEL_ID = "ai.model_id"
@@ -160,20 +172,39 @@
     """
 
     AI_LOGIT_BIAS = "ai.response_format"
     """
     For an AI model call, the logit bias
     """
 
+    AI_PREAMBLE = "ai.preamble"
+    """
+    For an AI model call, the preamble parameter.
+    Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style.
+    Example: "You are now a clown."
+    """
+
+    AI_RAW_PROMPTING = "ai.raw_prompting"
+    """
+    Minimize pre-processing done to the prompt sent to the LLM.
+    Example: true
+    """
+
     AI_RESPONSES = "ai.responses"
     """
     The responses to an AI model call. Always as a list.
     Example: ["hello", "world"]
     """
 
+    AI_SEED = "ai.seed"
+    """
+    The seed, ideally models given the same seed and same other parameters will produce the exact same output.
+    Example: 123.45
+    """
+
     DB_NAME = "db.name"
     """
     The name of the database being accessed. For commands that switch the database, this should be set to the target database (even if the command fails).
     Example: myDatabase
     """
 
     DB_USER = "db.user"
@@ -229,14 +260,35 @@
 
     HTTP_STATUS_CODE = "http.response.status_code"
     """
     The HTTP status code as an integer.
     Example: 418
     """
 
+    MESSAGING_DESTINATION_NAME = "messaging.destination.name"
+    """
+    The destination name where the message is being consumed from,
+    e.g. the queue name or topic.
+    """
+
+    MESSAGING_MESSAGE_ID = "messaging.message.id"
+    """
+    The message's identifier.
+    """
+
+    MESSAGING_MESSAGE_RETRY_COUNT = "messaging.message.retry.count"
+    """
+    Number of retries/attempts to process a message.
+    """
+
+    MESSAGING_SYSTEM = "messaging.system"
+    """
+    The messaging system's name, e.g. `kafka`, `aws_sqs`
+    """
+
     SERVER_ADDRESS = "server.address"
     """
     Name of the database host.
     Example: example.com
     """
 
     SERVER_PORT = "server.port"
@@ -294,14 +346,16 @@
     Example: "MainThread"
     """
 
 
 class OP:
     ANTHROPIC_MESSAGES_CREATE = "ai.messages.create.anthropic"
     CACHE_GET_ITEM = "cache.get_item"
+    COHERE_CHAT_COMPLETIONS_CREATE = "ai.chat_completions.create.cohere"
+    COHERE_EMBEDDINGS_CREATE = "ai.embeddings.create.cohere"
     DB = "db"
     DB_REDIS = "db.redis"
     EVENT_DJANGO = "event.django"
     FUNCTION = "function"
     FUNCTION_AWS = "function.aws"
     FUNCTION_GCP = "function.gcp"
     GRAPHQL_EXECUTE = "graphql.execute"
@@ -329,14 +383,15 @@
         "ai.chat_completions.create.huggingface_hub"
     )
     LANGCHAIN_PIPELINE = "ai.pipeline.langchain"
     LANGCHAIN_RUN = "ai.run.langchain"
     LANGCHAIN_TOOL = "ai.tool.langchain"
     LANGCHAIN_AGENT = "ai.agent.langchain"
     LANGCHAIN_CHAT_COMPLETIONS_CREATE = "ai.chat_completions.create.langchain"
+    QUEUE_PROCESS = "queue.process"
     QUEUE_SUBMIT_ARQ = "queue.submit.arq"
     QUEUE_TASK_ARQ = "queue.task.arq"
     QUEUE_SUBMIT_CELERY = "queue.submit.celery"
     QUEUE_TASK_CELERY = "queue.task.celery"
     QUEUE_TASK_RQ = "queue.task.rq"
     QUEUE_SUBMIT_HUEY = "queue.submit.huey"
     QUEUE_TASK_HUEY = "queue.task.huey"
@@ -429,8 +484,8 @@
     return dict(zip(a.args[-len(defaults) :], defaults))
 
 
 DEFAULT_OPTIONS = _get_default_options()
 del _get_default_options
 
 
-VERSION = "2.1.1"
+VERSION = "2.2.0"
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk/crons/api.py` & `sentry_sdk-2.2.0/sentry_sdk/crons/api.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/crons/decorator.py` & `sentry_sdk-2.2.0/sentry_sdk/crons/decorator.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/__init__.py` & `sentry_sdk-2.2.0/sentry_sdk/db/explain_plan/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/django.py` & `sentry_sdk-2.2.0/sentry_sdk/db/explain_plan/django.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/db/explain_plan/sqlalchemy.py` & `sentry_sdk-2.2.0/sentry_sdk/db/explain_plan/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/debug.py` & `sentry_sdk-2.2.0/sentry_sdk/debug.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/envelope.py` & `sentry_sdk-2.2.0/sentry_sdk/envelope.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/hub.py` & `sentry_sdk-2.2.0/sentry_sdk/hub.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/__init__.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,22 +65,24 @@
     "sentry_sdk.integrations.modules.ModulesIntegration",
     "sentry_sdk.integrations.stdlib.StdlibIntegration",
     "sentry_sdk.integrations.threading.ThreadingIntegration",
 ]
 
 _AUTO_ENABLING_INTEGRATIONS = [
     "sentry_sdk.integrations.aiohttp.AioHttpIntegration",
+    "sentry_sdk.integrations.anthropic.AnthropicIntegration",
     "sentry_sdk.integrations.ariadne.AriadneIntegration",
     "sentry_sdk.integrations.arq.ArqIntegration",
     "sentry_sdk.integrations.asyncpg.AsyncPGIntegration",
     "sentry_sdk.integrations.boto3.Boto3Integration",
     "sentry_sdk.integrations.bottle.BottleIntegration",
     "sentry_sdk.integrations.celery.CeleryIntegration",
     "sentry_sdk.integrations.chalice.ChaliceIntegration",
     "sentry_sdk.integrations.clickhouse_driver.ClickhouseDriverIntegration",
+    "sentry_sdk.integrations.cohere.CohereIntegration",
     "sentry_sdk.integrations.django.DjangoIntegration",
     "sentry_sdk.integrations.falcon.FalconIntegration",
     "sentry_sdk.integrations.fastapi.FastApiIntegration",
     "sentry_sdk.integrations.flask.FlaskIntegration",
     "sentry_sdk.integrations.gql.GQLIntegration",
     "sentry_sdk.integrations.graphene.GrapheneIntegration",
     "sentry_sdk.integrations.httpx.HttpxIntegration",
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/_asgi_common.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/_asgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/_wsgi_common.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/_wsgi_common.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/aiohttp.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/aiohttp.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/anthropic.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,27 @@
 from sentry_sdk.utils import (
     capture_internal_exceptions,
     ensure_integration_enabled,
     event_from_exception,
     package_version,
 )
 
-from anthropic.resources import Messages
-
 from typing import TYPE_CHECKING
 
+try:
+    from anthropic.resources import Messages
+
+    if TYPE_CHECKING:
+        from anthropic.types import MessageStreamEvent
+except ImportError:
+    raise DidNotEnable("Anthropic not installed")
+
+
 if TYPE_CHECKING:
     from typing import Any, Iterator
-    from anthropic.types import MessageStreamEvent
     from sentry_sdk.tracing import Span
 
 
 class AnthropicIntegration(Integration):
     identifier = "anthropic"
 
     def __init__(self, include_prompts=True):
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/argv.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/argv.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/ariadne.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/ariadne.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/arq.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/arq.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/asgi.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/asyncio.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/asyncio.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/asyncpg.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/asyncpg.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/atexit.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/atexit.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/aws_lambda.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/aws_lambda.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/beam.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/beam.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/boto3.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/boto3.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/bottle.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/bottle.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/celery/__init__.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/celery/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import sys
 from functools import wraps
 
 import sentry_sdk
 from sentry_sdk import isolation_scope
 from sentry_sdk.api import continue_trace
-from sentry_sdk.consts import OP
+from sentry_sdk.consts import OP, SPANDATA
 from sentry_sdk.integrations import Integration, DidNotEnable
 from sentry_sdk.integrations.celery.beat import (
     _patch_beat_apply_entry,
     _patch_redbeat_maybe_due,
     _setup_celery_beat_signals,
 )
 from sentry_sdk.integrations.celery.utils import _now_seconds_since_epoch
@@ -321,28 +321,58 @@
                 },
             ):
                 return f(*args, **kwargs)
 
     return _inner  # type: ignore
 
 
+def _set_messaging_destination_name(task, span):
+    # type: (Any, Span) -> None
+    """Set "messaging.destination.name" tag for span"""
+    with capture_internal_exceptions():
+        delivery_info = task.request.delivery_info
+        routing_key = delivery_info.get("routing_key")
+        if delivery_info.get("exchange") == "" and routing_key is not None:
+            # Empty exchange indicates the default exchange, meaning the tasks
+            # are sent to the queue with the same name as the routing key.
+            span.set_data(SPANDATA.MESSAGING_DESTINATION_NAME, routing_key)
+
+
 def _wrap_task_call(task, f):
     # type: (Any, F) -> F
 
     # Need to wrap task call because the exception is caught before we get to
     # see it. Also celery's reported stacktrace is untrustworthy.
 
     # functools.wraps is important here because celery-once looks at this
-    # method's name.
+    # method's name. @ensure_integration_enabled internally calls functools.wraps,
+    # but if we ever remove the @ensure_integration_enabled decorator, we need
+    # to add @functools.wraps(f) here.
     # https://github.com/getsentry/sentry-python/issues/421
-    @wraps(f)
+    @ensure_integration_enabled(CeleryIntegration, f)
     def _inner(*args, **kwargs):
         # type: (*Any, **Any) -> Any
         try:
-            return f(*args, **kwargs)
+            with sentry_sdk.start_span(
+                op=OP.QUEUE_PROCESS, description=task.name
+            ) as span:
+                _set_messaging_destination_name(task, span)
+                with capture_internal_exceptions():
+                    span.set_data(SPANDATA.MESSAGING_MESSAGE_ID, task.request.id)
+                with capture_internal_exceptions():
+                    span.set_data(
+                        SPANDATA.MESSAGING_MESSAGE_RETRY_COUNT, task.request.retries
+                    )
+                with capture_internal_exceptions():
+                    span.set_data(
+                        SPANDATA.MESSAGING_SYSTEM,
+                        task.app.connection().transport.driver_type,
+                    )
+
+                return f(*args, **kwargs)
         except Exception:
             exc_info = sys.exc_info()
             with capture_internal_exceptions():
                 _capture_exception(task, exc_info)
             reraise(*exc_info)
 
     return _inner  # type: ignore
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/celery/beat.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/celery/beat.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/celery/utils.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/celery/utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/chalice.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/chalice.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/clickhouse_driver.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/clickhouse_driver.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/cloud_resource_context.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/cloud_resource_context.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/dedupe.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/dedupe.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/django/__init__.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/django/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/django/asgi.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/django/asgi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/django/caching.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/django/caching.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/django/middleware.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/django/middleware.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/django/signals_handlers.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/django/signals_handlers.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/django/templates.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/django/templates.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/django/transactions.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/django/transactions.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/django/views.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/django/views.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/excepthook.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/excepthook.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/executing.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/executing.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/falcon.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/falcon.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/fastapi.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/fastapi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/flask.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/flask.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/gcp.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/gcp.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/gnu_backtrace.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/gnu_backtrace.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/gql.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/gql.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/graphene.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/graphene.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/__init__.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/grpc/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/aio/client.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/grpc/aio/client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/aio/server.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/grpc/aio/server.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/client.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/grpc/client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/grpc/server.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/grpc/server.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/httpx.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/httpx.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/huey.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/huey.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/huggingface_hub.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/huggingface_hub.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/langchain.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/langchain.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,20 @@
     "response_format": SPANDATA.AI_RESPONSE_FORMAT,
     "logit_bias": SPANDATA.AI_LOGIT_BIAS,
     "tags": SPANDATA.AI_TAGS,
 }
 
 # To avoid double collecting tokens, we do *not* measure
 # token counts for models for which we have an explicit integration
-NO_COLLECT_TOKEN_MODELS = ["openai-chat"]  # TODO add huggingface and anthropic
+NO_COLLECT_TOKEN_MODELS = [
+    "openai-chat",
+    "anthropic-chat",
+    "cohere-chat",
+    "huggingface_endpoint",
+]
 
 
 class LangchainIntegration(Integration):
     identifier = "langchain"
 
     # The most number of spans (e.g., LLM calls) that can be processed at the same time.
     max_spans = 1024
@@ -212,14 +217,15 @@
             span = watched_span.span
             model = all_params.get(
                 "model", all_params.get("model_name", all_params.get("model_id"))
             )
             watched_span.no_collect_tokens = any(
                 x in all_params.get("_type", "") for x in NO_COLLECT_TOKEN_MODELS
             )
+
             if not model and "anthropic" in all_params.get("_type"):
                 model = "claude-2"
             if model:
                 span.set_data(SPANDATA.AI_MODEL_ID, model)
             if should_send_default_pii() and self.include_prompts:
                 set_data_normalized(
                     span,
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/logging.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/logging.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/loguru.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/loguru.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/modules.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/modules.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/openai.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/openai.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/integration.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/opentelemetry/integration.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/propagator.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/opentelemetry/propagator.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/opentelemetry/span_processor.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/opentelemetry/span_processor.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/pure_eval.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/pure_eval.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/pymongo.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/pymongo.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/pyramid.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/pyramid.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/quart.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/quart.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/redis/__init__.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/redis/asyncio.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/redis/asyncio.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/rq.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/rq.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/sanic.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/sanic.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/serverless.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/serverless.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/socket.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/socket.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/spark/spark_driver.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/spark/spark_driver.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/spark/spark_worker.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/spark/spark_worker.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/sqlalchemy.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/starlette.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/starlette.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/starlite.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/starlite.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/stdlib.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/stdlib.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/strawberry.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/strawberry.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/threading.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/threading.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/tornado.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/tornado.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/trytond.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/trytond.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/integrations/wsgi.py` & `sentry_sdk-2.2.0/sentry_sdk/integrations/wsgi.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/metrics.py` & `sentry_sdk-2.2.0/sentry_sdk/metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -922,15 +922,15 @@
         aggregator.add(
             "d", key, value, unit, tags, timestamp, local_aggregator, stacklevel
         )
 
 
 def set(
     key,  # type: str
-    value,  # type: MetricValue
+    value,  # type: Union[int, str]
     unit="none",  # type: MeasurementUnit
     tags=None,  # type: Optional[MetricTags]
     timestamp=None,  # type: Optional[Union[float, datetime]]
     stacklevel=0,  # type: int
 ):
     # type: (...) -> None
     """Emits a set."""
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk/monitor.py` & `sentry_sdk-2.2.0/sentry_sdk/monitor.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/profiler.py` & `sentry_sdk-2.2.0/sentry_sdk/profiler.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/scope.py` & `sentry_sdk-2.2.0/sentry_sdk/scope.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,14 +181,15 @@
         "_session",
         "_attachments",
         "_force_auto_session_tracking",
         "_profile",
         "_propagation_context",
         "client",
         "_type",
+        "_last_event_id",
     )
 
     def __init__(self, ty=None, client=None):
         # type: (Optional[ScopeType], Optional[sentry_sdk.Client]) -> None
         self._type = ty
 
         self._event_processors = []  # type: List[EventProcessor]
@@ -203,14 +204,17 @@
             self.set_client(client)
 
         self.clear()
 
         incoming_trace_information = self._load_trace_data_from_env()
         self.generate_propagation_context(incoming_data=incoming_trace_information)
 
+        # self._last_event_id is only applicable to isolation scopes
+        self._last_event_id = None  # type: Optional[str]
+
     def __copy__(self):
         # type: () -> Scope
         """
         Returns a copy of this scope.
         This also creates a copy of all referenced data structures.
         """
         rv = object.__new__(self.__class__)  # type: Scope
@@ -304,14 +308,31 @@
         """
         global _global_scope
         if _global_scope is None:
             _global_scope = Scope(ty=ScopeType.GLOBAL)
 
         return _global_scope
 
+    @classmethod
+    def last_event_id(cls):
+        # type: () -> Optional[str]
+        """
+        .. versionadded:: 2.2.0
+
+        Returns event ID of the event most recently captured by the isolation scope, or None if no event
+        has been captured. We do not consider events that are dropped, e.g. by a before_send hook.
+        Transactions also are not considered events in this context.
+
+        The event corresponding to the returned event ID is NOT guaranteed to actually be sent to Sentry;
+        whether the event is sent depends on the transport. The event could be sent later or not at all.
+        Even a sent event could fail to arrive in Sentry due to network issues, exhausted quotas, or
+        various other reasons.
+        """
+        return cls.get_isolation_scope()._last_event_id
+
     def _merge_scopes(self, additional_scope=None, additional_scope_kwargs=None):
         # type: (Optional[Scope], Optional[Dict[str, Any]]) -> Scope
         """
         Merges global, isolation and current scope into a new scope and
         adds the given additional scope or additional scope kwargs to it.
         """
         if additional_scope and additional_scope_kwargs:
@@ -1085,15 +1106,20 @@
             For supported `**scope_kwargs` see :py:meth:`sentry_sdk.Scope.update_from_kwargs`.
             The `scope` and `scope_kwargs` parameters are mutually exclusive.
 
         :returns: An `event_id` if the SDK decided to send the event (see :py:meth:`sentry_sdk.client._Client.capture_event`).
         """
         scope = self._merge_scopes(scope, scope_kwargs)
 
-        return Scope.get_client().capture_event(event=event, hint=hint, scope=scope)
+        event_id = Scope.get_client().capture_event(event=event, hint=hint, scope=scope)
+
+        if event_id is not None and event.get("type") != "transaction":
+            self.get_isolation_scope()._last_event_id = event_id
+
+        return event_id
 
     def capture_message(self, message, level=None, scope=None, **scope_kwargs):
         # type: (str, Optional[LogLevelStr], Optional[Scope], Any) -> Optional[str]
         """
         Captures a message.
 
         :param message: The string to send as the message.
@@ -1636,7 +1662,10 @@
     # type: () -> bool
     """Shortcut for `Scope.get_client().should_send_default_pii()`."""
     return Scope.get_client().should_send_default_pii()
 
 
 # Circular imports
 from sentry_sdk.client import NonRecordingClient
+
+if TYPE_CHECKING:
+    import sentry_sdk.client
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk/scrubber.py` & `sentry_sdk-2.2.0/sentry_sdk/scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/serializer.py` & `sentry_sdk-2.2.0/sentry_sdk/serializer.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/session.py` & `sentry_sdk-2.2.0/sentry_sdk/session.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/sessions.py` & `sentry_sdk-2.2.0/sentry_sdk/sessions.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/spotlight.py` & `sentry_sdk-2.2.0/sentry_sdk/spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/tracing.py` & `sentry_sdk-2.2.0/sentry_sdk/tracing.py`

 * *Files 0% similar despite different names*

```diff
@@ -422,20 +422,26 @@
     def iter_headers(self):
         # type: () -> Iterator[Tuple[str, str]]
         """
         Creates a generator which returns the span's ``sentry-trace`` and ``baggage`` headers.
         If the span's containing transaction doesn't yet have a ``baggage`` value,
         this will cause one to be generated and stored.
         """
+        if not self.containing_transaction:
+            # Do not propagate headers if there is no containing transaction. Otherwise, this
+            # span ends up being the root span of a new trace, and since it does not get sent
+            # to Sentry, the trace will be missing a root transaction. The dynamic sampling
+            # context will also be missing, breaking dynamic sampling & traces.
+            return
+
         yield SENTRY_TRACE_HEADER_NAME, self.to_traceparent()
 
-        if self.containing_transaction:
-            baggage = self.containing_transaction.get_baggage().serialize()
-            if baggage:
-                yield BAGGAGE_HEADER_NAME, baggage
+        baggage = self.containing_transaction.get_baggage().serialize()
+        if baggage:
+            yield BAGGAGE_HEADER_NAME, baggage
 
     @classmethod
     def from_traceparent(
         cls,
         traceparent,  # type: Optional[str]
         **kwargs,  # type: Any
     ):
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk/tracing_utils.py` & `sentry_sdk-2.2.0/sentry_sdk/tracing_utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/transport.py` & `sentry_sdk-2.2.0/sentry_sdk/transport.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/types.py` & `sentry_sdk-2.2.0/sentry_sdk/types.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/utils.py` & `sentry_sdk-2.2.0/sentry_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk/worker.py` & `sentry_sdk-2.2.0/sentry_sdk/worker.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/sentry_sdk.egg-info/PKG-INFO` & `sentry_sdk-2.2.0/sentry_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sentry-sdk
-Version: 2.1.1
+Version: 2.2.0
 Summary: Python client for Sentry (https://sentry.io)
 Home-page: https://github.com/getsentry/sentry-python
 Author: Sentry Team and Contributors
 Author-email: hello@sentry.io
 License: MIT
 Project-URL: Documentation, https://docs.sentry.io/platforms/python/
 Project-URL: Changelog, https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk.egg-info/SOURCES.txt` & `sentry_sdk-2.2.0/sentry_sdk.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -64,14 +64,15 @@
 sentry_sdk/integrations/aws_lambda.py
 sentry_sdk/integrations/beam.py
 sentry_sdk/integrations/boto3.py
 sentry_sdk/integrations/bottle.py
 sentry_sdk/integrations/chalice.py
 sentry_sdk/integrations/clickhouse_driver.py
 sentry_sdk/integrations/cloud_resource_context.py
+sentry_sdk/integrations/cohere.py
 sentry_sdk/integrations/dedupe.py
 sentry_sdk/integrations/excepthook.py
 sentry_sdk/integrations/executing.py
 sentry_sdk/integrations/falcon.py
 sentry_sdk/integrations/fastapi.py
 sentry_sdk/integrations/flask.py
 sentry_sdk/integrations/gcp.py
```

### Comparing `sentry_sdk-2.1.1/sentry_sdk.egg-info/requires.txt` & `sentry_sdk-2.2.0/sentry_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/setup.py` & `sentry_sdk-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 def get_file_text(file_name):
     with open(os.path.join(here, file_name)) as in_file:
         return in_file.read()
 
 
 setup(
     name="sentry-sdk",
-    version="2.1.1",
+    version="2.2.0",
     author="Sentry Team and Contributors",
     author_email="hello@sentry.io",
     url="https://github.com/getsentry/sentry-python",
     project_urls={
         "Documentation": "https://docs.sentry.io/platforms/python/",
         "Changelog": "https://github.com/getsentry/sentry-python/blob/master/CHANGELOG.md",
     },
```

### Comparing `sentry_sdk-2.1.1/tests/test_api.py` & `sentry_sdk-2.2.0/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_basics.py` & `sentry_sdk-2.2.0/tests/test_basics.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from sentry_sdk import (
     push_scope,
     configure_scope,
     capture_event,
     capture_exception,
     capture_message,
     start_transaction,
+    last_event_id,
     add_breadcrumb,
     Hub,
     Scope,
 )
 from sentry_sdk.integrations import (
     _AUTO_ENABLING_INTEGRATIONS,
     Integration,
@@ -774,7 +775,28 @@
 
     sentry_init(functions_to_trace=[{"qualified_name": test_classmethod_name}])
 
     for instance_or_class in (TracingTestClass, TracingTestClass()):
         with patch_start_tracing_child() as fake_start_child:
             assert instance_or_class.class_(1) == (TracingTestClass, 1)
             assert fake_start_child.call_count == 1
+
+
+def test_last_event_id(sentry_init):
+    sentry_init(enable_tracing=True)
+
+    assert last_event_id() is None
+
+    capture_exception(Exception("test"))
+
+    assert last_event_id() is not None
+
+
+def test_last_event_id_transaction(sentry_init):
+    sentry_init(enable_tracing=True)
+
+    assert last_event_id() is None
+
+    with start_transaction(name="test"):
+        pass
+
+    assert last_event_id() is None, "Transaction should not set last_event_id"
```

### Comparing `sentry_sdk-2.1.1/tests/test_client.py` & `sentry_sdk-2.2.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_conftest.py` & `sentry_sdk-2.2.0/tests/test_conftest.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_crons.py` & `sentry_sdk-2.2.0/tests/test_crons.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_envelope.py` & `sentry_sdk-2.2.0/tests/test_envelope.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_exceptiongroup.py` & `sentry_sdk-2.2.0/tests/test_exceptiongroup.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_lru_cache.py` & `sentry_sdk-2.2.0/tests/test_lru_cache.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_metrics.py` & `sentry_sdk-2.2.0/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_monitor.py` & `sentry_sdk-2.2.0/tests/test_monitor.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_new_scopes_compat.py` & `sentry_sdk-2.2.0/tests/test_new_scopes_compat.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_new_scopes_compat_event.py` & `sentry_sdk-2.2.0/tests/test_new_scopes_compat_event.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_profiler.py` & `sentry_sdk-2.2.0/tests/test_profiler.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_propagationcontext.py` & `sentry_sdk-2.2.0/tests/test_propagationcontext.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_scope.py` & `sentry_sdk-2.2.0/tests/test_scope.py`

 * *Files 6% similar despite different names*

```diff
@@ -818,7 +818,28 @@
     event = scope.apply_to_event({}, {})
 
     assert event["tags"] == {
         "tag1": "value1",
         "tag2": "updated",
         "tag3": "new",
     }, "Updating tags with empty dict changed tags"
+
+
+def test_last_event_id(sentry_init):
+    sentry_init(enable_tracing=True)
+
+    assert Scope.last_event_id() is None
+
+    sentry_sdk.capture_exception(Exception("test"))
+
+    assert Scope.last_event_id() is not None
+
+
+def test_last_event_id_transaction(sentry_init):
+    sentry_init(enable_tracing=True)
+
+    assert Scope.last_event_id() is None
+
+    with sentry_sdk.start_transaction(name="test"):
+        pass
+
+    assert Scope.last_event_id() is None, "Transaction should not set last_event_id"
```

### Comparing `sentry_sdk-2.1.1/tests/test_scrubber.py` & `sentry_sdk-2.2.0/tests/test_scrubber.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_serializer.py` & `sentry_sdk-2.2.0/tests/test_serializer.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_sessions.py` & `sentry_sdk-2.2.0/tests/test_sessions.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_spotlight.py` & `sentry_sdk-2.2.0/tests/test_spotlight.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_transport.py` & `sentry_sdk-2.2.0/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_types.py` & `sentry_sdk-2.2.0/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `sentry_sdk-2.1.1/tests/test_utils.py` & `sentry_sdk-2.2.0/tests/test_utils.py`

 * *Files identical despite different names*

