# Comparing `tmp/kubeyard-1.0.0.tar.gz` & `tmp/kubeyard-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kubeyard-1.0.0.tar", last modified: Fri Dec  8 12:36:36 2023, max compression
+gzip compressed data, was "kubeyard-1.1.0.tar", last modified: Tue May 21 10:22:55 2024, max compression
```

## Comparing `kubeyard-1.0.0.tar` & `kubeyard-1.1.0.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     2201 2023-12-08 12:36:36.000000 kubeyard-1.0.0/CHANGELOG.md
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1511 2023-12-08 12:36:36.000000 kubeyard-1.0.0/LICENSE
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      210 2023-12-08 12:36:36.000000 kubeyard-1.0.0/MANIFEST.in
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1931 2023-12-08 12:36:36.976469 kubeyard-1.0.0/PKG-INFO
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1155 2023-12-08 12:36:36.000000 kubeyard-1.0.0/README.md
--rw-rw-r--   0 kubag     (1000) kubag     (1000)       84 2023-12-08 12:36:36.000000 kubeyard-1.0.0/base_requirements.txt
--rw-rw-r--   0 kubag     (1000) kubag     (1000)       30 2023-12-08 12:36:36.000000 kubeyard-1.0.0/dev_requirements.txt
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.960469 kubeyard-1.0.0/kubeyard/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/__init__.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      261 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/ascii_art.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     2103 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/base_command.py
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.964469 kubeyard-1.0.0/kubeyard/commands/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1035 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/__init__.py
--rwxrwxr-x   0 kubag     (1000) kubag     (1000)     1257 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/bash_completion.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      924 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/build.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1352 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/custom_script.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      548 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/debug.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)    14861 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/deploy.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)    10066 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/dev_requirements.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     5936 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/devel.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1499 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/fix_code_style.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     3717 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/global_commands.py
--rwxrwxr-x   0 kubag     (1000) kubag     (1000)     2870 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/init.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      647 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/push.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     3068 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/shell.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     7983 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/test.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1085 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/commands/update_requirements.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     7079 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/context_factories.py
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.952468 kubeyard-1.0.0/kubeyard/definitions/
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.964469 kubeyard-1.0.0/kubeyard/definitions/dev_requirements/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      647 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/definitions/dev_requirements/cassandra.yaml
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      681 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/definitions/dev_requirements/cockroachdb.yaml
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      689 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/definitions/dev_requirements/elasticsearch.yaml
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      530 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/definitions/dev_requirements/postgres.yaml
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      399 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/definitions/dev_requirements/pubsub-emulator.yaml
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      385 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/definitions/dev_requirements/rabbitmq.yaml
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      491 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/definitions/dev_requirements/redis.yaml
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     2895 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/dependencies.py
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.964469 kubeyard-1.0.0/kubeyard/entrypoints/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/entrypoints/__init__.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1911 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/entrypoints/custom_command_loader.py
--rwxrwxr-x   0 kubag     (1000) kubag     (1000)     7767 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/entrypoints/kubeyard.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     2699 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/files_generator.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      119 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/io_utils.py
--rwxrwxr-x   0 kubag     (1000) kubag     (1000)     6663 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/kubernetes.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1596 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/logging.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     7665 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/minikube.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1561 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/settings.py
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.964469 kubeyard-1.0.0/kubeyard/templates/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      648 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/kubeyard-completion.sh
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.956468 kubeyard-1.0.0/kubeyard/templates/new_repositories/
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.956468 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.964469 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/config/
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.952468 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/config/kubernetes/
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.964469 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/config/kubernetes/deploy/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      260 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/config/kubernetes/deploy/01_service.yml.template
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      593 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/config/kubernetes/deploy/02_deployment.yml.template
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      201 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/config/kubernetes/deploy/03_ingress.yml.template
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.968469 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/config/kubernetes/dev_secrets/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/config/kubernetes/dev_secrets/secrets.yml
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.968469 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/config/kubernetes/development_overrides/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      177 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/config/kubernetes/development_overrides/02_deployment.yml.template
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      381 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/config/kubeyard.yml.template
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.968469 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      129 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/Dockerfile.template
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.968469 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/requirements/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      239 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/requirements/python.txt
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.968469 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/__init__.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)       30 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/base_requirements.txt
--rwxrwxr-x   0 kubag     (1000) kubag     (1000)      563 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/manage.py.template
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      572 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/setup.py.template
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.968469 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/tests/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/tests/__init__.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)       80 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/tests/test_hello_world.py.template
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      192 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/uwsgi.ini.template
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.968469 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/__init__.py
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.968469 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/commands/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/commands/__init__.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      478 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/commands/start_service.py.template
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     3143 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/settings.py.template
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      761 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/urls.py.template
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      426 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/wsgi.py.template
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.968469 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/scripts/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      135 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/django/scripts/.gitkeep
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.956468 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.968469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/config/
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.956468 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/config/kubernetes/
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.968469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/config/kubernetes/development_overrides/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      247 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/config/kubernetes/development_overrides/01_service.yml.template
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      276 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/config/kubernetes/development_overrides/02_live_reload_service.yml.template
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1593 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/config/kubernetes/development_overrides/03_deployment.yml.template
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1349 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/config/kubeyard.yml.template
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.968469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      412 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/Dockerfile
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.972469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)       60 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/.bowerrc
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      368 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/.editorconfig
--rw-rw-r--   0 kubag     (1000) kubag     (1000)       55 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/.ember-cli
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      188 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/.eslintrc.js
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      346 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/.gitignore
--rw-rw-r--   0 kubag     (1000) kubag     (1000)       37 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/.watchmanconfig
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.972469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      362 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/app.js
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.972469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/components/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/components/.gitkeep
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.972469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/controllers/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/controllers/.gitkeep
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.972469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/helpers/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/helpers/.gitkeep
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      669 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/index.html
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.972469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/models/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/models/.gitkeep
--rw-rw-r--   0 kubag     (1000) kubag     (1000)       65 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/resolver.js
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      224 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/router.js
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.972469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/routes/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/routes/.gitkeep
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.972469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/styles/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/styles/app.css
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.972469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/templates/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      143 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/templates/application.hbs
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.972469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/templates/components/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/templates/components/.gitkeep
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.972469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/bin/
--rwxrwxr-x   0 kubag     (1000) kubag     (1000)       99 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/bin/collect_statics_tar.sh
--rwxrwxr-x   0 kubag     (1000) kubag     (1000)       23 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/bin/run_tests.sh
--rw-rw-r--   0 kubag     (1000) kubag     (1000)       51 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/bower.json
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.972469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/config/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1165 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/config/environment.js
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      164 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/config/target.js
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      815 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/ember-cli-build.js
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      850 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/package.json
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/public/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      585 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/public/crossdomain.xml
--rw-rw-r--   0 kubag     (1000) kubag     (1000)       51 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/public/robots.txt
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      206 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/testem.js
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)       55 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/.eslintrc.js
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/helpers/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      117 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/helpers/destroy-app.js
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      609 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/helpers/module-for-acceptance.js
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      255 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/helpers/resolver.js
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      474 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/helpers/start-app.js
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1056 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/index.html
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/integration/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/integration/.gitkeep
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      162 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/test-helper.js
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/unit/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/unit/.gitkeep
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/vendor/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/vendor/.gitkeep
--rw-rw-r--   0 kubag     (1000) kubag     (1000)   194187 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/yarn.lock
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/scripts/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      135 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/scripts/.gitkeep
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.956468 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/config/
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.956468 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/config/kubernetes/
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/config/kubernetes/deploy/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      223 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/config/kubernetes/deploy/01_service.yml.template
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      592 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/config/kubernetes/deploy/02_deployment.yml.template
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/config/kubernetes/dev_secrets/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/config/kubernetes/dev_secrets/secrets.yml
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/config/kubernetes/development_overrides/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      177 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/config/kubernetes/development_overrides/02_deployment.yml.template
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      338 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/config/kubeyard.yml.template
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/docker/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)       40 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/docker/Dockerfile
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/docker/requirements/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/docker/requirements/python.txt
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/docker/source/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/docker/source/__init__.py
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/docker/source/base_requirements.txt
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      406 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/docker/source/setup.py.template
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/docker/source/tests/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/docker/source/tests/__init__.py
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.976469 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/scripts/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      135 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard/templates/new_repositories/python/scripts/.gitkeep
-drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2023-12-08 12:36:36.960469 kubeyard-1.0.0/kubeyard.egg-info/
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1931 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard.egg-info/PKG-INFO
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     7902 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard.egg-info/SOURCES.txt
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        1 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard.egg-info/dependency_links.txt
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      148 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard.egg-info/entry_points.txt
--rw-rw-r--   0 kubag     (1000) kubag     (1000)       84 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard.egg-info/requires.txt
--rw-rw-r--   0 kubag     (1000) kubag     (1000)        9 2023-12-08 12:36:36.000000 kubeyard-1.0.0/kubeyard.egg-info/top_level.txt
--rw-rw-r--   0 kubag     (1000) kubag     (1000)      250 2023-12-08 12:36:36.980469 kubeyard-1.0.0/setup.cfg
--rw-rw-r--   0 kubag     (1000) kubag     (1000)     1995 2023-12-08 12:36:36.000000 kubeyard-1.0.0/setup.py
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.496798 kubeyard-1.1.0/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     2416 2024-05-21 10:22:55.000000 kubeyard-1.1.0/CHANGELOG.md
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1511 2024-05-21 10:22:55.000000 kubeyard-1.1.0/LICENSE
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      210 2024-05-21 10:22:55.000000 kubeyard-1.1.0/MANIFEST.in
+-rw-r--r--   0 kubag     (1000) kubag     (1000)     2101 2024-05-21 10:22:55.496798 kubeyard-1.1.0/PKG-INFO
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1155 2024-05-21 10:22:55.000000 kubeyard-1.1.0/README.md
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)       84 2024-05-21 10:22:55.000000 kubeyard-1.1.0/base_requirements.txt
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)       30 2024-05-21 10:22:55.000000 kubeyard-1.1.0/dev_requirements.txt
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.484798 kubeyard-1.1.0/kubeyard/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/__init__.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      261 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/ascii_art.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     2103 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/base_command.py
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.484798 kubeyard-1.1.0/kubeyard/commands/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1035 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/__init__.py
+-rwxrwxr-x   0 kubag     (1000) kubag     (1000)     1257 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/bash_completion.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      924 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/build.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1352 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/custom_script.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      548 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/debug.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)    14861 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/deploy.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)    10066 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/dev_requirements.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     5936 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/devel.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1499 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/fix_code_style.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     3717 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/global_commands.py
+-rwxrwxr-x   0 kubag     (1000) kubag     (1000)     2870 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/init.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      647 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/push.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     3068 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/shell.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     7983 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/test.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1085 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/commands/update_requirements.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     7079 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/context_factories.py
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.476798 kubeyard-1.1.0/kubeyard/definitions/
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/definitions/dev_requirements/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      647 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/definitions/dev_requirements/cassandra.yaml
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      681 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/definitions/dev_requirements/cockroachdb.yaml
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      689 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/definitions/dev_requirements/elasticsearch.yaml
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      530 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/definitions/dev_requirements/postgres.yaml
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      399 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/definitions/dev_requirements/pubsub-emulator.yaml
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      385 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/definitions/dev_requirements/rabbitmq.yaml
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      491 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/definitions/dev_requirements/redis.yaml
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     2895 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/dependencies.py
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/entrypoints/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/entrypoints/__init__.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1911 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/entrypoints/custom_command_loader.py
+-rwxrwxr-x   0 kubag     (1000) kubag     (1000)     7767 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/entrypoints/kubeyard.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     2699 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/files_generator.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      119 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/io_utils.py
+-rwxrwxr-x   0 kubag     (1000) kubag     (1000)     6663 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/kubernetes.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1596 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/logging.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     7665 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/minikube.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1561 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/settings.py
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      648 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/kubeyard-completion.sh
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.480798 kubeyard-1.1.0/kubeyard/templates/new_repositories/
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.480798 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/config/
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.480798 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/config/kubernetes/
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/config/kubernetes/deploy/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      260 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/config/kubernetes/deploy/01_service.yml.template
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      593 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/config/kubernetes/deploy/02_deployment.yml.template
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      201 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/config/kubernetes/deploy/03_ingress.yml.template
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/config/kubernetes/dev_secrets/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/config/kubernetes/dev_secrets/secrets.yml
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/config/kubernetes/development_overrides/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      177 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/config/kubernetes/development_overrides/02_deployment.yml.template
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      381 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/config/kubeyard.yml.template
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      129 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/Dockerfile.template
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/requirements/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      239 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/requirements/python.txt
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/__init__.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)       30 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/base_requirements.txt
+-rwxrwxr-x   0 kubag     (1000) kubag     (1000)      563 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/manage.py.template
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      572 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/setup.py.template
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/tests/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/tests/__init__.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)       80 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/tests/test_hello_world.py.template
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      192 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/uwsgi.ini.template
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/__init__.py
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/commands/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/commands/__init__.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      478 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/commands/start_service.py.template
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     3143 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/settings.py.template
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      761 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/urls.py.template
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      426 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/wsgi.py.template
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/scripts/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      135 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/django/scripts/.gitkeep
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.480798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/config/
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.480798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/config/kubernetes/
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/config/kubernetes/development_overrides/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      247 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/config/kubernetes/development_overrides/01_service.yml.template
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      276 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/config/kubernetes/development_overrides/02_live_reload_service.yml.template
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1593 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/config/kubernetes/development_overrides/03_deployment.yml.template
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1349 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/config/kubeyard.yml.template
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.488798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      412 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/Dockerfile
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)       60 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/.bowerrc
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      368 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/.editorconfig
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)       55 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/.ember-cli
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      188 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/.eslintrc.js
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      346 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/.gitignore
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)       37 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/.watchmanconfig
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      362 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/app.js
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/components/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/components/.gitkeep
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/controllers/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/controllers/.gitkeep
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/helpers/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/helpers/.gitkeep
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      669 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/index.html
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/models/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/models/.gitkeep
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)       65 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/resolver.js
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      224 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/router.js
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/routes/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/routes/.gitkeep
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/styles/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/styles/app.css
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/templates/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      143 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/templates/application.hbs
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/templates/components/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/templates/components/.gitkeep
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/bin/
+-rwxrwxr-x   0 kubag     (1000) kubag     (1000)       99 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/bin/collect_statics_tar.sh
+-rwxrwxr-x   0 kubag     (1000) kubag     (1000)       23 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/bin/run_tests.sh
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)       51 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/bower.json
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/config/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1165 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/config/environment.js
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      164 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/config/target.js
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      815 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/ember-cli-build.js
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      850 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/package.json
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/public/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      585 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/public/crossdomain.xml
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)       51 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/public/robots.txt
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      206 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/testem.js
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)       55 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/.eslintrc.js
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/helpers/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      117 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/helpers/destroy-app.js
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      609 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/helpers/module-for-acceptance.js
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      255 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/helpers/resolver.js
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      474 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/helpers/start-app.js
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1056 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/index.html
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/integration/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/integration/.gitkeep
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      162 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/test-helper.js
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/unit/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/unit/.gitkeep
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/vendor/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/vendor/.gitkeep
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)   194187 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/yarn.lock
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/scripts/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      135 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/scripts/.gitkeep
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.480798 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/config/
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.480798 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/config/kubernetes/
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/config/kubernetes/deploy/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      223 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/config/kubernetes/deploy/01_service.yml.template
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      592 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/config/kubernetes/deploy/02_deployment.yml.template
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/config/kubernetes/dev_secrets/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/config/kubernetes/dev_secrets/secrets.yml
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/config/kubernetes/development_overrides/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      177 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/config/kubernetes/development_overrides/02_deployment.yml.template
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      338 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/config/kubeyard.yml.template
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.492798 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/docker/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)       40 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/docker/Dockerfile
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.496798 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/docker/requirements/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/docker/requirements/python.txt
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.496798 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/docker/source/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/docker/source/__init__.py
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/docker/source/base_requirements.txt
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      406 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/docker/source/setup.py.template
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.496798 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/docker/source/tests/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/docker/source/tests/__init__.py
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.496798 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/scripts/
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      135 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard/templates/new_repositories/python/scripts/.gitkeep
+drwxrwxr-x   0 kubag     (1000) kubag     (1000)        0 2024-05-21 10:22:55.496798 kubeyard-1.1.0/kubeyard.egg-info/
+-rw-r--r--   0 kubag     (1000) kubag     (1000)     2101 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard.egg-info/PKG-INFO
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     7902 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard.egg-info/SOURCES.txt
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        1 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard.egg-info/dependency_links.txt
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      148 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard.egg-info/entry_points.txt
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)       84 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard.egg-info/requires.txt
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)        9 2024-05-21 10:22:55.000000 kubeyard-1.1.0/kubeyard.egg-info/top_level.txt
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)      205 2024-05-21 10:22:55.496798 kubeyard-1.1.0/setup.cfg
+-rw-rw-r--   0 kubag     (1000) kubag     (1000)     1947 2024-05-21 10:22:55.000000 kubeyard-1.1.0/setup.py
```

### Comparing `kubeyard-1.0.0/CHANGELOG.md` & `kubeyard-1.1.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+## 1.1.0 (2024-05-21)
+---------------------
+
+- Support applying HorizontalPodAutoscaler (via kubepy).
+- Run linting with tox and GitHub Actions.
+- Drop support for Python 3.7 and 3.8, add support for Python 3.12.
+
+
 ## 1.0.0 (2023-12-08)
 ----------------------
 
 - Add support for "docker" driver in minikube.
 
 
 ## 0.13.0 (2023-11-08)
