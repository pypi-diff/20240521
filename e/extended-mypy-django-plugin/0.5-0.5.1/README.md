# Comparing `tmp/extended_mypy_django_plugin-0.5.tar.gz` & `tmp/extended_mypy_django_plugin-0.5.1.tar.gz`

## Comparing `extended_mypy_django_plugin-0.5.tar` & `extended_mypy_django_plugin-0.5.1.tar`

### file list

```diff
@@ -1,99 +1,99 @@
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/.readthedocs.yaml
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/DEVELOPMENT.rst
--rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/find
--rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/format
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/lint
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/mypy.ini
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/pytest.ini
--rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/run.sh
--rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/test.sh
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/tox.ini
--rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/types
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/.github/workflows/ciold.yml
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/.github/workflows/lintold.yml
--rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/.github/workflows/release.yml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/.gitignore
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/README.rst
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/conf.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/index.rst
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/_static/css/extra.css
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/api/changelog.rst
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/api/installation.rst
--rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/api/primer.rst
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/api/tracking-changes.rst
--rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/api/usage.rst
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/api/internals/actions.rst
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/api/internals/config.rst
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/api/internals/dependencies.rst
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/api/internals/hook.rst
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/api/internals/index.rst
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/api/internals/plugin.rst
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/api/internals/reports.rst
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/docs/api/internals/store.rst
--rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/manage.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/mypy.ini
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/pyproject.toml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/__init__.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/asgi.py
--rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/settings.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/urls.py
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/version.py
--rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/views.py
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/exampleapp/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/exampleapp/apps.py
--rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/exampleapp/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/exampleapp/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/exampleapp2/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/exampleapp2/apps.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/exampleapp2/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/example/djangoexample/exampleapp2/migrations/__init__.py
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/__init__.py
--rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/annotations.py
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/entry.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/py.typed
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/version.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/__init__.py
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/_config.py
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/_debug.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/_dependencies.py
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/_hook.py
--rw-r--r--   0        0        0     8747 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/_plugin.py
--rw-r--r--   0        0        0    14982 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/_reports.py
--rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/_store.py
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/actions/__init__.py
--rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/actions/_sem_analyze.py
--rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/actions/_type_analyze.py
--rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/actions/_type_checker.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/scripts/__init__.py
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/scripts/find_models.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/scripts/get_installed_apps.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/scripts/__init__.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/scripts/make_old.patch
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/scripts/mypy.ini
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/scripts/py.typed
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/scripts/test_settings.py
--rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/scripts/tests_extension_hook.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/scripts/myapp/__init__.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/scripts/myapp/apps.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/scripts/myapp/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/scripts/myapp2/__init__.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/scripts/myapp2/apps.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/scripts/myapp2/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/tests/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/tests/test_concrete_annotation.yml
--rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/tests/test_works.yml
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/tools/.gitignore
--rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/tools/bootstrap_venvstarter.py
--rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/tools/devtools.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/tools/requirements.dev.txt
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/tools/requirements.docs.txt
--rwxr-xr-x   0        0        0     1108 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/tools/venv
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/LICENSE
--rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/README.rst
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/pyproject.toml
--rw-r--r--   0        0        0     2248 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5/PKG-INFO
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.readthedocs.yaml
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/DEVELOPMENT.rst
+-rwxr-xr-x   0        0        0      359 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/find
+-rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/format
+-rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/lint
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/mypy.ini
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/pytest.ini
+-rwxr-xr-x   0        0        0     1195 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/run.sh
+-rwxr-xr-x   0        0        0      171 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/test.sh
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tox.ini
+-rwxr-xr-x   0        0        0      199 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/types
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.github/workflows/ciold.yml
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.github/workflows/lintold.yml
+-rw-r--r--   0        0        0     1477 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/.gitignore
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/README.rst
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/conf.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/index.rst
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/_static/css/extra.css
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/changelog.rst
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/installation.rst
+-rw-r--r--   0        0        0     6405 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/primer.rst
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/tracking-changes.rst
+-rw-r--r--   0        0        0     3489 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/usage.rst
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/actions.rst
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/config.rst
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/dependencies.rst
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/hook.rst
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/index.rst
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/plugin.rst
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/reports.rst
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/docs/api/internals/store.rst
+-rwxr-xr-x   0        0        0      670 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/manage.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/mypy.ini
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/pyproject.toml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/__init__.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/asgi.py
+-rw-r--r--   0        0        0     3506 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/settings.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/urls.py
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/version.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/views.py
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp/apps.py
+-rw-r--r--   0        0        0     1003 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp2/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp2/apps.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp2/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp2/migrations/__init__.py
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/__init__.py
+-rw-r--r--   0        0        0     2483 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/annotations.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/entry.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/py.typed
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/version.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/__init__.py
+-rw-r--r--   0        0        0     4794 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_config.py
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_debug.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_dependencies.py
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_hook.py
+-rw-r--r--   0        0        0     8914 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_plugin.py
+-rw-r--r--   0        0        0    15489 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_reports.py
+-rw-r--r--   0        0        0     8851 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_store.py
+-rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/__init__.py
+-rw-r--r--   0        0        0     2683 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/_sem_analyze.py
+-rw-r--r--   0        0        0     3797 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/_type_analyze.py
+-rw-r--r--   0        0        0     6893 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/_type_checker.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/scripts/__init__.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/scripts/determine_django_state.py
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/scripts/find_models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/__init__.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/make_old.patch
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/mypy.ini
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/py.typed
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/test_settings.py
+-rw-r--r--   0        0        0     5987 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/tests_extension_hook.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/myapp/__init__.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/myapp/apps.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/myapp/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/myapp2/__init__.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/myapp2/apps.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/scripts/myapp2/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tests/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tests/test_concrete_annotation.yml
+-rw-r--r--   0        0        0     3045 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tests/test_works.yml
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tools/.gitignore
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tools/bootstrap_venvstarter.py
+-rw-r--r--   0        0        0     4146 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tools/devtools.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tools/requirements.dev.txt
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tools/requirements.docs.txt
+-rwxr-xr-x   0        0        0     1108 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/tools/venv
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/README.rst
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 extended_mypy_django_plugin-0.5.1/PKG-INFO
```

