# Comparing `tmp/girder-worker-0.9.1.dev2.tar.gz` & `tmp/girder-worker-0.9.1.dev6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/girder-worker-0.9.1.dev2.tar", last modified: Thu Nov 17 13:29:26 2022, max compression
+gzip compressed data, was "girder-worker-0.9.1.dev6.tar", last modified: Fri Oct  6 18:31:43 2023, max compression
```

## Comparing `girder-worker-0.9.1.dev2.tar` & `girder-worker-0.9.1.dev6.tar`

### file list

```diff
@@ -1,94 +1,93 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/.circleci/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4340 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/.circleci/config.yml
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker/_test_plugins/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/_test_plugins/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      734 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/_test_plugins/plugins.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      295 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/_test_plugins/tasks.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker/context/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      285 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/context/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3733 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/context/girder_context.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4805 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/context/nongirder_context.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker/docker/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker/docker/io/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11038 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/docker/io/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1060 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/docker/io/girder.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker/docker/tasks/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16503 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/docker/tasks/__init__.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker/docker/transforms/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    13362 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/docker/transforms/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    12428 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/docker/transforms/girder.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      238 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/docker/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      190 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/docker/nvidia.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4016 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/docker/stream_adapter.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3374 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/docker/utils.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/api/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/api/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1937 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/api/worker.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/stylesheets/
--rw-r--r--   0 circleci  (3434) circleci  (3434)      201 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/stylesheets/jobDetailsWidget.styl
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1253 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/stylesheets/taskStatusView.styl
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/templates/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1214 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/templates/configView.pug
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2901 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/templates/taskStatusView.pug
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/views/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2985 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/views/ConfigView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3321 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/views/taskStatusView.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1210 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/JobStatus.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      131 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/main.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)      637 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/package.json
--rw-r--r--   0 circleci  (3434) circleci  (3434)      601 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/routes.js
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2880 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1348 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/celery.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1236 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/constants.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5661 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/event_handlers.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3545 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/status.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6321 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/girder_plugin/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       17 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1343 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      181 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/__main__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     7743 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/app.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      436 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/celeryconfig.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2166 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/configure.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2625 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/entrypoint.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      728 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/log_utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6645 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/task.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10978 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/utils.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      265 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/girder_worker/worker.dist.cfg
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2276 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2379 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)      737 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (3434) circleci  (3434)      299 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       14 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/girder_worker.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/scripts/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1956 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/scripts/install_requirements.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       97 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/.codecov.yml
--rw-r--r--   0 circleci  (3434) circleci  (3434)      161 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/.coveragerc.pytest
--rw-r--r--   0 circleci  (3434) circleci  (3434)        4 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/.dockerignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)      157 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/.gitignore
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3177 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/CHANGELOG.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)      779 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/CMakeLists.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3473 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/CONTRIBUTING.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1176 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/Dockerfile
--rw-r--r--   0 circleci  (3434) circleci  (3434)    33717 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/HACKING.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)      362 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/MANIFEST.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)      219 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/NOTICE
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1542 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/README.rst
--rw-r--r--   0 circleci  (3434) circleci  (3434)    16366 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/TRANSITION.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)      233 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/docker-compose.yml
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)      317 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/docker-entrypoint.sh
--rw-r--r--   0 circleci  (3434) circleci  (3434)      121 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/docker.env
--rw-r--r--   0 circleci  (3434) circleci  (3434)      404 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/requirements-dev.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)      248 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/requirements.in
--rw-r--r--   0 circleci  (3434) circleci  (3434)     6174 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/requirements.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4450 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/setup.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3474 2022-11-17 13:29:08.000000 girder-worker-0.9.1.dev2/tox.ini
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2276 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2022-11-17 13:29:26.000000 girder-worker-0.9.1.dev2/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.694027 girder-worker-0.9.1.dev6/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.686027 girder-worker-0.9.1.dev6/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4336 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/.circleci/config.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       97 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/.codecov.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      161 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/.coveragerc.pytest
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        4 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/.dockerignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      157 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/CHANGELOG.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3473 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/CONTRIBUTING.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/Dockerfile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33717 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/HACKING.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      362 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      219 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/NOTICE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2850 2023-10-06 18:31:43.694027 girder-worker-0.9.1.dev6/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1542 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16366 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/TRANSITION.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/docker-compose.yml
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      317 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/docker-entrypoint.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      121 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/docker.env
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.686027 girder-worker-0.9.1.dev6/girder_worker/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       17 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1335 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      181 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/__main__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.690027 girder-worker-0.9.1.dev6/girder_worker/_test_plugins/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/_test_plugins/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      734 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/_test_plugins/plugins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/_test_plugins/tasks.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7727 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/app.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      421 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/celeryconfig.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2166 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/configure.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.690027 girder-worker-0.9.1.dev6/girder_worker/context/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      285 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/context/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3733 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/context/girder_context.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4773 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/context/nongirder_context.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.690027 girder-worker-0.9.1.dev6/girder_worker/docker/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      238 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/docker/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.690027 girder-worker-0.9.1.dev6/girder_worker/docker/io/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10922 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/docker/io/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1016 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/docker/io/girder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      190 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/docker/nvidia.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3984 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/docker/stream_adapter.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.690027 girder-worker-0.9.1.dev6/girder_worker/docker/tasks/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16520 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/docker/tasks/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.690027 girder-worker-0.9.1.dev6/girder_worker/docker/transforms/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13156 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/docker/transforms/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12102 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/docker/transforms/girder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3374 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/docker/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2606 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/entrypoint.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.690027 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2848 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.694027 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1901 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/api/worker.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1309 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/celery.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1204 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5622 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/event_handlers.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3537 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/status.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6297 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.694027 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1210 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/JobStatus.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/main.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      637 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/package.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      601 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.694027 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/stylesheets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      201 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/stylesheets/jobDetailsWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1253 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/stylesheets/taskStatusView.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.694027 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1214 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/templates/configView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2901 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/templates/taskStatusView.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.694027 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2985 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/views/ConfigView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3321 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/views/taskStatusView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/log_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6569 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10896 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      262 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/girder_worker/worker.dist.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.690027 girder-worker-0.9.1.dev6/girder_worker.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2850 2023-10-06 18:31:43.000000 girder-worker-0.9.1.dev6/girder_worker.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2364 2023-10-06 18:31:43.000000 girder-worker-0.9.1.dev6/girder_worker.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-10-06 18:31:43.000000 girder-worker-0.9.1.dev6/girder_worker.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      736 2023-10-06 18:31:43.000000 girder-worker-0.9.1.dev6/girder_worker.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-10-06 18:31:43.000000 girder-worker-0.9.1.dev6/girder_worker.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      295 2023-10-06 18:31:43.000000 girder-worker-0.9.1.dev6/girder_worker.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       14 2023-10-06 18:31:43.000000 girder-worker-0.9.1.dev6/girder_worker.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/requirements-dev.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/requirements.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7599 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/requirements.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-10-06 18:31:43.694027 girder-worker-0.9.1.dev6/scripts/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1956 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/scripts/install_requirements.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-10-06 18:31:43.694027 girder-worker-0.9.1.dev6/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4502 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/setup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3138 2023-10-06 18:31:28.000000 girder-worker-0.9.1.dev6/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `girder-worker-0.9.1.dev2/.circleci/config.yml` & `girder-worker-0.9.1.dev6/.circleci/config.yml`

 * *Files 6% similar despite different names*