```

### Comparing `kubeyard-1.0.0/LICENSE` & `kubeyard-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/PKG-INFO` & `kubeyard-1.1.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: kubeyard
-Version: 1.0.0
+Version: 1.1.0
 Summary: A utility to develop, test and deploy Kubernetes microservices.
 Home-page: https://github.com/socialwifi/kubeyard
 Author: Social WiFi
 Author-email: it@socialwifi.com
 License: BSD
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: colorlog
+Requires-Dist: jinja2
+Requires-Dist: kubepy>=1.20.0
+Requires-Dist: pyYAML
+Requires-Dist: cached-property
+Requires-Dist: sh<2
+Requires-Dist: pyfiglet
+Requires-Dist: termcolor
 
 # kubeyard
 [![Latest Version](https://img.shields.io/pypi/v/kubeyard.svg)](https://pypi.python.org/pypi/kubeyard/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/kubeyard.svg)](https://pypi.python.org/pypi/kubeyard/)
 [![Wheel Status](https://img.shields.io/pypi/wheel/kubeyard.svg)](https://pypi.python.org/pypi/kubeyard/)
 [![License](https://img.shields.io/pypi/l/kubeyard.svg)](https://github.com/socialwifi/kubeyard/blob/master/LICENSE)
 [![Build](https://img.shields.io/circleci/project/github/socialwifi/kubeyard/master.svg)](https://circleci.com/gh/socialwifi/kubeyard)
```

### Comparing `kubeyard-1.0.0/README.md` & `kubeyard-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/base_command.py` & `kubeyard-1.1.0/kubeyard/base_command.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/__init__.py` & `kubeyard-1.1.0/kubeyard/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/bash_completion.py` & `kubeyard-1.1.0/kubeyard/commands/bash_completion.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/build.py` & `kubeyard-1.1.0/kubeyard/commands/build.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/custom_script.py` & `kubeyard-1.1.0/kubeyard/commands/custom_script.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/debug.py` & `kubeyard-1.1.0/kubeyard/commands/debug.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/deploy.py` & `kubeyard-1.1.0/kubeyard/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/dev_requirements.py` & `kubeyard-1.1.0/kubeyard/commands/dev_requirements.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/devel.py` & `kubeyard-1.1.0/kubeyard/commands/devel.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/fix_code_style.py` & `kubeyard-1.1.0/kubeyard/commands/fix_code_style.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/global_commands.py` & `kubeyard-1.1.0/kubeyard/commands/global_commands.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/init.py` & `kubeyard-1.1.0/kubeyard/commands/init.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/push.py` & `kubeyard-1.1.0/kubeyard/commands/push.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/shell.py` & `kubeyard-1.1.0/kubeyard/commands/shell.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/test.py` & `kubeyard-1.1.0/kubeyard/commands/test.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/commands/update_requirements.py` & `kubeyard-1.1.0/kubeyard/commands/update_requirements.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/context_factories.py` & `kubeyard-1.1.0/kubeyard/context_factories.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/definitions/dev_requirements/cassandra.yaml` & `kubeyard-1.1.0/kubeyard/definitions/dev_requirements/cassandra.yaml`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/definitions/dev_requirements/cockroachdb.yaml` & `kubeyard-1.1.0/kubeyard/definitions/dev_requirements/cockroachdb.yaml`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/definitions/dev_requirements/elasticsearch.yaml` & `kubeyard-1.1.0/kubeyard/definitions/dev_requirements/elasticsearch.yaml`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/definitions/dev_requirements/postgres.yaml` & `kubeyard-1.1.0/kubeyard/definitions/dev_requirements/postgres.yaml`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/dependencies.py` & `kubeyard-1.1.0/kubeyard/dependencies.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/entrypoints/custom_command_loader.py` & `kubeyard-1.1.0/kubeyard/entrypoints/custom_command_loader.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/entrypoints/kubeyard.py` & `kubeyard-1.1.0/kubeyard/entrypoints/kubeyard.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/files_generator.py` & `kubeyard-1.1.0/kubeyard/files_generator.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/kubernetes.py` & `kubeyard-1.1.0/kubeyard/kubernetes.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/logging.py` & `kubeyard-1.1.0/kubeyard/logging.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/minikube.py` & `kubeyard-1.1.0/kubeyard/minikube.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/settings.py` & `kubeyard-1.1.0/kubeyard/settings.py`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/kubeyard-completion.sh` & `kubeyard-1.1.0/kubeyard/templates/kubeyard-completion.sh`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/django/config/kubernetes/deploy/02_deployment.yml.template` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/django/config/kubernetes/deploy/02_deployment.yml.template`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/manage.py.template` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/manage.py.template`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/setup.py.template` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/setup.py.template`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/settings.py.template` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/settings.py.template`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/urls.py.template` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/django/docker/source/{{ UNDERSCORED_PROJECT_NAME }}/urls.py.template`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/config/kubernetes/development_overrides/03_deployment.yml.template` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/config/kubernetes/development_overrides/03_deployment.yml.template`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/config/kubeyard.yml.template` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/config/kubeyard.yml.template`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/app/index.html` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/app/index.html`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/config/environment.js` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/config/environment.js`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/ember-cli-build.js` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/ember-cli-build.js`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/package.json` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/package.json`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/public/crossdomain.xml` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/public/crossdomain.xml`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/helpers/module-for-acceptance.js` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/helpers/module-for-acceptance.js`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/tests/index.html` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/tests/index.html`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/ember/docker/source/yarn.lock` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/ember/docker/source/yarn.lock`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard/templates/new_repositories/python/config/kubernetes/deploy/02_deployment.yml.template` & `kubeyard-1.1.0/kubeyard/templates/new_repositories/python/config/kubernetes/deploy/02_deployment.yml.template`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/kubeyard.egg-info/PKG-INFO` & `kubeyard-1.1.0/kubeyard.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 Metadata-Version: 2.1
 Name: kubeyard
-Version: 1.0.0
+Version: 1.1.0
 Summary: A utility to develop, test and deploy Kubernetes microservices.
 Home-page: https://github.com/socialwifi/kubeyard
 Author: Social WiFi
 Author-email: it@socialwifi.com
 License: BSD
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: click
+Requires-Dist: colorlog
+Requires-Dist: jinja2
+Requires-Dist: kubepy>=1.20.0
+Requires-Dist: pyYAML
+Requires-Dist: cached-property
+Requires-Dist: sh<2
+Requires-Dist: pyfiglet
+Requires-Dist: termcolor
 
 # kubeyard
 [![Latest Version](https://img.shields.io/pypi/v/kubeyard.svg)](https://pypi.python.org/pypi/kubeyard/)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/kubeyard.svg)](https://pypi.python.org/pypi/kubeyard/)
 [![Wheel Status](https://img.shields.io/pypi/wheel/kubeyard.svg)](https://pypi.python.org/pypi/kubeyard/)
 [![License](https://img.shields.io/pypi/l/kubeyard.svg)](https://github.com/socialwifi/kubeyard/blob/master/LICENSE)
 [![Build](https://img.shields.io/circleci/project/github/socialwifi/kubeyard/master.svg)](https://circleci.com/gh/socialwifi/kubeyard)
```

### Comparing `kubeyard-1.0.0/kubeyard.egg-info/SOURCES.txt` & `kubeyard-1.1.0/kubeyard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kubeyard-1.0.0/setup.py` & `kubeyard-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 def get_long_description():
     with open('README.md') as readme_file:
         return readme_file.read()
 
 
 setup(
     name='kubeyard',
-    version='1.0.0',
+    version='1.1.0',
     description='A utility to develop, test and deploy Kubernetes microservices.',
     long_description=get_long_description(),
     long_description_content_type='text/markdown',
     author='Social WiFi',
     author_email='it@socialwifi.com',
     url='https://github.com/socialwifi/kubeyard',
     packages=find_packages(exclude=['tests']),
@@ -45,14 +45,13 @@
     license='BSD',
     classifiers=[
         'Environment :: Console',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
     ],
 )
```