### Comparing `extended_mypy_django_plugin-0.5/DEVELOPMENT.rst` & `extended_mypy_django_plugin-0.5.1/DEVELOPMENT.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/run.sh` & `extended_mypy_django_plugin-0.5.1/run.sh`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/.github/workflows/ci.yml` & `extended_mypy_django_plugin-0.5.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/.github/workflows/ciold.yml` & `extended_mypy_django_plugin-0.5.1/.github/workflows/ciold.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/.github/workflows/lint.yml` & `extended_mypy_django_plugin-0.5.1/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/.github/workflows/lintold.yml` & `extended_mypy_django_plugin-0.5.1/.github/workflows/lintold.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/.github/workflows/release.yml` & `extended_mypy_django_plugin-0.5.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/docs/conf.py` & `extended_mypy_django_plugin-0.5.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/docs/api/installation.rst` & `extended_mypy_django_plugin-0.5.1/docs/api/installation.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 Installation
 ============
 
-.. note:: This plugin hasn't been published on pypi at this point
+Install from pypi::
+
+    python -m pip install extended-mypy-django-plugin
 
 Enabling this plugin in a project is adding either to ``mypy.ini``::
 
     [mypy]
     plugins =
         extended_mypy_django_plugin.main
     mypy_path = $MYPY_CONFIG_FILE_DIR/./path/relative/to/config/where/information/is/cached