```diff
@@ -67,69 +67,69 @@
 
 jobs:
   py3_integration_tests:
     machine: true
     working_directory: /home/circleci/project
     steps:
       - run:
-          name: Set up Python 3.6
+          name: Set up Python 3.8
           command: |
-             pyenv install 3.6.3 || true
-             pyenv global 3.6.3
+             pyenv install 3.8 || true
+             pyenv global 3.8
 
       - *ssh-keys
       - checkout
       - *update-pip
       - *install-docker-compose
       - *run-env
       - *run-tests
       - *dump-girder-logs
       - *dump-worker-logs
 
   unit_tests:
     docker:
-      - image: cimg/python:3.6
+      - image: cimg/python:3.8
     steps:
       - checkout
       - *virtual-env
       - *update-pip
       - *ci-deps
       - run:
           name: Run unit tests
-          command: tox -e py36
+          command: tox -e py38
       - *upload-coverage
 
-  unit_tests_310:
+  unit_tests_311:
     docker:
-      - image: cimg/python:3.10
+      - image: cimg/python:3.11
     steps:
       - checkout
       - *virtual-env
       - *update-pip
       - *ci-deps
       - run:
           name: Run unit tests
-          command: tox -e py310
+          command: tox -e py311
       - *upload-coverage
 
   lint:
     docker:
-      - image: cimg/python:3.6
+      - image: cimg/python:3.8
     steps:
       - checkout
       - *virtual-env
       - *update-pip
       - *ci-deps
       - run:
           name: Run linting tests
           command: tox -e lint
 
   release:
     docker:
-      - image: cimg/python:3.6
+      - image: cimg/python:3.8
     steps:
       - checkout
       - *virtual-env
       - *update-pip
       - *ci-deps
       - run:
           name: Release to PyPI
@@ -159,15 +159,15 @@
 
   ci:
     jobs:
       - unit_tests:
           filters:
             tags:
               only: /^v.*/
-      - unit_tests_310:
+      - unit_tests_311:
           filters:
             tags:
               only: /^v.*/
       - lint:
           filters:
             tags:
               only: /^v.*/
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/_test_plugins/plugins.py` & `girder-worker-0.9.1.dev6/girder_worker/_test_plugins/plugins.py`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/girder_worker/context/girder_context.py` & `girder-worker-0.9.1.dev6/girder_worker/context/girder_context.py`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/girder_worker/context/nongirder_context.py` & `girder-worker-0.9.1.dev6/girder_worker/context/nongirder_context.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,18 +59,18 @@
 
         try:
             response = gc.post('job', parameters=parameters, jsonResp=False)
             if response.ok:
                 headers['jobInfoSpec'] = response.json().get('jobInfoSpec')
                 return response.json()
         except requests.exceptions.RequestException as e:
-            logger.warn('Failed to post job: {}'.format(e))
+            logger.warn(f'Failed to post job: {e}')
 
     except MissingJobArguments as e:
-        logger.warn('Girder job not created: {}'.format(str(e)))
+        logger.warn(f'Girder job not created: {str(e)}')
 
 
 def attach_girder_api_url(sender=None, body=None, exchange=None,
                           routing_key=None, headers=None, properties=None,
                           declare=None, retry_policy=None, **kwargs):
     parent_task = current_app.current_task
     try:
@@ -79,15 +79,15 @@
         if parent_task.request is None:
             raise MissingJobArguments("Parent task's request is None")
         if not hasattr(parent_task.request, 'girder_api_url'):
             raise MissingJobArguments(
                 "Parent task's request does not contain girder_api_url")
         headers['girder_api_url'] = parent_task.request.girder_api_url
     except MissingJobArguments as e:
-        logger.warn('Could not get girder_api_url from parent task: {}'.format(str(e)))
+        logger.warn(f'Could not get girder_api_url from parent task: {str(e)}')
 
 
 def attach_girder_client_token(sender=None, body=None, exchange=None,
                                routing_key=None, headers=None, properties=None,
                                declare=None, retry_policy=None, **kwargs):
     parent_task = current_app.current_task
     try:
@@ -97,13 +97,13 @@
             raise MissingJobArguments("Parent task's request is None")
         if not hasattr(parent_task.request, 'girder_client_token'):
             raise MissingJobArguments(
                 "Parent task's request does not contain girder_client_token")
 
         headers['girder_client_token'] = parent_task.request.girder_client_token
     except MissingJobArguments as e:
-        logger.warn('Could not get token from parent task: {}'.format(str(e)))
+        logger.warn(f'Could not get token from parent task: {str(e)}')
 
 
 def get_async_result_job_property(async_result):
     # NOT IMPLEMENTED!
     return None
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/docker/io/__init__.py` & `girder-worker-0.9.1.dev6/girder_worker/docker/io/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import os
 import errno
 import stat
 import abc
+import urllib
 import ssl
 import sys
-import six
-from six.moves import http_client as httplib, urllib
+from http import client as httplib
 
 
-@six.add_metaclass(abc.ABCMeta)
-class FDStreamConnector(object):
+class FDStreamConnector(metaclass=abc.ABCMeta):
     """
     FDStreamConnector is an abstract base class used to connect a read(input) and write(output)
     stream.
     """
 
     def __init__(self, input, output):
         self.input = input
@@ -145,16 +144,15 @@
         """
         Closes the output side of this connector, followed by the input side.
         """
         self.input.close()
         self.output.close()
 
 
-@six.add_metaclass(abc.ABCMeta)
-class StreamReader(object):
+class StreamReader(metaclass=abc.ABCMeta):
     """
     This represents the interface that must be implemented by a stream reader.
     """
 
     @abc.abstractmethod
     def read(self, buf_len):
         """
@@ -167,16 +165,15 @@
     def close(self):
         """
         Close the input stream. Called after the last data is read.
         """
         pass
 
 
-@six.add_metaclass(abc.ABCMeta)
-class StreamWriter(object):
+class StreamWriter(metaclass=abc.ABCMeta):
     """
     This represents the interface that must be implemented by a stream writer.
     """
 
     @abc.abstractmethod
     def write(self, buf):
         """
@@ -235,15 +232,15 @@
         return self._stream.write(buf)
 
     def close(self):
         # Don't close std streams!
         self._stream.flush()
 
 
-class NamedPipe(object):
+class NamedPipe:
     """
     A named pipe.
     """
     def __init__(self, path):
         self.path = path
         self._fd = None
         os.mkfifo(self.path)
@@ -267,15 +264,15 @@
 
 
 class NamedPipeReader(FileDescriptorReader):
     """
     Reader to read from a named pipe.
     """
     def __init__(self, pipe, container_path=None):
-        super(NamedPipeReader, self).__init__(None)
+        super().__init__(None)
         self._pipe = pipe
         self._container_path = container_path
 
     def open(self):
         self._pipe.open(os.O_RDONLY | os.O_NONBLOCK)
 
     def path(self):
@@ -290,15 +287,15 @@
 
 
 class NamedPipeWriter(FileDescriptorWriter):
     """
     Write to write to a named pipe.
     """
     def __init__(self, pipe, container_path=None):
-        super(NamedPipeWriter, self).__init__(None)
+        super().__init__(None)
         self._pipe = pipe
         self._container_path = container_path
 
     def open(self):
         self._pipe.open(os.O_WRONLY | os.O_NONBLOCK)
 
     def path(self):
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/docker/io/girder.py` & `girder-worker-0.9.1.dev6/girder_worker/docker/io/girder.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import six
-
 from . import StreamReader
 
 
 class GirderFileStreamReader(StreamReader):
     """
     Stream a file from Girder.
     """
     def __init__(self, client, file_id):
         """
         :param client: The GirderClient instance to use.
         :type client: girder_client.GirderClient
         """
-        super(GirderFileStreamReader, self).__init__()
+        super().__init__()
         self._client = client
         self._file_id = file_id
         self._iter = None
 
     def read(self, buf_len):
         """
         Implementation note: due to a constraint of the requests library, the
@@ -24,10 +22,10 @@
         all future requests to ``read`` to have the same ``buf_len`` even if
         a different ``buf_len`` is passed in on subsequent requests.
         """
         if self._iter is None:  # lazy load response body iterator
             self._iter = self._client.downloadFileAsIterator(self._file_id, buf_len)
 
         try:
-            return six.next(self._iter)
+            return next(self._iter)
         except StopIteration:
             return b''
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/docker/tasks/__init__.py` & `girder-worker-0.9.1.dev6/girder_worker/docker/tasks/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -223,14 +223,16 @@
         # Run select loop
         utils.select_loop(exit_condition=exit_condition,
                           readers=read_stream_connectors,
                           writers=write_stream_connectors)
 
         if task.canceled:
             try:
+                msg = 'Asking to stop container: %s' % container.id
+                logger.info(msg)
                 container.stop()
             # Catch the ReadTimeout from requests and wait for container to
             # exit. See https://github.com/docker/docker-py/issues/1374 for
             # more details.
             except ReadTimeout:
                 tries = 10
                 while tries > 0:
@@ -282,29 +284,29 @@
         processed_args.append(arg)
 
     return (processed_args, read_streams, write_streams)
 
 
 class _RequestDefaultTemporaryVolume(_TemporaryVolumeBase):
     def __init__(self):
-        super(_RequestDefaultTemporaryVolume, self).__init__(None, None)
+        super().__init__(None, None)
         self._make_paths()
 
     def transform(self, **kwargs):
         self._transformed = True
 
 
 class DockerTask(Task):
 
     def _maybe_transform_argument(self, arg):
-        return super(DockerTask, self)._maybe_transform_argument(
+        return super()._maybe_transform_argument(
             arg, task=self, _default_temp_volume=self.request._default_temp_volume)
 
     def _maybe_transform_result(self, idx, result):
-        return super(DockerTask, self)._maybe_transform_result(
+        return super()._maybe_transform_result(
             idx, result, _default_temp_volume=self.request._default_temp_volume)
 
     def __call__(self, *args, **kwargs):
         default_temp_volume = _RequestDefaultTemporaryVolume()
         self.request._default_temp_volume = default_temp_volume
 
         volumes = kwargs.setdefault('volumes', {})
@@ -330,15 +332,15 @@
             # We then need to merge them into a single dict and it will be ready
             # for docker-py.
             volumes = {k: v for volume in volumes for k, v in volume.items()}
             kwargs['volumes'] = volumes
 
         volumes.update(default_temp_volume._repr_json_())
 
-        super(DockerTask, self).__call__(*args, **kwargs)
+        super().__call__(*args, **kwargs)
         threading.Thread(
             target=self._cleanup_temp_volumes,
             args=(temp_volumes, default_temp_volume),
             daemon=True).start()
 
     def _cleanup_temp_volumes(self, temp_volumes, default_temp_volume):
         # Set the permission to allow cleanup of temp directories
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/docker/transforms/__init__.py` & `girder-worker-0.9.1.dev6/girder_worker/docker/transforms/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import sys
 import uuid
 import os
 import tempfile
-import six
 import abc
 
 from girder_worker_utils.transform import Transform
 
 
 TEMP_VOLUME_MOUNT_PREFIX = '/mnt/girder_worker'
 
 
 def _maybe_transform(obj, *args, **kwargs):
-    if hasattr(obj, 'transform') and six.callable(obj.transform):
+    if hasattr(obj, 'transform') and callable(obj.transform):
         return obj.transform(*args, **kwargs)
 
     return obj
 
 
 class HostStdOut(Transform):
     """
@@ -114,15 +113,15 @@
         This returns the default temporary volume that is always mounted into the container.
         """
         return _DefaultTemporaryVolume()
 
 
 class _TemporaryVolumeBase(BindMountVolume):
     def __init__(self, *arg, **kwargs):
-        super(_TemporaryVolumeBase, self).__init__(*arg, **kwargs)
+        super().__init__(*arg, **kwargs)
         self._transformed = False
 
     def _make_paths(self, host_dir=None, mode=0o755):
         if host_dir is not None and not os.path.exists(host_dir):
             os.makedirs(host_dir)
             # Sometimes we need to explicitly set the mode of the
             # directory to 0o777 (e.g. when running the integration
@@ -130,16 +129,15 @@
             # getting in the way) we must make a separate call to
             # os.chmod.
             os.chmod(host_dir, mode)
         self._host_path = tempfile.mkdtemp(dir=host_dir)
         self._container_path = os.path.join(TEMP_VOLUME_MOUNT_PREFIX, uuid.uuid4().hex)
 
 
-@six.add_metaclass(_TemporaryVolumeMetaClass)
-class TemporaryVolume(_TemporaryVolumeBase):
+class TemporaryVolume(_TemporaryVolumeBase, metaclass=_TemporaryVolumeMetaClass):
     """
     This is a class used to represent a temporary directory on the host that will
     be mounted into a docker container. girder_worker will automatically attach a default
     temporary volume. This can be reference using `TemporaryVolume.default` class attribute.
     A temporary volume can also be create in a particular host directory by providing the
     `host_dir` param.
 
@@ -149,26 +147,26 @@
     :param mode: The default mode applied to the temporary volume if it does
         not already exist.
     :type mode: int
     """
     # Note that this mode is explicitly set with os.chmod. What you
     # set, is what you get - no os.makedirs umask shenanigans.
     def __init__(self, host_dir=None, mode=0o755):
-        super(TemporaryVolume, self).__init__(None, None)
+        super().__init__(None, None)
         self.host_dir = host_dir
         self._mode = mode
         self._instance = None
         self._transformed = False
 
     def transform(self, **kwargs):
         if not self._transformed:
             self._transformed = True
             self._make_paths(self.host_dir, mode=self._mode)
 
-        return super(TemporaryVolume, self).transform(**kwargs)
+        return super().transform(**kwargs)
 
 
 class _DefaultTemporaryVolume(TemporaryVolume):
     """
     Place holder who delegates implementation to instance provide by transform(...) method
     An instance of the class is returned each time `TemporaryVolume.default` is accessed.
     When the docker_run task is executed the transform(...) method is call with an instance
@@ -188,15 +186,15 @@
     @property
     def host_path(self):
         return self._instance.host_path
 
 
 class NamedPipeBase(Transform):
     def __init__(self, name, container_path=None, host_path=None, volume=TemporaryVolume.default):
-        super(NamedPipeBase, self).__init__()
+        super().__init__()
         self._container_path = None
         self._host_path = None
         self._volume = None
 
         if container_path is not None and host_path is not None:
             self._container_path = container_path
             self._host_path = host_path
@@ -246,22 +244,22 @@
     :type host_path: str
     :param volume: Alternatively a :py:class:`girder_worker.docker.transforms.BindMountVolume`
         instance can be provided. In which case the container_path and host_paths from
         the volume will be used when creating the pipe. The default location is
         :py:obj:`girder_worker.docker.transforms.TemporaryVolume.default`
     """
     def __init__(self, name,  container_path=None, host_path=None, volume=TemporaryVolume.default):
-        super(NamedInputPipe, self).__init__(name, container_path, host_path, volume)
+        super().__init__(name, container_path, host_path, volume)
 
     def transform(self, **kwargs):
         from girder_worker.docker.io import (
             NamedPipe,
             NamedPipeWriter
         )
-        super(NamedInputPipe, self).transform(**kwargs)
+        super().transform(**kwargs)
 
         pipe = NamedPipe(self.host_path)
         return NamedPipeWriter(pipe, self.container_path)
 
 
 class NamedOutputPipe(NamedPipeBase):
     """
@@ -276,22 +274,22 @@
     :type host_path: str
     :param volume: Alternatively a :py:class:`girder_worker.docker.transforms.BindMountVolume`
         instance can be provided. In which can the container_path and host_paths from
         the volume will be use when creating the pipe. The default location is
         :py:attr:`girder_worker.docker.transforms.TemporaryVolume.default`
     """
     def __init__(self, name, container_path=None, host_path=None, volume=TemporaryVolume.default):
-        super(NamedOutputPipe, self).__init__(name, container_path, host_path, volume)
+        super().__init__(name, container_path, host_path, volume)
 
     def transform(self, **kwargs):
         from girder_worker.docker.io import (
             NamedPipe,
             NamedPipeReader
         )
-        super(NamedOutputPipe, self).transform(**kwargs)
+        super().transform(**kwargs)
 
         pipe = NamedPipe(self.host_path)
         return NamedPipeReader(pipe, self.container_path)
 
 
 class VolumePath(Transform):
     """
@@ -337,15 +335,15 @@
     :param output: The output side of the connection
     :type output: :py:class:`girder_worker.docker.transforms.NamedInputPipe` or
         :py:class:`girder_worker.docker.transforms.ChunkedTransferEncodingStream` or
         :py:class:`girder_worker.docker.transforms.HostStdOut` or
         :py:class:`girder_worker.docker.transforms.HostStdErr`
     """
     def __init__(self, input, output):
-        super(Connect, self).__init__()
+        super().__init__()
         self._input = input
         self._output = output
 
     def transform(self, **kwargs):
         from girder_worker.docker.io import (
             FDWriteStreamConnector,
             FDReadStreamConnector,
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/docker/transforms/girder.py` & `girder-worker-0.9.1.dev6/girder_worker/docker/transforms/girder.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     This can be used to stream a Girder file into a docker container. See
     :ref:`docker-run-streaming-input` for example usage.
 
     :param _id: The Girder file ID.
     :type _id: str or ObjectId
     """
     def __init__(self, _id, **kwargs):
-        super(GirderFileIdToStream, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.file_id = _id
 
     def transform(self, **kwargs):
         from girder_worker.docker.io.girder import (
             GirderFileStreamReader
         )
         return GirderFileStreamReader(self.gc, self.file_id)
@@ -66,15 +66,15 @@
     :type _id: str or ObjectId
     :param volume: The bind mount volume where the file will reside.
     :type volume: :py:class:`girder_worker.docker.transforms.BindMountVolume`
     :param filename: Alternate name for the file. Default is to use the name from Girder.
     :type filename: str
     """
     def __init__(self, _id, volume=TemporaryVolume.default, filename=None, **kwargs):
-        super(GirderFileIdToVolume, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self._file_id = str(_id)
         self._volume = volume
         self._filename = filename
         self._file_path = None
 
     def _create_file_path(self, root):
         if self._filename is None:
@@ -104,17 +104,17 @@
 
     def cleanup(self, **kwargs):
         if self._file_path is not None:
             shutil.rmtree(self._file_path, ignore_errors=True)
 
     def _repr_model_(self):
         if self._filename:
-            template = u'<{module}.{cls}: File ID={id} -> "{fname}">'
+            template = '<{module}.{cls}: File ID={id} -> "{fname}">'
         else:
-            template = u'<{module}.{cls}: File ID={id}>'
+            template = '<{module}.{cls}: File ID={id}>'
         return template.format(
             module=self.__module__, cls=self.__class__.__name__, id=self._file_id,
             fname=self._filename)
 
 
 class GirderFolderIdToVolume(GirderClientTransform):
     """
@@ -125,15 +125,15 @@
     :type _id: str or ObjectId
     :param volume: The bind mount volume where the directory will reside.
     :type volume: :py:class:`girder_worker.docker.transforms.BindMountVolume`
     :param folder_name: Alternate name for the directory. Default is to use the name from Girder.
     :type folder_name: str
     """
     def __init__(self, _id, volume=TemporaryVolume.default, folder_name=None, **kwargs):
-        super(GirderFolderIdToVolume, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self._folder_id = str(_id)
         self._volume = volume
         self._folder_name = folder_name
         self._folder_path = None
 
     def _create_folder_path(self, root):
         if self._folder_name is None:
@@ -177,15 +177,15 @@
     :type _id: str or ObjectId
     :param volume: The bind mount volume where the item will reside.
     :type volume: :py:class:`girder_worker.docker.transforms.BindMountVolume`
     :param item_name: Alternate name for the file. Default is to use the name from Girder.
     :type item_name: str
     """
     def __init__(self, _id, volume=TemporaryVolume.default, **kwargs):
-        super(GirderItemIdToVolume, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self._item_id = str(_id)
         self._volume = volume
         self._item_path = None
 
     def _create_item_path(self, root):
         path = os.path.join(root, self._item_id)
         try:
@@ -228,22 +228,22 @@
     :param item_id: The item ID in Girder.
     :type item_id: str or ObjectId
     :param delete_file: Whether to delete the file afterward.
     :type delete_file: bool
     """
     def __init__(self, volumepath, item_id, delete_file=False, **kwargs):
         item_id = str(item_id)
-        super(GirderUploadVolumePathToItem, self).__init__(item_id, delete_file, **kwargs)
+        super().__init__(item_id, delete_file, **kwargs)
         self._volumepath = volumepath
 
     # We ignore the "result"
     def transform(self, *args, **kwargs):
         path = _maybe_transform(self._volumepath, *args, **kwargs)
 
-        return super(GirderUploadVolumePathToItem, self).transform(path)
+        return super().transform(path)
 
 
 class GirderUploadVolumePathToFolder(GirderUploadToFolder):
     """
     This transform uploads data in a bind mount volume to a Girder folder. This should be used
     in ``girder_result_hooks`` to upload data produced by the task.
 
@@ -251,20 +251,20 @@
     :type volumepath: :py:class:`girder_worker.docker.transforms.VolumePath`
     :param folder_id: The folder ID in Girder.
     :type folder_id: str or ObjectId
     :param delete_file: Whether to delete the data afterward.
     :type delete_file: bool
     """
     def __init__(self, volumepath, folder_id, delete_file=False, **kwargs):
-        super(GirderUploadVolumePathToFolder, self).__init__(str(folder_id), delete_file, **kwargs)
+        super().__init__(str(folder_id), delete_file, **kwargs)
         self._volumepath = volumepath
 
     def transform(self, *args, **kwargs):
         path = _maybe_transform(self._volumepath, *args, **kwargs)
-        return super(GirderUploadVolumePathToFolder, self).transform(path)
+        return super().transform(path)
 
 
 class GirderUploadVolumePathJobArtifact(GirderUploadJobArtifact):
     """
     This transform can be used to upload artifacts produced during a docker task execution
     and attach them to the corresponding job in Girder. This can be useful for tracing and
     debugging jobs, or simply collecting intermediate information during job execution. If
@@ -283,18 +283,18 @@
     :param upload_on_exception: If True, this transform will occur even if the docker task
         fails. This can be used to debug failed ``docker_run`` tasks.
     :type upload_on_exception: bool
     """
     def __init__(self, volumepath, job_id=None, name=None, upload_on_exception=False, **kwargs):
         if job_id is not None:
             job_id = str(job_id)
-        super(GirderUploadVolumePathJobArtifact, self).__init__(job_id, name, **kwargs)
+        super().__init__(job_id, name, **kwargs)
         self._volumepath = volumepath
         self._upload_on_exception = upload_on_exception
 
     def transform(self, *args, **kwargs):
         path = _maybe_transform(self._volumepath, *args, **kwargs)
-        return super(GirderUploadVolumePathJobArtifact, self).transform(path)
+        return super().transform(path)
 
     def exception(self):
         if self._upload_on_exception:
             return self.transform()
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/docker/stream_adapter.py` & `girder-worker-0.9.1.dev6/girder_worker/docker/stream_adapter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import struct
 import json
 
 
-class StreamPushAdapter(object):
+class StreamPushAdapter:
     """
     This represents the interface that must be implemented by push adapters for
     IO modes that want to implement streaming output.
     """
 
     def write(self, buf):
         """
@@ -27,15 +27,15 @@
     them as progress events via the JobManager.
 
     :param job_manager: The job manager to use to send the progress events.
     :type job_manager: girder_worker.utils.JobManager
     """
 
     def __init__(self, job_manager):
-        super(JobProgressAdapter, self).__init__()
+        super().__init__()
 
         self.job_manager = job_manager
         self._buf = b''
 
     def write(self, buf):
         lines = buf.split(b'\n')
         if self._buf:
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/docker/utils.py` & `girder-worker-0.9.1.dev6/girder_worker/docker/utils.py`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/api/worker.py` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/api/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 ###############################################################################
 #  Copyright Kitware Inc.
 #
 #  Licensed under the Apache License, Version 2.0 ( the "License" );
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
@@ -24,15 +23,15 @@
 from girder.api.rest import Resource
 
 from ..celery import getCeleryApp
 
 
 class Worker(Resource):
     def __init__(self):
-        super(Worker, self).__init__()
+        super().__init__()
         self.resourceName = 'worker'
         self.route('GET', ('status',), self.getWorkerStatus)
 
     @autoDescribeRoute(
         Description('Get worker status and task information.')
         .notes('Return -1 if the broker is inaccessible.')
     )
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/stylesheets/taskStatusView.styl` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/stylesheets/taskStatusView.styl`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/templates/configView.pug` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/templates/configView.pug`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/templates/taskStatusView.pug` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/templates/taskStatusView.pug`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/views/ConfigView.js` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/views/ConfigView.js`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/views/taskStatusView.js` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/views/taskStatusView.js`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/JobStatus.js` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/JobStatus.js`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/package.json` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/package.json`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/web_client/routes.js` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/web_client/routes.js`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/__init__.py` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 ###############################################################################
 #  Copyright Kitware Inc.
 #
 #  Licensed under the Apache License, Version 2.0 ( the "License" );
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
@@ -61,9 +60,9 @@
             events.bind('jobs.status.validate', 'worker', event_handlers.validateJobStatus)
             events.bind('jobs.status.validTransitions', 'worker', event_handlers.validTransitions)
             events.bind('jobs.cancel', 'worker', event_handlers.cancel)
             events.bind('model.job.save.after', 'worker', event_handlers.attachJobInfoSpec)
             events.bind('model.job.save', 'worker', event_handlers.attachParentJob)
             Job().exposeFields(AccessType.SITE_ADMIN, {'celeryTaskId', 'celeryQueue'})
 else:
-    class WorkerPlugin(object):
+    class WorkerPlugin:
         pass
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/celery.py` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/celery.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 ###############################################################################
 
-from __future__ import absolute_import
 
 import celery
 
 from girder.models.setting import Setting
 
 from .constants import PluginSettings
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/constants.py` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/constants.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 ###############################################################################
 #  Copyright Kitware Inc.
 #
 #  Licensed under the Apache License, Version 2.0 ( the "License" );
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
@@ -21,12 +20,12 @@
 DOCKER_DATA_VOLUME = '/mnt/girder_worker/data'
 
 # The path that will be mounted in docker containers for utility scripts
 DOCKER_SCRIPTS_VOLUME = '/mnt/girder_worker/scripts'
 
 
 # Settings where plugin information is stored
-class PluginSettings(object):
+class PluginSettings:
     BROKER = 'worker.broker'
     BACKEND = 'worker.backend'
     API_URL = 'worker.api_url'
     DIRECT_PATH = 'worker.direct_path'
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/event_handlers.py` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/event_handlers.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 ###############################################################################
 
-from __future__ import absolute_import
 
 from girder import logger
 from girder.exceptions import ValidationException
 from girder.utility import setting_utilities
 from girder_jobs.constants import JobStatus
 from girder_jobs.models.job import Job
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/status.py` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/status.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 ###############################################################################
 
 from girder_jobs.constants import JobStatus
 
 