```

### Comparing `extended_mypy_django_plugin-0.5/docs/api/primer.rst` & `extended_mypy_django_plugin-0.5.1/docs/api/primer.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/docs/api/usage.rst` & `extended_mypy_django_plugin-0.5.1/docs/api/usage.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/docs/api/internals/actions.rst` & `extended_mypy_django_plugin-0.5.1/docs/api/internals/actions.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/example/manage.py` & `extended_mypy_django_plugin-0.5.1/example/manage.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/example/djangoexample/settings.py` & `extended_mypy_django_plugin-0.5.1/example/djangoexample/settings.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/example/djangoexample/urls.py` & `extended_mypy_django_plugin-0.5.1/example/djangoexample/urls.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/example/djangoexample/views.py` & `extended_mypy_django_plugin-0.5.1/example/djangoexample/views.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/example/djangoexample/exampleapp/models.py` & `extended_mypy_django_plugin-0.5.1/example/djangoexample/exampleapp/models.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/annotations.py` & `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/annotations.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/entry.py` & `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/entry.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,27 +22,33 @@
 
     def __init__(
         self, plugin_cls: type[ExtendedMypyStubs], locals: MutableMapping[str, object], /
     ) -> None:
         self.locals = locals
         self.instance: ExtendedMypyStubs | None = None
         self.plugin_cls = plugin_cls
+        self.previous_version: int | None = None
+
+    def _change_version(self, instance: ExtendedMypyStubs) -> None:
+        new_version = instance.determine_plugin_version(self.previous_version)
+        self.previous_version = new_version
+        self.locals["__version__"] = str(new_version)
 
     def __call__(self, version: str) -> type[MypyPlugin]:
         if self.instance is not None:
-            self.locals["__version__"] = str(self.instance.determine_plugin_version())
+            self._change_version(self.instance)
 
             # Inside dmypy, don't create a new plugin
             return MypyPlugin
 
         provider = self
         major, minor, _ = version.split(".", 2)
 
         def __init__(instance: ExtendedMypyStubs, options: Options) -> None:
             super(instance.__class__, instance).__init__(
                 options,
                 mypy_version_tuple=(int(major), int(minor)),  # type: ignore[call-arg]
             )
             provider.instance = instance
-            provider.locals["__version__"] = str(instance.determine_plugin_version())
+            provider._change_version(instance)
 
         return type("Plugin", (provider.plugin_cls,), {"__init__": __init__})
```

### Comparing `extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/_config.py` & `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -29,18 +29,18 @@
 
 
 class Config(DjangoPluginConfig):
     __slots__ = (
         "django_settings_module",
         "strict_settings",
         "scratch_path",
-        "installed_apps_script",
+        "determine_django_state_script",
     )
     scratch_path: Path
-    installed_apps_script: Path | None
+    determine_django_state_script: Path | None
 
     def parse_toml_file(self, filepath: pathlib.Path) -> None:
         toml_exit: Callable[[str], NoReturn] = partial(exit_with_error, is_toml=True)
         try:
             with filepath.open(mode="rb") as f:
                 data = tomllib.load(f)
         except (tomllib.TOMLDecodeError, OSError):
@@ -63,19 +63,21 @@
 
         if not isinstance(config["scratch_path"], str):
             toml_exit("invalid 'scratch_path': the setting must be a string")
         self.scratch_path = filepath.parent / config["scratch_path"]
         self.scratch_path.mkdir(parents=True, exist_ok=True)
 
         if "installed_apps_path" in config:
-            if not isinstance(config["installed_apps_script"], str):
-                toml_exit("invalid 'installed_apps_script': the setting must be a string")
-            self.installed_apps_script = filepath.parent / config["installed_apps_script"]
+            if not isinstance(config["determine_django_state_script"], str):
+                toml_exit("invalid 'determine_django_state_script': the setting must be a string")
+            self.determine_django_state_script = (
+                filepath.parent / config["determine_django_state_script"]
+            )
         else:
-            self.installed_apps_script = None
+            self.determine_django_state_script = None
 
         self.strict_settings = config.get("strict_settings", True)
         if not isinstance(self.strict_settings, bool):
             toml_exit(INVALID_BOOL_SETTING.format(key="strict_settings"))
 
     def parse_ini_file(self, filepath: Path) -> None:
         parser = configparser.ConfigParser()
@@ -96,29 +98,31 @@
             exit_with_error(MISSING_SCRATCH_PATH)
 
         self.django_settings_module = parser.get(section, "django_settings_module").strip("'\"")
 
         self.scratch_path = filepath.parent / parser.get(section, "scratch_path").strip("'\"")
         self.scratch_path.mkdir(parents=True, exist_ok=True)
 