-class CustomJobStatus(object):
+class CustomJobStatus:
     """
     The custom job status flags for the worker.
     """
     FETCHING_INPUT = 820
     CONVERTING_INPUT = 821
     CONVERTING_OUTPUT = 822
     PUSHING_OUTPUT = 823
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/girder_plugin/utils.py` & `girder-worker-0.9.1.dev6/girder_worker/girder_plugin/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 ###############################################################################
 #  Copyright Kitware Inc.
 #
 #  Licensed under the Apache License, Version 2.0 ( the "License" );
 #  you may not use this file except in compliance with the License.
 #  You may obtain a copy of the License at
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/__init__.py` & `girder-worker-0.9.1.dev6/girder_worker/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 config.read([os.path.join(PACKAGE_DIR, f) for f in _cfgs])
 
 # Create and configure our logger
 logger = log_utils.setupLogger(config)
 
 
-class GirderWorkerPluginABC(object):
+class GirderWorkerPluginABC:
     """
     Abstract base class for Girder Worker plugins. Plugins must descend from this
     class; see the :ref:`plugins` section for more information.
     """
     def __init__(*args, **kwargs):
         pass
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/app.py` & `girder-worker-0.9.1.dev6/girder_worker/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,16 +32,14 @@
     is_revoked
 )
 from girder_worker_utils.transform import ResultTransform
 
 import jsonpickle
 from kombu.serialization import register
 
-import six
-
 
 @before_task_publish.connect  # noqa: C901
 def girder_before_task_publish(sender=None, body=None, exchange=None,
                                routing_key=None, headers=None, properties=None,
                                declare=None, retry_policy=None, **kwargs):
 
     if is_builtin_celery_task(sender):
@@ -198,15 +196,15 @@
         task.job_manager._flush()
     except AttributeError:
         pass
     finally:
         # Release stdout/stderr
         if hasattr(task, 'job_manager') and \
            hasattr(task.job_manager, 'cleanup') and \
-           six.callable(task.job_manager.cleanup):
+           callable(task.job_manager.cleanup):
             task.job_manager.cleanup()
 
 
 @task_revoked.connect
 def gw_task_revoked(sender=None, request=None, **rest):
     try:
         sender.job_manager = _job_manager(headers=request.message.headers,
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/configure.py` & `girder-worker-0.9.1.dev6/girder_worker/configure.py`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/girder_worker/entrypoint.py` & `girder-worker-0.9.1.dev6/girder_worker/entrypoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from importlib import import_module
 import celery
 from girder_worker_utils import decorators
 
-import six
-
 from stevedore import extension
 
 
 #: Defines the namespace used for plugin entrypoints
 NAMESPACE = 'girder_worker_plugins'
 
 
@@ -54,15 +52,15 @@
     """
     module = import_module(module_name)
     tasks = {}
 
     if module is None:
         return tasks
 
-    for name, func in six.iteritems(vars(module)):
+    for name, func in vars(module).items():
         full_name = '%s.%s' % (module_name, name)
         if not hasattr(func, '__call__'):
             # filter out objects that are not callable
             continue
 
         try:
             decorators.get_description_attribute(func)
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/log_utils.py` & `girder-worker-0.9.1.dev6/girder_worker/log_utils.py`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/girder_worker/task.py` & `girder-worker-0.9.1.dev6/girder_worker/task.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 from celery.result import AsyncResult
 
 from girder_worker.context import get_context
 from girder_worker.utils import is_builtin_celery_task, is_revoked
 
 from girder_worker_utils import _walk_obj
 from girder_worker_utils.decorators import describe_function
-import six
 
 
 class GirderAsyncResult(AsyncResult):
     def __init__(self, *args, **kwargs):
         self._job = None
-        super(GirderAsyncResult, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
     @property
     def job(self):
         context = get_context()
         if self._job is None:
             self._job = context.get_async_result_job_property(self)
         return self._job
@@ -67,15 +66,15 @@
         return GirderAsyncResult(task_id, backend=self.backend,
                                  task_name=self.name, app=self.app, **kwargs)
 
     def apply_async(self, args=None, kwargs=None, task_id=None, producer=None,
                     link=None, link_error=None, shadow=None, **options):
 
         if is_builtin_celery_task(self.name):
-            return super(Task, self).apply_async(
+            return super().apply_async(
                 args=args, kwargs=kwargs, task_id=task_id, producer=producer,
                 link=link, link_error=link_error, shadow=shadow, **options)
 
         # Pass girder related job information through to
         # the signals by adding this information to options['headers']
         # This sets defaults for reserved_options based on the class defaults,
         # or values defined by the girder_job() dectorator
@@ -103,15 +102,15 @@
             if options['headers'] is None:
                 options['headers'] = headers
             else:
                 options['headers'].update(headers)
         else:
             options['headers'] = headers
 
-        return super(Task, self).apply_async(
+        return super().apply_async(
             args=args, kwargs=kwargs, task_id=task_id, producer=producer,
             link=link, link_error=link_error, shadow=shadow, serializer='girder_io', **options)
 
     @property
     def canceled(self):
         """
         A property to indicate if a task has been canceled.
@@ -127,35 +126,35 @@
     def call_item_task(self, inputs, outputs={}):
         return self.run.call_item_task(inputs, outputs)
 
     def _maybe_transform_result(self, idx, result, **kwargs):
         try:
             grh = self.request.girder_result_hooks[idx]
             if hasattr(grh, 'transform') and \
-               six.callable(grh.transform):
+               callable(grh.transform):
                 return grh.transform(result, **kwargs)
             return result
         except IndexError:
             return result
 
     def _maybe_transform_argument(self, arg, **kwargs):
-        if hasattr(arg, 'transform') and six.callable(arg.transform):
+        if hasattr(arg, 'transform') and callable(arg.transform):
             return arg.transform(**kwargs)
         return arg
 
     def _maybe_cleanup(self, arg, **kwargs):
-        if hasattr(arg, 'cleanup') and six.callable(arg.cleanup):
+        if hasattr(arg, 'cleanup') and callable(arg.cleanup):
             arg.cleanup(**kwargs)
 
     def __call__(self, *args, **kwargs):
         try:
             _t_args = _walk_obj(args, self._maybe_transform_argument)
             _t_kwargs = _walk_obj(kwargs, self._maybe_transform_argument)
 
-            results = super(Task, self).__call__(*_t_args, **_t_kwargs)
+            results = super().__call__(*_t_args, **_t_kwargs)
 
             if hasattr(self.request, 'girder_result_hooks'):
                 if isinstance(results, tuple):
                     results = tuple([self._maybe_transform_result(i, r)
                                      for i, r in enumerate(results)])
                 else:
                     results = self._maybe_transform_result(0, results)
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker/utils.py` & `girder-worker-0.9.1.dev6/girder_worker/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import time
 
 from girder_worker_utils.tee import Tee, tee_stderr, tee_stdout
 
 import requests
 from requests import HTTPError
 
-import six
-
 # Disable urllib3 warnings about certificate validation. As they are printed in the console, the
 # messages are sent to Girder, creating an infinite loop.
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
 
 BUILTIN_CELERY_TASKS = [
@@ -26,15 +24,15 @@
 
 
 def is_builtin_celery_task(task):
     return task in BUILTIN_CELERY_TASKS
 
 
 def _maybe_model_repr(obj):
-    if hasattr(obj, '_repr_model_') and six.callable(obj._repr_model_):
+    if hasattr(obj, '_repr_model_') and callable(obj._repr_model_):
         return obj._repr_model_()
     return obj
 
 
 # Access to the correct "Inspect" instance for this worker
 _inspector = None
 
@@ -144,15 +142,15 @@
         task_obj._girder_job_handler = handler
         task_obj._girder_job_other_fields = otherFields
         return task_obj
 
     return _girder_job
 
 
-class JobStatus(object):
+class JobStatus:
     INACTIVE = 0
     QUEUED = 1
     RUNNING = 2
     SUCCESS = 3
     ERROR = 4
     CANCELED = 5
 
@@ -165,33 +163,33 @@
 
 class StateTransitionException(Exception):
     pass
 
 
 class TeeCustomWrite(Tee):
     def __init__(self, func, *args, **kwargs):
-        super(TeeCustomWrite, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
         self._write_func = func
 
     def write(self, *args, **kwargs):
         self._write_func(*args, **kwargs)
-        super(TeeCustomWrite, self).write(*args, **kwargs)
+        super().write(*args, **kwargs)
 
 
 @tee_stdout
 class TeeStdOutCustomWrite(TeeCustomWrite):
     pass
 
 
 @tee_stderr
 class TeeStdErrCustomWrite(TeeCustomWrite):
     pass
 
 
-class JobManager(object):
+class JobManager:
     """
     This class can be used to write log messages to Girder by capturing
     stdout/stderr printed within the context and sending them in a
     rate-limited manner to Girder. This is not threadsafe since it changes
     the global values of sys.stdout/sys.stderr.
 
     It also exposes utilities for updating other job fields such as progress
@@ -277,15 +275,15 @@
 
         :param message: The message to append to the job log.
         :type message: str
         :param forceFlush: Whether to force the write of this event to the
             server. Useful if you don't expect another update for some time.
         :type forceFlush: bool
         """
-        if isinstance(message, six.text_type):
+        if isinstance(message, str):
             message = message.encode('utf8')
 
         self._buf += message
 
         if forceFlush or time.time() - self._last > self.interval:
             self._flush()
             self._last = time.time()
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker.egg-info/PKG-INFO` & `girder-worker-0.9.1.dev6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 Metadata-Version: 2.1
 Name: girder-worker
-Version: 0.9.1.dev2
+Version: 0.9.1.dev6
 Summary: Batch execution engine built on celery.
 Home-page: https://github.com/girder/girder_worker
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Provides-Extra: girder
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: pyyaml>=4.2b1
+Requires-Dist: Jinja2>=2.10.1
+Requires-Dist: urllib3>=1.24.2
+Requires-Dist: celery<5; python_version < "3.7"
+Requires-Dist: celery; python_version >= "3.7"
+Requires-Dist: girder-client>=2
+Requires-Dist: pymongo>=3
+Requires-Dist: requests[security]>=2.20.0
+Requires-Dist: setuptools_scm
+Requires-Dist: stevedore
+Requires-Dist: jsonpickle
+Requires-Dist: girder_worker_utils>=0.8.4
+Requires-Dist: docker>=2.6.0
+Provides-Extra: girder
+Requires-Dist: girder>=3.0.0a1; extra == "girder"
+Requires-Dist: girder-jobs>=3.0.0a1; extra == "girder"
 
 |logo| Girder Worker |build-status| |docs-status| |license-badge| |gitter-badge|
 ================================================================================
 
 A flexible, simple script execution engine that integrates with the
 `Girder <http://girder.readthedocs.org>`_ data management system to run
 distributed batch jobs.
@@ -52,9 +67,7 @@
 .. |license-badge| image:: docs/license.png
     :target: https://pypi.python.org/pypi/girder_worker
     :alt: License
 
 .. |gitter-badge| image:: https://badges.gitter.im/Join Chat.svg
     :target: https://gitter.im/girder/girder_worker?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
     :alt: Gitter Chat
-
-
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker.egg-info/SOURCES.txt` & `girder-worker-0.9.1.dev6/girder_worker.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .codecov.yml
 .coveragerc.pytest
 .dockerignore
 .gitignore
 CHANGELOG.rst
-CMakeLists.txt
 CONTRIBUTING.md
 Dockerfile
 HACKING.md
 LICENSE
 MANIFEST.in
 NOTICE
 README.rst
```

### Comparing `girder-worker-0.9.1.dev2/girder_worker.egg-info/entry_points.txt` & `girder-worker-0.9.1.dev6/girder_worker.egg-info/entry_points.txt`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,7 @@
 
 [girder_worker._test_plugins.valid_plugins]
 plugin1 = girder_worker._test_plugins.plugins:TestPlugin1
 plugin2 = girder_worker._test_plugins.plugins:TestPlugin2
 
 [girder_worker_plugins]
 docker = girder_worker.docker:DockerPlugin [docker]
-
```

### Comparing `girder-worker-0.9.1.dev2/scripts/install_requirements.py` & `girder-worker-0.9.1.dev6/scripts/install_requirements.py`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/CHANGELOG.rst` & `girder-worker-0.9.1.dev6/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/CONTRIBUTING.md` & `girder-worker-0.9.1.dev6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/Dockerfile` & `girder-worker-0.9.1.dev6/Dockerfile`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-FROM ubuntu:bionic as base
+FROM ubuntu:22.04 as base
 
 RUN apt-get update && DEBIAN_FRONTEND=noninteractive apt-get install -qy tzdata && \
   apt-get install -qy software-properties-common python3-software-properties && \
   apt-get update && apt-get install -qy \
   build-essential \
   wget \
   python3 \
@@ -11,15 +11,15 @@
   libssl-dev \
   libjpeg-dev \
   zlib1g-dev \
   r-base \
   libpython3-dev && \
   apt-get clean && rm -rf /var/lib/apt/lists/*
 
-RUN wget https://bootstrap.pypa.io/pip/3.6/get-pip.py && python3 get-pip.py
+RUN wget https://bootstrap.pypa.io/pip/get-pip.py && python3 get-pip.py
 
 
 FROM base as build
 
 RUN apt-get update && apt-get install -qy git
 
 COPY ./ /girder_worker/
@@ -31,15 +31,15 @@
 FROM base
 COPY --from=build /girder_worker/dist/*.tar.gz /
 COPY --from=build /girder_worker/docker-entrypoint.sh /docker-entrypoint.sh
 RUN pip3 install /*.tar.gz
 
 RUN useradd -D --shell=/bin/bash && useradd -m worker
 
-RUN chown -R worker:worker /usr/local/lib/python3.6/dist-packages/girder_worker/
+RUN chown -R worker:worker /usr/local/lib/python3.10/dist-packages/girder_worker/
 
 USER worker
 
 RUN girder-worker-config set celery broker "amqp://%(RABBITMQ_USER)s:%(RABBITMQ_PASS)s@%(RABBITMQ_HOST)s/"
 
 
 VOLUME /girder_worker
```

### Comparing `girder-worker-0.9.1.dev2/HACKING.md` & `girder-worker-0.9.1.dev6/HACKING.md`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/LICENSE` & `girder-worker-0.9.1.dev6/LICENSE`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/README.rst` & `girder-worker-0.9.1.dev6/README.rst`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/TRANSITION.md` & `girder-worker-0.9.1.dev6/TRANSITION.md`

 * *Files identical despite different names*

### Comparing `girder-worker-0.9.1.dev2/setup.py` & `girder-worker-0.9.1.dev6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,29 +84,30 @@
     license='Apache 2.0',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'License :: OSI Approved :: Apache Software License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8'
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
 
     ],
     extras_require=extras_require,
     packages=setuptools.find_packages(
         exclude=('tests.*', 'tests')
     ),
     include_package_data=True,
     cmdclass={
         'install': CustomInstall
     },
     install_requires=install_reqs,
-    python_requires='>=3.6',
+    python_requires='>=3.8',
     zip_safe=False,
     entry_points={
         'console_scripts': [
             'girder-worker = girder_worker.__main__:main',
             'girder-worker-config = girder_worker.configure:main'
         ],
         'girder_worker_plugins': [
```

### Comparing `girder-worker-0.9.1.dev2/tox.ini` & `girder-worker-0.9.1.dev6/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,53 @@
 [tox]
-envlist = coverage-erase, py36, lint, coverage-report, py310
+envlist = coverage-erase, py38, lint, coverage-report, py311
 skip_missing_interpreters = false
 
 [testenv:coverage-erase]
 skip_install = true
 skipsdist = true
-basepython = python3.6
 deps = coverage
 commands = coverage erase --rcfile=.coveragerc.pytest
 
 [testenv]
 commands = pytest \
   --cov=girder_worker \
   --cov-append \
   --cov-config=.coveragerc.pytest \
   # Surpress printing coverage, defer this to testenv:coverage-report
   --cov-report= \
   --mock-db \
   {posargs}
 
-[testenv:py36]
+[testenv:py38]
 deps = -rrequirements.txt
 
-[testenv:py310]
+[testenv:py311]
 deps =
   -rrequirements.in
   -rrequirements-dev.in
-basepython = python3.10
 
-# This report is used to merge coverage reports from testenv and from
-# the legacy tests run by ctest. When just running 'tox' it will print
-# the pytest coverage report. When running ctest && tox it will print
-# the combine coverage.
 [testenv:coverage-report]
 skip_install = true
-basepython = python3.6
 deps = coverage
 commands =
   - coverage combine
   coverage report
 
 [testenv:lint]
 skip_install = true
-basepython = python3.6
 deps =
   flake8
   flake8-docstrings
   flake8-quotes
 commands = flake8 {posargs} girder_worker tests
 
 [testenv:release]
 skip_install = true
 skipsdist = true
-basepython = python3.6
 passenv =
   CIRCLE_BRANCH
   TWINE_USERNAME
   TWINE_PASSWORD
   TWINE_REPOSITORY_URL
 deps =
   setuptools_scm
@@ -68,14 +59,15 @@
 [pytest]
 testpaths =
   tests
 addopts =
   # Ignore the integration tests directory which has its own method of
   # running tests.
   --ignore=tests/integration/
+  --showlocals
 markers =
   namespace: namespace for plugin entrypoints
 
 [flake8]
 exclude =
  # Prevent running flake8 against ansible roles downloaded for use
  # with integration framework.
```

### Comparing `girder-worker-0.9.1.dev2/PKG-INFO` & `girder-worker-0.9.1.dev6/girder_worker.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,43 @@
 Metadata-Version: 2.1
 Name: girder-worker
-Version: 0.9.1.dev2
+Version: 0.9.1.dev6
 Summary: Batch execution engine built on celery.
 Home-page: https://github.com/girder/girder_worker
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.6
-Provides-Extra: girder
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.8
 License-File: LICENSE
 License-File: NOTICE
+Requires-Dist: pyyaml>=4.2b1
+Requires-Dist: Jinja2>=2.10.1
+Requires-Dist: urllib3>=1.24.2
+Requires-Dist: celery<5; python_version < "3.7"
+Requires-Dist: celery; python_version >= "3.7"
+Requires-Dist: girder-client>=2
+Requires-Dist: pymongo>=3
+Requires-Dist: requests[security]>=2.20.0
+Requires-Dist: setuptools_scm
+Requires-Dist: stevedore
+Requires-Dist: jsonpickle
+Requires-Dist: girder_worker_utils>=0.8.4
+Requires-Dist: docker>=2.6.0
+Provides-Extra: girder
+Requires-Dist: girder>=3.0.0a1; extra == "girder"
+Requires-Dist: girder-jobs>=3.0.0a1; extra == "girder"
 
 |logo| Girder Worker |build-status| |docs-status| |license-badge| |gitter-badge|
 ================================================================================
 
 A flexible, simple script execution engine that integrates with the
 `Girder <http://girder.readthedocs.org>`_ data management system to run
 distributed batch jobs.
@@ -52,9 +67,7 @@
 .. |license-badge| image:: docs/license.png
     :target: https://pypi.python.org/pypi/girder_worker
     :alt: License
 
 .. |gitter-badge| image:: https://badges.gitter.im/Join Chat.svg
     :target: https://gitter.im/girder/girder_worker?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
     :alt: Gitter Chat
-
-
```