-        if parser.has_option(section, "installed_apps_script"):
-            self.installed_apps_script = filepath.parent / parser.get(
-                section, "installed_apps_script"
+        if parser.has_option(section, "determine_django_state_script"):
+            self.determine_django_state_script = filepath.parent / parser.get(
+                section, "determine_django_state_script"
             ).strip("'\"")
         else:
-            self.installed_apps_script = None
+            self.determine_django_state_script = None
 
         try:
             self.strict_settings = parser.getboolean(section, "strict_settings", fallback=True)
         except ValueError:
             exit_with_error(INVALID_BOOL_SETTING.format(key="strict_settings"))
 
     def to_json(self) -> dict[str, Any]:
         """We use this method to reset mypy cache via `report_config_data` hook."""
         return {
             "django_settings_module": self.django_settings_module,
             "scratch_path": str(self.scratch_path),
-            "installed_apps_script": (
-                None if self.installed_apps_script is None else str(self.installed_apps_script)
+            "determine_django_state_script": (
+                None
+                if self.determine_django_state_script is None
+                else str(self.determine_django_state_script)
             ),
             "strict_settings": self.strict_settings,
         }
```

### Comparing `extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/_dependencies.py` & `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_dependencies.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/_hook.py` & `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_hook.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/_plugin.py` & `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,14 +52,16 @@
     .. autoattribute:: get_type_analyze_hook
 
     .. autoattribute:: get_function_hook
 
     .. autoattribute:: get_attribute_hook
     """
 
+    plugin_config: _config.Config
+
     class Annotations(enum.Enum):
         CONCRETE = "extended_mypy_django_plugin.annotations.Concrete"
         CONCRETE_QUERYSET = "extended_mypy_django_plugin.annotations.ConcreteQuerySet"
         DEFAULT_QUERYSET = "extended_mypy_django_plugin.annotations.DefaultQuerySet"
 
     def __init__(self, options: Options, mypy_version_tuple: tuple[int, int]) -> None:
         super(main.NewSemanalDjangoPlugin, self).__init__(options)
@@ -69,15 +71,15 @@
         # Add paths from MYPYPATH env var
         sys.path.extend(mypy_path())
         # Add paths from mypy_path config option
         sys.path.extend(options.mypy_path)
 
         self.running_in_daemon: bool = "dmypy" in sys.argv[0]
         self.report = _reports.Reports.create(
-            installed_apps_script=self.plugin_config.installed_apps_script,
+            determine_django_state_script=self.plugin_config.determine_django_state_script,
             django_settings_module=self.plugin_config.django_settings_module,
             scratch_path=self.plugin_config.scratch_path,
         )
 
         self.django_context = DjangoContext(self.plugin_config.django_settings_module)
         self.store = _store.Store(
             get_model_class_by_fullname=self.django_context.get_model_class_by_fullname,
@@ -103,24 +105,26 @@
     def _lookup_info(self, fullname: str) -> TypeInfo | None:
         sym = self.lookup_fully_qualified(fullname)
         if sym and isinstance(sym.node, TypeInfo):
             return sym.node
         else:
             return None
 
-    def determine_plugin_version(self) -> int:
+    def determine_plugin_version(self, previous_version: int | None = None) -> int:
         """
         Used to set `__version__' where the plugin is defined.
 
         This lets us tell dmypy to restart itself as necessary.
         """
         if not self.running_in_daemon:
             return 0
         else:
-            return self.report.determine_version_hash()
+            return self.report.determine_version_hash(
+                self.plugin_config.scratch_path, previous_version
+            )
 
     def get_additional_deps(self, file: MypyFile) -> list[tuple[int, str, int]]:
         """
         Ensure that models are re-analyzed if any other models that depend on
         them change.
 
         We use a generated "report" to re-analyze a file if a new dependency
```

### Comparing `extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/_reports.py` & `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_reports.py`

 * *Files 8% similar despite different names*

```diff
@@ -252,57 +252,57 @@
     Further documentation has yet to be added.
     """
 
     @classmethod
     def create(
         cls,
         *,
-        installed_apps_script: pathlib.Path | None,
+        determine_django_state_script: pathlib.Path | None,
         django_settings_module: str,
         scratch_path: pathlib.Path,
         reports_dir_prefix: str = "__virtual_extended_mypy_django_plugin_report__",
     ) -> "Reports":
-        if installed_apps_script is not None:
-            if not installed_apps_script.exists():
+        if determine_django_state_script is not None:
+            if not determine_django_state_script.exists():
                 raise ValueError("The provided script for finding installed apps does not exist")
 
-            if not installed_apps_script.stat().st_mode & stat.S_IXUSR:
+            if not determine_django_state_script.stat().st_mode & stat.S_IXUSR:
                 raise ValueError(
                     "The provided script for finding installed apps is not executable!"
                 )
 
-        if installed_apps_script is None:
-            installed_apps_script = pathlib.Path(
+        if determine_django_state_script is None:
+            determine_django_state_script = pathlib.Path(
                 str(
                     importlib.resources.files("extended_mypy_django_plugin")
                     / "scripts"
-                    / "get_installed_apps.py"
+                    / "determine_django_state.py"
                 )
             )
 
         reports_dir = scratch_path / reports_dir_prefix
         if reports_dir.exists() and not reports_dir.is_dir():
             reports_dir.unlink()
         reports_dir.mkdir(parents=True, exist_ok=True)
 
         return cls(
             store=_Store.read(prefix=reports_dir_prefix, reports_dir=reports_dir),
-            installed_apps_script=installed_apps_script,
+            determine_django_state_script=determine_django_state_script,
             django_settings_module=django_settings_module,
         )
 
     def __init__(
         self,
         *,
         store: _Store,
-        installed_apps_script: pathlib.Path,
+        determine_django_state_script: pathlib.Path,
         django_settings_module: str,
     ) -> None:
         self._store = store
-        self._installed_apps_script = installed_apps_script
+        self._determine_django_state_script = determine_django_state_script
         self._django_settings_module = django_settings_module
         self._known_concrete_models: MutableMapping[str, set[str]] = defaultdict(set)
 
     def known_concrete_models(self, fullname: str) -> set[str]:
         return self._known_concrete_models[fullname]
 
     def lines_hash(self) -> str:
@@ -313,26 +313,28 @@
                 buffer.write(b"\n")
                 buffer.write(path.name.encode())
                 buffer.write(b"\n")
                 buffer.write(path.read_bytes())
 
         return str(zlib.adler32(buffer.getbuffer()))
 
-    def determine_version_hash(self) -> int:
+    def determine_version_hash(
+        self, scratch_path: pathlib.Path, previous_version: int | None
+    ) -> int:
         result_file_cm = tempfile.NamedTemporaryFile()
         known_models_file_cm = tempfile.NamedTemporaryFile()
         with result_file_cm as result_file, known_models_file_cm as known_models_file:
-            if self._installed_apps_script is not None:
-                script = self._installed_apps_script
+            if self._determine_django_state_script is not None:
+                script = self._determine_django_state_script
             else:
                 script = pathlib.Path(
                     str(
                         importlib.resources.files("extended_mypy_django_plugin")
                         / "scripts"
-                        / "get_installed_apps.py"
+                        / "determine_django_state.py"
                     )
                 )
 
             cmd: list[str] = []
 
             if script.suffix == ".py":
                 cmd.append(sys.executable)
@@ -347,18 +349,27 @@
                     str(script),
                     "--django-settings-module",
                     self._django_settings_module,
                     "--apps-file",
                     result_file.name,
                     "--known-models-file",
                     known_models_file.name,
+                    "--scratch-path",
+                    str(scratch_path),
                 ]
             )
 
-            subprocess.run(cmd, capture_output=True, check=True)
+            try:
+                subprocess.run(cmd, capture_output=True, check=True)
+            except subprocess.CalledProcessError as err:
+                if err.returncode == 2:
+                    return 1 if previous_version is None else previous_version
+                else:
+                    raise
+
             installed_apps_hash = str(zlib.adler32(pathlib.Path(result_file.name).read_bytes()))
             known_models_hash = str(
                 zlib.adler32(pathlib.Path(known_models_file.name).read_bytes())
             )
             return zlib.adler32(
                 f"{installed_apps_hash}.{known_models_hash}.{self.lines_hash()}".encode()
             )
```

### Comparing `extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/_store.py` & `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/_store.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/actions/_sem_analyze.py` & `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/_sem_analyze.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/actions/_type_analyze.py` & `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/_type_analyze.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/plugin/actions/_type_checker.py` & `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/plugin/actions/_type_checker.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/scripts/find_models.py` & `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/scripts/find_models.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/extended_mypy_django_plugin/scripts/get_installed_apps.py` & `extended_mypy_django_plugin-0.5.1/extended_mypy_django_plugin/scripts/determine_django_state.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 
 import argparse
 import os
 import pathlib
 import sys
+from collections.abc import Callable
 
 from extended_mypy_django_plugin.scripts import record_known_models
 
 
 def make_parser() -> argparse.ArgumentParser:
     parser = argparse.ArgumentParser()
     parser.add_argument(
@@ -19,22 +20,34 @@
         type=pathlib.Path,
     )
     parser.add_argument(
         "--known-models-file",
         help="The file to print the known models to",
         type=pathlib.Path,
     )
+    parser.add_argument(
+        "--scratch-path",
+        help="The folder that the plugin is allowed to write in",
+        type=pathlib.Path,
+    )
     return parser
 
 
-def main(argv: list[str] | None = None) -> None:
+def main(
+    argv: list[str] | None = None, additional_django_setup: Callable[[], None] | None = None
+) -> None:
     parser = make_parser()
     args = parser.parse_args(argv)
 
+    if (args.scratch_path / "__assume_django_state_unchanged__").exists():
+        sys.exit(2)
+
     os.environ["DJANGO_SETTINGS_MODULE"] = args.django_settings_module
+    if additional_django_setup:
+        additional_django_setup()
 
     # add current directory to sys.path
     sys.path.append(str(pathlib.Path.cwd()))
 
     from django.apps import apps
     from django.conf import settings
```

### Comparing `extended_mypy_django_plugin-0.5/scripts/make_old.patch` & `extended_mypy_django_plugin-0.5.1/scripts/make_old.patch`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/scripts/tests_extension_hook.py` & `extended_mypy_django_plugin-0.5.1/scripts/tests_extension_hook.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/scripts/myapp/models.py` & `extended_mypy_django_plugin-0.5.1/scripts/myapp/models.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/tests/test_concrete_annotation.yml` & `extended_mypy_django_plugin-0.5.1/tests/test_concrete_annotation.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/tests/test_works.yml` & `extended_mypy_django_plugin-0.5.1/tests/test_works.yml`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/tools/bootstrap_venvstarter.py` & `extended_mypy_django_plugin-0.5.1/tools/bootstrap_venvstarter.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/tools/devtools.py` & `extended_mypy_django_plugin-0.5.1/tools/devtools.py`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/tools/venv` & `extended_mypy_django_plugin-0.5.1/tools/venv`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/LICENSE` & `extended_mypy_django_plugin-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/README.rst` & `extended_mypy_django_plugin-0.5.1/README.rst`

 * *Files identical despite different names*

### Comparing `extended_mypy_django_plugin-0.5/pyproject.toml` & `extended_mypy_django_plugin-0.5.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
-name = "extended_mypy_django_plugin"
+name = "extended-mypy-django-plugin"
 dynamic = ["version"]
 description = "Trying to make mypy understand .objects on abstract django models"
 readme = "README.rst"
 license = { text = "MIT" }
 authors = [
     { name = "Stephen Moore", email = "stephen@delfick.com" },
 ]
```

### Comparing `extended_mypy_django_plugin-0.5/PKG-INFO` & `extended_mypy_django_plugin-0.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
-Name: extended_mypy_django_plugin
-Version: 0.5
+Name: extended-mypy-django-plugin
+Version: 0.5.1
 Summary: Trying to make mypy understand .objects on abstract django models
 Author-email: Stephen Moore <stephen@delfick.com>
 License: MIT
 License-File: LICENSE
 Provides-Extra: stubs-latest
 Requires-Dist: django-stubs==5.0.0; extra == 'stubs-latest'
 Requires-Dist: mypy==1.10.0; extra == 'stubs-latest'
```

