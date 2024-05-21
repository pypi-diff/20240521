# Comparing `tmp/esmerald-3.1.5.tar.gz` & `tmp/esmerald-3.2.0.tar.gz`

## Comparing `esmerald-3.1.5.tar` & `esmerald-3.2.0.tar`

### file list

```diff
@@ -1,230 +1,230 @@
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/__main__.py
--rw-r--r--   0        0        0    91539 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/applications.py
--rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/backgound.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/concurrency.py
--rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/context.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/enums.py
--rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/exception_handlers.py
--rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/exceptions.py
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/injector.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/logging.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/param_functions.py
--rw-r--r--   0        0        0    22336 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/params.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/parsers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/py.typed
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/requests.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/staticfiles.py
--rw-r--r--   0        0        0     6319 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/testclient.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/types.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/typing.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/websockets.py
--rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/__init__.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/enums.py
--rw-r--r--   0        0        0    47620 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/global_settings.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/app_template/__init__.py-tpl
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/app_template/tests.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/app_template/directives/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/app_template/directives/operations/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/app_template/v1/__init__.py-tpl
--rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/app_template/v1/controllers.py-tpl
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/app_template/v1/schemas.py-tpl
--rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/app_template/v1/urls.py-tpl
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
--rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl
--rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/.gitignore.e-tpl
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/Makefile.e-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/__init__.py-tpl
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/main.py-tpl
--rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/serve.py-tpl
--rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/urls.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/apps/__init__.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/configs/__init__.py-tpl
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/configs/development/__init__.py-tpl
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/configs/development/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/configs/testing/__init__.py-tpl
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/configs/testing/settings.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/tests/__init__.py-tpl
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/tests/conftest.py-tpl
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/tests/test_app.py-tpl
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/requirements/base.txt.e-tpl
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/requirements/development.txt.e-tpl
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/conf/directives/project_template/requirements/testing.txt.e-tpl
--rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/config/__init__.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/config/asyncexit.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/config/cors.py
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/config/csrf.py
--rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/config/jwt.py
--rw-r--r--   0        0        0    14614 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/config/openapi.py
--rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/config/session.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/config/static_files.py
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/config/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/__init__.py
--rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/encoding.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/__init__.py
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/constants.py
--rw-r--r--   0        0        0     8672 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/hashers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/common/__init__.py
--rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/common/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/edgy/__init__.py
--rw-r--r--   0        0        0     3912 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/edgy/base_user.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/edgy/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/mongoz/__init__.py
--rw-r--r--   0        0        0     4018 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/mongoz/base_user.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/mongoz/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/saffier/__init__.py
--rw-r--r--   0        0        0     3862 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/saffier/base_user.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/contrib/auth/saffier/middleware.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/di/__init__.py
--rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/di/provider.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/__init__.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/base.py
--rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/cli.py
--rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/constants.py
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/env.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/exceptions.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/parsers.py
--rw-r--r--   0        0        0     8906 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/templates.py
--rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/utils.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/__init__.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/_constants.py
--rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/createapp.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/createdeployment.py
--rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/createproject.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/list.py
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/run.py
--rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/runserver.py
--rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/show_urls.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/shell/__init__.py
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/shell/base.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/shell/enums.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/shell/ipython.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/shell/ptpython.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/directives/operations/shell/utils.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/terminal/__init__.py
--rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/terminal/base.py
--rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/terminal/print.py
--rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/terminal/terminal.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/urls/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/core/urls/base.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/datastructures/__init__.py
--rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/datastructures/base.py
--rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/datastructures/encoders.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/datastructures/file.py
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/datastructures/json.py
--rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/datastructures/msgspec.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/datastructures/redirect.py
--rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/datastructures/stream.py
--rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/datastructures/template.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/datastructures/types.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/interceptors/__init__.py
--rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/interceptors/interceptor.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/interceptors/types.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/__init__.py
--rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/_exception_handlers.py
--rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/app_settings.py
--rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/asyncexitstack.py
--rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/authentication.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/cors.py
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/csrf.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/errors.py
--rw-r--r--   0        0        0     5898 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/exceptions.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/gzip.py
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/https.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/sessions.py
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/settings_middleware.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/trustedhost.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/middleware/wsgi.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/__init__.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/_internal.py
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/constants.py
--rw-r--r--   0        0        0     3034 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/datastructures.py
--rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/docs.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/enums.py
--rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/models.py
--rw-r--r--   0        0        0    20721 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/openapi.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/params.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/responses.py
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/utils.py
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/validation.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/security/__init__.py
--rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/security/base.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/security/api_key/__init__.py
--rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/security/api_key/base.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/security/http/__init__.py
--rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/security/http/base.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/security/oauth2/__init__.py
--rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/security/oauth2/base.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/security/openid_connect/__init__.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/openapi/security/openid_connect/base.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/permissions/__init__.py
--rw-r--r--   0        0        0     9319 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/permissions/base.py
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/permissions/types.py
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/permissions/utils.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/pluggables/__init__.py
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/pluggables/base.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/protocols/__init__.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/protocols/asyncdao.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/protocols/dao.py
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/protocols/extension.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/protocols/interceptor.py
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/protocols/middleware.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/protocols/template.py
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/responses/__init__.py
--rw-r--r--   0        0        0     5561 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/responses/base.py
--rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/responses/encoders.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/responses/json.py
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/responses/template.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/__init__.py
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/_internal.py
--rw-r--r--   0        0        0    23730 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/base.py
--rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/events.py
--rw-r--r--   0        0        0    23680 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/gateways.py
--rw-r--r--   0        0        0   108795 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/handlers.py
--rw-r--r--   0        0        0    72909 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/router.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/views.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/apis/__init__.py
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/apis/_metaclasses.py
--rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/apis/_mixins.py
--rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/apis/base.py
--rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/apis/generics.py
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/apis/views.py
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/webhooks/__init__.py
--rw-r--r--   0        0        0   106388 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/routing/webhooks/handlers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/security/__init__.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/security/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/security/jwt/__init__.py
--rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/security/jwt/token.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/template/__init__.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/template/jinja.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/template/mako.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/transformers/__init__.py
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/transformers/constants.py
--rw-r--r--   0        0        0     4826 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/transformers/datastructures.py
--rw-r--r--   0        0        0    20139 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/transformers/model.py
--rw-r--r--   0        0        0     5751 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/transformers/signature.py
--rw-r--r--   0        0        0     6798 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/transformers/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/utils/__init__.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/utils/constants.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/utils/crypto.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/utils/dependency.py
--rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/utils/functional.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/utils/helpers.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/utils/inspect.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/utils/models.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/utils/module_loading.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/utils/sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/utils/url.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/utils/pydantic/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esmerald-3.1.5/esmerald/utils/pydantic/schema.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 esmerald-3.1.5/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-3.1.5/LICENSE
--rw-r--r--   0        0        0    17034 2020-02-02 00:00:00.000000 esmerald-3.1.5/README.md
--rw-r--r--   0        0        0     7452 2020-02-02 00:00:00.000000 esmerald-3.1.5/pyproject.toml
--rw-r--r--   0        0        0    20683 2020-02-02 00:00:00.000000 esmerald-3.1.5/PKG-INFO
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/__main__.py
+-rw-r--r--   0        0        0    93812 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/applications.py
+-rw-r--r--   0        0        0     2209 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/backgound.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/concurrency.py
+-rw-r--r--   0        0        0     4456 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/context.py
+-rw-r--r--   0        0        0     2676 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/encoders.py
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/enums.py
+-rw-r--r--   0        0        0     3893 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/exception_handlers.py
+-rw-r--r--   0        0        0     4894 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/exceptions.py
+-rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/injector.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/logging.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/param_functions.py
+-rw-r--r--   0        0        0    22336 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/params.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/parsers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/py.typed
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/requests.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/staticfiles.py
+-rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/testclient.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/types.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/typing.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/websockets.py
+-rw-r--r--   0        0        0     2408 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/__init__.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/enums.py
+-rw-r--r--   0        0        0    48576 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/global_settings.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/app_template/tests.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/app_template/directives/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/app_template/directives/operations/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/app_template/v1/__init__.py-tpl
+-rw-r--r--   0        0        0     1186 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/app_template/v1/controllers.py-tpl
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/app_template/v1/schemas.py-tpl
+-rw-r--r--   0        0        0      361 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/app_template/v1/urls.py-tpl
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl
+-rw-r--r--   0        0        0     5726 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/.gitignore.e-tpl
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/Makefile.e-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/__init__.py-tpl
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/main.py-tpl
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/serve.py-tpl
+-rw-r--r--   0        0        0      756 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/urls.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/apps/__init__.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/configs/__init__.py-tpl
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/configs/development/__init__.py-tpl
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/configs/development/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/configs/testing/__init__.py-tpl
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/configs/testing/settings.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/tests/__init__.py-tpl
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/tests/conftest.py-tpl
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/tests/test_app.py-tpl
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/requirements/base.txt.e-tpl
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/requirements/development.txt.e-tpl
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/conf/directives/project_template/requirements/testing.txt.e-tpl
+-rw-r--r--   0        0        0      352 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/config/__init__.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/config/asyncexit.py
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/config/cors.py
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/config/csrf.py
+-rw-r--r--   0        0        0     5665 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/config/jwt.py
+-rw-r--r--   0        0        0    14614 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/config/openapi.py
+-rw-r--r--   0        0        0     2790 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/config/session.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/config/static_files.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/config/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/__init__.py
+-rw-r--r--   0        0        0     7517 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/encoding.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/__init__.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/constants.py
+-rw-r--r--   0        0        0     8684 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/hashers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/common/__init__.py
+-rw-r--r--   0        0        0     2865 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/common/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/edgy/__init__.py
+-rw-r--r--   0        0        0     3918 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/edgy/base_user.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/edgy/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/mongoz/__init__.py
+-rw-r--r--   0        0        0     4024 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/mongoz/base_user.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/mongoz/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/saffier/__init__.py
+-rw-r--r--   0        0        0     3868 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/saffier/base_user.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/contrib/auth/saffier/middleware.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/di/__init__.py
+-rw-r--r--   0        0        0     2569 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/di/provider.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/__init__.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/base.py
+-rw-r--r--   0        0        0     4107 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/cli.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/constants.py
+-rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/env.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/exceptions.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/parsers.py
+-rw-r--r--   0        0        0     8906 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/templates.py
+-rw-r--r--   0        0        0     5660 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/utils.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/__init__.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/_constants.py
+-rw-r--r--   0        0        0     1296 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/createapp.py
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/createdeployment.py
+-rw-r--r--   0        0        0     1587 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/createproject.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/list.py
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/run.py
+-rw-r--r--   0        0        0     2773 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/runserver.py
+-rw-r--r--   0        0        0     4075 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/show_urls.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/shell/__init__.py
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/shell/base.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/shell/enums.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/shell/ipython.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/shell/ptpython.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/directives/operations/shell/utils.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/terminal/__init__.py
+-rw-r--r--   0        0        0     8301 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/terminal/base.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/terminal/print.py
+-rw-r--r--   0        0        0     1223 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/terminal/terminal.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/urls/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/core/urls/base.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/datastructures/__init__.py
+-rw-r--r--   0        0        0     4237 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/datastructures/base.py
+-rw-r--r--   0        0        0     3631 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/datastructures/encoders.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/datastructures/file.py
+-rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/datastructures/json.py
+-rw-r--r--   0        0        0     2485 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/datastructures/msgspec.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/datastructures/redirect.py
+-rw-r--r--   0        0        0     1541 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/datastructures/stream.py
+-rw-r--r--   0        0        0     3219 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/datastructures/template.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/datastructures/types.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/interceptors/__init__.py
+-rw-r--r--   0        0        0     1811 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/interceptors/interceptor.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/interceptors/types.py
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/__init__.py
+-rw-r--r--   0        0        0     2559 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/_exception_handlers.py
+-rw-r--r--   0        0        0      846 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/app_settings.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/asyncexitstack.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/authentication.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/cors.py
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/csrf.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/errors.py
+-rw-r--r--   0        0        0     5897 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/exceptions.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/gzip.py
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/https.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/sessions.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/settings_middleware.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/trustedhost.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/middleware/wsgi.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/__init__.py
+-rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/_internal.py
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/constants.py
+-rw-r--r--   0        0        0     3344 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/datastructures.py
+-rw-r--r--   0        0        0     7303 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/docs.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/enums.py
+-rw-r--r--   0        0        0     4853 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/models.py
+-rw-r--r--   0        0        0    20721 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/openapi.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/params.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/responses.py
+-rw-r--r--   0        0        0     2805 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/utils.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/validation.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/security/__init__.py
+-rw-r--r--   0        0        0     1160 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/security/base.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/security/api_key/__init__.py
+-rw-r--r--   0        0        0     2197 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/security/api_key/base.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/security/http/__init__.py
+-rw-r--r--   0        0        0     2714 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/security/http/base.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/security/oauth2/__init__.py
+-rw-r--r--   0        0        0     1500 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/security/oauth2/base.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/security/openid_connect/__init__.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/openapi/security/openid_connect/base.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/permissions/__init__.py
+-rw-r--r--   0        0        0     9319 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/permissions/base.py
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/permissions/types.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/permissions/utils.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/pluggables/__init__.py
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/pluggables/base.py
+-rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/protocols/__init__.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/protocols/asyncdao.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/protocols/dao.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/protocols/extension.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/protocols/interceptor.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/protocols/middleware.py
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/protocols/template.py
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/responses/__init__.py
+-rw-r--r--   0        0        0     6019 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/responses/base.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/responses/encoders.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/responses/json.py
+-rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/responses/template.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/__init__.py
+-rw-r--r--   0        0        0     4733 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/_internal.py
+-rw-r--r--   0        0        0    23730 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/base.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/events.py
+-rw-r--r--   0        0        0    23680 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/gateways.py
+-rw-r--r--   0        0        0   108795 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/handlers.py
+-rw-r--r--   0        0        0    72904 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/router.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/views.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/apis/__init__.py
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/apis/_metaclasses.py
+-rw-r--r--   0        0        0     4656 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/apis/_mixins.py
+-rw-r--r--   0        0        0    12069 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/apis/base.py
+-rw-r--r--   0        0        0     2839 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/apis/generics.py
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/apis/views.py
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/webhooks/__init__.py
+-rw-r--r--   0        0        0   106388 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/routing/webhooks/handlers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/security/__init__.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/security/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/security/jwt/__init__.py
+-rw-r--r--   0        0        0     2937 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/security/jwt/token.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/template/__init__.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/template/jinja.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/template/mako.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/transformers/__init__.py
+-rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/transformers/constants.py
+-rw-r--r--   0        0        0    28174 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/transformers/model.py
+-rw-r--r--   0        0        0    20662 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/transformers/signature.py
+-rw-r--r--   0        0        0     6784 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/transformers/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/utils/__init__.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/utils/constants.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/utils/crypto.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/utils/dependency.py
+-rw-r--r--   0        0        0     4969 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/utils/functional.py
+-rw-r--r--   0        0        0     1319 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/utils/helpers.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/utils/inspect.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/utils/models.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/utils/module_loading.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/utils/sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/utils/url.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/utils/pydantic/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 esmerald-3.2.0/esmerald/utils/pydantic/schema.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 esmerald-3.2.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 esmerald-3.2.0/LICENSE
+-rw-r--r--   0        0        0    17034 2020-02-02 00:00:00.000000 esmerald-3.2.0/README.md
+-rw-r--r--   0        0        0     7613 2020-02-02 00:00:00.000000 esmerald-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0    21586 2020-02-02 00:00:00.000000 esmerald-3.2.0/PKG-INFO
```

### Comparing `esmerald-3.1.5/esmerald/__init__.py` & `esmerald-3.2.0/esmerald/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "3.1.5"
+__version__ = "3.2.0"
 
 
 from lilya import status
 
 from esmerald.conf import settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.context import Context
```

### Comparing `esmerald-3.1.5/esmerald/applications.py` & `esmerald-3.2.0/esmerald/applications.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,28 +10,30 @@
     Sequence,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
+from lilya._internal._module_loading import import_string
 from lilya.apps import Lilya
 from lilya.middleware import DefineMiddleware  # noqa
 from lilya.types import Lifespan, Receive, Scope, Send
 from openapi_schemas_pydantic.v3_1_0 import Contact, License, SecurityScheme
 from openapi_schemas_pydantic.v3_1_0.open_api import OpenAPI
 from pydantic import AnyUrl, ValidationError
 from typing_extensions import Annotated, Doc
 
 from esmerald.conf import reload_settings, settings as esmerald_settings
 from esmerald.conf.global_settings import EsmeraldAPISettings
 from esmerald.config import CORSConfig, CSRFConfig, SessionConfig
 from esmerald.config.openapi import OpenAPIConfig
 from esmerald.config.static_files import StaticFilesConfig
 from esmerald.datastructures import State
+from esmerald.encoders import Encoder, MsgSpecEncoder, PydanticEncoder, register_esmerald_encoder
 from esmerald.exception_handlers import (
     improperly_configured_exception_handler,
     pydantic_validation_error_handler,
     validation_error_exception_handler,
 )
 from esmerald.exceptions import ImproperlyConfigured, ValidationErrorException
 from esmerald.interceptors.types import Interceptor
@@ -134,21 +136,22 @@
         "summary",
         "tags",
         "template_config",
         "terms_of_service",
         "timezone",
         "title",
         "version",
+        "encoders",
     )
 
     def __init__(
         self: AppType,
         *,
         settings_module: Annotated[
-            Optional["SettingsType"],
+            Union[Optional["SettingsType"], Optional[str]],
             Doc(
                 """
                 Alternative settings parameter. This parameter is an alternative to
                 `ESMERALD_SETTINGS_MODULE` way of loading your settings into an Esmerald application.
 
                 When the `settings_module` is provided, it will make sure it takes priority over
                 any other settings provided for the instance.
@@ -1077,14 +1080,54 @@
                         DefineMiddleware(HTTPSRedirectMiddleware),
                     ],
                 )
                 ```
                 """
             ),
         ] = None,
+        encoders: Annotated[
+            Sequence[Optional[Encoder]],
+            Doc(
+                """
+            A `list` of encoders to be used by the application once it
+            starts.
+
+            Returns:
+                List of encoders
+
+            **Example**
+
+            ```python
+            from typing import Any
+
+            from attrs import asdict, define, field, has
+            from esmerald.encoders import Encoder
+
+
+            class AttrsEncoder(Encoder):
+
+                def is_type(self, value: Any) -> bool:
+                    return has(value)
+
+                def serialize(self, obj: Any) -> Any:
+                    return asdict(obj)
+
+                def encode(self, annotation: Any, value: Any) -> Any:
+                    return annotation(**value)
+
+
+            class AppSettings(EsmeraldAPISettings):
+
+                @property
+                def encoders(self) -> Union[List[Encoder], None]:
+                    return [AttrsEncoder]
+            ```
+            """
+            ),
+        ] = None,
         exception_handlers: Annotated[
             Optional["ExceptionHandlerMap"],
             Doc(
                 """
                 A global dictionary with handlers for exceptions.
 
                 **Note** almost everything in Esmerald can be done in [levels](https://esmerald.dev/application/levels/), which means
@@ -1463,14 +1506,18 @@
                 app = Esmerald(openapi_url="/api/v1/openapi.json")
                 ```
                 """
             ),
         ] = None,
     ) -> None:
         self.settings_module = None
+
+        if settings_module is not None and isinstance(settings_module, str):
+            settings_module = import_string(settings_module)
+
         if settings_module is not None:
             if not isinstance(settings_module, EsmeraldAPISettings) and not is_class_and_subclass(
                 settings_module, EsmeraldAPISettings
             ):
                 raise ImproperlyConfigured(
                     "settings_module must be a subclass of EsmeraldSettings"
                 )
@@ -1572,33 +1619,50 @@
 
                 Learn more in the [Lilya documentation](https://www.lilya.dev/applications/#storing-state-on-the-app-instance).
                 """
             ),
         ] = State()
         self.async_exit_config = esmerald_settings.async_exit_config
 
+        self.encoders = self.load_settings_value("encoders", encoders) or []
+        self._register_application_encoders()
+
         self.router: "Router" = Router(
             on_shutdown=self.on_shutdown,
             on_startup=self.on_startup,
             routes=routes,
             app=self,
             lifespan=self.lifespan,
             deprecated=deprecated,
             security=security,
             redirect_slashes=self.redirect_slashes,
         )
-
         self.get_default_exception_handlers()
         self.user_middleware = self.build_user_middleware_stack()
         self.middleware_stack = self.build_middleware_stack()
         self.pluggable_stack = self.build_pluggable_stack()
         self.template_engine = self.get_template_engine(self.template_config)
 
         self._configure()
 
+    def _register_application_encoders(self) -> None:
+        """
+        Registers the default Esmerald encoders.
+
+        This allows backwards compatibility with the previous
+        versions of Esmerald supporting Pydantic and MsgSpec by default.
+
+        This way, the support still remains but using the Lilya Encoders.
+        """
+        self.register_encoder(cast(Encoder[Any], PydanticEncoder))
+        self.register_encoder(cast(Encoder[Any], MsgSpecEncoder))
+
+        for encoder in self.encoders:
+            self.register_encoder(encoder)
+
     def _configure(self) -> None:
         """
         Starts the Esmerald configurations.
         """
         if self.static_files_config:
             for config in (
                 self.static_files_config
@@ -2545,14 +2609,20 @@
         Check: https://www.esmerald.dev/lifespan-events/
         """
         return self.router.on_event(event_type)
 
     def add_event_handler(self, event_type: str, func: Callable) -> None:  # pragma: no cover
         self.router.add_event_handler(event_type, func)
 
+    def register_encoder(self, encoder: Encoder[Any]) -> None:
+        """
+        Registers a Encoder into the list of predefined encoders of the system.
+        """
+        register_esmerald_encoder(encoder)
+
 
 class ChildEsmerald(Esmerald):
     """
     `ChildEsmerald` application object. The main entry-point for a modular application/API
     with Esmerald.
 
     The `ChildEsmerald` inherits directly from the `Esmerald` object which means all the same
```

### Comparing `esmerald-3.1.5/esmerald/backgound.py` & `esmerald-3.2.0/esmerald/backgound.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/context.py` & `esmerald-3.2.0/esmerald/context.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/enums.py` & `esmerald-3.2.0/esmerald/enums.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/exception_handlers.py` & `esmerald-3.2.0/esmerald/exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/exceptions.py` & `esmerald-3.2.0/esmerald/exceptions.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/injector.py` & `esmerald-3.2.0/esmerald/injector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Type, Union
 
 from esmerald.core.di.provider import load_provider
 from esmerald.parsers import ArbitraryHashableBaseModel
-from esmerald.transformers.datastructures import Signature
+from esmerald.transformers.signature import SignatureModel
 from esmerald.typing import Void
 from esmerald.utils.helpers import is_async_callable
 
 if TYPE_CHECKING:  # pragma: no cover
     from esmerald.typing import AnyCallable
 
 
@@ -52,15 +52,15 @@
         return value
 
 
 class Inject(ArbitraryHashableBaseModel):
     def __init__(self, dependency: "AnyCallable", use_cache: bool = False, **kwargs: Any):
         super().__init__(**kwargs)
         self.dependency = dependency
-        self.signature_model: Optional["Type[Signature]"] = None
+        self.signature_model: Optional["Type[SignatureModel]"] = None
         self.use_cache = use_cache
         self.value: Any = Void
 
     async def __call__(self, **kwargs: Dict[str, Any]) -> Any:
         if self.use_cache and self.value is not Void:
             return self.value
```

### Comparing `esmerald-3.1.5/esmerald/logging.py` & `esmerald-3.2.0/esmerald/logging.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/params.py` & `esmerald-3.2.0/esmerald/params.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/parsers.py` & `esmerald-3.2.0/esmerald/parsers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/requests.py` & `esmerald-3.2.0/esmerald/requests.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/testclient.py` & `esmerald-3.2.0/esmerald/testclient.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 from httpx._client import CookieTypes
 from lilya.testclient import TestClient  # noqa
 from openapi_schemas_pydantic.v3_1_0 import Contact, License, SecurityScheme
 from pydantic import AnyUrl
 
 from esmerald.applications import Esmerald
+from esmerald.encoders import Encoder
 from esmerald.utils.crypto import get_random_secret_key
 
 if TYPE_CHECKING:  # pragma: no cover
     from typing_extensions import Literal
 
     from esmerald.config import (
         CORSConfig,
@@ -73,15 +74,15 @@
     def __enter__(self, *args: Any, **kwargs: Dict[str, Any]) -> "EsmeraldTestClient":
         return cast("EsmeraldTestClient", super().__enter__(*args, **kwargs))
 
 
 def create_client(
     routes: Union["APIGateHandler", List["APIGateHandler"]],
     *,
-    settings_module: Optional["SettingsType"] = None,
+    settings_module: Union[Optional["SettingsType"], Optional[str]] = None,
     debug: Optional[bool] = None,
     app_name: Optional[str] = None,
     title: Optional[str] = None,
     version: Optional[str] = None,
     summary: Optional[str] = None,
     description: Optional[str] = None,
     contact: Optional[Contact] = None,
@@ -119,14 +120,15 @@
     static_files_config: Optional["StaticFilesConfig"] = None,
     template_config: Optional["TemplateConfig"] = None,
     lifespan: Optional[Callable[["Esmerald"], "AsyncContextManager"]] = None,
     cookies: Optional[CookieTypes] = None,
     redirect_slashes: Optional[bool] = None,
     tags: Optional[List[str]] = None,
     webhooks: Optional[Sequence["WebhookGateway"]] = None,
+    encoders: Optional[Sequence[Encoder]] = None,
 ) -> EsmeraldTestClient:
     return EsmeraldTestClient(
         app=Esmerald(
             settings_module=settings_module,
             debug=debug,
             title=title,
             version=version,
@@ -163,14 +165,15 @@
             redirect_slashes=redirect_slashes,
             enable_openapi=enable_openapi,
             openapi_version=openapi_version,
             include_in_schema=include_in_schema,
             tags=tags,
             webhooks=webhooks,
             pluggables=pluggables,
+            encoders=encoders,
         ),
         base_url=base_url,
         backend=backend,
         backend_options=backend_options,
         root_path=root_path,
         raise_server_exceptions=raise_server_exceptions,
         cookies=cookies,
```

### Comparing `esmerald-3.1.5/esmerald/types.py` & `esmerald-3.2.0/esmerald/types.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/websockets.py` & `esmerald-3.2.0/esmerald/websockets.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/conf/__init__.py` & `esmerald-3.2.0/esmerald/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/conf/global_settings.py` & `esmerald-3.2.0/esmerald/conf/global_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
     CSRFConfig,
     OpenAPIConfig,
     SessionConfig,
     StaticFilesConfig,
 )
 from esmerald.config.asyncexit import AsyncExitConfig
 from esmerald.datastructures import Secret
+from esmerald.encoders import Encoder
 from esmerald.interceptors.types import Interceptor
 from esmerald.permissions.types import Permission
 from esmerald.pluggables import Pluggable
 from esmerald.routing import gateways
 from esmerald.types import (
     APIGateHandler,
     Dependencies,
@@ -1421,14 +1422,53 @@
                 return {
                     "my-extension": pluggable
                 }
         ```
         """
         return {}
 
+    @property
+    def encoders(self) -> Union[List[Encoder], None]:
+        """
+        A `list` of encoders to be used by the application once it
+        starts.
+
+        Returns:
+            List of encoders
+
+        **Example**
+
+        ```python
+        from typing import Any
+
+        from attrs import asdict, define, field, has
+        from esmerald.encoders import Encoder
+
+
+        class AttrsEncoder(Encoder):
+
+            def is_type(self, value: Any) -> bool:
+                return has(value)
+
+            def serialize(self, obj: Any) -> Any:
+                return asdict(obj)
+
+            def encode(self, annotation: Any, value: Any) -> Any:
+                return annotation(**value)
+
+
+        class AppSettings(EsmeraldAPISettings):
+
+            @property
+            def encoders(self) -> Union[List[Encoder], None]:
+                return [AttrsEncoder]
+        ```
+        """
+        return []
+
     def __hash__(self) -> int:
         values: Dict[str, Any] = {}
         for key, value in self.__dict__.items():
             values[key] = None
             if isinstance(value, (list, set)):
                 values[key] = tuple(value)
             else:
```

### Comparing `esmerald-3.1.5/esmerald/conf/directives/app_template/v1/controllers.py-tpl` & `esmerald-3.2.0/esmerald/conf/directives/app_template/v1/controllers.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl` & `esmerald-3.2.0/esmerald/conf/directives/deployment_template/docker/Dockerfile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl` & `esmerald-3.2.0/esmerald/conf/directives/deployment_template/gunicorn/gunicorn_conf.py.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl` & `esmerald-3.2.0/esmerald/conf/directives/deployment_template/nginx/nginx.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl` & `esmerald-3.2.0/esmerald/conf/directives/deployment_template/nginx/nginx.json-logging.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl` & `esmerald-3.2.0/esmerald/conf/directives/deployment_template/supervisor/supervisord.conf.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/conf/directives/project_template/.gitignore.e-tpl` & `esmerald-3.2.0/esmerald/conf/directives/project_template/.gitignore.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/conf/directives/project_template/Makefile.e-tpl` & `esmerald-3.2.0/esmerald/conf/directives/project_template/Makefile.e-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/main.py-tpl` & `esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/main.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/serve.py-tpl` & `esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/serve.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/urls.py-tpl` & `esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/urls.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl` & `esmerald-3.2.0/esmerald/conf/directives/project_template/project_name/configs/settings.py-tpl`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/config/cors.py` & `esmerald-3.2.0/esmerald/config/cors.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/config/csrf.py` & `esmerald-3.2.0/esmerald/config/csrf.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/config/jwt.py` & `esmerald-3.2.0/esmerald/config/jwt.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/config/openapi.py` & `esmerald-3.2.0/esmerald/config/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/config/session.py` & `esmerald-3.2.0/esmerald/config/session.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/config/static_files.py` & `esmerald-3.2.0/esmerald/config/static_files.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/config/template.py` & `esmerald-3.2.0/esmerald/config/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/contrib/encoding.py` & `esmerald-3.2.0/esmerald/contrib/encoding.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/contrib/auth/hashers.py` & `esmerald-3.2.0/esmerald/contrib/auth/hashers.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     """
     Return True if this password wasn't generated by
     User.set_unusable_password(), i.e. make_password(None).
     """
     return encoded is None or not encoded.startswith(UNUSABLE_PASSWORD_PREFIX)
 
 
-def check_password(
+async def check_password(
     password: str,
     encoded: str,
     setter: Callable[..., Any] = None,
     preferred: str = "default",
 ) -> bool:
     """
     Return a boolean of whether the raw password matches the three
@@ -50,15 +50,15 @@
         return False
 
     hasher_changed = hasher_handler.algorithm != preferred_hasher.algorithm
     must_update: bool = hasher_changed or preferred_hasher.must_update(encoded)
     is_correct: bool = hasher_handler.hasher.verify(password, encoded)
 
     if setter and is_correct and must_update:
-        setter(password)
+        await setter(password)
     return is_correct
 
 
 def make_password(password: Optional[str], hasher: str = "default") -> str:
     """
     Turn a plain-text password into a hash for database storage
```

### Comparing `esmerald-3.1.5/esmerald/contrib/auth/common/middleware.py` & `esmerald-3.2.0/esmerald/contrib/auth/common/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/contrib/auth/edgy/base_user.py` & `esmerald-3.2.0/esmerald/contrib/auth/edgy/base_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         async def setter(raw_password: str) -> None:
             await self.set_password(raw_password)
             # Password hash upgrades shouldn't be considered password changes.
             self._password = None
             await self.update(password=self.password)
 
-        return check_password(raw_password, str(self.password), setter)
+        return await check_password(raw_password, str(self.password), setter)
 
     async def set_unusable_password(self) -> None:
         # Set a value that will never be a valid hash
         self.password = make_password(None)
 
     async def has_usable_password(self) -> bool:
         """
```

### Comparing `esmerald-3.1.5/esmerald/contrib/auth/edgy/middleware.py` & `esmerald-3.2.0/esmerald/contrib/auth/edgy/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/contrib/auth/mongoz/base_user.py` & `esmerald-3.2.0/esmerald/contrib/auth/mongoz/base_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
         async def setter(raw_password: str) -> None:
             await self.set_password(raw_password)
             # Password hash upgrades shouldn't be considered password changes.
             self._password = None
             await self.update(password=self.password)
 
-        return check_password(raw_password, str(self.password), setter)
+        return await check_password(raw_password, str(self.password), setter)
 
     async def set_unusable_password(self) -> None:
         # Set a value that will never be a valid hash
         self.password = make_password(None)
 
     async def has_usable_password(self) -> bool:
         """
```

### Comparing `esmerald-3.1.5/esmerald/contrib/auth/mongoz/middleware.py` & `esmerald-3.2.0/esmerald/contrib/auth/mongoz/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/contrib/auth/saffier/base_user.py` & `esmerald-3.2.0/esmerald/contrib/auth/saffier/base_user.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         async def setter(raw_password: str) -> None:
             await self.set_password(raw_password)
             # Password hash upgrades shouldn't be considered password changes.
             self._password = None
             await self.update(password=self.password)
 
-        return check_password(raw_password, str(self.password), setter)
+        return await check_password(raw_password, str(self.password), setter)
 
     async def set_unusable_password(self) -> None:
         # Set a value that will never be a valid hash
         self.password = make_password(None)  # type: ignore
 
     async def has_usable_password(self) -> bool:
         """
```

### Comparing `esmerald-3.1.5/esmerald/contrib/auth/saffier/middleware.py` & `esmerald-3.2.0/esmerald/contrib/auth/saffier/middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/di/provider.py` & `esmerald-3.2.0/esmerald/core/di/provider.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/cli.py` & `esmerald-3.2.0/esmerald/core/directives/cli.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/env.py` & `esmerald-3.2.0/esmerald/core/directives/env.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/templates.py` & `esmerald-3.2.0/esmerald/core/directives/templates.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/utils.py` & `esmerald-3.2.0/esmerald/core/directives/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/operations/createapp.py` & `esmerald-3.2.0/esmerald/core/directives/operations/createapp.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/operations/createdeployment.py` & `esmerald-3.2.0/esmerald/core/directives/operations/createdeployment.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/operations/createproject.py` & `esmerald-3.2.0/esmerald/core/directives/operations/createproject.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/operations/list.py` & `esmerald-3.2.0/esmerald/core/directives/operations/list.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/operations/run.py` & `esmerald-3.2.0/esmerald/core/directives/operations/run.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/operations/runserver.py` & `esmerald-3.2.0/esmerald/core/directives/operations/runserver.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/operations/show_urls.py` & `esmerald-3.2.0/esmerald/core/directives/operations/show_urls.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/operations/shell/base.py` & `esmerald-3.2.0/esmerald/core/directives/operations/shell/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/operations/shell/ipython.py` & `esmerald-3.2.0/esmerald/core/directives/operations/shell/ipython.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/operations/shell/ptpython.py` & `esmerald-3.2.0/esmerald/core/directives/operations/shell/ptpython.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/directives/operations/shell/utils.py` & `esmerald-3.2.0/esmerald/core/directives/operations/shell/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/terminal/base.py` & `esmerald-3.2.0/esmerald/core/terminal/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/terminal/print.py` & `esmerald-3.2.0/esmerald/core/terminal/print.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/terminal/terminal.py` & `esmerald-3.2.0/esmerald/core/terminal/terminal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/core/urls/base.py` & `esmerald-3.2.0/esmerald/core/urls/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/datastructures/__init__.py` & `esmerald-3.2.0/esmerald/datastructures/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/datastructures/base.py` & `esmerald-3.2.0/esmerald/datastructures/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/datastructures/encoders.py` & `esmerald-3.2.0/esmerald/datastructures/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/datastructures/file.py` & `esmerald-3.2.0/esmerald/datastructures/file.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/datastructures/json.py` & `esmerald-3.2.0/esmerald/datastructures/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/datastructures/msgspec.py` & `esmerald-3.2.0/esmerald/datastructures/msgspec.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/datastructures/redirect.py` & `esmerald-3.2.0/esmerald/datastructures/redirect.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/datastructures/stream.py` & `esmerald-3.2.0/esmerald/datastructures/stream.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/datastructures/template.py` & `esmerald-3.2.0/esmerald/datastructures/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/interceptors/interceptor.py` & `esmerald-3.2.0/esmerald/interceptors/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/middleware/__init__.py` & `esmerald-3.2.0/esmerald/middleware/__init__.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/middleware/_exception_handlers.py` & `esmerald-3.2.0/esmerald/middleware/_exception_handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/middleware/app_settings.py` & `esmerald-3.2.0/esmerald/middleware/app_settings.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/middleware/asyncexitstack.py` & `esmerald-3.2.0/esmerald/middleware/asyncexitstack.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/middleware/authentication.py` & `esmerald-3.2.0/esmerald/middleware/authentication.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/middleware/exceptions.py` & `esmerald-3.2.0/esmerald/middleware/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Any, Callable, Dict, List, Mapping, Optional, Type, Union
 
 from lilya import status
-
 from lilya.exceptions import HTTPException as LilyaException
 from lilya.middleware.exceptions import ExceptionMiddleware as LilyaExceptionMiddleware
 from lilya.responses import Response as LilyaResponse
 from lilya.types import ASGIApp, Receive, Scope, Send
 from pydantic import BaseModel
 
 from esmerald.enums import MediaType, ScopeType
```

### Comparing `esmerald-3.1.5/esmerald/middleware/settings_middleware.py` & `esmerald-3.2.0/esmerald/middleware/settings_middleware.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/openapi/_internal.py` & `esmerald-3.2.0/esmerald/openapi/_internal.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/openapi/datastructures.py` & `esmerald-3.2.0/esmerald/openapi/datastructures.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Type, Union
+from typing import Any, List, Optional, Type, Union
 
 from pydantic import BaseModel, field_validator
 from typing_extensions import Annotated, Doc
 
 from esmerald.datastructures.msgspec import Struct
 from esmerald.enums import MediaType
 
@@ -31,15 +31,22 @@
     @post(path='/create', summary="Creates an item", responses={200: OpenAPIResponse(model=ItemOut, description="Successfully created an item")})
     async def create() -> Union[None, ItemOut]:
         ...
     ```
     """
 
     model: Annotated[
-        Union[Type[BaseModel], List[Type[BaseModel]], Type[Struct], List[Type[Struct]]],
+        Union[
+            Type[BaseModel],
+            List[Type[BaseModel]],
+            Type[Struct],
+            List[Type[Struct]],
+            Type[Any],
+            List[Type[Any]],
+        ],
         Doc(
             """
             A `pydantic.BaseModel` type of object of a `list` of
             `pydantic.BaseModel` types of objects.
 
             This is parsed and displayed in the [OpenAPI](https://esmerald.dev/openapi/)
             documentation.
@@ -89,14 +96,28 @@
             """
         ),
     ] = None
 
     @field_validator("model", mode="before")
     def validate_model(
         cls,
-        model: Union[Type[BaseModel], List[Type[BaseModel]], Type[Struct], List[Type[Struct]]],
-    ) -> Union[Type[BaseModel], List[Type[BaseModel]], Type[Struct], List[Type[Struct]]]:
+        model: Union[
+            Type[BaseModel],
+            List[Type[BaseModel]],
+            Type[Struct],
+            List[Type[Struct]],
+            Type[Any],
+            List[Type[Any]],
+        ],
+    ) -> Union[
+        Type[BaseModel],
+        List[Type[BaseModel]],
+        Type[Struct],
+        List[Type[Struct]],
+        Type[Any],
+        List[Type[Any]],
+    ]:
         if isinstance(model, list) and len(model) > 1:
             raise ValueError(
                 "The representation of a list of models in OpenAPI can only be a total of one. Example: OpenAPIResponse(model=[MyModel])."
             )
         return model
```

### Comparing `esmerald-3.1.5/esmerald/openapi/docs.py` & `esmerald-3.2.0/esmerald/openapi/docs.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/openapi/models.py` & `esmerald-3.2.0/esmerald/openapi/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/openapi/openapi.py` & `esmerald-3.2.0/esmerald/openapi/openapi.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/openapi/responses.py` & `esmerald-3.2.0/esmerald/openapi/responses.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/openapi/validation.py` & `esmerald-3.2.0/esmerald/openapi/validation.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/openapi/security/base.py` & `esmerald-3.2.0/esmerald/openapi/security/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/openapi/security/api_key/base.py` & `esmerald-3.2.0/esmerald/openapi/security/api_key/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/openapi/security/http/base.py` & `esmerald-3.2.0/esmerald/openapi/security/http/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/openapi/security/oauth2/base.py` & `esmerald-3.2.0/esmerald/openapi/security/oauth2/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/openapi/security/openid_connect/base.py` & `esmerald-3.2.0/esmerald/openapi/security/openid_connect/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/permissions/base.py` & `esmerald-3.2.0/esmerald/permissions/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/permissions/utils.py` & `esmerald-3.2.0/esmerald/permissions/utils.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/pluggables/base.py` & `esmerald-3.2.0/esmerald/pluggables/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/protocols/asyncdao.py` & `esmerald-3.2.0/esmerald/protocols/asyncdao.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/protocols/dao.py` & `esmerald-3.2.0/esmerald/protocols/dao.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/protocols/interceptor.py` & `esmerald-3.2.0/esmerald/protocols/interceptor.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/protocols/template.py` & `esmerald-3.2.0/esmerald/protocols/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/responses/base.py` & `esmerald-3.2.0/esmerald/responses/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,36 @@
-import dataclasses
-from dataclasses import is_dataclass
-from typing import TYPE_CHECKING, Any, Dict, Generic, NoReturn, Optional, TypeVar, Union, cast
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Dict,
+    Generic,
+    NoReturn,
+    Optional,
+    Sequence,
+    TypeVar,
+    Union,
+    cast,
+)
 
-import msgspec
 from lilya import status
 from lilya.responses import (
     Error as Error,
     FileResponse as FileResponse,  # noqa
     HTMLResponse as HTMLResponse,  # noqa
     JSONResponse as JSONResponse,  # noqa
     Ok as Ok,
     PlainText as PlainText,  # noqa
     RedirectResponse as RedirectResponse,  # noqa
     Response as LilyaResponse,  # noqa
     StreamingResponse as StreamingResponse,  # noqa
 )
 from orjson import OPT_OMIT_MICROSECONDS, OPT_SERIALIZE_NUMPY, dumps
-from pydantic import BaseModel
 from typing_extensions import Annotated, Doc
 
+from esmerald.encoders import Encoder, json_encoder
 from esmerald.enums import MediaType
 from esmerald.exceptions import ImproperlyConfigured
 
 PlainTextResponse = PlainText
 
 if TYPE_CHECKING:  # pragma: no cover
     from esmerald.backgound import BackgroundTask, BackgroundTasks
@@ -77,15 +85,15 @@
             Doc(
                 """
                 The response status code.
                 """
             ),
         ] = status.HTTP_200_OK,
         media_type: Annotated[
-            Optional[Union["MediaType", str]],
+            Optional[Union[MediaType, str]],
             Doc(
                 """
                 The media type used in the response.
                 """
             ),
         ] = MediaType.JSON,
         background: Annotated[
@@ -128,38 +136,56 @@
                 ]
 
                 Response(response_cookies=response_cookies)
                 ```
                 """
             ),
         ] = None,
+        encoders: Annotated[
+            Union[Sequence[Encoder], None],
+            Doc(
+                """
+                A sequence of `esmerald.encoders.Encoder` type of objects to be used
+                by the response object directly.
+
+                **Example**
+
+                ```python
+                from esmerald import Response
+                from esmerald.encoders import PydanticEncoder, MsgSpecEncoder
+
+                response_cookies=[
+                    encoders=[PydanticEncoder, MsgSpecEncoder]
+                ]
+
+                Response(response_cookies=response_cookies)
+                ```
+                """
+            ),
+        ] = None,
     ) -> None:
+
         super().__init__(
             content=content,
             status_code=status_code,
             headers=headers or {},
             media_type=media_type,
             background=cast("BackgroundTask", background),
+            encoders=encoders,
         )
         self.cookies = cookies or []
 
     @staticmethod
     def transform(value: Any) -> Dict[str, Any]:
         """
         The transformation of the data being returned.
 
-        It supports Pydantic models, `dataclasses` and `msgspec.Struct`.
+        Supports all the default encoders from Lilya and custom from Esmerald.
         """
-        if isinstance(value, BaseModel):
-            return value.model_dump()
-        if is_dataclass(value):
-            return dataclasses.asdict(value)
-        if isinstance(value, msgspec.Struct):
-            return msgspec.structs.asdict(value)
-        raise TypeError("unsupported type")  # pragma: no cover
+        return cast(Dict[str, Any], json_encoder(value))
 
     def make_response(self, content: Any) -> Union[bytes, str]:
         try:
             if (
                 content is None
                 or content is NoReturn
                 and (
```

### Comparing `esmerald-3.1.5/esmerald/responses/encoders.py` & `esmerald-3.2.0/esmerald/responses/encoders.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/responses/json.py` & `esmerald-3.2.0/esmerald/responses/json.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/responses/template.py` & `esmerald-3.2.0/esmerald/responses/template.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/routing/base.py` & `esmerald-3.2.0/esmerald/routing/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/routing/events.py` & `esmerald-3.2.0/esmerald/routing/events.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/routing/gateways.py` & `esmerald-3.2.0/esmerald/routing/gateways.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/routing/handlers.py` & `esmerald-3.2.0/esmerald/routing/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/routing/router.py` & `esmerald-3.2.0/esmerald/routing/router.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,21 +54,21 @@
     ValidationErrorException,
 )
 from esmerald.interceptors.types import Interceptor
 from esmerald.openapi.datastructures import OpenAPIResponse
 from esmerald.openapi.utils import is_status_code_allowed
 from esmerald.requests import Request
 from esmerald.responses import Response
-from esmerald.routing._internal import FieldInfoMixin
+from esmerald.routing._internal import OpenAPIFieldInfoMixin
 from esmerald.routing.apis.base import View
 from esmerald.routing.base import BaseInterceptorMixin
 from esmerald.routing.events import handle_lifespan_events
 from esmerald.routing.gateways import Gateway, WebhookGateway, WebSocketGateway
-from esmerald.transformers.datastructures import EsmeraldSignature as SignatureModel
 from esmerald.transformers.model import TransformerModel
+from esmerald.transformers.signature import SignatureModel
 from esmerald.transformers.utils import get_signature
 from esmerald.typing import Void, VoidType
 from esmerald.utils.constants import DATA, PAYLOAD, REDIRECT_STATUS_CODES, REQUEST, SOCKET
 from esmerald.utils.helpers import is_async_callable, is_class_and_subclass
 from esmerald.websockets import WebSocket, WebSocketClose
 
 if TYPE_CHECKING:  # pragma: no cover
@@ -993,15 +993,15 @@
             middleware=middleware,
         )
         self.validate_root_route_parent(websocket_gateway)
         self.create_signature_models(websocket_gateway)
         self.routes.append(websocket_gateway)
 
 
-class HTTPHandler(BaseInterceptorMixin, FieldInfoMixin, LilyaPath):
+class HTTPHandler(BaseInterceptorMixin, OpenAPIFieldInfoMixin, LilyaPath):
     __slots__ = (
         "path",
         "_interceptors",
         "_permissions",
         "_dependencies",
         "_response_handler",
         "_middleware",
@@ -1319,15 +1319,15 @@
         self.validate_reserved_kwargs()
 
     async def to_response(self, app: "Esmerald", data: Any) -> LilyaResponse:
         response_handler = self.get_response_handler()
         return await response_handler(app=app, data=data)  # type: ignore[call-arg]
 
 
-class WebhookHandler(HTTPHandler, FieldInfoMixin, LilyaPath):
+class WebhookHandler(HTTPHandler, OpenAPIFieldInfoMixin, LilyaPath):
     """
     Base for a webhook handler.
     """
 
     _slots__ = (
         "path",
         "_permissions",
```

### Comparing `esmerald-3.1.5/esmerald/routing/apis/_metaclasses.py` & `esmerald-3.2.0/esmerald/routing/apis/_metaclasses.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/routing/apis/_mixins.py` & `esmerald-3.2.0/esmerald/routing/apis/_mixins.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/routing/apis/base.py` & `esmerald-3.2.0/esmerald/routing/apis/base.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/routing/apis/generics.py` & `esmerald-3.2.0/esmerald/routing/apis/generics.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/routing/apis/views.py` & `esmerald-3.2.0/esmerald/routing/apis/views.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/routing/webhooks/handlers.py` & `esmerald-3.2.0/esmerald/routing/webhooks/handlers.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/security/jwt/token.py` & `esmerald-3.2.0/esmerald/security/jwt/token.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/template/jinja.py` & `esmerald-3.2.0/esmerald/template/jinja.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/template/mako.py` & `esmerald-3.2.0/esmerald/template/mako.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/transformers/model.py` & `esmerald-3.2.0/esmerald/transformers/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pydantic.fields import FieldInfo
 
 from esmerald.context import Context
 from esmerald.enums import EncodingType, ParamType
 from esmerald.exceptions import ImproperlyConfigured
 from esmerald.parsers import ArbitraryExtraBaseModel, parse_form_data
 from esmerald.requests import Request
-from esmerald.transformers.datastructures import EsmeraldSignature as SignatureModel
+from esmerald.transformers.signature import SignatureModel
 from esmerald.transformers.utils import (
     Dependency,
     ParamSetting,
     create_parameter_setting,
     get_request_params,
     get_signature,
     merge_sets,
@@ -26,27 +26,56 @@
 
 
 MEDIA_TYPES = [EncodingType.MULTI_PART, EncodingType.URL_ENCODED]
 MappingUnion = Mapping[Union[int, str], Any]
 
 
 class TransformerModel(ArbitraryExtraBaseModel):
+    """
+    Represents a transformer model with parameters and dependencies.
+
+    Attributes:
+        cookies (Set[ParamSetting]): Set of cookie parameters.
+        dependencies (Set[Dependency]): Set of dependencies.
+        form_data (Optional[Tuple[EncodingType, FieldInfo]]): Optional form data information.
+        headers (Set[ParamSetting]): Set of header parameters.
+        path_params (Set[ParamSetting]): Set of path parameters.
+        query_params (Set[ParamSetting]): Set of query parameters.
+        reserved_kwargs (Set[str]): Set of reserved keyword arguments.
+        has_kwargs (bool): Flag indicating if any kwargs are present.
+        is_optional (bool): Flag indicating if the model is optional.
+    """
+
     def __init__(
         self,
         cookies: Set[ParamSetting],
         dependencies: Set[Dependency],
         form_data: Optional[Tuple[EncodingType, FieldInfo]],
         headers: Set[ParamSetting],
         path_params: Set[ParamSetting],
         query_params: Set[ParamSetting],
         reserved_kwargs: Set[str],
         query_param_names: Set[ParamSetting],
         is_optional: bool,
         **kwargs: Any,
     ):
+        """
+        Initialize a TransformerModel instance.
+
+        Args:
+            cookies (Set[ParamSetting]): Set of cookie parameters.
+            dependencies (Set[Dependency]): Set of dependencies.
+            form_data (Optional[Tuple[EncodingType, FieldInfo]]): Optional form data information.
+            headers (Set[ParamSetting]): Set of header parameters.
+            path_params (Set[ParamSetting]): Set of path parameters.
+            query_params (Set[ParamSetting]): Set of query parameters.
+            reserved_kwargs (Set[str]): Set of reserved keyword arguments.
+            is_optional (bool): Flag indicating if the model is optional.
+            **kwargs (Any): Additional keyword arguments.
+        """
         super().__init__(**kwargs)
         self.cookies = cookies
         self.dependencies = dependencies
         self.form_data = form_data
         self.headers = headers
         self.path_params = path_params
         self.query_params = query_params
@@ -60,23 +89,47 @@
             or path_params
             or query_params
             or reserved_kwargs
         )
         self.is_optional = is_optional
 
     def get_cookie_params(self) -> Set[ParamSetting]:
+        """
+        Get cookie parameters.
+
+        Returns:
+            Set[ParamSetting]: Set of cookie parameters.
+        """
         return self.cookies
 
     def get_path_params(self) -> Set[ParamSetting]:
+        """
+        Get path parameters.
+
+        Returns:
+            Set[ParamSetting]: Set of path parameters.
+        """
         return self.path_params
 
     def get_query_params(self) -> Set[ParamSetting]:
+        """
+        Get query parameters.
+
+        Returns:
+            Set[ParamSetting]: Set of query parameters.
+        """
         return self.query_params
 
     def get_header_params(self) -> Set[ParamSetting]:
+        """
+        Get header parameters.
+
+        Returns:
+            Set[ParamSetting]: Set of header parameters.
+        """
         return self.headers
 
     def to_kwargs(
         self,
         connection: Union["WebSocket", "Request"],
         handler: Union["HTTPHandler", "WebSocketHandler"] = None,
     ) -> Any:
@@ -116,24 +169,216 @@
             path_params=path_params,
             query_params=query_params,
             headers=headers,
             cookies=cookies,
             handler=handler,
         )
 
+    async def get_request_data(self, request: Request) -> Any:
+        """
+        Get request data asynchronously.
+
+        Args:
+            request (Request): HTTP Request object.
+
+        Returns:
+            Any: Parsed form data or JSON payload.
+        """
+        if not self.form_data:
+            return await request.json()
+
+        media_type, field = self.form_data
+        form_data = await request.form()
+        parsed_form = parse_form_data(media_type, form_data, field)
+        return parsed_form if parsed_form or not self.is_optional else None
+
+    def get_request_context(
+        self, handler: Union["HTTPHandler", "WebSocketHandler"], request: Request
+    ) -> Context:
+        """
+        Get request context.
+
+        Args:
+            handler (Union[HTTPHandler, WebSocketHandler]): HTTP or WebSocket handler.
+            request (Request): HTTP Request object.
+
+        Returns:
+            Context: Context object containing handler and request information.
+        """
+        return Context(__handler__=handler, __request__=request)
+
+    async def get_dependencies(
+        self, dependency: Dependency, connection: Union["WebSocket", Request], **kwargs: Any
+    ) -> Any:
+        """
+        Get dependencies asynchronously.
+
+        Args:
+            dependency (Dependency): Dependency object.
+            connection (Union[WebSocket, Request]): WebSocket or HTTP Request object.
+            **kwargs (Any): Additional keyword arguments.
+
+        Returns:
+            Any: Dependencies resolved from the connection and dependencies.
+        """
+        signature_model = get_signature(dependency.inject)
+        for _dependency in dependency.dependencies:
+            kwargs[_dependency.key] = await self.get_dependencies(
+                dependency=_dependency, connection=connection, **kwargs
+            )
+        dependency_kwargs = signature_model.parse_values_for_connection(
+            connection=connection, **kwargs
+        )
+        return await dependency.inject(**dependency_kwargs)
+
+    def to_dict(self) -> Dict[str, Any]:
+        """
+        Convert TransformerModel instance to dictionary.
+
+        Returns:
+            Dict[str, Any]: Dictionary representation of TransformerModel instance.
+        """
+        return {
+            "cookies": [param.dict() for param in self.cookies],
+            "dependencies": [dep.dict() for dep in self.dependencies],
+            "form_data": self.form_data,
+            "headers": [param.dict() for param in self.headers],
+            "path_params": [param.dict() for param in self.path_params],
+            "query_params": [param.dict() for param in self.query_params],
+            "reserved_kwargs": list(self.reserved_kwargs),
+            "is_optional": self.is_optional,
+        }
+
+    @classmethod
+    def from_dict(cls, data: Dict[str, Any]) -> "TransformerModel":
+        """
+        Create TransformerModel instance from dictionary.
+
+        Args:
+            data (Dict[str, Any]): Dictionary containing TransformerModel attributes.
+
+        Returns:
+            TransformerModel: TransformerModel instance created from dictionary.
+        """
+        return cls(
+            cookies={ParamSetting(**param) for param in data.get("cookies", [])},
+            dependencies={Dependency(**dep) for dep in data.get("dependencies", [])},
+            form_data=data.get("form_data"),
+            headers={ParamSetting(**param) for param in data.get("headers", [])},
+            path_params={ParamSetting(**param) for param in data.get("path_params", [])},
+            query_params={ParamSetting(**param) for param in data.get("query_params", [])},
+            query_param_names={
+                ParamSetting(**param) for param in data.get("query_param_names", [])
+            },
+            reserved_kwargs=set(data.get("reserved_kwargs", [])),
+            is_optional=data.get("is_optional", False),
+        )
+
+    def merge_with(self, other: "TransformerModel") -> "TransformerModel":
+        """
+        Merge with another TransformerModel instance.
+
+        Args:
+            other (TransformerModel): Another TransformerModel instance to merge with.
+
+        Returns:
+            TransformerModel: Merged TransformerModel instance.
+        """
+        return TransformerModel(
+            cookies=merge_sets(self.cookies, other.cookies),
+            dependencies=merge_sets(self.dependencies, other.dependencies),  # type: ignore
+            form_data=self.form_data if self.form_data == other.form_data else None,
+            headers=merge_sets(self.headers, other.headers),
+            path_params=merge_sets(self.path_params, other.path_params),
+            query_params=merge_sets(self.query_params, other.query_params),
+            query_param_names=merge_sets(self.query_param_names, other.query_param_names),
+            reserved_kwargs=self.reserved_kwargs.union(other.reserved_kwargs),
+            is_optional=self.is_optional or other.is_optional,
+        )
+
+    def _get_request_params(
+        self,
+        connection: Union["WebSocket", "Request"],
+        handler: Union["HTTPHandler", "WebSocketHandler"] = None,
+    ) -> Any:
+        """
+        Get request parameters.
+
+        Args:
+            connection (Union["WebSocket", "Request"]): Connection object.
+            handler (Union["HTTPHandler", "WebSocketHandler"], optional): Handler object. Defaults to None.
+
+        Returns:
+            Any: Request parameters.
+        """
+        connection_params: Dict[str, Any] = {}
+        for key, value in connection.query_params.items():
+            if key not in self.query_param_names and len(value) == 1:
+                value = value[0]
+                connection_params[key] = value
+
+        query_params = get_request_params(
+            params=cast("MappingUnion", connection.query_params),
+            expected=self.query_params,
+            url=connection.url,
+        )
+        path_params = get_request_params(
+            params=cast("MappingUnion", connection.path_params),
+            expected=self.path_params,
+            url=connection.url,
+        )
+        headers = get_request_params(
+            params=cast("MappingUnion", connection.headers),
+            expected=self.headers,
+            url=connection.url,
+        )
+        cookies = get_request_params(
+            params=cast("MappingUnion", connection.cookies),
+            expected=self.cookies,
+            url=connection.url,
+        )
+
+        if not self.reserved_kwargs:
+            return {**query_params, **path_params, **headers, **cookies}
+
+        return self.handle_reserved_kwargs(
+            connection=connection,
+            connection_params=connection_params,
+            path_params=path_params,
+            query_params=query_params,
+            headers=headers,
+            cookies=cookies,
+            handler=handler,
+        )
+
     def handle_reserved_kwargs(
         self,
         connection: Union["WebSocket", "Request"],
         connection_params: Any,
         path_params: Any,
         query_params: Any,
         headers: Any,
         cookies: Any,
         handler: Optional[Any] = None,
     ) -> Any:
+        """
+        Handle reserved keyword arguments.
+
+        Args:
+            connection (Union["WebSocket", "Request"]): Connection object.
+            connection_params (Any): Connection parameters.
+            path_params (Any): Path parameters.
+            query_params (Any): Query parameters.
+            headers (Any): Headers.
+            cookies (Any): Cookies.
+            handler (Optional[Any], optional): Handler object. Defaults to None.
+
+        Returns:
+            Any: Reserved keyword arguments.
+        """
         reserved_kwargs: Any = {}
         if DATA in self.reserved_kwargs:
             reserved_kwargs[DATA] = self.get_request_data(request=cast("Request", connection))
         if PAYLOAD in self.reserved_kwargs:
             reserved_kwargs[PAYLOAD] = self.get_request_data(request=cast("Request", connection))
 
         if CONTEXT in self.reserved_kwargs and handler is not None:
@@ -152,124 +397,75 @@
         if "query" in self.reserved_kwargs:
             reserved_kwargs["query"] = connection_params
         if "state" in self.reserved_kwargs:
             reserved_kwargs["state"] = connection.app.state.copy()  # pragma: no cover
 
         return {**reserved_kwargs, **path_params, **query_params, **headers, **cookies}
 
-    async def get_request_data(self, request: "Request") -> Any:
-        # Fast exit principle
-        if not self.form_data:
-            return await request.json()
-
-        media_type, field = self.form_data
-        form_data = await request.form()
-        parsed_form = parse_form_data(media_type, form_data, field)
-        return parsed_form if parsed_form or not self.is_optional else None
-
-    def get_request_context(
-        self, handler: Union["HTTPHandler", "WebSocketHandler"], request: "Request"
-    ) -> Context:
-        """
-        Generates the context of the handler where additional information can be provided and passed properly.
-        """
-        return Context(__handler__=handler, __request__=request)
 
-    async def get_dependencies(
-        self,
-        dependency: "Dependency",
-        connection: Union["WebSocket", "Request"],
-        **kwargs: Any,
-    ) -> Any:
-        signature_model = get_signature(dependency.inject)
-        for _dependency in dependency.dependencies:
-            kwargs[_dependency.key] = await self.get_dependencies(
-                dependency=_dependency, connection=connection, **kwargs
-            )
-        dependency_kwargs = signature_model.parse_values_for_connection(
-            connection=connection, **kwargs
-        )
-        return await dependency.inject(**dependency_kwargs)
+def dependency_tree(key: str, dependencies: "Dependencies") -> Dependency:
+    """
+    Recursively build a dependency tree starting from a given key.
 
+    Args:
+        key (str): Key of the dependency to start building from.
+        dependencies (Dependencies): Dictionary of dependencies.
 
-def dependency_tree(key: str, dependencies: "Dependencies") -> Dependency:
+    Returns:
+        Dependency: Constructed dependency tree starting from the specified key.
+    """
     inject = dependencies[key]
     dependency_keys = [key for key in get_signature(inject).model_fields if key in dependencies]
     return Dependency(
         key=key,
         inject=inject,
         dependencies=[
             dependency_tree(key=key, dependencies=dependencies) for key in dependency_keys
         ],
     )
 
 
 def get_parameter_settings(
     path_parameters: Set[str], dependencies: Dict[str, Any], signature_fields: Dict[str, Any]
-) -> Tuple[Set[ParamSetting], Set["Dependency"]]:
+) -> Tuple[Set[ParamSetting], Set[Dependency]]:
     """
-    Get parameter settings and dependencies for given inputs.
+    Get parameter settings and dependencies based on input data.
 
     Args:
-        path_parameters (set): Set of path parameters.
-        dependencies (dict): Dependency information.
-        signature_fields (dict): Dictionary containing field information.
+        path_parameters (Set[str]): Set of path parameters.
+        dependencies (Dict[str, Any]): Dictionary of dependencies.
+        signature_fields (Dict[str, Any]): Dictionary containing field information.
 
     Returns:
-        tuple: A tuple containing sets of parameter settings and dependencies.
+        Tuple[Set[ParamSetting], Set[Dependency]]: Tuple containing sets of parameter settings
+        and dependencies.
     """
-
-    # Set to store dependencies
-    _dependencies: Any = set()
-
-    # Set to store ignored keys
+    _dependencies: Set[Dependency] = set()
     ignored_keys = {
         *RESERVED_KWARGS,
         *(dependency.key for dependency in _dependencies),
     }
+    parameter_definitions: Set[ParamSetting] = set()
 
-    # Set to store parameter definitions
-    parameter_definitions = set()
-
-    # Iterate through dependencies to add relevant dependencies
     for key in dependencies:
         if key in signature_fields:
             _dependencies.add(dependency_tree(key=key, dependencies=dependencies))
 
-    # Iterate through signature fields to create parameter settings
     for field_name, model_field in signature_fields.items():
         if field_name not in ignored_keys:
             allow_none = getattr(model_field, "allow_none", True)
             parameter_definitions.add(
                 create_parameter_setting(
                     allow_none=allow_none,
                     field_name=field_name,
                     field_info=model_field,
                     path_parameters=path_parameters,
                 )
             )
 
-    # Filter out ignored keys and create parameter settings
-    filtered = [
-        (field_name, model_field)
-        for field_name, model_field in signature_fields.items()
-        if field_name not in ignored_keys
-    ]
-    for field_name, model_field in filtered:
-        signature_field = model_field
-        allow_none = getattr(signature_field, "allow_none", True)
-        parameter_definitions.add(
-            create_parameter_setting(
-                allow_none=allow_none,
-                field_name=field_name,
-                field_info=signature_field,
-                path_parameters=path_parameters,
-            )
-        )
-
     return parameter_definitions, _dependencies
 
 
 def _filter_param_settings_by_type(
     param_settings: Set[ParamSetting], param_type: ParamType
 ) -> Set[ParamSetting]:
     """
@@ -282,38 +478,39 @@
     Returns:
         Set[ParamSetting]: Filtered parameter settings.
     """
     return {param for param in param_settings if param.param_type == param_type}
 
 
 def _get_form_data(
-    signature_model: Type[SignatureModel],
-) -> Optional[Tuple["EncodingType", "FieldInfo"]]:
+    signature_model: Type["SignatureModel"],
+) -> Optional[Tuple[EncodingType, FieldInfo]]:
     """
     Get form data from the signature model.
 
     Args:
         signature_model (Type[SignatureModel]): The signature model.
 
     Returns:
-        Optional[Tuple[str, Any]]: Tuple containing media type and data field, or None.
+        Optional[Tuple[EncodingType, FieldInfo]]: Tuple containing media type and data
+        field information, or None if not found.
     """
     data_field = signature_model.model_fields.get(DATA) or signature_model.model_fields.get(
         PAYLOAD
     )
     if data_field:
         extra = getattr(data_field, "json_schema_extra", None) or {}
         media_type = extra.get("media_type")
         if media_type in MEDIA_TYPES:
             return media_type, data_field
     return None
 
 
 def create_signature(
-    signature_model: Type[SignatureModel],
+    signature_model: Type["SignatureModel"],
     dependencies: "Dependencies",
     path_parameters: Set[str],
 ) -> "TransformerModel":
     """
     Create a transformer model based on the signature model.
 
     Args:
@@ -341,17 +538,16 @@
     )
 
     path_params = _filter_param_settings_by_type(param_settings, ParamType.PATH)
     query_params = _filter_param_settings_by_type(param_settings, ParamType.QUERY)
     cookies = _filter_param_settings_by_type(param_settings, ParamType.COOKIE)
     headers = _filter_param_settings_by_type(param_settings, ParamType.HEADER)
 
-    form_data: Union[Tuple["EncodingType", "FieldInfo"], None] = _get_form_data(signature_model)
+    form_data = _get_form_data(signature_model)
 
-    # Update parameters
     (
         path_params,
         query_params,
         cookies,
         headers,
         reserved_kwargs,
     ) = update_parameters(
@@ -367,34 +563,34 @@
     )
 
     is_optional = False
     if DATA in reserved_kwargs and PAYLOAD in reserved_kwargs:
         raise ImproperlyConfigured("Only 'data' or 'payload' must be provided but not both.")
 
     if DATA in reserved_kwargs:
-        is_optional = is_field_optional(signature_model.model_fields["data"])
+        is_optional = is_field_optional(signature_model.model_fields[DATA])
     elif PAYLOAD in reserved_kwargs:
-        is_optional = is_field_optional(signature_model.model_fields["payload"])
+        is_optional = is_field_optional(signature_model.model_fields[PAYLOAD])
 
-    query_param_names: Any = set()
+    query_param_names: Set[ParamSetting] = set()
     return TransformerModel(
         form_data=form_data,
         dependencies=_dependencies,
         path_params=path_params,
         query_params=query_params,
         cookies=cookies,
         headers=headers,
         reserved_kwargs=reserved_kwargs,
         query_param_names=query_param_names,
         is_optional=is_optional,
     )
 
 
 def _update_parameters_with_dependency(
-    dependency: "Dependency",
+    dependency: Dependency,
     global_dependencies: "Dependencies",
     path_params: Any,
     query_params: Any,
     cookies: Any,
     headers: Any,
     reserved_kwargs: Any,
     path_parameters: Any,
@@ -434,15 +630,15 @@
     reserved_kwargs.update(dependency_model.reserved_kwargs)
 
     return path_params, query_params, cookies, headers, reserved_kwargs
 
 
 def update_parameters(
     global_dependencies: "Dependencies",
-    local_dependencies: Set["Dependency"],
+    local_dependencies: Set[Dependency],
     path_params: Any,
     query_params: Any,
     cookies: Any,
     headers: Any,
     reserved_kwargs: Any,
     path_parameters: Any,
     form_data: Any,
@@ -480,67 +676,78 @@
         )
 
     return path_params, query_params, cookies, headers, reserved_kwargs
 
 
 def validate_data(
     form_data: Optional[Tuple[EncodingType, FieldInfo]],
-    dependency_model: "TransformerModel",
-) -> None:  # pragma: no cover
+    dependency_model: TransformerModel,
+) -> None:
+    """
+    Validate compatibility of form data
+    between two models.
+
+    Args:
+        form_data (Optional[Tuple[EncodingType, FieldInfo]]): Form data tuple containing
+            media type and data field information, or None.
+        dependency_model (TransformerModel): Transformer model to validate against.
+
+    Raises:
+        ImproperlyConfigured: If dependencies have incompatible form-data encoding or
+            incompatible 'data' kwarg types.
+    """
     if form_data and dependency_model.form_data:
         media_type, _ = form_data
         dependency_media_type, _ = dependency_model.form_data
         if media_type != dependency_media_type:
             raise ImproperlyConfigured(
                 "Dependencies have incompatible form-data encoding. "
                 "They should both be the same. Either url-encoded or multi-part."
             )
-    if (
-        (form_data and not dependency_model.form_data)
-        or not form_data
-        and dependency_model.form_data
+    if (form_data and not dependency_model.form_data) or (
+        not form_data and dependency_model.form_data
     ):
         raise ImproperlyConfigured(
-            "Dependencies haev incompativle 'data' kwarg types. "
+            "Dependencies have incompatible 'data' kwarg types. "
             "One expects JSON and the other expects form-data."
         )
 
 
 def _get_names_from_model_fields(model_fields: Dict[str, FieldInfo]) -> Set[str]:
     """
-    Extract names from model fields.
+    Extract names from model fields that have additional metadata relevant for parameters.
 
     Args:
         model_fields (Dict[str, FieldInfo]): Dictionary of model fields.
 
     Returns:
         Set[str]: Set of names extracted from model fields.
     """
     names = set()
     for key, value in model_fields.items():
         if value.json_schema_extra is not None:
-            extra = cast("Dict[str, Any]", value.json_schema_extra)
+            extra = cast(Dict[str, Any], value.json_schema_extra)
             if (
                 extra.get(ParamType.QUERY)
                 or extra.get(ParamType.HEADER)
                 or extra.get(ParamType.COOKIE)
             ):
                 names.add(key)
     return names
 
 
 def _check_ambiguity_in_kwargs(
-    path_parameters: Set[str], dependencies: "Dependencies", model_fields: Dict[str, FieldInfo]
+    path_parameters: Set[str], dependencies: Dict[str, Any], model_fields: Dict[str, FieldInfo]
 ) -> None:
     """
-    Check ambiguity in keyword argument resolution.
+    Check for ambiguity in keyword argument resolution.
 
     Args:
         path_parameters (Set[str]): Set of path parameters.
-        dependencies (Dependencies): Dependency information.
+        dependencies (Dict[str, Any]): Dependency information.
         model_fields (Dict[str, FieldInfo]): Dictionary of model fields.
 
     Raises:
         ImproperlyConfigured: If ambiguity in keyword argument resolution is detected.
     """
     keys = set(dependencies.keys())
     names = _get_names_from_model_fields(model_fields)
@@ -555,23 +762,23 @@
             f"Ambiguity in kwarg resolution: {', '.join(intersection)}. "
             f"Please make sure to use unique distinct keys for your dependencies and path parameters."
         )
 
 
 def validate_kwargs(
     path_parameters: Set[str],
-    dependencies: "Dependencies",
+    dependencies: Dict[str, Any],
     model_fields: Dict[str, FieldInfo],
 ) -> None:
     """
-    Validate keyword arguments.
+    Validate keyword arguments for parameter and dependency definitions.
 
     Args:
         path_parameters (Set[str]): Set of path parameters.
-        dependencies (Dependencies): Dependency information.
+        dependencies (Dict[str, Any]): Dependency information.
         model_fields (Dict[str, FieldInfo]): Dictionary of model fields.
 
     Raises:
         ImproperlyConfigured: If keyword arguments are invalid.
     """
     _check_ambiguity_in_kwargs(path_parameters, dependencies, model_fields)
```

### Comparing `esmerald-3.1.5/esmerald/transformers/utils.py` & `esmerald-3.2.0/esmerald/transformers/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from esmerald.parsers import ArbitraryExtraBaseModel, HashableBaseModel
 from esmerald.requests import Request
 from esmerald.typing import Undefined
 from esmerald.utils.constants import REQUIRED
 
 if TYPE_CHECKING:  # pragma: no cover
     from esmerald.injector import Inject
-    from esmerald.transformers.datastructures import EsmeraldSignature, Parameter
+    from esmerald.transformers.signature import Parameter, SignatureModel
     from esmerald.types import ConnectionType
 
 
 class ParamSetting(NamedTuple):
     default_value: Any
     field_alias: str
     field_name: str
@@ -197,17 +197,17 @@
     """
     Extacts the information from the ConnectionType.
     """
     method = connection.method if isinstance(connection, Request) else ScopeType.WEBSOCKET
     return method, connection.url
 
 
-def get_signature(value: Any) -> Type["EsmeraldSignature"]:
+def get_signature(value: Any) -> Type["SignatureModel"]:
     try:
-        return cast("Type[EsmeraldSignature]", value.signature_model)
+        return cast("Type[SignatureModel]", value.signature_model)
     except AttributeError as exc:
         raise ImproperlyConfigured(f"The 'signature' attribute for {value} is not set.") from exc
 
 
 def get_field_definition_from_param(param: "Parameter") -> Tuple[Any, Any]:
     if param.default_defined:
         definition = param.annotation, param.default
```

### Comparing `esmerald-3.1.5/esmerald/utils/constants.py` & `esmerald-3.2.0/esmerald/utils/constants.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/utils/dependency.py` & `esmerald-3.2.0/esmerald/utils/dependency.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/utils/functional.py` & `esmerald-3.2.0/esmerald/utils/functional.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/utils/helpers.py` & `esmerald-3.2.0/esmerald/utils/helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,27 @@
 import sys
 import typing
 from inspect import isclass
 from typing import Any, Union
 
 import slugify
+from lilya._utils import is_class_and_subclass as is_class_and_subclass
 from lilya.compat import is_async_callable as is_async_callable
 from typing_extensions import get_args, get_origin
 
 from esmerald.datastructures.msgspec import Struct
 
 if sys.version_info >= (3, 10):
     from types import UnionType
 
     UNION_TYPES = {UnionType, Union}
 else:  # pragma: no cover
     UNION_TYPES = {Union}
 
 
-def is_class_and_subclass(value: typing.Any, _type: typing.Any) -> bool:
-    original = get_origin(value)
-    if not original and not isclass(value):
-        return False
-
-    try:
-        if original:
-            return original and issubclass(original, _type)
-        return issubclass(value, _type)
-    except TypeError:
-        return False
-
-
 def is_msgspec_struct(value: typing.Any) -> bool:
     """
     Analyses if is a msgspec.Struct and uses this for OpenAPI
     documentation generation.
     """
     original = get_origin(value)
     if not original and not isclass(value):
```

### Comparing `esmerald-3.1.5/esmerald/utils/models.py` & `esmerald-3.2.0/esmerald/utils/models.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/utils/sync.py` & `esmerald-3.2.0/esmerald/utils/sync.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/esmerald/utils/pydantic/schema.py` & `esmerald-3.2.0/esmerald/utils/pydantic/schema.py`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/LICENSE` & `esmerald-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/README.md` & `esmerald-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `esmerald-3.1.5/pyproject.toml` & `esmerald-3.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,34 @@
 schedulers = ["asyncz>=0.4.0"]
 all = [
     "esmerald[test,dev,templates,jwt,encoders,schedulers]",
     "ipython",
     "ptpython",
     "a2wsgi",
 ]
+testing = [
+    "ipdb",
+    "pdbpp",
+    "pytest>=7.1.3,<9.0.0",
+    "pytest-cov>=4.1.0,<6.0.0",
+    "pytest-asyncio>=0.20.0",
+    "mypy==1.9.0",
+    "anyio[trio]>=3.6.2,<5.0.0",
+    "brotli>=1.0.9,<2.0.0",
+    "flask>=1.1.2,<4.0.0",
+    "freezegun>=1.2.2,<2.0.0",
+    "polyfactory>=2.5.0,<3.0.0",
+    "saffier[postgres]>=1.3.7",
+    "edgy[postgres]>=0.4.0",
+    "mongoz>=0.6.0",
+
+    # types
+    "types-ujson==5.10.0.20240515",
+    "types-orjson==3.6.2",
+]
 
 [tool.hatch.envs.default]
 dependencies = ["ruff", "pre-commit>=2.17.0,<3.0.0", "twine"]
 
 [tool.hatch.envs.default.scripts]
 clean_pyc = "find . -type f -name \"*.pyc\" -delete"
 clean_pyi = "find . -type f -name \"*.pyi\" -delete"
@@ -138,37 +158,21 @@
     "pyyaml>=6.0,<7.0.0",
 ]
 [tool.hatch.envs.docs.scripts]
 build = "mkdocs build"
 serve = "mkdocs serve --dev-addr localhost:8000"
 
 [tool.hatch.envs.test]
-features = ["all"]
-dependencies = [
-    "pytest>=7.1.3,<9.0.0",
-    "pytest-cov>=4.1.0,<6.0.0",
-    "pytest-asyncio>=0.20.0",
-    "mypy==1.9.0",
-    "anyio[trio]>=3.6.2,<5.0.0",
-    "brotli>=1.0.9,<2.0.0",
-    "flask>=1.1.2,<4.0.0",
-    "freezegun>=1.2.2,<2.0.0",
-    "polyfactory>=2.5.0,<3.0.0",
-    "saffier[postgres]>=1.3.7",
-    "edgy[postgres]>=0.4.0",
-    "mongoz>=0.6.0",
+features = ["all", "testing"]
 
-    # types
-    "types-ujson==5.9.0.0",
-    "types-orjson==3.6.2",
-]
 [tool.hatch.envs.test.scripts]
 # needs docker services running
 test = "ESMERALD_SETTINGS_MODULE='tests.settings.TestSettings' pytest {args}"
-coverage = "ESMERALD_SETTINGS_MODULE='tests.settings.TestSettings' pytest --cov=asyncz --cov=tests --cov-report=term-missing:skip-covered --cov-report=html tests {args}"
+test_man = "ESMERALD_SETTINGS_MODULE='tests.settings.TestSettings' pytest {args} -s -vv"
+coverage = "ESMERALD_SETTINGS_MODULE='tests.settings.TestSettings' pytest --cov=esmerald --cov=tests --cov-report=term-missing:skip-covered --cov-report=html tests {args}"
 check_types = "mypy -p esmerald"
 
 [tool.hatch.envs.hatch-test]
 features = ["all"]
 template = "test"
 installer = "pip"
 
@@ -203,14 +207,17 @@
 exclude = "esmerald/conf,esmerald/utils"
 warn_unused_ignores = true
 warn_redundant_casts = true
 no_implicit_optional = false
 strict_equality = false
 strict_optional = false
 
+[tool.ruff]
+line-length = 99
+
 [tool.ruff.lint]
 select = ["E", "W", "F", "C", "B", "I"]
 ignore = ["E501", "B008", "C901", "B026"]
 
 exclude = ["docs_src/*"]
 
 [tool.coverage.run]
```

### Comparing `esmerald-3.1.5/PKG-INFO` & `esmerald-3.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 330a 4e61 6d65 3a20 6573 6d65  : 2.3.Name: esme
 00000020: 7261 6c64 0a56 6572 7369 6f6e 3a20 332e  rald.Version: 3.
-00000030: 312e 350a 5375 6d6d 6172 793a 2048 6967  1.5.Summary: Hig
+00000030: 322e 300a 5375 6d6d 6172 793a 2048 6967  2.0.Summary: Hig
 00000040: 686c 7920 7363 616c 6162 6c65 2c20 7065  hly scalable, pe
 00000050: 7266 6f72 6d61 6e74 2c20 6561 7379 2074  rformant, easy t
 00000060: 6f20 6c65 6172 6e2c 2065 6173 7920 746f  o learn, easy to
 00000070: 2063 6f64 6520 616e 6420 666f 7220 6576   code and for ev
 00000080: 6572 7920 6170 706c 6963 6174 696f 6e2e  ery application.
 00000090: 0a50 726f 6a65 6374 2d55 524c 3a20 486f  .Project-URL: Ho
 000000a0: 6d65 7061 6765 2c20 6874 7470 733a 2f2f  mepage, https://
@@ -219,1075 +219,1132 @@
 00000da0: 7374 3a20 6d61 6b6f 3c32 2e30 2e30 2c3e  st: mako<2.0.0,>
 00000db0: 3d31 2e32 2e34 3b20 6578 7472 6120 3d3d  =1.2.4; extra ==
 00000dc0: 2027 7465 6d70 6c61 7465 7327 0a50 726f   'templates'.Pro
 00000dd0: 7669 6465 732d 4578 7472 613a 2074 6573  vides-Extra: tes
 00000de0: 740a 5265 7175 6972 6573 2d44 6973 743a  t.Requires-Dist:
 00000df0: 2068 7474 7078 3c30 2e33 302e 302c 3e3d   httpx<0.30.0,>=
 00000e00: 302e 3235 2e30 3b20 6578 7472 6120 3d3d  0.25.0; extra ==
-00000e10: 2027 7465 7374 270a 4465 7363 7269 7074   'test'.Descript
-00000e20: 696f 6e2d 436f 6e74 656e 742d 5479 7065  ion-Content-Type
-00000e30: 3a20 7465 7874 2f6d 6172 6b64 6f77 6e0a  : text/markdown.
-00000e40: 0a23 2045 736d 6572 616c 640a 0a3c 7020  .# Esmerald..<p 
-00000e50: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
-00000e60: 2020 3c61 2068 7265 663d 2268 7474 7073    <a href="https
-00000e70: 3a2f 2f65 736d 6572 616c 642e 6465 7622  ://esmerald.dev"
-00000e80: 3e3c 696d 6720 7372 633d 2268 7474 7073  ><img src="https
-00000e90: 3a2f 2f72 6573 2e63 6c6f 7564 696e 6172  ://res.cloudinar
-00000ea0: 792e 636f 6d2f 6479 6d6d 6f6e 642f 696d  y.com/dymmond/im
-00000eb0: 6167 652f 7570 6c6f 6164 2f76 3136 3733  age/upload/v1673
-00000ec0: 3631 3933 3432 2f65 736d 6572 616c 642f  619342/esmerald/
-00000ed0: 696d 672f 6c6f 676f 2d67 725f 7a31 6f74  img/logo-gr_z1ot
-00000ee0: 386f 2e70 6e67 2220 616c 743d 2745 736d  8o.png" alt='Esm
-00000ef0: 6572 616c 6427 3e3c 2f61 3e0a 3c2f 703e  erald'></a>.</p>
-00000f00: 0a0a 3c70 2061 6c69 676e 3d22 6365 6e74  ..<p align="cent
-00000f10: 6572 223e 0a20 2020 203c 656d 3ef0 9f9a  er">.    <em>...
-00000f20: 8020 4869 6768 6c79 2073 6361 6c61 626c  . Highly scalabl
-00000f30: 652c 2070 6572 666f 726d 616e 742c 2065  e, performant, e
-00000f40: 6173 7920 746f 206c 6561 726e 2c20 6561  asy to learn, ea
-00000f50: 7379 2074 6f20 636f 6465 2061 6e64 2066  sy to code and f
-00000f60: 6f72 2065 7665 7279 2061 7070 6c69 6361  or every applica
-00000f70: 7469 6f6e 2e20 f09f 9a80 3c2f 656d 3e0a  tion. ....</em>.
-00000f80: 3c2f 703e 0a0a 3c70 2061 6c69 676e 3d22  </p>..<p align="
-00000f90: 6365 6e74 6572 223e 0a3c 6120 6872 6566  center">.<a href
-00000fa0: 3d22 6874 7470 733a 2f2f 6769 7468 7562  ="https://github
-00000fb0: 2e63 6f6d 2f64 796d 6d6f 6e64 2f65 736d  .com/dymmond/esm
-00000fc0: 6572 616c 642f 776f 726b 666c 6f77 732f  erald/workflows/
-00000fd0: 5465 7374 2532 3053 7569 7465 2f62 6164  Test%20Suite/bad
-00000fe0: 6765 2e73 7667 3f65 7665 6e74 3d70 7573  ge.svg?event=pus
-00000ff0: 6826 6272 616e 6368 3d6d 6169 6e22 2074  h&branch=main" t
-00001000: 6172 6765 743d 225f 626c 616e 6b22 3e0a  arget="_blank">.
-00001010: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-00001020: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00001030: 2f64 796d 6d6f 6e64 2f65 736d 6572 616c  /dymmond/esmeral
-00001040: 642f 776f 726b 666c 6f77 732f 5465 7374  d/workflows/Test
-00001050: 2532 3053 7569 7465 2f62 6164 6765 2e73  %20Suite/badge.s
-00001060: 7667 3f65 7665 6e74 3d70 7573 6826 6272  vg?event=push&br
-00001070: 616e 6368 3d6d 6169 6e22 2061 6c74 3d22  anch=main" alt="
-00001080: 5465 7374 2053 7569 7465 223e 0a3c 2f61  Test Suite">.</a
-00001090: 3e0a 0a3c 6120 6872 6566 3d22 6874 7470  >..<a href="http
-000010a0: 733a 2f2f 7079 7069 2e6f 7267 2f70 726f  s://pypi.org/pro
-000010b0: 6a65 6374 2f65 736d 6572 616c 6422 2074  ject/esmerald" t
-000010c0: 6172 6765 743d 225f 626c 616e 6b22 3e0a  arget="_blank">.
-000010d0: 2020 2020 3c69 6d67 2073 7263 3d22 6874      <img src="ht
-000010e0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
-000010f0: 732e 696f 2f70 7970 692f 762f 6573 6d65  s.io/pypi/v/esme
-00001100: 7261 6c64 3f63 6f6c 6f72 3d25 3233 3334  rald?color=%2334
-00001110: 4430 3538 266c 6162 656c 3d70 7970 6925  D058&label=pypi%
-00001120: 3230 7061 636b 6167 6522 2061 6c74 3d22  20package" alt="
-00001130: 5061 636b 6167 6520 7665 7273 696f 6e22  Package version"
-00001140: 3e0a 3c2f 613e 0a0a 3c61 2068 7265 663d  >.</a>..<a href=
-00001150: 2268 7474 7073 3a2f 2f70 7970 692e 6f72  "https://pypi.or
-00001160: 672f 7072 6f6a 6563 742f 6573 6d65 7261  g/project/esmera
-00001170: 6c64 2220 7461 7267 6574 3d22 5f62 6c61  ld" target="_bla
-00001180: 6e6b 223e 0a20 2020 203c 696d 6720 7372  nk">.    <img sr
-00001190: 633d 2268 7474 7073 3a2f 2f69 6d67 2e73  c="https://img.s
-000011a0: 6869 656c 6473 2e69 6f2f 7079 7069 2f70  hields.io/pypi/p
-000011b0: 7976 6572 7369 6f6e 732f 6573 6d65 7261  yversions/esmera
-000011c0: 6c64 2e73 7667 3f63 6f6c 6f72 3d25 3233  ld.svg?color=%23
-000011d0: 3334 4430 3538 2220 616c 743d 2253 7570  34D058" alt="Sup
-000011e0: 706f 7274 6564 2050 7974 686f 6e20 7665  ported Python ve
-000011f0: 7273 696f 6e73 223e 0a3c 2f61 3e0a 3c2f  rsions">.</a>.</
-00001200: 703e 0a0a 2d2d 2d0a 0a2a 2a44 6f63 756d  p>..---..**Docum
-00001210: 656e 7461 7469 6f6e 2a2a 3a20 5b68 7474  entation**: [htt
-00001220: 7073 3a2f 2f65 736d 6572 616c 642e 6465  ps://esmerald.de
-00001230: 765d 2868 7474 7073 3a2f 2f77 7777 2e65  v](https://www.e
-00001240: 736d 6572 616c 642e 6465 7629 20f0 9f93  smerald.dev) ...
-00001250: 9a0a 0a2a 2a53 6f75 7263 6520 436f 6465  ...**Source Code
-00001260: 2a2a 3a20 5b68 7474 7073 3a2f 2f67 6974  **: [https://git
-00001270: 6875 622e 636f 6d2f 6479 6d6d 6f6e 642f  hub.com/dymmond/
-00001280: 6573 6d65 7261 6c64 5d28 6874 7470 733a  esmerald](https:
-00001290: 2f2f 6769 7468 7562 2e63 6f6d 2f64 796d  //github.com/dym
-000012a0: 6d6f 6e64 2f65 736d 6572 616c 6429 0a0a  mond/esmerald)..
-000012b0: 2a2a 5468 6520 6f66 6669 6369 616c 2073  **The official s
-000012c0: 7570 706f 7274 6564 2076 6572 7369 6f6e  upported version
-000012d0: 2069 7320 616c 7761 7973 2074 6865 206c   is always the l
-000012e0: 6174 6573 7420 7265 6c65 6173 6564 2a2a  atest released**
-000012f0: 2e0a 0a2d 2d2d 0a0a 4573 6d65 7261 6c64  ...---..Esmerald
-00001300: 2069 7320 6120 6d6f 6465 726e 2c20 706f   is a modern, po
-00001310: 7765 7266 756c 2c20 666c 6578 6962 6c65  werful, flexible
-00001320: 2c20 6869 6768 2070 6572 666f 726d 616e  , high performan
-00001330: 742c 2077 6562 2066 7261 6d65 776f 726b  t, web framework
-00001340: 2064 6573 6967 6e65 6420 746f 2062 7569   designed to bui
-00001350: 6c64 206e 6f74 206f 6e6c 7920 4150 4973  ld not only APIs
-00001360: 0a62 7574 2061 6c73 6f20 6675 6c6c 2073  .but also full s
-00001370: 6361 6c61 626c 6520 6170 706c 6963 6174  calable applicat
-00001380: 696f 6e73 2066 726f 6d20 7468 6520 736d  ions from the sm
-00001390: 616c 6c65 7374 2074 6f20 656e 7465 7270  allest to enterp
-000013a0: 7269 7365 206c 6576 656c 2e0a 0a45 736d  rise level...Esm
-000013b0: 6572 616c 6420 6973 2064 6573 6967 6e65  erald is designe
-000013c0: 6420 746f 2062 7569 6c64 2077 6974 6820  d to build with 
-000013d0: 7079 7468 6f6e 2033 2e38 2b20 616e 6420  python 3.8+ and 
-000013e0: 6261 7365 6420 6f6e 2073 7461 6e64 6172  based on standar
-000013f0: 6420 7079 7468 6f6e 2074 7970 6520 6869  d python type hi
-00001400: 6e74 732e 2049 6e69 7469 616c 6c79 0a62  nts. Initially.b
-00001410: 7569 6c74 206f 6e20 7468 6520 746f 7020  uilt on the top 
-00001420: 6f66 205b 5374 6172 6c65 7474 655d 2868  of [Starlette](h
-00001430: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00001440: 6d2f 656e 636f 6465 2f73 7461 726c 6574  m/encode/starlet
-00001450: 7465 2920 616e 6420 6c61 7465 7220 6f6e  te) and later on
-00001460: 206d 6f76 6564 2074 6f20 5b4c 696c 7961   moved to [Lilya
-00001470: 5d28 6874 7470 733a 2f2f 6c69 6c79 612e  ](https://lilya.
-00001480: 6465 7629 2061 6e64 205b 5079 6461 6e74  dev) and [Pydant
-00001490: 6963 5d28 6874 7470 733a 2f2f 6769 7468  ic](https://gith
-000014a0: 7562 2e63 6f6d 2f73 616d 7565 6c63 6f6c  ub.com/samuelcol
-000014b0: 7669 6e2f 7079 6461 6e74 6963 292f 5b6d  vin/pydantic)/[m
-000014c0: 7367 7370 6563 5d28 6874 7470 733a 2f2f  sgspec](https://
-000014d0: 6a63 7269 7374 6861 7269 662e 636f 6d2f  jcristharif.com/
-000014e0: 6d73 6773 7065 632f 292e 0a0a 4368 6563  msgspec/)...Chec
-000014f0: 6b20 6f75 7420 7468 6520 5b45 736d 6572  k out the [Esmer
-00001500: 616c 6420 646f 6375 6d65 6e74 6174 696f  ald documentatio
-00001510: 6e20 f09f 939a 5d28 6874 7470 733a 2f2f  n ....](https://
-00001520: 6573 6d65 7261 6c64 2e64 6576 290a 0a2a  esmerald.dev)..*
-00001530: 2a54 6865 206f 6666 6963 6961 6c20 7375  *The official su
-00001540: 7070 6f72 7465 6420 7665 7273 696f 6e20  pported version 
-00001550: 6973 2061 6c77 6179 7320 7468 6520 6c61  is always the la
-00001560: 7465 7374 2072 656c 6561 7365 642a 2a2e  test released**.
-00001570: 0a0a 2323 204d 6f74 6976 6174 696f 6e0a  ..## Motivation.
-00001580: 0a54 6865 7265 2061 7265 2067 7265 6174  .There are great
-00001590: 2066 7261 6d65 776f 726b 7320 6f75 7420   frameworks out 
-000015a0: 7468 6572 6520 6c69 6b65 2046 6173 7441  there like FastA
-000015b0: 5049 2c20 5374 6172 6c69 7465 2c20 466c  PI, Starlite, Fl
-000015c0: 616d 612c 2046 6c61 736b 2c20 446a 616e  ama, Flask, Djan
-000015d0: 676f 2e2e 2e20 416c 6c20 6f66 2074 6865  go... All of the
-000015e0: 6d20 736f 6c76 696e 6720 6d61 6a6f 7269  m solving majori
-000015f0: 7479 0a6f 6620 7468 6520 6375 7272 656e  ty.of the curren
-00001600: 7420 6461 792d 746f 2d64 6179 2070 726f  t day-to-day pro
-00001610: 626c 656d 7320 6f66 2039 3925 206f 6620  blems of 99% of 
-00001620: 7468 6520 6170 706c 6963 6174 696f 6e73  the applications
-00001630: 2062 7574 206c 6561 7669 6e67 2074 6865   but leaving the
-00001640: 2031 2520 7468 6174 2069 7320 7573 7561   1% that is usua
-00001650: 6c6c 7920 6172 6f75 6e64 2073 7472 7563  lly around struc
-00001660: 7475 7265 0a61 6e64 2064 6573 6967 6e2f  ture.and design/
-00001670: 6275 7369 6e65 7373 2077 6974 686f 7574  business without
-00001680: 2074 6f20 6d75 6368 2074 6f20 646f 2e0a   to much to do..
-00001690: 0a45 736d 6572 616c 6420 676f 7420 7468  .Esmerald got th
-000016a0: 6520 696e 7370 6972 6174 696f 6e20 6672  e inspiration fr
-000016b0: 6f6d 2074 686f 7365 2067 7265 6174 2066  om those great f
-000016c0: 7261 6d65 776f 726b 7320 6f75 7420 7468  rameworks out th
-000016d0: 6572 6520 616e 6420 7761 7320 6275 696c  ere and was buil
-000016e0: 7420 7769 7468 2061 6c6c 2074 6865 206b  t with all the k
-000016f0: 6e6f 776e 2061 6d61 7a69 6e67 0a66 6561  nown amazing.fea
-00001700: 7475 7265 7320 6275 7420 7769 7468 2062  tures but with b
-00001710: 7573 696e 6573 7320 696e 206d 696e 6420  usiness in mind 
-00001720: 6173 2077 656c 6c2e 2053 7461 726c 6974  as well. Starlit
-00001730: 652c 2066 6f72 2065 7861 6d70 6c65 2c20  e, for example, 
-00001740: 6761 7665 2074 6865 2069 6e73 7069 7261  gave the inspira
-00001750: 7469 6f6e 2066 6f72 2074 6865 2074 7261  tion for the tra
-00001760: 6e73 666f 726d 6572 7320 616e 6420 666f  nsformers and fo
-00001770: 7220 7468 6520 5369 676e 6174 7572 6520  r the Signature 
-00001780: 6d6f 6465 6c73 2c0a 736f 6d65 7468 696e  models,.somethin
-00001790: 6720 7665 7279 2075 7365 6675 6c20 7468  g very useful th
-000017a0: 6174 2068 656c 7065 6420 4573 6d65 7261  at helped Esmera
-000017b0: 6c64 2069 6e74 6567 6572 6174 696e 6720  ld integerating 
-000017c0: 7769 7468 2070 7964 616e 7469 632e 0a46  with pydantic..F
-000017d0: 6173 7441 5049 2067 6176 6520 7468 6520  astAPI gave the 
-000017e0: 696e 7370 6972 6174 696f 6e20 666f 7220  inspiration for 
-000017f0: 4150 4920 6465 7369 676e 696e 672c 2044  API designing, D
-00001800: 6a61 6e67 6f20 666f 7220 7468 6520 7065  jango for the pe
-00001810: 726d 6973 7369 6f6e 732c 2046 6c61 736b  rmissions, Flask
-00001820: 2066 6f72 2074 6865 2073 696d 706c 6963   for the simplic
-00001830: 6974 792c 204e 6573 744a 5320 666f 7220  ity, NestJS for 
-00001840: 7468 650a 636f 6e74 726f 6c6c 6572 7320  the.controllers 
-00001850: 616e 6420 7468 6520 6c69 7374 2067 6f65  and the list goe
-00001860: 7320 6f6e 2e0a 0a46 6f72 2061 206a 6f62  s on...For a job
-00001870: 2074 6f20 6265 2064 6f6e 6520 7072 6f70   to be done prop
-00001880: 6572 6c79 2c20 7573 7561 6c6c 7920 6974  erly, usually it
-00001890: 2069 7320 6e65 7665 7220 646f 6e65 2061   is never done a
-000018a0: 6c6f 6e65 2061 6e64 2074 6865 7265 2069  lone and there i
-000018b0: 7320 616c 7761 7973 2061 2064 7269 7665  s always a drive
-000018c0: 7220 616e 6420 696e 7370 6972 6174 696f  r and inspiratio
-000018d0: 6e20 746f 2069 742e 0a0a 2323 2052 6571  n to it...## Req
-000018e0: 7569 7265 6d65 6e74 730a 0a2a 2070 7974  uirements..* pyt
-000018f0: 686f 6e20 332e 382b 0a0a 4573 6d65 7261  hon 3.8+..Esmera
-00001900: 6c64 2077 6f75 6c64 6e27 7420 6265 2070  ld wouldn't be p
-00001910: 6f73 7369 626c 6520 7769 7468 6f75 7420  ossible without 
-00001920: 7477 6f20 636f 6c6f 7373 616c 733a 0a0a  two colossals:..
-00001930: 2a20 3c61 2068 7265 663d 2268 7474 7073  * <a href="https
-00001940: 3a2f 2f77 7777 2e6c 696c 7961 2e64 6576  ://www.lilya.dev
-00001950: 2f22 2063 6c61 7373 3d22 6578 7465 726e  /" class="extern
-00001960: 616c 2d6c 696e 6b22 2074 6172 6765 743d  al-link" target=
-00001970: 225f 626c 616e 6b22 3e53 7461 726c 6574  "_blank">Starlet
-00001980: 7465 3c2f 613e 0a2a 203c 6120 6872 6566  te</a>.* <a href
-00001990: 3d22 6874 7470 733a 2f2f 7079 6461 6e74  ="https://pydant
-000019a0: 6963 2d64 6f63 732e 6865 6c70 6d61 6e75  ic-docs.helpmanu
-000019b0: 616c 2e69 6f2f 2220 636c 6173 733d 2265  al.io/" class="e
-000019c0: 7874 6572 6e61 6c2d 6c69 6e6b 2220 7461  xternal-link" ta
-000019d0: 7267 6574 3d22 5f62 6c61 6e6b 223e 5079  rget="_blank">Py
-000019e0: 6461 6e74 6963 3c2f 613e 0a0a 2323 2049  dantic</a>..## I
-000019f0: 6e73 7461 6c6c 6174 696f 6e0a 0a60 6060  nstallation..```
-00001a00: 7368 656c 6c0a 2420 7069 7020 696e 7374  shell.$ pip inst
-00001a10: 616c 6c20 6573 6d65 7261 6c64 0a60 6060  all esmerald.```
-00001a20: 0a0a 416e 2041 5347 4920 7365 7276 6572  ..An ASGI server
-00001a30: 2069 7320 616c 736f 206e 6565 6465 6420   is also needed 
-00001a40: 746f 2072 756e 2069 6e20 7072 6f64 7563  to run in produc
-00001a50: 7469 6f6e 2c20 7765 2072 6563 6f6d 6d65  tion, we recomme
-00001a60: 6e64 205b 5576 6963 6f72 6e5d 2868 7474  nd [Uvicorn](htt
-00001a70: 7073 3a2f 2f77 7777 2e75 7669 636f 726e  ps://www.uvicorn
-00001a80: 2e6f 7267 2920 6275 7420 6974 2069 7320  .org) but it is 
-00001a90: 656e 7469 7265 6c79 0a75 7020 746f 2079  entirely.up to y
-00001aa0: 6f75 2e0a 0a60 6060 7368 656c 6c0a 2420  ou...```shell.$ 
-00001ab0: 7069 7020 696e 7374 616c 6c20 7576 6963  pip install uvic
-00001ac0: 6f72 6e0a 0a60 6060 0a0a 4966 2079 6f75  orn..```..If you
-00001ad0: 2077 616e 7420 696e 7374 616c 6c20 6573   want install es
-00001ae0: 6d65 7261 6c64 2077 6974 6820 7370 6563  merald with spec
-00001af0: 6966 6963 733a 0a0a 2a2a 5375 7070 6f72  ifics:..**Suppor
-00001b00: 7420 666f 7220 7465 6d70 6c61 7465 2073  t for template s
-00001b10: 7973 7465 6d20 7375 6368 2061 7320 6a69  ystem such as ji
-00001b20: 6e6a 6132 2061 6e64 206d 616b 6f2a 2a3a  nja2 and mako**:
-00001b30: 0a0a 6060 6073 6865 6c6c 0a24 2070 6970  ..```shell.$ pip
-00001b40: 2069 6e73 7461 6c6c 2065 736d 6572 616c   install esmeral
-00001b50: 645b 7465 6d70 6c61 7465 735d 0a60 6060  d[templates].```
-00001b60: 0a0a 2a2a 5375 7070 6f72 7420 666f 7220  ..**Support for 
-00001b70: 7468 6520 696e 7465 726e 616c 2073 6368  the internal sch
-00001b80: 6564 756c 6572 2a2a 3a0a 0a60 6060 7368  eduler**:..```sh
-00001b90: 656c 6c0a 2420 7069 7020 696e 7374 616c  ell.$ pip instal
-00001ba0: 6c20 6573 6d65 7261 6c64 5b73 6368 6564  l esmerald[sched
-00001bb0: 756c 6572 735d 0a60 6060 0a0a 2a2a 5375  ulers].```..**Su
-00001bc0: 7070 6f72 7420 666f 7220 7468 6520 6a77  pport for the jw
-00001bd0: 7420 7573 6564 2069 6e74 6572 6e61 6c6c  t used internall
-00001be0: 7920 6279 2045 736d 6572 616c 642a 2a3a  y by Esmerald**:
-00001bf0: 0a0a 6060 6073 6865 6c6c 0a24 2070 6970  ..```shell.$ pip
-00001c00: 2069 6e73 7461 6c6c 2065 736d 6572 616c   install esmeral
-00001c10: 645b 6a77 745d 0a60 6060 0a0a 2a2a 5375  d[jwt].```..**Su
-00001c20: 7070 6f72 7420 666f 7220 4f52 4a53 4f4e  pport for ORJSON
-00001c30: 2061 6e64 2055 4a53 4f4e 2a2a 3a0a 0a60   and UJSON**:..`
-00001c40: 6060 7368 656c 6c0a 2420 7069 7020 696e  ``shell.$ pip in
-00001c50: 7374 616c 6c20 6573 6d65 7261 6c64 5b65  stall esmerald[e
-00001c60: 6e63 6f64 6572 735d 0a60 6060 0a0a 2a2a  ncoders].```..**
-00001c70: 4966 2079 6f75 2077 616e 7420 746f 2075  If you want to u
-00001c80: 7365 2074 6865 2065 736d 6572 616c 6420  se the esmerald 
-00001c90: 7465 7374 696e 6720 636c 6965 6e74 2a2a  testing client**
-00001ca0: 3a0a 0a60 6060 7368 656c 6c0a 2420 7069  :..```shell.$ pi
-00001cb0: 7020 696e 7374 616c 6c20 6573 6d65 7261  p install esmera
-00001cc0: 6c64 5b74 6573 745d 0a60 6060 0a0a 2a2a  ld[test].```..**
-00001cd0: 4966 2079 6f75 2077 616e 7420 746f 2075  If you want to u
-00001ce0: 7365 2074 6865 2065 736d 6572 616c 6420  se the esmerald 
-00001cf0: 7368 656c 6c2a 2a3a 0a0a 4d6f 7265 205b  shell**:..More [
-00001d00: 6465 7461 696c 735d 2868 7474 7073 3a2f  details](https:/
-00001d10: 2f65 736d 6572 616c 642e 6465 762f 6469  /esmerald.dev/di
-00001d20: 7265 6374 6976 6573 2f73 6865 6c6c 2920  rectives/shell) 
-00001d30: 6162 6f75 7420 7468 6973 2074 6f70 6963  about this topic
-00001d40: 205b 696e 2074 6865 2064 6f63 735d 2868   [in the docs](h
-00001d50: 7474 7073 3a2f 2f65 736d 6572 616c 642e  ttps://esmerald.
-00001d60: 6465 762f 6469 7265 6374 6976 6573 2f73  dev/directives/s
-00001d70: 6865 6c6c 290a 0a60 6060 7368 656c 6c0a  hell)..```shell.
-00001d80: 2420 7069 7020 696e 7374 616c 6c20 6573  $ pip install es
-00001d90: 6d65 7261 6c64 5b69 7079 7468 6f6e 5d20  merald[ipython] 
-00001da0: 2320 6465 6661 756c 7420 7368 656c 6c0a  # default shell.
-00001db0: 2420 7069 7020 696e 7374 616c 6c20 6573  $ pip install es
-00001dc0: 6d65 7261 6c64 5b70 7470 7974 686f 6e5d  merald[ptpython]
-00001dd0: 2023 2070 7470 7974 686f 6e20 7368 656c   # ptpython shel
-00001de0: 6c0a 6060 600a 0a23 2323 2053 7461 7274  l.```..### Start
-00001df0: 2061 2070 726f 6a65 6374 2075 7369 6e67   a project using
-00001e00: 2064 6972 6563 7469 7665 730a 0a21 2121   directives..!!!
-00001e10: 2057 6172 6e69 6e67 0a20 2020 2054 6869   Warning.    Thi
-00001e20: 7320 6973 2066 6f72 206d 6f72 6520 6164  s is for more ad
-00001e30: 7661 6e63 6564 2075 7365 7273 2074 6861  vanced users tha
-00001e40: 7420 6172 6520 616c 7265 6164 7920 636f  t are already co
-00001e50: 6d66 6f72 7461 626c 6520 7769 7468 2045  mfortable with E
-00001e60: 736d 6572 616c 6420 286f 7220 5079 7468  smerald (or Pyth
-00001e70: 6f6e 2069 6e20 6765 6e65 7261 6c29 0a20  on in general). 
-00001e80: 2020 206f 7220 6665 656c 206c 696b 6520     or feel like 
-00001e90: 6974 2069 7320 6e6f 7420 6120 7072 6f62  it is not a prob
-00001ea0: 6c65 6d20 7573 696e 6720 7468 6573 6520  lem using these 
-00001eb0: 6469 7265 6374 6976 6573 2e20 4966 2079  directives. If y
-00001ec0: 6f75 2064 6f20 6e6f 7420 6665 656c 2063  ou do not feel c
-00001ed0: 6f6d 666f 7274 6162 6c65 2079 6574 2074  omfortable yet t
-00001ee0: 6f20 7573 6520 7468 6973 2c0a 2020 2020  o use this,.    
-00001ef0: 706c 6561 7365 2063 6f6e 7469 6e75 6520  please continue 
-00001f00: 7265 6164 696e 6720 7468 6520 646f 6375  reading the docu
-00001f10: 6d65 6e74 6174 696f 6e20 616e 6420 6c65  mentation and le
-00001f20: 6172 6e69 6e67 206d 6f72 6520 6162 6f75  arning more abou
-00001f30: 7420 4573 6d65 7261 6c64 2e0a 0a49 6620  t Esmerald...If 
-00001f40: 796f 7520 7769 7368 2074 6f20 7374 6172  you wish to star
-00001f50: 7420 616e 2045 736d 6572 616c 6420 7072  t an Esmerald pr
-00001f60: 6f6a 6563 7420 7769 7468 2061 2064 6566  oject with a def
-00001f70: 6175 6c74 2073 7567 6765 7374 6564 2073  ault suggested s
-00001f80: 7472 7563 7475 7265 2e0a 0a60 6060 7368  tructure...```sh
-00001f90: 656c 6c0a 6573 6d65 7261 6c64 2063 7265  ell.esmerald cre
-00001fa0: 6174 6570 726f 6a65 6374 203c 594f 5552  ateproject <YOUR
-00001fb0: 2d50 524f 4a45 4354 2d4e 414d 453e 0a60  -PROJECT-NAME>.`
-00001fc0: 6060 0a0a 5468 6973 2077 696c 6c20 6765  ``..This will ge
-00001fd0: 6e65 7261 7465 2061 2073 6361 6666 6f6c  nerate a scaffol
-00001fe0: 6420 666f 7220 796f 7572 2070 726f 6a65  d for your proje
-00001ff0: 6374 2077 6974 6820 736f 6d65 2070 7265  ct with some pre
-00002000: 2d64 6566 696e 6564 2066 696c 6573 2069  -defined files i
-00002010: 6e20 6120 7369 6d70 6c65 2066 6173 6869  n a simple fashi
-00002020: 6f6e 2e0a 5468 6973 2077 696c 6c20 616c  on..This will al
-00002030: 736f 2067 656e 6572 6174 6520 6120 6669  so generate a fi
-00002040: 6c65 2066 6f72 2074 6865 2074 6573 7473  le for the tests
-00002050: 2075 7369 6e67 2074 6865 2045 736d 6572   using the Esmer
-00002060: 616c 6454 6573 7443 6c69 656e 742c 2073  aldTestClient, s
-00002070: 6f20 6d61 6b65 2073 7572 6520 796f 7520  o make sure you 
-00002080: 7275 6e3a 0a0a 6060 6073 6865 6c6c 0a24  run:..```shell.$
-00002090: 2070 6970 2069 6e73 7461 6c6c 2065 736d   pip install esm
-000020a0: 6572 616c 645b 7465 7374 5d0a 6060 600a  erald[test].```.
-000020b0: 0a4f 7220 796f 7520 6361 6e20 736b 6970  .Or you can skip
-000020c0: 2074 6869 7320 7374 6570 2069 6620 796f   this step if yo
-000020d0: 7520 646f 6e27 7420 7761 6e74 2074 6f20  u don't want to 
-000020e0: 7573 6520 7468 6520 4573 6d65 7261 6c64  use the Esmerald
-000020f0: 5465 7374 436c 6965 6e74 2e0a 0a59 6f75  TestClient...You
-00002100: 2063 616e 2066 696e 6420 5b6d 6f72 6520   can find [more 
-00002110: 696e 666f 726d 6174 696f 6e5d 2868 7474  information](htt
-00002120: 7073 3a2f 2f65 736d 6572 616c 642e 6465  ps://esmerald.de
-00002130: 762f 6d61 6e61 6765 6d65 6e74 2f64 6972  v/management/dir
-00002140: 6563 7469 7665 7329 2061 626f 7574 2074  ectives) about t
-00002150: 6869 7320 6469 7265 6374 6976 6520 616e  his directive an
-00002160: 6420 686f 7720 746f 0a75 7365 2069 742e  d how to.use it.
-00002170: 0a0a 2323 204b 6579 2046 6561 7475 7265  ..## Key Feature
-00002180: 730a 0a2a 202a 2a46 6c75 6964 2061 6e64  s..* **Fluid and
-00002190: 2046 6173 742a 2a3a 2054 6861 6e6b 7320   Fast**: Thanks 
-000021a0: 746f 2053 7461 726c 6574 7465 2061 6e64  to Starlette and
-000021b0: 2050 7964 616e 7469 632f 6d73 6773 7065   Pydantic/msgspe
-000021c0: 632e 0a2a 202a 2a46 6173 7420 746f 2064  c..* **Fast to d
-000021d0: 6576 656c 6f70 2a2a 3a20 5468 616e 6b73  evelop**: Thanks
-000021e0: 2074 6f20 7468 6520 7369 6d70 6c69 6369   to the simplici
-000021f0: 7479 206f 6620 6465 7369 676e 2c20 7468  ty of design, th
-00002200: 6520 6465 7665 6c6f 706d 656e 7420 7469  e development ti
-00002210: 6d65 7320 6361 6e20 6265 2072 6564 7563  mes can be reduc
-00002220: 6564 2065 7870 6f6e 656e 7469 616c 6c79  ed exponentially
-00002230: 2e0a 2a20 2a2a 496e 7475 6974 6976 652a  ..* **Intuitive*
-00002240: 2a3a 2049 6620 796f 7520 6172 6520 7573  *: If you are us
-00002250: 6564 2074 6f20 7468 6520 6f74 6865 7220  ed to the other 
-00002260: 6672 616d 6577 6f72 6b73 2c20 4573 6d65  frameworks, Esme
-00002270: 7261 6c64 2069 7320 6120 6e6f 2062 7261  rald is a no bra
-00002280: 696e 6572 2074 6f20 6465 7665 6c6f 702e  iner to develop.
-00002290: 0a2a 202a 2a45 6173 792a 2a3a 2044 6576  .* **Easy**: Dev
-000022a0: 656c 6f70 6564 2077 6974 6820 6465 7369  eloped with desi
-000022b0: 676e 2069 6e20 6d69 6e64 2061 6e64 2065  gn in mind and e
-000022c0: 6173 7920 6c65 6172 6e69 6e67 2e0a 2a20  asy learning..* 
-000022d0: 2a2a 5368 6f72 742a 2a3a 2057 6974 6820  **Short**: With 
-000022e0: 7468 6520 4f4f 5020 6176 6169 6c61 626c  the OOP availabl
-000022f0: 6520 6e61 7469 7665 6c79 2074 6865 7265  e natively there
-00002300: 2069 7320 6e6f 206e 6565 6420 666f 7220   is no need for 
-00002310: 636f 6465 2064 7570 6c69 6361 7469 6f6e  code duplication
-00002320: 2e20 534f 4c49 442e 0a2a 202a 2a52 6561  . SOLID..* **Rea
-00002330: 6479 2a2a 3a20 4765 7420 796f 7572 2061  dy**: Get your a
-00002340: 7070 6c69 6361 7469 6f6e 2075 7020 616e  pplication up an
-00002350: 6420 7275 6e6e 696e 6720 7769 7468 2070  d running with p
-00002360: 726f 6475 6374 696f 6e2d 7265 6164 7920  roduction-ready 
-00002370: 636f 6465 2e0a 2a20 2a2a 4f4f 5020 616e  code..* **OOP an
-00002380: 6420 4675 6e63 7469 6f6e 616c 2a2a 3a20  d Functional**: 
-00002390: 4465 7369 676e 2041 5049 7320 696e 2061  Design APIs in a
-000023a0: 6e79 2064 6573 6972 6564 2077 6179 2e20  ny desired way. 
-000023b0: 4f4f 5020 6f72 2046 756e 6374 696f 6e61  OOP or Functiona
-000023c0: 6c20 6973 2061 7661 696c 6162 6c65 2e0a  l is available..
-000023d0: 2a20 2a2a 4173 796e 6320 616e 6420 5379  * **Async and Sy
-000023e0: 6e63 2a2a 3a20 446f 2079 6f75 2070 7265  nc**: Do you pre
-000023f0: 6665 7220 7379 6e63 206f 7220 6173 796e  fer sync or asyn
-00002400: 633f 2059 6f75 2063 616e 2068 6176 6520  c? You can have 
-00002410: 626f 7468 2e0a 2a20 2a2a 4d69 6464 6c65  both..* **Middle
-00002420: 7761 7265 2a2a 3a20 4170 706c 7920 6d69  ware**: Apply mi
-00002430: 6464 6c65 7761 7265 7320 6f6e 2074 6865  ddlewares on the
-00002440: 2061 7070 6c69 6361 7469 6f6e 206c 6576   application lev
-00002450: 656c 206f 7220 4150 4920 6c65 7665 6c2e  el or API level.
-00002460: 0a2a 202a 2a45 7863 6570 7469 6f6e 2048  .* **Exception H
-00002470: 616e 646c 6572 732a 2a3a 2041 7070 6c79  andlers**: Apply
-00002480: 2065 7863 6570 7469 6f6e 2068 616e 646c   exception handl
-00002490: 6572 7320 6f6e 2061 6e79 2064 6573 6972  ers on any desir
-000024a0: 6564 206c 6576 656c 2e0a 2a20 2a2a 5065  ed level..* **Pe
-000024b0: 726d 6973 7369 6f6e 732a 2a3a 2041 7070  rmissions**: App
-000024c0: 6c79 2073 7065 6369 6669 6320 7275 6c65  ly specific rule
-000024d0: 7320 616e 6420 7065 726d 6973 7369 6f6e  s and permission
-000024e0: 7320 6f6e 2065 6163 6820 4150 492e 0a2a  s on each API..*
-000024f0: 202a 2a49 6e74 6572 6365 7074 6f72 732a   **Interceptors*
-00002500: 2a3a 2049 6e74 6572 6365 7074 2072 6571  *: Intercept req
-00002510: 7565 7374 7320 616e 6420 6164 6420 6c6f  uests and add lo
-00002520: 6769 6320 6265 666f 7265 2072 6561 6368  gic before reach
-00002530: 696e 6720 7468 6520 656e 6470 6f69 6e74  ing the endpoint
-00002540: 2e0a 2a20 2a2a 506c 7567 6761 626c 6573  ..* **Pluggables
-00002550: 2a2a 3a20 4372 6561 7465 2070 6c75 6769  **: Create plugi
-00002560: 6e73 2066 6f72 2045 736d 6572 616c 6420  ns for Esmerald 
-00002570: 616e 6420 686f 6f6b 2074 6865 6d20 696e  and hook them in
-00002580: 746f 2061 6e79 2061 7070 6c69 6361 7469  to any applicati
-00002590: 6f6e 2061 6e64 2f6f 720a 6469 7374 7269  on and/or.distri
-000025a0: 6275 7465 2074 6865 6d2e 0a2a 202a 2a44  bute them..* **D
-000025b0: 414f 2061 6e64 2041 7379 6e63 4441 4f2a  AO and AsyncDAO*
-000025c0: 2a3a 2041 766f 6964 2064 6174 6162 6173  *: Avoid databas
-000025d0: 6520 6361 6c6c 7320 6469 7265 6374 6c79  e calls directly
-000025e0: 2066 726f 6d20 7468 6520 4150 4973 2e20   from the APIs. 
-000025f0: 5573 6520 6275 7369 6e65 7373 206f 626a  Use business obj
-00002600: 6563 7473 2069 6e73 7465 6164 2e0a 2a20  ects instead..* 
-00002610: 2a2a 4f52 4d20 5375 7070 6f72 742a 2a3a  **ORM Support**:
-00002620: 204e 6174 6976 6520 7375 7070 6f72 7420   Native support 
-00002630: 666f 7220 5b53 6166 6669 6572 5d5b 7361  for [Saffier][sa
-00002640: 6666 6965 725f 6f72 6d5d 2061 6e64 205b  ffier_orm] and [
-00002650: 4564 6779 5d5b 6564 6779 5f6f 726d 5d2e  Edgy][edgy_orm].
-00002660: 0a2a 202a 2a4f 444d 2053 7570 706f 7274  .* **ODM Support
-00002670: 2a2a 3a20 4e61 7469 7665 2073 7570 706f  **: Native suppo
-00002680: 7274 2066 6f72 205b 4d6f 6e67 6f7a 5d5b  rt for [Mongoz][
-00002690: 6d6f 6e67 6f7a 5f6f 646d 5d2e 0a2a 202a  mongoz_odm]..* *
-000026a0: 2a41 5049 5669 6577 2a2a 3a20 436c 6173  *APIView**: Clas
-000026b0: 7320 4261 7365 6420 656e 6470 6f69 6e74  s Based endpoint
-000026c0: 7320 666f 7220 796f 7572 2062 656c 6f76  s for your belov
-000026d0: 6564 204f 4f50 2064 6573 6967 6e2e 0a2a  ed OOP design..*
-000026e0: 202a 2a4a 534f 4e20 7365 7269 616c 697a   **JSON serializ
-000026f0: 6174 696f 6e2f 6465 7365 7269 616c 697a  ation/deserializ
-00002700: 6174 696f 6e2a 2a3a 2042 6f74 6820 554a  ation**: Both UJ
-00002710: 534f 4e20 616e 6420 4f52 4a4f 4e20 7375  SON and ORJON su
-00002720: 7070 6f72 742e 0a2a 202a 2a4c 6966 6573  pport..* **Lifes
-00002730: 7061 6e2a 2a3a 2053 7570 706f 7274 2066  pan**: Support f
-00002740: 6f72 2074 6865 206e 6577 6c79 206c 6966  or the newly lif
-00002750: 6573 7061 6e20 616e 6420 6f6e 5f73 7461  espan and on_sta
-00002760: 7274 2f6f 6e5f 7368 7574 646f 776e 2065  rt/on_shutdown e
-00002770: 7665 6e74 732e 0a2a 202a 2a53 6368 6564  vents..* **Sched
-00002780: 756c 6572 2a2a 3a20 5965 732c 2074 6861  uler**: Yes, tha
-00002790: 7427 7320 7269 6768 742c 2069 7420 636f  t's right, it co
-000027a0: 6d65 7320 7769 7468 2061 2073 6368 6564  mes with a sched
-000027b0: 756c 6572 2066 6f72 2074 686f 7365 2061  uler for those a
-000027c0: 7574 6f6d 6174 6564 2074 6173 6b73 2e0a  utomated tasks..
-000027d0: 2a20 2a2a 4465 7065 6e64 656e 6379 2049  * **Dependency I
-000027e0: 6e6a 6563 7469 6f6e 2a2a 3a20 4c69 6b65  njection**: Like
-000027f0: 2061 6e79 206f 7468 6572 2067 7265 6174   any other great
-00002800: 2066 7261 6d65 776f 726b 206f 7574 2074   framework out t
-00002810: 6865 7265 2e0a 2a20 2a2a 5369 6d70 6c69  here..* **Simpli
-00002820: 6369 7479 2066 726f 6d20 7365 7474 696e  city from settin
-00002830: 6773 2a2a 3a20 5965 732c 2077 6520 6861  gs**: Yes, we ha
-00002840: 7665 2061 2077 6179 2074 6f20 6d61 6b65  ve a way to make
-00002850: 2074 6865 2063 6f64 6520 6576 656e 2063   the code even c
-00002860: 6c65 616e 6572 2062 7920 696e 7472 6f64  leaner by introd
-00002870: 7563 696e 6720 7365 7474 696e 6773 0a62  ucing settings.b
-00002880: 6173 6564 2073 7973 7465 6d73 2e0a 2a20  ased systems..* 
-00002890: 2a2a 6d73 6773 7065 632a 2a20 2d20 5375  **msgspec** - Su
-000028a0: 7070 6f72 7420 666f 7220 606d 7367 7370  pport for `msgsp
-000028b0: 6563 602e 0a0a 2323 2052 656c 6174 696f  ec`...## Relatio
-000028c0: 6e20 746f 2053 7461 726c 6574 7465 2061  n to Starlette a
-000028d0: 6e64 206f 7468 6572 2066 7261 6d65 776f  nd other framewo
-000028e0: 726b 730a 0a45 736d 6572 616c 6420 7573  rks..Esmerald us
-000028f0: 6573 2053 7461 726c 6574 7465 2075 6e64  es Starlette und
-00002900: 6572 2074 6865 2068 6f6f 642e 2054 6865  er the hood. The
-00002910: 2072 6561 736f 6e20 6265 6869 6e64 2074   reason behind t
-00002920: 6869 7320 6465 6369 736f 6e20 636f 6d65  his decison come
-00002930: 7320 7769 7468 2074 6865 2066 6163 7420  s with the fact 
-00002940: 7468 6174 2070 6572 666f 726d 616e 6365  that performance
-00002950: 2069 7320 7468 6572 650a 616e 6420 6e6f   is there.and no
-00002960: 2069 7373 7565 7320 7769 7468 2072 6f75   issues with rou
-00002970: 7469 6e67 2e0a 0a4f 6e63 6520 7468 6520  ting...Once the 
-00002980: 6170 706c 6963 6174 696f 6e20 6973 2075  application is u
-00002990: 702c 2061 6c6c 2074 6865 2072 6f75 7465  p, all the route
-000029a0: 7320 6172 6520 6d6f 756e 7465 6420 616e  s are mounted an
-000029b0: 6420 7468 6572 6566 6f72 6520 7468 6520  d therefore the 
-000029c0: 7572 6c20 7061 7468 7320 6172 6520 6465  url paths are de
-000029d0: 6669 6e65 642e 0a45 736d 6572 616c 6420  fined..Esmerald 
-000029e0: 656e 636f 7572 6167 6573 2073 7461 6e64  encourages stand
-000029f0: 6172 6420 7072 6163 7469 6365 7320 616e  ard practices an
-00002a00: 6420 6465 7369 676e 2069 6e20 6d69 6e64  d design in mind
-00002a10: 2077 6869 6368 206d 6561 6e73 2074 6861   which means tha
-00002a20: 7420 616e 7920 6170 706c 6963 6174 696f  t any applicatio
-00002a30: 6e2c 2062 6967 206f 7220 736d 616c 6c2c  n, big or small,
-00002a40: 0a63 7573 746f 6d20 6f72 2065 6e74 6572  .custom or enter
-00002a50: 7072 6973 652c 2066 6974 7320 7769 7468  prise, fits with
-00002a60: 696e 2045 736d 6572 616c 6420 6563 6f73  in Esmerald ecos
-00002a70: 7973 7465 6d20 7769 7468 6f75 7420 7363  ystem without sc
-00002a80: 616c 6162 696c 6974 7920 6973 7375 6573  alability issues
-00002a90: 2e0a 0a23 2320 5365 7474 696e 6773 0a0a  ...## Settings..
-00002aa0: 4c69 6b65 2065 7665 7279 206f 7468 6572  Like every other
-00002ab0: 2066 7261 6d65 776f 726b 2c20 7768 656e   framework, when
-00002ac0: 2073 7461 7274 696e 6720 616e 2061 7070   starting an app
-00002ad0: 6c69 6361 7469 6f6e 2c20 6120 6c6f 7420  lication, a lot 
-00002ae0: 6f66 205b 7365 7474 696e 6773 5d28 2e2f  of [settings](./
-00002af0: 6170 706c 6963 6174 696f 6e2f 7365 7474  application/sett
-00002b00: 696e 6773 2e6d 6429 2063 616e 2f6e 6565  ings.md) can/nee
-00002b10: 6420 746f 2062 650a 7061 7373 6564 2074  d to be.passed t
-00002b20: 6f20 7468 6520 6d61 696e 206f 626a 6563  o the main objec
-00002b30: 7420 616e 6420 7468 6973 2063 616e 2062  t and this can b
-00002b40: 6520 7665 7279 2064 6175 7469 6e67 2061  e very dauting a
-00002b50: 6e64 2075 676c 7920 746f 206d 6169 6e74  nd ugly to maint
-00002b60: 6169 6e20 616e 6420 7365 652e 0a0a 4573  ain and see...Es
-00002b70: 6d65 7261 6c64 2063 6f6d 6573 2077 6974  merald comes wit
-00002b80: 6820 7468 650a 5b73 6574 7469 6e67 735d  h the.[settings]
-00002b90: 282e 2f61 7070 6c69 6361 7469 6f6e 2f73  (./application/s
-00002ba0: 6574 7469 6e67 732e 6d64 2920 696e 206d  ettings.md) in m
-00002bb0: 696e 642e 2041 2073 6574 206f 6620 6465  ind. A set of de
-00002bc0: 6661 756c 7473 2074 6861 7420 6361 6e20  faults that can 
-00002bd0: 6265 206f 7665 7272 6964 6465 6e20 6279  be overridden by
-00002be0: 2079 6f75 7220 7665 7279 206f 776e 2073   your very own s
-00002bf0: 6574 7469 6e67 730a 6d6f 6475 6c65 2062  ettings.module b
-00002c00: 7574 206e 6f74 206c 696d 6974 6564 2074  ut not limited t
-00002c10: 6f20 6974 2c20 6173 2079 6f75 2063 616e  o it, as you can
-00002c20: 2073 7469 6c6c 2075 7365 2074 6865 2063   still use the c
-00002c30: 6c61 7373 6963 2061 7070 726f 6163 6820  lassic approach 
-00002c40: 6f66 2070 6173 7369 6e67 2065 7665 7279  of passing every
-00002c50: 7468 696e 6720 696e 746f 2061 0a45 736d  thing into a.Esm
-00002c60: 6572 616c 6420 696e 7374 616e 6365 2064  erald instance d
-00002c70: 6972 6563 746c 7920 7768 656e 2069 6e73  irectly when ins
-00002c80: 7461 6e74 6961 7469 6e67 2e0a 0a2a 2a45  tantiating...**E
-00002c90: 7861 6d70 6c65 206f 6620 636c 6173 7369  xample of classi
-00002ca0: 6320 6170 7072 6f61 6368 2a2a 3a0a 0a60  c approach**:..`
-00002cb0: 6060 7079 7468 6f6e 0a66 726f 6d20 6578  ``python.from ex
-00002cc0: 616d 706c 6520 696d 706f 7274 2045 7861  ample import Exa
-00002cd0: 6d70 6c65 4f62 6a65 6374 0a0a 2320 4578  mpleObject..# Ex
-00002ce0: 616d 706c 654f 626a 6563 7420 6973 2061  ampleObject is a
-00002cf0: 6e20 696e 7374 616e 6365 206f 6620 616e  n instance of an
-00002d00: 6f74 6865 7220 6170 706c 6963 6174 696f  other applicatio
-00002d10: 6e0a 2320 616e 6420 6974 2073 6572 7665  n.# and it serve
-00002d20: 7320 6f6e 6c79 2066 6f72 2065 7861 6d70  s only for examp
-00002d30: 6c65 0a0a 6170 7020 3d20 4578 616d 706c  le..app = Exampl
-00002d40: 654f 626a 6563 7428 7365 7474 696e 675f  eObject(setting_
-00002d50: 6f6e 653d 2e2e 2e2c 2073 6574 7469 6e67  one=..., setting
-00002d60: 5f74 776f 3d2e 2e2e 2c20 7365 7474 696e  _two=..., settin
-00002d70: 675f 7468 7265 653d 2e2e 2e29 0a0a 6060  g_three=...)..``
-00002d80: 600a 0a49 6e73 7069 7265 6420 6279 2074  `..Inspired by t
-00002d90: 6865 2067 7265 6174 205b 446a 616e 676f  he great [Django
-00002da0: 5d28 6874 7470 733a 2f2f 7777 772e 646a  ](https://www.dj
-00002db0: 616e 676f 7072 6f6a 6563 742e 636f 6d2f  angoproject.com/
-00002dc0: 2920 616e 6420 7573 696e 6720 7079 6461  ) and using pyda
-00002dd0: 6e74 6963 2c20 4573 6d65 7261 6c64 2068  ntic, Esmerald h
-00002de0: 6173 2061 2064 6566 6175 6c74 206f 626a  as a default obj
-00002df0: 6563 740a 7265 6164 7920 746f 2062 6520  ect.ready to be 
-00002e00: 7573 6564 206f 7574 2d6f 662d 7468 652d  used out-of-the-
-00002e10: 626f 782e 0a0a 2a2a 4573 6d65 7261 6c64  box...**Esmerald
-00002e20: 2a2a 3a0a 0a60 6060 7079 7468 6f6e 0a66  **:..```python.f
-00002e30: 726f 6d20 6573 6d65 7261 6c64 2069 6d70  rom esmerald imp
-00002e40: 6f72 7420 4573 6d65 7261 6c64 0a0a 6170  ort Esmerald..ap
-00002e50: 7020 3d20 4573 6d65 7261 6c64 2829 0a0a  p = Esmerald()..
-00002e60: 6060 600a 0a41 6e64 2074 6861 7427 7320  ```..And that's 
-00002e70: 6974 2120 416c 6c20 7468 6520 6465 6661  it! All the defa
-00002e80: 756c 7420 7365 7474 696e 6773 2061 7265  ult settings are
-00002e90: 206c 6f61 6465 6421 2054 6869 7320 6973   loaded! This is
-00002ea0: 2073 696d 706c 6520 6f66 2063 6f75 7273   simple of cours
-00002eb0: 6520 6275 7420 6361 6e20 796f 7520 6f76  e but can you ov
-00002ec0: 6572 7269 6465 0a69 6e73 6964 6520 7468  erride.inside th
-00002ed0: 6520 6f62 6a65 6374 2061 7320 7765 6c6c  e object as well
-00002ee0: 3f20 5965 7321 0a0a 6060 6070 7974 686f  ? Yes!..```pytho
-00002ef0: 6e0a 6672 6f6d 2065 736d 6572 616c 6420  n.from esmerald 
-00002f00: 696d 706f 7274 2045 736d 6572 616c 640a  import Esmerald.
-00002f10: 0a61 7070 203d 2045 736d 6572 616c 6428  .app = Esmerald(
-00002f20: 6170 705f 6e61 6d65 3d27 4d79 2041 7070  app_name='My App
-00002f30: 272c 2074 6974 6c65 3d27 4d79 2074 6974  ', title='My tit
-00002f40: 6c65 2729 0a0a 6060 600a 0a53 616d 6520  le')..```..Same 
-00002f50: 6173 2074 6865 2063 6c61 7373 6963 732e  as the classics.
-00002f60: 0a0a 536f 2068 6f77 2064 6f65 7320 4573  ..So how does Es
-00002f70: 6d65 7261 6c64 206b 6e6f 7720 6162 6f75  merald know abou
-00002f80: 7420 7468 6520 6465 6661 756c 7420 7365  t the default se
-00002f90: 7474 696e 6773 3f20 456e 7465 7273 205b  ttings? Enters [
-00002fa0: 4573 6d65 7261 6c64 2073 6574 7469 6e67  Esmerald setting
-00002fb0: 7320 6d6f 6475 6c65 5d28 2365 736d 6572  s module](#esmer
-00002fc0: 616c 642d 7365 7474 696e 6773 2d6d 6f64  ald-settings-mod
-00002fd0: 756c 6529 2e0a 0a23 2323 2045 736d 6572  ule)...### Esmer
-00002fe0: 616c 6420 5365 7474 696e 6773 204d 6f64  ald Settings Mod
-00002ff0: 756c 650a 0a54 6869 7320 6973 2074 6865  ule..This is the
-00003000: 2077 6179 2045 736d 6572 616c 6420 6465   way Esmerald de
-00003010: 6661 756c 7473 2074 6865 2076 616c 7565  faults the value
-00003020: 732e 2057 6865 6e20 7374 6172 7469 6e67  s. When starting
-00003030: 2061 6e20 6170 706c 6963 6174 696f 6e2c   an application,
-00003040: 2074 6865 2073 7973 7465 6d20 6c6f 6f6b   the system look
-00003050: 7320 666f 7220 610a 6045 534d 4552 414c  s for a.`ESMERAL
-00003060: 445f 5345 5454 494e 4753 5f4d 4f44 554c  D_SETTINGS_MODUL
-00003070: 4560 2065 6e76 6972 6f6e 6d65 6e74 2076  E` environment v
-00003080: 6172 6961 626c 652e 2049 6620 6e6f 2076  ariable. If no v
-00003090: 6172 6961 626c 6520 6973 2073 7570 706c  ariable is suppl
-000030a0: 6965 6420 7468 656e 2074 6865 2073 7973  ied then the sys
-000030b0: 7465 6d20 7769 6c6c 2064 6566 6175 6c74  tem will default
-000030c0: 2074 6f0a 6045 736d 6572 616c 6441 5049   to.`EsmeraldAPI
-000030d0: 5365 7474 696e 6773 6020 7365 7474 696e  Settings` settin
-000030e0: 6773 2061 6e64 2073 7461 7274 2e0a 0a23  gs and start...#
-000030f0: 2323 2043 7573 746f 6d20 5365 7474 696e  ## Custom Settin
-00003100: 6773 0a0a 5365 7061 7261 7469 6f6e 206f  gs..Separation o
-00003110: 6620 7365 7474 696e 6773 2062 7920 656e  f settings by en
-00003120: 7669 726f 6d6d 656e 7420 6973 2061 206d  viromment is a m
-00003130: 7573 7420 6861 7665 2074 6865 7365 2064  ust have these d
-00003140: 6179 7320 616e 6420 7374 6172 7469 6e67  ays and starting
-00003150: 2077 6974 6820 6465 6661 756c 7420 6f66   with default of
-00003160: 2045 736d 6572 616c 6420 7769 6c6c 206e   Esmerald will n
-00003170: 6f74 2062 650a 656e 6f75 6768 2066 6f72  ot be.enough for
-00003180: 2061 6e79 2061 7070 6c69 6361 7469 6f6e   any application
-00003190: 2e0a 0a54 6865 2073 6574 7469 6e67 7320  ...The settings 
-000031a0: 6172 6520 7079 6461 6e74 6963 2073 7461  are pydantic sta
-000031b0: 6e64 6172 6420 7365 7474 696e 6773 2061  ndard settings a
-000031c0: 6e64 2074 6865 7265 666f 7265 2063 6f6d  nd therefore com
-000031d0: 7061 7469 626c 6520 7769 7468 2045 736d  patible with Esm
-000031e0: 6572 616c 642e 0a54 6865 2073 7973 7465  erald..The syste
-000031f0: 6d20 6272 696e 6773 2073 6f6d 6520 6465  m brings some de
-00003200: 6661 756c 7473 2074 6861 7420 6361 6e20  faults that can 
-00003210: 6265 2075 7365 6420 6f75 742d 6f66 2d74  be used out-of-t
-00003220: 6865 2d62 6f78 2062 7574 2069 7427 7320  he-box but it's 
-00003230: 6e6f 7420 6d61 6e64 6174 6f72 7920 746f  not mandatory to
-00003240: 2062 6520 7573 6564 2e0a 5468 6520 656e   be used..The en
-00003250: 7669 726f 6e6d 656e 7420 6465 6661 756c  vironment defaul
-00003260: 7473 2074 6f20 2a2a 7072 6f64 7563 7469  ts to **producti
-00003270: 6f6e 2a2a 2e0a 0a60 6060 7079 7468 6f6e  on**...```python
-00003280: 0a0a 6672 6f6d 2065 736d 6572 616c 6420  ..from esmerald 
-00003290: 696d 706f 7274 2045 736d 6572 616c 6441  import EsmeraldA
-000032a0: 5049 5365 7474 696e 6773 0a66 726f 6d20  PISettings.from 
-000032b0: 6573 6d65 7261 6c64 2e63 6f6e 662e 656e  esmerald.conf.en
-000032c0: 756d 7320 696d 706f 7274 2045 6e76 6972  ums import Envir
-000032d0: 6f6e 6d65 6e74 5479 7065 0a0a 636c 6173  onmentType..clas
-000032e0: 7320 4465 7665 6c6f 706d 656e 7428 4573  s Development(Es
-000032f0: 6d65 7261 6c64 4150 4953 6574 7469 6e67  meraldAPISetting
-00003300: 7329 3a0a 2020 2020 6170 705f 6e61 6d65  s):.    app_name
-00003310: 3a20 7374 7220 3d20 274d 7920 6170 7020  : str = 'My app 
-00003320: 696e 2064 6576 270a 2020 2020 656e 7669  in dev'.    envi
-00003330: 726f 6e6d 656e 743a 2073 7472 203d 2045  ronment: str = E
-00003340: 6e76 6972 6f6e 6d65 6e74 5479 7065 2e44  nvironmentType.D
-00003350: 4556 454c 4f50 4d45 4e54 0a0a 6060 600a  EVELOPMENT..```.
-00003360: 0a2a 2a4c 6f61 6420 7468 6520 7365 7474  .**Load the sett
-00003370: 696e 6773 2069 6e74 6f20 796f 7572 2045  ings into your E
-00003380: 736d 6572 616c 6420 6170 706c 6963 6174  smerald applicat
-00003390: 696f 6e2a 2a3a 0a0a 4173 7375 6d69 6e67  ion**:..Assuming
-000033a0: 2079 6f75 7220 4573 6d65 7261 6c64 2061   your Esmerald a
-000033b0: 7070 2069 7320 696e 7369 6465 2061 6e20  pp is inside an 
-000033c0: 6073 7263 2f61 7070 2e70 7960 2e0a 0a60  `src/app.py`...`
-000033d0: 6060 636f 6e73 6f6c 650a 0a45 534d 4552  ``console..ESMER
-000033e0: 414c 445f 5345 5454 494e 4753 5f4d 4f44  ALD_SETTINGS_MOD
-000033f0: 554c 453d 276d 7961 7070 2e73 6574 7469  ULE='myapp.setti
-00003400: 6e67 732e 4465 7665 6c6f 706d 656e 7427  ngs.Development'
-00003410: 2070 7974 686f 6e20 2d6d 2073 7263 2e61   python -m src.a
-00003420: 7070 2e70 790a 0a60 6060 0a0a 2323 2047  pp.py..```..## G
-00003430: 6174 6577 6179 2c20 5765 6253 6f63 6b65  ateway, WebSocke
-00003440: 7447 6174 6577 6179 2061 6e64 2049 6e63  tGateway and Inc
-00003450: 6c75 6465 0a0a 5374 6172 6c65 7474 6520  lude..Starlette 
-00003460: 6f66 6665 7273 2074 6865 2052 6f75 7465  offers the Route
-00003470: 2063 6c61 7373 6573 2066 6f72 2073 696d   classes for sim
-00003480: 706c 6520 7061 7468 2061 7373 6967 6e6d  ple path assignm
-00003490: 656e 7473 2062 7574 2074 6869 7320 6973  ents but this is
-000034a0: 2061 6c73 6f20 7665 7279 206c 696d 6974   also very limit
-000034b0: 696e 6720 6966 2073 6f6d 6574 6869 6e67  ing if something
-000034c0: 206d 6f72 650a 636f 6d70 6c65 7820 696e   more.complex in
-000034d0: 206d 696e 642e 2045 736d 6572 616c 6420   mind. Esmerald 
-000034e0: 6578 7465 6e64 7320 7468 6174 2066 756e  extends that fun
-000034f0: 6374 696f 6e61 6c69 7479 2061 6e64 2061  ctionality and a
-00003500: 6464 7320 736f 6d65 2060 666c 6169 7260  dds some `flair`
-00003510: 2061 6e64 206c 6576 656c 7320 7570 2062   and levels up b
-00003520: 7920 6861 7669 6e67 2074 6865 0a47 6174  y having the.Gat
-00003530: 6577 6179 2c20 5765 6253 6f63 6b65 7447  eway, WebSocketG
-00003540: 6174 6577 6179 2061 6e64 2049 6e63 6c75  ateway and Inclu
-00003550: 6465 2e0a 0a54 686f 7365 2061 7265 2073  de...Those are s
-00003560: 7065 6369 616c 206f 626a 6563 7473 2074  pecial objects t
-00003570: 6861 7420 616c 6c6f 7720 616c 6c20 7468  hat allow all th
-00003580: 6520 6d61 6769 6320 6f66 2045 736d 6572  e magic of Esmer
-00003590: 616c 6420 746f 2068 6170 7065 6e2e 0a0a  ald to happen...
-000035a0: 466f 7220 6120 636c 6173 7369 632c 2064  For a classic, d
-000035b0: 6972 6563 742c 206f 6e65 2066 696c 6520  irect, one file 
-000035c0: 7369 6e67 6c65 2061 7070 726f 6163 682e  single approach.
-000035d0: 0a0a 2a2a 496e 2061 206e 7574 7368 656c  ..**In a nutshel
-000035e0: 6c2a 2a3a 0a0a 6060 6070 7974 686f 6e20  l**:..```python 
-000035f0: 7469 746c 653d 2773 7263 2f61 7070 2e70  title='src/app.p
-00003600: 7927 0a66 726f 6d20 6573 6d65 7261 6c64  y'.from esmerald
-00003610: 2069 6d70 6f72 7420 4573 6d65 7261 6c64   import Esmerald
-00003620: 2c20 6765 742c 2073 7461 7475 732c 2052  , get, status, R
-00003630: 6571 7565 7374 2c20 554a 534f 4e52 6573  equest, UJSONRes
-00003640: 706f 6e73 652c 2047 6174 6577 6179 2c20  ponse, Gateway, 
-00003650: 5765 6253 6f63 6b65 7447 6174 6577 6179  WebSocketGateway
-00003660: 2c20 5765 6273 6f63 6b65 740a 0a40 6765  , Websocket..@ge
-00003670: 7428 7374 6174 7573 5f63 6f64 653d 7374  t(status_code=st
-00003680: 6174 7573 2e48 5454 505f 3230 305f 4f4b  atus.HTTP_200_OK
-00003690: 290a 6173 796e 6320 6465 6620 686f 6d65  ).async def home
-000036a0: 2829 202d 3e20 554a 534f 4e52 6573 706f  () -> UJSONRespo
-000036b0: 6e73 653a 0a20 2020 2072 6574 7572 6e20  nse:.    return 
-000036c0: 554a 534f 4e52 6573 706f 6e73 6528 7b0a  UJSONResponse({.
-000036d0: 2020 2020 2020 2020 2264 6574 6169 6c22          "detail"
-000036e0: 3a20 2248 656c 6c6f 2077 6f72 6c64 220a  : "Hello world".
-000036f0: 2020 2020 7d29 0a0a 0a40 6765 7428 290a      })...@get().
-00003700: 6173 796e 6320 6465 6620 616e 6f74 6865  async def anothe
-00003710: 7228 7265 7175 6573 743a 2052 6571 7565  r(request: Reque
-00003720: 7374 2920 2d3e 2064 6963 743a 0a20 2020  st) -> dict:.   
-00003730: 2072 6574 7572 6e20 7b0a 2020 2020 2020   return {.      
-00003740: 2020 2264 6574 6169 6c22 3a20 2241 6e6f    "detail": "Ano
-00003750: 7468 6572 2077 6f72 6c64 2122 0a20 2020  ther world!".   
-00003760: 207d 0a0a 4077 6562 736f 636b 6574 2870   }..@websocket(p
-00003770: 6174 683d 222f 7b70 6174 685f 7061 7261  ath="/{path_para
-00003780: 6d3a 7374 727d 2229 0a61 7379 6e63 2064  m:str}").async d
-00003790: 6566 2077 6f72 6c64 5f73 6f63 6b65 7428  ef world_socket(
-000037a0: 736f 636b 6574 3a20 5765 6273 6f63 6b65  socket: Websocke
-000037b0: 7429 202d 3e20 4e6f 6e65 3a0a 2020 2020  t) -> None:.    
-000037c0: 6177 6169 7420 736f 636b 6574 2e61 6363  await socket.acc
-000037d0: 6570 7428 290a 2020 2020 6d73 6720 3d20  ept().    msg = 
-000037e0: 6177 6169 7420 736f 636b 6574 2e72 6563  await socket.rec
-000037f0: 6569 7665 5f6a 736f 6e28 290a 2020 2020  eive_json().    
-00003800: 6173 7365 7274 206d 7367 0a20 2020 2061  assert msg.    a
-00003810: 7373 6572 7420 736f 636b 6574 0a20 2020  ssert socket.   
-00003820: 2061 7761 6974 2073 6f63 6b65 742e 636c   await socket.cl
-00003830: 6f73 6528 290a 0a0a 6170 7020 3d20 4573  ose()...app = Es
-00003840: 6d65 7261 6c64 2872 6f75 7465 733d 5b0a  merald(routes=[.
-00003850: 2020 2020 4761 7465 7761 7928 6861 6e64      Gateway(hand
-00003860: 6c65 723d 686f 6d65 292c 0a20 2020 2047  ler=home),.    G
-00003870: 6174 6577 6179 2868 616e 646c 6572 3d61  ateway(handler=a
-00003880: 6e6f 7468 6572 292c 0a20 2020 2057 6562  nother),.    Web
-00003890: 536f 636b 6574 4761 7465 7761 7928 6861  SocketGateway(ha
-000038a0: 6e64 6c65 723d 776f 726c 645f 736f 636b  ndler=world_sock
-000038b0: 6574 292c 0a5d 290a 0a60 6060 0a0a 2323  et),.])..```..##
-000038c0: 2044 6573 6967 6e20 696e 206d 696e 640a   Design in mind.
-000038d0: 0a47 6f6f 6420 6465 7369 676e 2069 7320  .Good design is 
-000038e0: 616c 7761 7973 2065 6e63 6f75 7261 6765  always encourage
-000038f0: 6420 616e 6420 4573 6d65 7261 6c64 2061  d and Esmerald a
-00003900: 6c6c 6f77 7320 636f 6d70 6c65 7820 726f  llows complex ro
-00003910: 7574 696e 6720 6f6e 2061 6e79 206c 6576  uting on any lev
-00003920: 656c 2e0a 0a23 2323 2054 6865 2068 616e  el...### The han
-00003930: 646c 6572 7320 2876 6965 7773 290a 0a60  dlers (views)..`
-00003940: 6060 7079 7468 6f6e 2074 6974 6c65 3d22  ``python title="
-00003950: 6d79 6170 702f 6163 636f 756e 7473 2f76  myapp/accounts/v
-00003960: 6965 7773 2e70 7922 0a66 726f 6d20 6573  iews.py".from es
-00003970: 6d65 7261 6c64 2069 6d70 6f72 7420 6765  merald import ge
-00003980: 742c 2070 6f73 742c 2070 7574 2c20 7374  t, post, put, st
-00003990: 6174 7573 2c20 7765 6273 6f63 6b65 742c  atus, websocket,
-000039a0: 2041 5049 5669 6577 2c20 5265 7175 6573   APIView, Reques
-000039b0: 742c 204a 534f 4e52 6573 706f 6e73 652c  t, JSONResponse,
-000039c0: 2052 6573 706f 6e73 652c 2057 6562 536f   Response, WebSo
-000039d0: 636b 6574 0a66 726f 6d20 7079 6461 6e74  cket.from pydant
-000039e0: 6963 2069 6d70 6f72 7420 4261 7365 4d6f  ic import BaseMo
-000039f0: 6465 6c0a 0a0a 636c 6173 7320 5072 6f64  del...class Prod
-00003a00: 7563 7428 4261 7365 4d6f 6465 6c29 3a0a  uct(BaseModel):.
-00003a10: 2020 2020 6e61 6d65 3a20 7374 720a 2020      name: str.  
-00003a20: 2020 736b 753a 2073 7472 0a20 2020 2070    sku: str.    p
-00003a30: 7269 6365 3a20 666c 6f61 740a 0a0a 4070  rice: float...@p
-00003a40: 7574 2827 2f70 726f 6475 6374 2f7b 7072  ut('/product/{pr
-00003a50: 6f64 7563 745f 6964 7d27 290a 6465 6620  oduct_id}').def 
-00003a60: 7570 6461 7465 5f70 726f 6475 6374 2870  update_product(p
-00003a70: 726f 6475 6374 5f69 643a 2069 6e74 2c20  roduct_id: int, 
-00003a80: 6461 7461 3a20 5072 6f64 7563 7429 202d  data: Product) -
-00003a90: 3e20 6469 6374 3a0a 2020 2020 7265 7475  > dict:.    retu
-00003aa0: 726e 207b 2270 726f 6475 6374 5f69 6422  rn {"product_id"
-00003ab0: 3a20 7072 6f64 7563 745f 6964 2c20 2270  : product_id, "p
-00003ac0: 726f 6475 6374 5f6e 616d 6522 3a20 7072  roduct_name": pr
-00003ad0: 6f64 7563 742e 6e61 6d65 207d 0a0a 0a40  oduct.name }...@
-00003ae0: 6765 7428 7374 6174 7573 5f63 6f64 653d  get(status_code=
-00003af0: 7374 6174 7573 2e48 5454 505f 3230 305f  status.HTTP_200_
-00003b00: 4f4b 290a 6173 796e 6320 6465 6620 686f  OK).async def ho
-00003b10: 6d65 2829 202d 3e20 4a53 4f4e 5265 7370  me() -> JSONResp
-00003b20: 6f6e 7365 3a0a 2020 2020 7265 7475 726e  onse:.    return
-00003b30: 204a 534f 4e52 6573 706f 6e73 6528 7b0a   JSONResponse({.
-00003b40: 2020 2020 2020 2020 2264 6574 6169 6c22          "detail"
-00003b50: 3a20 2248 656c 6c6f 2077 6f72 6c64 220a  : "Hello world".
-00003b60: 2020 2020 7d29 0a0a 0a40 6765 7428 290a      })...@get().
-00003b70: 6173 796e 6320 6465 6620 616e 6f74 6865  async def anothe
-00003b80: 7228 7265 7175 6573 743a 2052 6571 7565  r(request: Reque
-00003b90: 7374 2920 2d3e 2064 6963 743a 0a20 2020  st) -> dict:.   
-00003ba0: 2072 6574 7572 6e20 7b0a 2020 2020 2020   return {.      
-00003bb0: 2020 2264 6574 6169 6c22 3a20 2241 6e6f    "detail": "Ano
-00003bc0: 7468 6572 2077 6f72 6c64 2122 0a20 2020  ther world!".   
-00003bd0: 207d 0a0a 0a40 7765 6273 6f63 6b65 7428   }...@websocket(
-00003be0: 7061 7468 3d22 2f7b 7061 7468 5f70 6172  path="/{path_par
-00003bf0: 616d 3a73 7472 7d22 290a 6173 796e 6320  am:str}").async 
-00003c00: 6465 6620 776f 726c 645f 736f 636b 6574  def world_socket
-00003c10: 2873 6f63 6b65 743a 2057 6562 736f 636b  (socket: Websock
-00003c20: 6574 2920 2d3e 204e 6f6e 653a 0a20 2020  et) -> None:.   
-00003c30: 2061 7761 6974 2073 6f63 6b65 742e 6163   await socket.ac
-00003c40: 6365 7074 2829 0a20 2020 206d 7367 203d  cept().    msg =
-00003c50: 2061 7761 6974 2073 6f63 6b65 742e 7265   await socket.re
-00003c60: 6365 6976 655f 6a73 6f6e 2829 0a20 2020  ceive_json().   
-00003c70: 2061 7373 6572 7420 6d73 670a 2020 2020   assert msg.    
-00003c80: 6173 7365 7274 2073 6f63 6b65 740a 2020  assert socket.  
-00003c90: 2020 6177 6169 7420 736f 636b 6574 2e63    await socket.c
-00003ca0: 6c6f 7365 2829 0a0a 0a63 6c61 7373 2057  lose()...class W
-00003cb0: 6f72 6c64 2841 5049 5669 6577 293a 0a0a  orld(APIView):..
-00003cc0: 2020 2020 4067 6574 2870 6174 683d 272f      @get(path='/
-00003cd0: 7b75 726c 7d27 290a 2020 2020 6173 796e  {url}').    asyn
-00003ce0: 6320 6465 6620 686f 6d65 2872 6571 7565  c def home(reque
-00003cf0: 7374 3a20 5265 7175 6573 742c 2075 726c  st: Request, url
-00003d00: 3a20 7374 7229 202d 3e20 5265 7370 6f6e  : str) -> Respon
-00003d10: 7365 3a0a 2020 2020 2020 2020 7265 7475  se:.        retu
-00003d20: 726e 2052 6573 706f 6e73 6528 6622 5552  rn Response(f"UR
-00003d30: 4c3a 207b 7572 6c7d 2229 0a0a 2020 2020  L: {url}")..    
-00003d40: 4070 6f73 7428 7061 7468 3d27 2f7b 7572  @post(path='/{ur
-00003d50: 6c7d 272c 2073 7461 7475 735f 636f 6465  l}', status_code
-00003d60: 3d73 7461 7475 732e 4854 5450 5f32 3031  =status.HTTP_201
-00003d70: 5f43 5245 4154 4544 290a 2020 2020 6173  _CREATED).    as
-00003d80: 796e 6320 6465 6620 6d61 7273 2872 6571  ync def mars(req
-00003d90: 7565 7374 3a20 5265 7175 6573 742c 2075  uest: Request, u
-00003da0: 726c 3a20 7374 7229 202d 3e20 4a53 4f4e  rl: str) -> JSON
-00003db0: 5265 7370 6f6e 7365 3a0a 2020 2020 2020  Response:.      
-00003dc0: 2020 2e2e 2e0a 0a20 2020 2040 7765 6273    .....    @webs
-00003dd0: 6f63 6b65 7428 7061 7468 3d22 2f7b 7061  ocket(path="/{pa
-00003de0: 7468 5f70 6172 616d 3a73 7472 7d22 290a  th_param:str}").
-00003df0: 2020 2020 6173 796e 6320 6465 6620 706c      async def pl
-00003e00: 7574 6f28 7365 6c66 2c20 736f 636b 6574  uto(self, socket
-00003e10: 3a20 5765 6273 6f63 6b65 7429 202d 3e20  : Websocket) -> 
-00003e20: 4e6f 6e65 3a0a 2020 2020 2020 2020 6177  None:.        aw
-00003e30: 6169 7420 736f 636b 6574 2e61 6363 6570  ait socket.accep
-00003e40: 7428 290a 2020 2020 2020 2020 6d73 6720  t().        msg 
-00003e50: 3d20 6177 6169 7420 736f 636b 6574 2e72  = await socket.r
-00003e60: 6563 6569 7665 5f6a 736f 6e28 290a 2020  eceive_json().  
-00003e70: 2020 2020 2020 6173 7365 7274 206d 7367        assert msg
-00003e80: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00003e90: 736f 636b 6574 0a20 2020 2020 2020 2061  socket.        a
-00003ea0: 7761 6974 2073 6f63 6b65 742e 636c 6f73  wait socket.clos
-00003eb0: 6528 290a 0a0a 6060 600a 0a49 6620 6120  e()...```..If a 
-00003ec0: 6070 6174 6860 2069 7320 6e6f 7420 7072  `path` is not pr
-00003ed0: 6f76 6964 6564 2c20 6465 6661 756c 7473  ovided, defaults
-00003ee0: 2074 6f20 602f 602e 0a0a 2323 2320 5468   to `/`...### Th
-00003ef0: 6520 6761 7465 7761 7973 2028 7572 6c73  e gateways (urls
-00003f00: 290a 0a60 6060 7079 7468 6f6e 2074 6974  )..```python tit
-00003f10: 6c65 3d22 6d79 6170 702f 6163 636f 756e  le="myapp/accoun
-00003f20: 7473 2f75 726c 732e 7079 220a 6672 6f6d  ts/urls.py".from
-00003f30: 2065 736d 6572 616c 6420 696d 706f 7274   esmerald import
-00003f40: 2047 6174 6577 6179 2c20 5765 6253 6f63   Gateway, WebSoc
-00003f50: 6b65 7447 6174 6577 6179 0a66 726f 6d20  ketGateway.from 
-00003f60: 2e76 6965 7773 2069 6d70 6f72 7420 686f  .views import ho
-00003f70: 6d65 2c20 616e 6f74 6865 722c 2077 6f72  me, another, wor
-00003f80: 6c64 5f73 6f63 6b65 742c 2057 6f72 6c64  ld_socket, World
-00003f90: 0a0a 726f 7574 655f 7061 7474 6572 6e73  ..route_patterns
-00003fa0: 203d 205b 0a20 2020 2047 6174 6577 6179   = [.    Gateway
-00003fb0: 2868 616e 646c 6572 3d75 7064 6174 655f  (handler=update_
-00003fc0: 7072 6f64 7563 7429 2c0a 2020 2020 4761  product),.    Ga
-00003fd0: 7465 7761 7928 6861 6e64 6c65 723d 686f  teway(handler=ho
-00003fe0: 6d65 292c 0a20 2020 2047 6174 6577 6179  me),.    Gateway
-00003ff0: 2868 616e 646c 6572 3d61 6e6f 7468 6572  (handler=another
-00004000: 292c 0a20 2020 2047 6174 6577 6179 2868  ),.    Gateway(h
-00004010: 616e 646c 6572 3d57 6f72 6c64 292c 0a20  andler=World),. 
-00004020: 2020 2057 6562 536f 636b 6574 4761 7465     WebSocketGate
-00004030: 7761 7928 6861 6e64 6c65 723d 776f 726c  way(handler=worl
-00004040: 645f 736f 636b 6574 292c 0a5d 0a0a 6060  d_socket),.]..``
-00004050: 600a 0a49 6620 6120 6070 6174 6860 2069  `..If a `path` i
-00004060: 7320 6e6f 7420 7072 6f76 6964 6564 2c20  s not provided, 
-00004070: 6465 6661 756c 7473 2074 6f20 602f 602e  defaults to `/`.
-00004080: 0a0a 2323 2320 5468 6520 496e 636c 7564  ..### The Includ
-00004090: 650a 0a54 6869 7320 6973 2061 2076 6572  e..This is a ver
-000040a0: 7920 7370 6563 6961 6c20 6f62 6a65 6374  y special object
-000040b0: 2074 6861 7420 616c 6c6f 7773 2074 6865   that allows the
-000040c0: 2069 6d70 6f72 7420 6f66 2061 6e79 2072   import of any r
-000040d0: 6f75 7465 2066 726f 6d20 616e 7977 6865  oute from anywhe
-000040e0: 7265 2069 6e20 7468 6520 6170 706c 6963  re in the applic
-000040f0: 6174 696f 6e2e 0a0a 6049 6e63 6c75 6465  ation...`Include
-00004100: 6020 6163 6365 7074 7320 7468 6520 696d  ` accepts the im
-00004110: 706f 7274 2076 6961 2060 6e61 6d65 7370  port via `namesp
-00004120: 6163 6560 206f 7220 7669 6120 6072 6f75  ace` or via `rou
-00004130: 7465 7360 206c 6973 7420 6275 7420 6e6f  tes` list but no
-00004140: 7420 626f 7468 2e0a 0a57 6865 6e20 7573  t both...When us
-00004150: 696e 6720 6120 606e 616d 6573 7061 6365  ing a `namespace
-00004160: 602c 2074 6865 2060 496e 636c 7564 6560  `, the `Include`
-00004170: 2077 696c 6c20 6c6f 6f6b 2066 6f72 2074   will look for t
-00004180: 6865 2064 6566 6175 6c74 2060 726f 7574  he default `rout
-00004190: 655f 7061 7474 6572 6e73 6020 6f62 6a65  e_patterns` obje
-000041a0: 6374 206c 6973 7420 696e 2074 6865 2069  ct list in the i
-000041b0: 6d70 6f72 7465 640a 6e61 6d65 7370 6163  mported.namespac
-000041c0: 6520 756e 6c65 7373 2061 2064 6966 6665  e unless a diffe
-000041d0: 7265 6e74 2060 7061 7474 6572 6e60 2069  rent `pattern` i
-000041e0: 7320 7370 6563 6966 6965 642e 0a0a 5468  s specified...Th
-000041f0: 6520 7061 7474 6572 6e20 6f6e 6c79 2077  e pattern only w
-00004200: 6f72 6b73 2069 6620 7468 6520 696d 706f  orks if the impo
-00004210: 7274 7320 6172 6520 646f 6e65 2076 6961  rts are done via
-00004220: 2060 6e61 6d65 7370 6163 6560 2061 6e64   `namespace` and
-00004230: 206e 6f74 2076 6961 2060 726f 7574 6573   not via `routes
-00004240: 602e 0a0a 2a2a 496d 706f 7274 696e 6720  `...**Importing 
-00004250: 7573 696e 6720 6e61 6d65 7370 6163 652a  using namespace*
-00004260: 2a3a 0a0a 6060 6070 7974 686f 6e20 7469  *:..```python ti
-00004270: 746c 653d 276d 7961 7070 2f75 726c 732e  tle='myapp/urls.
-00004280: 7079 270a 6672 6f6d 2065 736d 6572 616c  py'.from esmeral
-00004290: 6420 696d 706f 7274 2049 6e63 6c75 6465  d import Include
-000042a0: 0a0a 726f 7574 655f 7061 7474 6572 6e73  ..route_patterns
-000042b0: 203d 205b 0a20 2020 2049 6e63 6c75 6465   = [.    Include
-000042c0: 286e 616d 6573 7061 6365 3d27 6d79 6170  (namespace='myap
-000042d0: 702e 6163 636f 756e 7473 2e75 726c 7327  p.accounts.urls'
-000042e0: 290a 5d0a 0a60 6060 0a0a 2a2a 496d 706f  ).]..```..**Impo
-000042f0: 7274 696e 6720 7573 696e 6720 726f 7574  rting using rout
-00004300: 6573 2a2a 3a0a 0a60 6060 7079 7468 6f6e  es**:..```python
-00004310: 2074 6974 6c65 3d27 7372 632f 6d79 6170   title='src/myap
-00004320: 702f 7572 6c73 2e70 7927 0a66 726f 6d20  p/urls.py'.from 
-00004330: 6573 6d65 7261 6c64 2069 6d70 6f72 7420  esmerald import 
-00004340: 496e 636c 7564 650a 6672 6f6d 206d 7961  Include.from mya
-00004350: 7070 2e61 6363 6f75 6e74 7320 696d 706f  pp.accounts impo
-00004360: 7274 2075 726c 730a 0a72 6f75 7465 5f70  rt urls..route_p
-00004370: 6174 7465 726e 7320 3d20 5b0a 2020 2020  atterns = [.    
-00004380: 496e 636c 7564 6528 726f 7574 6573 3d75  Include(routes=u
-00004390: 726c 732e 726f 7574 655f 7061 7474 6572  rls.route_patter
-000043a0: 6e73 290a 5d0a 0a60 6060 0a0a 4966 2061  ns).]..```..If a
-000043b0: 2060 7061 7468 6020 6973 206e 6f74 2070   `path` is not p
-000043c0: 726f 7669 6465 642c 2064 6566 6175 6c74  rovided, default
-000043d0: 7320 746f 2060 2f60 2e0a 0a23 2323 2320  s to `/`...#### 
-000043e0: 5573 696e 6720 6120 6469 6666 6572 656e  Using a differen
-000043f0: 7420 7061 7474 6572 6e0a 0a60 6060 7079  t pattern..```py
-00004400: 7468 6f6e 2074 6974 6c65 3d22 7372 632f  thon title="src/
-00004410: 6d79 6170 702f 6163 636f 756e 7473 2f75  myapp/accounts/u
-00004420: 726c 732e 7079 220a 6672 6f6d 2065 736d  rls.py".from esm
-00004430: 6572 616c 6420 696d 706f 7274 2047 6174  erald import Gat
-00004440: 6577 6179 2c20 5765 6253 6f63 6b65 7447  eway, WebSocketG
-00004450: 6174 6577 6179 0a66 726f 6d20 2e76 6965  ateway.from .vie
-00004460: 7773 2069 6d70 6f72 7420 686f 6d65 2c20  ws import home, 
-00004470: 616e 6f74 6865 722c 2077 6f72 6c64 5f73  another, world_s
-00004480: 6f63 6b65 742c 2057 6f72 6c64 0a0a 6d79  ocket, World..my
-00004490: 5f75 726c 7320 3d20 5b0a 2020 2020 4761  _urls = [.    Ga
-000044a0: 7465 7761 7928 6861 6e64 6c65 723d 7570  teway(handler=up
-000044b0: 6461 7465 5f70 726f 6475 6374 292c 0a20  date_product),. 
-000044c0: 2020 2047 6174 6577 6179 2868 616e 646c     Gateway(handl
-000044d0: 6572 3d68 6f6d 6529 2c0a 2020 2020 4761  er=home),.    Ga
-000044e0: 7465 7761 7928 6861 6e64 6c65 723d 616e  teway(handler=an
-000044f0: 6f74 6865 7229 2c0a 2020 2020 4761 7465  other),.    Gate
-00004500: 7761 7928 6861 6e64 6c65 723d 576f 726c  way(handler=Worl
-00004510: 6429 2c0a 2020 2020 5765 6253 6f63 6b65  d),.    WebSocke
-00004520: 7447 6174 6577 6179 2868 616e 646c 6572  tGateway(handler
-00004530: 3d77 6f72 6c64 5f73 6f63 6b65 7429 2c0a  =world_socket),.
-00004540: 5d0a 0a60 6060 0a0a 2a2a 496d 706f 7274  ]..```..**Import
-00004550: 696e 6720 7573 696e 6720 6e61 6d65 7370  ing using namesp
-00004560: 6163 652a 2a3a 0a0a 6060 6070 7974 686f  ace**:..```pytho
-00004570: 6e20 7469 746c 653d 2773 7263 2f6d 7961  n title='src/mya
-00004580: 7070 2f75 726c 732e 7079 270a 6672 6f6d  pp/urls.py'.from
-00004590: 2065 736d 6572 616c 6420 696d 706f 7274   esmerald import
-000045a0: 2049 6e63 6c75 6465 0a0a 726f 7574 655f   Include..route_
-000045b0: 7061 7474 6572 6e73 203d 205b 0a20 2020  patterns = [.   
-000045c0: 2049 6e63 6c75 6465 286e 616d 6573 7061   Include(namespa
-000045d0: 6365 3d27 6d79 6170 702e 6163 636f 756e  ce='myapp.accoun
-000045e0: 7473 2e75 726c 7327 2c20 7061 7474 6572  ts.urls', patter
-000045f0: 6e3d 276d 795f 7572 6c73 2729 0a5d 0a0a  n='my_urls').]..
-00004600: 6060 600a 0a23 2320 496e 636c 7564 6520  ```..## Include 
-00004610: 616e 6420 4573 6d65 7261 6c64 0a0a 5468  and Esmerald..Th
-00004620: 6520 6049 6e63 6c75 6465 6020 6361 6e20  e `Include` can 
-00004630: 6265 2076 6572 7920 6865 6c70 6675 6c20  be very helpful 
-00004640: 6d6f 7374 6c79 2077 6865 6e20 7468 6520  mostly when the 
-00004650: 676f 616c 2069 7320 746f 2061 766f 6964  goal is to avoid
-00004660: 2061 206c 6f74 206f 6620 696d 706f 7274   a lot of import
-00004670: 7320 616e 6420 6d61 7373 6976 6520 6c69  s and massive li
-00004680: 7374 0a6f 6620 6f62 6a65 6374 7320 746f  st.of objects to
-00004690: 2062 6520 7061 7373 6564 2069 6e74 6f20   be passed into 
-000046a0: 6f6e 6520 7369 6e67 6c65 206f 626a 6563  one single objec
-000046b0: 742e 2054 6869 7320 6361 6e20 6265 2070  t. This can be p
-000046c0: 6172 7469 6375 6c61 7279 2075 7365 6675  articulary usefu
-000046d0: 6c20 746f 206d 616b 6520 6120 4573 6d65  l to make a Esme
-000046e0: 7261 6c64 2069 6e73 7461 6e63 652e 0a0a  rald instance...
-000046f0: 2a2a 4578 616d 706c 652a 2a3a 0a0a 6060  **Example**:..``
-00004700: 6070 7974 686f 6e20 7469 746c 653d 2773  `python title='s
-00004710: 7263 2f75 726c 732e 7079 270a 6672 6f6d  rc/urls.py'.from
-00004720: 2065 736d 6572 616c 6420 696d 706f 7274   esmerald import
-00004730: 2049 6e63 6c75 6465 0a0a 726f 7574 655f   Include..route_
-00004740: 7061 7474 6572 6e73 203d 205b 0a20 2020  patterns = [.   
-00004750: 2049 6e63 6c75 6465 286e 616d 6573 7061   Include(namespa
-00004760: 6365 3d27 6d79 6170 702e 6163 636f 756e  ce='myapp.accoun
-00004770: 7473 2e75 726c 7327 2c20 7061 7474 6572  ts.urls', patter
-00004780: 6e3d 276d 795f 7572 6c73 2729 0a5d 0a0a  n='my_urls').]..
-00004790: 6060 600a 0a60 6060 7079 7468 6f6e 2074  ```..```python t
-000047a0: 6974 6c65 3d27 7372 632f 6170 702e 7079  itle='src/app.py
-000047b0: 270a 6672 6f6d 2065 736d 6572 616c 6420  '.from esmerald 
-000047c0: 696d 706f 7274 2045 736d 6572 616c 642c  import Esmerald,
-000047d0: 2049 6e63 6c75 6465 0a0a 6170 7020 3d20   Include..app = 
-000047e0: 4573 6d65 7261 6c64 2872 6f75 7465 733d  Esmerald(routes=
-000047f0: 5b49 6e63 6c75 6465 2827 7372 632e 7572  [Include('src.ur
-00004800: 6c73 2729 5d29 0a0a 6060 600a 0a23 2320  ls')])..```..## 
-00004810: 5275 6e20 7468 6520 6170 706c 6963 6174  Run the applicat
-00004820: 696f 6e0a 0a41 7320 6d65 6e74 696f 6e65  ion..As mentione
-00004830: 6420 6265 666f 7265 2c20 7765 2072 6563  d before, we rec
-00004840: 6f6d 6d65 6e64 2075 7669 636f 726e 2066  ommend uvicorn f
-00004850: 6f72 2070 726f 6475 6374 696f 6e20 6275  or production bu
-00004860: 7420 6974 2773 206e 6f74 206d 616e 6461  t it's not manda
-00004870: 746f 7279 2e0a 0a2a 2a55 7369 6e67 2075  tory...**Using u
-00004880: 7669 636f 726e 2a2a 3a0a 0a60 6060 7368  vicorn**:..```sh
-00004890: 656c 6c0a 7576 6963 6f72 6e20 7372 633a  ell.uvicorn src:
-000048a0: 6170 7020 2d2d 7265 6c6f 6164 0a0a 494e  app --reload..IN
-000048b0: 464f 3a20 2020 2020 5576 6963 6f72 6e20  FO:     Uvicorn 
-000048c0: 7275 6e6e 696e 6720 6f6e 2068 7474 703a  running on http:
-000048d0: 2f2f 3132 372e 302e 302e 313a 3830 3030  //127.0.0.1:8000
-000048e0: 2028 5072 6573 7320 4354 524c 2b43 2074   (Press CTRL+C t
-000048f0: 6f20 7175 6974 290a 494e 464f 3a20 2020  o quit).INFO:   
-00004900: 2020 5374 6172 7465 6420 7265 6c6f 6164    Started reload
-00004910: 6572 2070 726f 6365 7373 205b 3238 3732  er process [2872
-00004920: 305d 0a49 4e46 4f3a 2020 2020 2053 7461  0].INFO:     Sta
-00004930: 7274 6564 2073 6572 7665 7220 7072 6f63  rted server proc
-00004940: 6573 7320 5b32 3837 3232 5d0a 494e 464f  ess [28722].INFO
-00004950: 3a20 2020 2020 5761 6974 696e 6720 666f  :     Waiting fo
-00004960: 7220 6170 706c 6963 6174 696f 6e20 7374  r application st
-00004970: 6172 7475 702e 0a49 4e46 4f3a 2020 2020  artup..INFO:    
-00004980: 2041 7070 6c69 6361 7469 6f6e 2073 7461   Application sta
-00004990: 7274 7570 2063 6f6d 706c 6574 652e 0a60  rtup complete..`
-000049a0: 6060 0a0a 2323 2052 756e 2074 6865 2061  ``..## Run the a
-000049b0: 7070 6c69 6361 7469 6f6e 2077 6974 6820  pplication with 
-000049c0: 6375 7374 6f6d 2073 6574 7469 6e67 730a  custom settings.
-000049d0: 0a2a 2a55 7369 6e67 2075 7669 636f 726e  .**Using uvicorn
-000049e0: 2a2a 3a0a 0a60 6060 7368 656c 6c0a 4553  **:..```shell.ES
-000049f0: 4d45 5241 4c44 5f53 4554 5449 4e47 535f  MERALD_SETTINGS_
-00004a00: 4d4f 4455 4c45 3d6d 7961 7070 2e41 7070  MODULE=myapp.App
-00004a10: 5365 7474 696e 6773 2075 7669 636f 726e  Settings uvicorn
-00004a20: 2073 7263 3a61 7070 202d 2d72 656c 6f61   src:app --reloa
-00004a30: 640a 0a49 4e46 4f3a 2020 2020 2055 7669  d..INFO:     Uvi
-00004a40: 636f 726e 2072 756e 6e69 6e67 206f 6e20  corn running on 
-00004a50: 6874 7470 3a2f 2f31 3237 2e30 2e30 2e31  http://127.0.0.1
-00004a60: 3a38 3030 3020 2850 7265 7373 2043 5452  :8000 (Press CTR
-00004a70: 4c2b 4320 746f 2071 7569 7429 0a49 4e46  L+C to quit).INF
-00004a80: 4f3a 2020 2020 2053 7461 7274 6564 2072  O:     Started r
-00004a90: 656c 6f61 6465 7220 7072 6f63 6573 7320  eloader process 
-00004aa0: 5b32 3837 3230 5d0a 494e 464f 3a20 2020  [28720].INFO:   
-00004ab0: 2020 5374 6172 7465 6420 7365 7276 6572    Started server
-00004ac0: 2070 726f 6365 7373 205b 3238 3732 325d   process [28722]
-00004ad0: 0a49 4e46 4f3a 2020 2020 2057 6169 7469  .INFO:     Waiti
-00004ae0: 6e67 2066 6f72 2061 7070 6c69 6361 7469  ng for applicati
-00004af0: 6f6e 2073 7461 7274 7570 2e0a 494e 464f  on startup..INFO
-00004b00: 3a20 2020 2020 4170 706c 6963 6174 696f  :     Applicatio
-00004b10: 6e20 7374 6172 7475 7020 636f 6d70 6c65  n startup comple
-00004b20: 7465 2e0a 6060 600a 0a23 2320 4f70 656e  te..```..## Open
-00004b30: 4150 4920 646f 6375 6d65 6e74 6174 696f  API documentatio
-00004b40: 6e0a 0a45 736d 6572 616c 6420 616c 736f  n..Esmerald also
-00004b50: 2063 6f6d 6573 2077 6974 6820 4f70 656e   comes with Open
-00004b60: 4150 4920 646f 6373 2069 6e74 6567 7261  API docs integra
-00004b70: 7465 642e 2046 6f72 2074 686f 7365 2075  ted. For those u
-00004b80: 7365 6420 746f 2074 6861 742c 2074 6869  sed to that, thi
-00004b90: 7320 6973 2072 6f75 6768 6c79 2074 6865  s is roughly the
-00004ba0: 2073 616d 6520 616e 6420 746f 206d 616b   same and to mak
-00004bb0: 6520 6974 0a68 6170 7065 6e2c 2074 6865  e it.happen, the
-00004bc0: 7265 2077 6572 6520 696e 7370 6972 6174  re were inspirat
-00004bd0: 696f 6e73 2074 6861 7420 6865 6c70 6564  ions that helped
-00004be0: 2045 736d 6572 616c 6420 6765 7474 696e   Esmerald gettin
-00004bf0: 6720 7468 6572 6520 6661 7374 2e0a 0a45  g there fast...E
-00004c00: 736d 6572 616c 6420 7374 6172 7473 2061  smerald starts a
-00004c10: 7574 6f6d 6174 6963 616c 6c79 2074 6865  utomatically the
-00004c20: 204f 7065 6e41 5049 2064 6f63 756d 656e   OpenAPI documen
-00004c30: 7461 7469 6f6e 2062 7920 696e 6a65 6374  tation by inject
-00004c40: 696e 6720 7468 6520 4f70 656e 4150 4943  ing the OpenAPIC
-00004c50: 6f6e 6669 6720 6465 6661 756c 7420 6672  onfig default fr
-00004c60: 6f6d 0a74 6865 2073 6574 7469 6e67 7320  om.the settings 
-00004c70: 616e 6420 6d61 6b65 7320 5377 6167 6765  and makes Swagge
-00004c80: 722c 2052 6544 6f63 2061 6e20 5374 6f70  r, ReDoc an Stop
-00004c90: 6c69 6768 7420 656c 656d 656e 7473 2061  light elements a
-00004ca0: 7661 696c 6162 6c65 2074 6f20 796f 7520  vailable to you 
-00004cb0: 6f75 7420 6f66 2074 6865 2062 6f78 2e0a  out of the box..
-00004cc0: 0a54 6f20 6163 6365 7373 2074 6865 204f  .To access the O
-00004cd0: 7065 6e41 5049 2c20 7369 6d70 6c79 2073  penAPI, simply s
-00004ce0: 7461 7274 2079 6f75 7220 6c6f 6361 6c20  tart your local 
-00004cf0: 6465 7665 6c6f 706d 656e 7420 616e 6420  development and 
-00004d00: 6163 6365 7373 3a0a 0a2a 202a 2a53 7761  access:..* **Swa
-00004d10: 6767 6572 2a2a 202d 2060 2f64 6f63 732f  gger** - `/docs/
-00004d20: 7377 6167 6765 7260 2e0a 2a20 2a2a 5265  swagger`..* **Re
-00004d30: 646f 632a 2a20 2d20 602f 646f 6373 2f72  doc** - `/docs/r
-00004d40: 6564 6f63 602e 0a2a 202a 2a53 746f 706c  edoc`..* **Stopl
-00004d50: 6967 6874 2045 6c65 6d65 6e74 732a 2a20  ight Elements** 
-00004d60: 2d20 602f 646f 6373 2f65 6c65 6d65 6e74  - `/docs/element
-00004d70: 7360 2e0a 0a54 6865 7265 2061 7265 206d  s`...There are m
-00004d80: 6f72 6520 6465 7461 696c 7320 6162 6f75  ore details abou
-00004d90: 7420 5b68 6f77 2074 6f20 636f 6e66 6967  t [how to config
-00004da0: 7572 6520 7468 6520 4f70 656e 4150 4943  ure the OpenAPIC
-00004db0: 6f6e 6669 675d 2868 7474 7073 3a2f 2f65  onfig](https://e
-00004dc0: 736d 6572 616c 642e 6465 762f 636f 6e66  smerald.dev/conf
-00004dd0: 6967 7572 6174 696f 6e73 2f6f 7065 6e61  igurations/opena
-00004de0: 7069 2f63 6f6e 6669 6729 0a77 6974 6869  pi/config).withi
-00004df0: 6e20 7468 6520 646f 6375 6d65 6e74 6174  n the documentat
-00004e00: 696f 6e2e 0a0a 5468 6572 6520 6973 2061  ion...There is a
-00004e10: 6c73 6f20 6120 676f 6f64 2065 7870 6c61  lso a good expla
-00004e20: 6e61 7469 6f6e 206f 6e20 686f 7720 746f  nation on how to
-00004e30: 2075 7365 2074 6865 205b 4f70 656e 4150   use the [OpenAP
-00004e40: 4952 6573 706f 6e73 655d 2868 7474 7073  IResponse](https
-00004e50: 3a2f 2f65 736d 6572 616c 642e 6465 762f  ://esmerald.dev/
-00004e60: 7265 7370 6f6e 7365 7323 6f70 656e 6170  responses#openap
-00004e70: 692d 7265 7370 6f6e 7365 7329 0a61 7320  i-responses).as 
-00004e80: 7765 6c6c 2e0a 0a23 2320 4e6f 7465 730a  well...## Notes.
-00004e90: 0a54 6869 7320 6973 206a 7573 7420 6120  .This is just a 
-00004ea0: 7665 7279 2068 6967 682d 6c65 7665 6c20  very high-level 
-00004eb0: 6465 6d6f 6e73 7472 6174 696f 6e20 6f66  demonstration of
-00004ec0: 2068 6f77 2074 6f20 7374 6172 7420 7175   how to start qu
-00004ed0: 6963 6b6c 7920 616e 6420 7768 6174 2045  ickly and what E
-00004ee0: 736d 6572 616c 6420 6361 6e20 646f 2e0a  smerald can do..
-00004ef0: 5468 6572 6520 6172 6520 706c 656e 7479  There are plenty
-00004f00: 206d 6f72 6520 7468 696e 6773 2079 6f75   more things you
-00004f10: 2063 616e 2064 6f20 7769 7468 2045 736d   can do with Esm
-00004f20: 6572 616c 642e 2045 6e6a 6f79 2120 f09f  erald. Enjoy! ..
-00004f30: 988a 0a0a 2323 2053 706f 6e73 6f72 730a  ....## Sponsors.
-00004f40: 0a43 7572 7265 6e74 6c79 2074 6865 7265  .Currently there
-00004f50: 2061 7265 206e 6f20 7370 6f6e 736f 7273   are no sponsors
-00004f60: 206f 6620 4573 6d65 7261 6c64 2062 7574   of Esmerald but
-00004f70: 2079 6f75 2063 616e 2066 696e 616e 6369   you can financi
-00004f80: 616c 6c79 2068 656c 7020 616e 6420 7375  ally help and su
-00004f90: 7070 6f72 7420 7468 6520 6175 7468 6f72  pport the author
-00004fa0: 2074 686f 7567 680a 5b47 6974 4875 6220   though.[GitHub 
-00004fb0: 7370 6f6e 736f 7273 5d28 6874 7470 733a  sponsors](https:
-00004fc0: 2f2f 6769 7468 7562 2e63 6f6d 2f73 706f  //github.com/spo
-00004fd0: 6e73 6f72 732f 7461 7273 696c 2920 616e  nsors/tarsil) an
-00004fe0: 6420 6265 636f 6d65 2061 202a 2a53 7065  d become a **Spe
-00004ff0: 6369 616c 206f 6e65 2a2a 206f 7220 6120  cial one** or a 
-00005000: 2a2a 4c65 6765 6e64 2a2a 2e0a 0a5b 7361  **Legend**...[sa
-00005010: 6666 6965 725f 6f72 6d5d 3a20 6874 7470  ffier_orm]: http
-00005020: 733a 2f2f 6573 6d65 7261 6c64 2e64 6576  s://esmerald.dev
-00005030: 2f64 6174 6162 6173 6573 2f73 6166 6669  /databases/saffi
-00005040: 6572 2f6d 6f74 6976 6174 696f 6e0a 5b65  er/motivation.[e
-00005050: 6467 795f 6f72 6d5d 3a20 6874 7470 733a  dgy_orm]: https:
-00005060: 2f2f 6573 6d65 7261 6c64 2e64 6576 2f64  //esmerald.dev/d
-00005070: 6174 6162 6173 6573 2f73 6166 6669 6572  atabases/saffier
-00005080: 2f6d 6f74 6976 6174 696f 6e0a 5b6d 6f6e  /motivation.[mon
-00005090: 676f 7a5f 6f64 6d5d 3a20 6874 7470 733a  goz_odm]: https:
-000050a0: 2f2f 6573 6d65 7261 6c64 2e64 6576 2f64  //esmerald.dev/d
-000050b0: 6174 6162 6173 6573 2f6d 6f6e 676f 7a2f  atabases/mongoz/
-000050c0: 6d6f 7469 7661 7469 6f6e 0a              motivation.
+00000e10: 2027 7465 7374 270a 5072 6f76 6964 6573   'test'.Provides
+00000e20: 2d45 7874 7261 3a20 7465 7374 696e 670a  -Extra: testing.
+00000e30: 5265 7175 6972 6573 2d44 6973 743a 2061  Requires-Dist: a
+00000e40: 6e79 696f 5b74 7269 6f5d 3c35 2e30 2e30  nyio[trio]<5.0.0
+00000e50: 2c3e 3d33 2e36 2e32 3b20 6578 7472 6120  ,>=3.6.2; extra 
+00000e60: 3d3d 2027 7465 7374 696e 6727 0a52 6571  == 'testing'.Req
+00000e70: 7569 7265 732d 4469 7374 3a20 6272 6f74  uires-Dist: brot
+00000e80: 6c69 3c32 2e30 2e30 2c3e 3d31 2e30 2e39  li<2.0.0,>=1.0.9
+00000e90: 3b20 6578 7472 6120 3d3d 2027 7465 7374  ; extra == 'test
+00000ea0: 696e 6727 0a52 6571 7569 7265 732d 4469  ing'.Requires-Di
+00000eb0: 7374 3a20 6564 6779 5b70 6f73 7467 7265  st: edgy[postgre
+00000ec0: 735d 3e3d 302e 342e 303b 2065 7874 7261  s]>=0.4.0; extra
+00000ed0: 203d 3d20 2774 6573 7469 6e67 270a 5265   == 'testing'.Re
+00000ee0: 7175 6972 6573 2d44 6973 743a 2066 6c61  quires-Dist: fla
+00000ef0: 736b 3c34 2e30 2e30 2c3e 3d31 2e31 2e32  sk<4.0.0,>=1.1.2
+00000f00: 3b20 6578 7472 6120 3d3d 2027 7465 7374  ; extra == 'test
+00000f10: 696e 6727 0a52 6571 7569 7265 732d 4469  ing'.Requires-Di
+00000f20: 7374 3a20 6672 6565 7a65 6775 6e3c 322e  st: freezegun<2.
+00000f30: 302e 302c 3e3d 312e 322e 323b 2065 7874  0.0,>=1.2.2; ext
+00000f40: 7261 203d 3d20 2774 6573 7469 6e67 270a  ra == 'testing'.
+00000f50: 5265 7175 6972 6573 2d44 6973 743a 2069  Requires-Dist: i
+00000f60: 7064 623b 2065 7874 7261 203d 3d20 2774  pdb; extra == 't
+00000f70: 6573 7469 6e67 270a 5265 7175 6972 6573  esting'.Requires
+00000f80: 2d44 6973 743a 206d 6f6e 676f 7a3e 3d30  -Dist: mongoz>=0
+00000f90: 2e36 2e30 3b20 6578 7472 6120 3d3d 2027  .6.0; extra == '
+00000fa0: 7465 7374 696e 6727 0a52 6571 7569 7265  testing'.Require
+00000fb0: 732d 4469 7374 3a20 6d79 7079 3d3d 312e  s-Dist: mypy==1.
+00000fc0: 392e 303b 2065 7874 7261 203d 3d20 2774  9.0; extra == 't
+00000fd0: 6573 7469 6e67 270a 5265 7175 6972 6573  esting'.Requires
+00000fe0: 2d44 6973 743a 2070 6462 7070 3b20 6578  -Dist: pdbpp; ex
+00000ff0: 7472 6120 3d3d 2027 7465 7374 696e 6727  tra == 'testing'
+00001000: 0a52 6571 7569 7265 732d 4469 7374 3a20  .Requires-Dist: 
+00001010: 706f 6c79 6661 6374 6f72 793c 332e 302e  polyfactory<3.0.
+00001020: 302c 3e3d 322e 352e 303b 2065 7874 7261  0,>=2.5.0; extra
+00001030: 203d 3d20 2774 6573 7469 6e67 270a 5265   == 'testing'.Re
+00001040: 7175 6972 6573 2d44 6973 743a 2070 7974  quires-Dist: pyt
+00001050: 6573 742d 6173 796e 6369 6f3e 3d30 2e32  est-asyncio>=0.2
+00001060: 302e 303b 2065 7874 7261 203d 3d20 2774  0.0; extra == 't
+00001070: 6573 7469 6e67 270a 5265 7175 6972 6573  esting'.Requires
+00001080: 2d44 6973 743a 2070 7974 6573 742d 636f  -Dist: pytest-co
+00001090: 763c 362e 302e 302c 3e3d 342e 312e 303b  v<6.0.0,>=4.1.0;
+000010a0: 2065 7874 7261 203d 3d20 2774 6573 7469   extra == 'testi
+000010b0: 6e67 270a 5265 7175 6972 6573 2d44 6973  ng'.Requires-Dis
+000010c0: 743a 2070 7974 6573 743c 392e 302e 302c  t: pytest<9.0.0,
+000010d0: 3e3d 372e 312e 333b 2065 7874 7261 203d  >=7.1.3; extra =
+000010e0: 3d20 2774 6573 7469 6e67 270a 5265 7175  = 'testing'.Requ
+000010f0: 6972 6573 2d44 6973 743a 2073 6166 6669  ires-Dist: saffi
+00001100: 6572 5b70 6f73 7467 7265 735d 3e3d 312e  er[postgres]>=1.
+00001110: 332e 373b 2065 7874 7261 203d 3d20 2774  3.7; extra == 't
+00001120: 6573 7469 6e67 270a 5265 7175 6972 6573  esting'.Requires
+00001130: 2d44 6973 743a 2074 7970 6573 2d6f 726a  -Dist: types-orj
+00001140: 736f 6e3d 3d33 2e36 2e32 3b20 6578 7472  son==3.6.2; extr
+00001150: 6120 3d3d 2027 7465 7374 696e 6727 0a52  a == 'testing'.R
+00001160: 6571 7569 7265 732d 4469 7374 3a20 7479  equires-Dist: ty
+00001170: 7065 732d 756a 736f 6e3d 3d35 2e31 302e  pes-ujson==5.10.
+00001180: 302e 3230 3234 3035 3135 3b20 6578 7472  0.20240515; extr
+00001190: 6120 3d3d 2027 7465 7374 696e 6727 0a44  a == 'testing'.D
+000011a0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+000011b0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+000011c0: 726b 646f 776e 0a0a 2320 4573 6d65 7261  rkdown..# Esmera
+000011d0: 6c64 0a0a 3c70 2061 6c69 676e 3d22 6365  ld..<p align="ce
+000011e0: 6e74 6572 223e 0a20 203c 6120 6872 6566  nter">.  <a href
+000011f0: 3d22 6874 7470 733a 2f2f 6573 6d65 7261  ="https://esmera
+00001200: 6c64 2e64 6576 223e 3c69 6d67 2073 7263  ld.dev"><img src
+00001210: 3d22 6874 7470 733a 2f2f 7265 732e 636c  ="https://res.cl
+00001220: 6f75 6469 6e61 7279 2e63 6f6d 2f64 796d  oudinary.com/dym
+00001230: 6d6f 6e64 2f69 6d61 6765 2f75 706c 6f61  mond/image/uploa
+00001240: 642f 7631 3637 3336 3139 3334 322f 6573  d/v1673619342/es
+00001250: 6d65 7261 6c64 2f69 6d67 2f6c 6f67 6f2d  merald/img/logo-
+00001260: 6772 5f7a 316f 7438 6f2e 706e 6722 2061  gr_z1ot8o.png" a
+00001270: 6c74 3d27 4573 6d65 7261 6c64 273e 3c2f  lt='Esmerald'></
+00001280: 613e 0a3c 2f70 3e0a 0a3c 7020 616c 6967  a>.</p>..<p alig
+00001290: 6e3d 2263 656e 7465 7222 3e0a 2020 2020  n="center">.    
+000012a0: 3c65 6d3e f09f 9a80 2048 6967 686c 7920  <em>.... Highly 
+000012b0: 7363 616c 6162 6c65 2c20 7065 7266 6f72  scalable, perfor
+000012c0: 6d61 6e74 2c20 6561 7379 2074 6f20 6c65  mant, easy to le
+000012d0: 6172 6e2c 2065 6173 7920 746f 2063 6f64  arn, easy to cod
+000012e0: 6520 616e 6420 666f 7220 6576 6572 7920  e and for every 
+000012f0: 6170 706c 6963 6174 696f 6e2e 20f0 9f9a  application. ...
+00001300: 803c 2f65 6d3e 0a3c 2f70 3e0a 0a3c 7020  .</em>.</p>..<p 
+00001310: 616c 6967 6e3d 2263 656e 7465 7222 3e0a  align="center">.
+00001320: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001330: 2f67 6974 6875 622e 636f 6d2f 6479 6d6d  /github.com/dymm
+00001340: 6f6e 642f 6573 6d65 7261 6c64 2f77 6f72  ond/esmerald/wor
+00001350: 6b66 6c6f 7773 2f54 6573 7425 3230 5375  kflows/Test%20Su
+00001360: 6974 652f 6261 6467 652e 7376 673f 6576  ite/badge.svg?ev
+00001370: 656e 743d 7075 7368 2662 7261 6e63 683d  ent=push&branch=
+00001380: 6d61 696e 2220 7461 7267 6574 3d22 5f62  main" target="_b
+00001390: 6c61 6e6b 223e 0a20 2020 203c 696d 6720  lank">.    <img 
+000013a0: 7372 633d 2268 7474 7073 3a2f 2f67 6974  src="https://git
+000013b0: 6875 622e 636f 6d2f 6479 6d6d 6f6e 642f  hub.com/dymmond/
+000013c0: 6573 6d65 7261 6c64 2f77 6f72 6b66 6c6f  esmerald/workflo
+000013d0: 7773 2f54 6573 7425 3230 5375 6974 652f  ws/Test%20Suite/
+000013e0: 6261 6467 652e 7376 673f 6576 656e 743d  badge.svg?event=
+000013f0: 7075 7368 2662 7261 6e63 683d 6d61 696e  push&branch=main
+00001400: 2220 616c 743d 2254 6573 7420 5375 6974  " alt="Test Suit
+00001410: 6522 3e0a 3c2f 613e 0a0a 3c61 2068 7265  e">.</a>..<a hre
+00001420: 663d 2268 7474 7073 3a2f 2f70 7970 692e  f="https://pypi.
+00001430: 6f72 672f 7072 6f6a 6563 742f 6573 6d65  org/project/esme
+00001440: 7261 6c64 2220 7461 7267 6574 3d22 5f62  rald" target="_b
+00001450: 6c61 6e6b 223e 0a20 2020 203c 696d 6720  lank">.    <img 
+00001460: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00001470: 2e73 6869 656c 6473 2e69 6f2f 7079 7069  .shields.io/pypi
+00001480: 2f76 2f65 736d 6572 616c 643f 636f 6c6f  /v/esmerald?colo
+00001490: 723d 2532 3333 3444 3035 3826 6c61 6265  r=%2334D058&labe
+000014a0: 6c3d 7079 7069 2532 3070 6163 6b61 6765  l=pypi%20package
+000014b0: 2220 616c 743d 2250 6163 6b61 6765 2076  " alt="Package v
+000014c0: 6572 7369 6f6e 223e 0a3c 2f61 3e0a 0a3c  ersion">.</a>..<
+000014d0: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+000014e0: 7079 7069 2e6f 7267 2f70 726f 6a65 6374  pypi.org/project
+000014f0: 2f65 736d 6572 616c 6422 2074 6172 6765  /esmerald" targe
+00001500: 743d 225f 626c 616e 6b22 3e0a 2020 2020  t="_blank">.    
+00001510: 3c69 6d67 2073 7263 3d22 6874 7470 733a  <img src="https:
+00001520: 2f2f 696d 672e 7368 6965 6c64 732e 696f  //img.shields.io
+00001530: 2f70 7970 692f 7079 7665 7273 696f 6e73  /pypi/pyversions
+00001540: 2f65 736d 6572 616c 642e 7376 673f 636f  /esmerald.svg?co
+00001550: 6c6f 723d 2532 3333 3444 3035 3822 2061  lor=%2334D058" a
+00001560: 6c74 3d22 5375 7070 6f72 7465 6420 5079  lt="Supported Py
+00001570: 7468 6f6e 2076 6572 7369 6f6e 7322 3e0a  thon versions">.
+00001580: 3c2f 613e 0a3c 2f70 3e0a 0a2d 2d2d 0a0a  </a>.</p>..---..
+00001590: 2a2a 446f 6375 6d65 6e74 6174 696f 6e2a  **Documentation*
+000015a0: 2a3a 205b 6874 7470 733a 2f2f 6573 6d65  *: [https://esme
+000015b0: 7261 6c64 2e64 6576 5d28 6874 7470 733a  rald.dev](https:
+000015c0: 2f2f 7777 772e 6573 6d65 7261 6c64 2e64  //www.esmerald.d
+000015d0: 6576 2920 f09f 939a 0a0a 2a2a 536f 7572  ev) ......**Sour
+000015e0: 6365 2043 6f64 652a 2a3a 205b 6874 7470  ce Code**: [http
+000015f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f64  s://github.com/d
+00001600: 796d 6d6f 6e64 2f65 736d 6572 616c 645d  ymmond/esmerald]
+00001610: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001620: 636f 6d2f 6479 6d6d 6f6e 642f 6573 6d65  com/dymmond/esme
+00001630: 7261 6c64 290a 0a2a 2a54 6865 206f 6666  rald)..**The off
+00001640: 6963 6961 6c20 7375 7070 6f72 7465 6420  icial supported 
+00001650: 7665 7273 696f 6e20 6973 2061 6c77 6179  version is alway
+00001660: 7320 7468 6520 6c61 7465 7374 2072 656c  s the latest rel
+00001670: 6561 7365 642a 2a2e 0a0a 2d2d 2d0a 0a45  eased**...---..E
+00001680: 736d 6572 616c 6420 6973 2061 206d 6f64  smerald is a mod
+00001690: 6572 6e2c 2070 6f77 6572 6675 6c2c 2066  ern, powerful, f
+000016a0: 6c65 7869 626c 652c 2068 6967 6820 7065  lexible, high pe
+000016b0: 7266 6f72 6d61 6e74 2c20 7765 6220 6672  rformant, web fr
+000016c0: 616d 6577 6f72 6b20 6465 7369 676e 6564  amework designed
+000016d0: 2074 6f20 6275 696c 6420 6e6f 7420 6f6e   to build not on
+000016e0: 6c79 2041 5049 730a 6275 7420 616c 736f  ly APIs.but also
+000016f0: 2066 756c 6c20 7363 616c 6162 6c65 2061   full scalable a
+00001700: 7070 6c69 6361 7469 6f6e 7320 6672 6f6d  pplications from
+00001710: 2074 6865 2073 6d61 6c6c 6573 7420 746f   the smallest to
+00001720: 2065 6e74 6572 7072 6973 6520 6c65 7665   enterprise leve
+00001730: 6c2e 0a0a 4573 6d65 7261 6c64 2069 7320  l...Esmerald is 
+00001740: 6465 7369 676e 6564 2074 6f20 6275 696c  designed to buil
+00001750: 6420 7769 7468 2070 7974 686f 6e20 332e  d with python 3.
+00001760: 382b 2061 6e64 2062 6173 6564 206f 6e20  8+ and based on 
+00001770: 7374 616e 6461 7264 2070 7974 686f 6e20  standard python 
+00001780: 7479 7065 2068 696e 7473 2e20 496e 6974  type hints. Init
+00001790: 6961 6c6c 790a 6275 696c 7420 6f6e 2074  ially.built on t
+000017a0: 6865 2074 6f70 206f 6620 5b53 7461 726c  he top of [Starl
+000017b0: 6574 7465 5d28 6874 7470 733a 2f2f 6769  ette](https://gi
+000017c0: 7468 7562 2e63 6f6d 2f65 6e63 6f64 652f  thub.com/encode/
+000017d0: 7374 6172 6c65 7474 6529 2061 6e64 206c  starlette) and l
+000017e0: 6174 6572 206f 6e20 6d6f 7665 6420 746f  ater on moved to
+000017f0: 205b 4c69 6c79 615d 2868 7474 7073 3a2f   [Lilya](https:/
+00001800: 2f6c 696c 7961 2e64 6576 2920 616e 6420  /lilya.dev) and 
+00001810: 5b50 7964 616e 7469 635d 2868 7474 7073  [Pydantic](https
+00001820: 3a2f 2f67 6974 6875 622e 636f 6d2f 7361  ://github.com/sa
+00001830: 6d75 656c 636f 6c76 696e 2f70 7964 616e  muelcolvin/pydan
+00001840: 7469 6329 2f5b 6d73 6773 7065 635d 2868  tic)/[msgspec](h
+00001850: 7474 7073 3a2f 2f6a 6372 6973 7468 6172  ttps://jcristhar
+00001860: 6966 2e63 6f6d 2f6d 7367 7370 6563 2f29  if.com/msgspec/)
+00001870: 2e0a 0a43 6865 636b 206f 7574 2074 6865  ...Check out the
+00001880: 205b 4573 6d65 7261 6c64 2064 6f63 756d   [Esmerald docum
+00001890: 656e 7461 7469 6f6e 20f0 9f93 9a5d 2868  entation ....](h
+000018a0: 7474 7073 3a2f 2f65 736d 6572 616c 642e  ttps://esmerald.
+000018b0: 6465 7629 0a0a 2a2a 5468 6520 6f66 6669  dev)..**The offi
+000018c0: 6369 616c 2073 7570 706f 7274 6564 2076  cial supported v
+000018d0: 6572 7369 6f6e 2069 7320 616c 7761 7973  ersion is always
+000018e0: 2074 6865 206c 6174 6573 7420 7265 6c65   the latest rele
+000018f0: 6173 6564 2a2a 2e0a 0a23 2320 4d6f 7469  ased**...## Moti
+00001900: 7661 7469 6f6e 0a0a 5468 6572 6520 6172  vation..There ar
+00001910: 6520 6772 6561 7420 6672 616d 6577 6f72  e great framewor
+00001920: 6b73 206f 7574 2074 6865 7265 206c 696b  ks out there lik
+00001930: 6520 4661 7374 4150 492c 2053 7461 726c  e FastAPI, Starl
+00001940: 6974 652c 2046 6c61 6d61 2c20 466c 6173  ite, Flama, Flas
+00001950: 6b2c 2044 6a61 6e67 6f2e 2e2e 2041 6c6c  k, Django... All
+00001960: 206f 6620 7468 656d 2073 6f6c 7669 6e67   of them solving
+00001970: 206d 616a 6f72 6974 790a 6f66 2074 6865   majority.of the
+00001980: 2063 7572 7265 6e74 2064 6179 2d74 6f2d   current day-to-
+00001990: 6461 7920 7072 6f62 6c65 6d73 206f 6620  day problems of 
+000019a0: 3939 2520 6f66 2074 6865 2061 7070 6c69  99% of the appli
+000019b0: 6361 7469 6f6e 7320 6275 7420 6c65 6176  cations but leav
+000019c0: 696e 6720 7468 6520 3125 2074 6861 7420  ing the 1% that 
+000019d0: 6973 2075 7375 616c 6c79 2061 726f 756e  is usually aroun
+000019e0: 6420 7374 7275 6374 7572 650a 616e 6420  d structure.and 
+000019f0: 6465 7369 676e 2f62 7573 696e 6573 7320  design/business 
+00001a00: 7769 7468 6f75 7420 746f 206d 7563 6820  without to much 
+00001a10: 746f 2064 6f2e 0a0a 4573 6d65 7261 6c64  to do...Esmerald
+00001a20: 2067 6f74 2074 6865 2069 6e73 7069 7261   got the inspira
+00001a30: 7469 6f6e 2066 726f 6d20 7468 6f73 6520  tion from those 
+00001a40: 6772 6561 7420 6672 616d 6577 6f72 6b73  great frameworks
+00001a50: 206f 7574 2074 6865 7265 2061 6e64 2077   out there and w
+00001a60: 6173 2062 7569 6c74 2077 6974 6820 616c  as built with al
+00001a70: 6c20 7468 6520 6b6e 6f77 6e20 616d 617a  l the known amaz
+00001a80: 696e 670a 6665 6174 7572 6573 2062 7574  ing.features but
+00001a90: 2077 6974 6820 6275 7369 6e65 7373 2069   with business i
+00001aa0: 6e20 6d69 6e64 2061 7320 7765 6c6c 2e20  n mind as well. 
+00001ab0: 5374 6172 6c69 7465 2c20 666f 7220 6578  Starlite, for ex
+00001ac0: 616d 706c 652c 2067 6176 6520 7468 6520  ample, gave the 
+00001ad0: 696e 7370 6972 6174 696f 6e20 666f 7220  inspiration for 
+00001ae0: 7468 6520 7472 616e 7366 6f72 6d65 7273  the transformers
+00001af0: 2061 6e64 2066 6f72 2074 6865 2053 6967   and for the Sig
+00001b00: 6e61 7475 7265 206d 6f64 656c 732c 0a73  nature models,.s
+00001b10: 6f6d 6574 6869 6e67 2076 6572 7920 7573  omething very us
+00001b20: 6566 756c 2074 6861 7420 6865 6c70 6564  eful that helped
+00001b30: 2045 736d 6572 616c 6420 696e 7465 6765   Esmerald intege
+00001b40: 7261 7469 6e67 2077 6974 6820 7079 6461  rating with pyda
+00001b50: 6e74 6963 2e0a 4661 7374 4150 4920 6761  ntic..FastAPI ga
+00001b60: 7665 2074 6865 2069 6e73 7069 7261 7469  ve the inspirati
+00001b70: 6f6e 2066 6f72 2041 5049 2064 6573 6967  on for API desig
+00001b80: 6e69 6e67 2c20 446a 616e 676f 2066 6f72  ning, Django for
+00001b90: 2074 6865 2070 6572 6d69 7373 696f 6e73   the permissions
+00001ba0: 2c20 466c 6173 6b20 666f 7220 7468 6520  , Flask for the 
+00001bb0: 7369 6d70 6c69 6369 7479 2c20 4e65 7374  simplicity, Nest
+00001bc0: 4a53 2066 6f72 2074 6865 0a63 6f6e 7472  JS for the.contr
+00001bd0: 6f6c 6c65 7273 2061 6e64 2074 6865 206c  ollers and the l
+00001be0: 6973 7420 676f 6573 206f 6e2e 0a0a 466f  ist goes on...Fo
+00001bf0: 7220 6120 6a6f 6220 746f 2062 6520 646f  r a job to be do
+00001c00: 6e65 2070 726f 7065 726c 792c 2075 7375  ne properly, usu
+00001c10: 616c 6c79 2069 7420 6973 206e 6576 6572  ally it is never
+00001c20: 2064 6f6e 6520 616c 6f6e 6520 616e 6420   done alone and 
+00001c30: 7468 6572 6520 6973 2061 6c77 6179 7320  there is always 
+00001c40: 6120 6472 6976 6572 2061 6e64 2069 6e73  a driver and ins
+00001c50: 7069 7261 7469 6f6e 2074 6f20 6974 2e0a  piration to it..
+00001c60: 0a23 2320 5265 7175 6972 656d 656e 7473  .## Requirements
+00001c70: 0a0a 2a20 7079 7468 6f6e 2033 2e38 2b0a  ..* python 3.8+.
+00001c80: 0a45 736d 6572 616c 6420 776f 756c 646e  .Esmerald wouldn
+00001c90: 2774 2062 6520 706f 7373 6962 6c65 2077  't be possible w
+00001ca0: 6974 686f 7574 2074 776f 2063 6f6c 6f73  ithout two colos
+00001cb0: 7361 6c73 3a0a 0a2a 203c 6120 6872 6566  sals:..* <a href
+00001cc0: 3d22 6874 7470 733a 2f2f 7777 772e 6c69  ="https://www.li
+00001cd0: 6c79 612e 6465 762f 2220 636c 6173 733d  lya.dev/" class=
+00001ce0: 2265 7874 6572 6e61 6c2d 6c69 6e6b 2220  "external-link" 
+00001cf0: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
+00001d00: 5374 6172 6c65 7474 653c 2f61 3e0a 2a20  Starlette</a>.* 
+00001d10: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001d20: 2f70 7964 616e 7469 632d 646f 6373 2e68  /pydantic-docs.h
+00001d30: 656c 706d 616e 7561 6c2e 696f 2f22 2063  elpmanual.io/" c
+00001d40: 6c61 7373 3d22 6578 7465 726e 616c 2d6c  lass="external-l
+00001d50: 696e 6b22 2074 6172 6765 743d 225f 626c  ink" target="_bl
+00001d60: 616e 6b22 3e50 7964 616e 7469 633c 2f61  ank">Pydantic</a
+00001d70: 3e0a 0a23 2320 496e 7374 616c 6c61 7469  >..## Installati
+00001d80: 6f6e 0a0a 6060 6073 6865 6c6c 0a24 2070  on..```shell.$ p
+00001d90: 6970 2069 6e73 7461 6c6c 2065 736d 6572  ip install esmer
+00001da0: 616c 640a 6060 600a 0a41 6e20 4153 4749  ald.```..An ASGI
+00001db0: 2073 6572 7665 7220 6973 2061 6c73 6f20   server is also 
+00001dc0: 6e65 6564 6564 2074 6f20 7275 6e20 696e  needed to run in
+00001dd0: 2070 726f 6475 6374 696f 6e2c 2077 6520   production, we 
+00001de0: 7265 636f 6d6d 656e 6420 5b55 7669 636f  recommend [Uvico
+00001df0: 726e 5d28 6874 7470 733a 2f2f 7777 772e  rn](https://www.
+00001e00: 7576 6963 6f72 6e2e 6f72 6729 2062 7574  uvicorn.org) but
+00001e10: 2069 7420 6973 2065 6e74 6972 656c 790a   it is entirely.
+00001e20: 7570 2074 6f20 796f 752e 0a0a 6060 6073  up to you...```s
+00001e30: 6865 6c6c 0a24 2070 6970 2069 6e73 7461  hell.$ pip insta
+00001e40: 6c6c 2075 7669 636f 726e 0a0a 6060 600a  ll uvicorn..```.
+00001e50: 0a49 6620 796f 7520 7761 6e74 2069 6e73  .If you want ins
+00001e60: 7461 6c6c 2065 736d 6572 616c 6420 7769  tall esmerald wi
+00001e70: 7468 2073 7065 6369 6669 6373 3a0a 0a2a  th specifics:..*
+00001e80: 2a53 7570 706f 7274 2066 6f72 2074 656d  *Support for tem
+00001e90: 706c 6174 6520 7379 7374 656d 2073 7563  plate system suc
+00001ea0: 6820 6173 206a 696e 6a61 3220 616e 6420  h as jinja2 and 
+00001eb0: 6d61 6b6f 2a2a 3a0a 0a60 6060 7368 656c  mako**:..```shel
+00001ec0: 6c0a 2420 7069 7020 696e 7374 616c 6c20  l.$ pip install 
+00001ed0: 6573 6d65 7261 6c64 5b74 656d 706c 6174  esmerald[templat
+00001ee0: 6573 5d0a 6060 600a 0a2a 2a53 7570 706f  es].```..**Suppo
+00001ef0: 7274 2066 6f72 2074 6865 2069 6e74 6572  rt for the inter
+00001f00: 6e61 6c20 7363 6865 6475 6c65 722a 2a3a  nal scheduler**:
+00001f10: 0a0a 6060 6073 6865 6c6c 0a24 2070 6970  ..```shell.$ pip
+00001f20: 2069 6e73 7461 6c6c 2065 736d 6572 616c   install esmeral
+00001f30: 645b 7363 6865 6475 6c65 7273 5d0a 6060  d[schedulers].``
+00001f40: 600a 0a2a 2a53 7570 706f 7274 2066 6f72  `..**Support for
+00001f50: 2074 6865 206a 7774 2075 7365 6420 696e   the jwt used in
+00001f60: 7465 726e 616c 6c79 2062 7920 4573 6d65  ternally by Esme
+00001f70: 7261 6c64 2a2a 3a0a 0a60 6060 7368 656c  rald**:..```shel
+00001f80: 6c0a 2420 7069 7020 696e 7374 616c 6c20  l.$ pip install 
+00001f90: 6573 6d65 7261 6c64 5b6a 7774 5d0a 6060  esmerald[jwt].``
+00001fa0: 600a 0a2a 2a53 7570 706f 7274 2066 6f72  `..**Support for
+00001fb0: 204f 524a 534f 4e20 616e 6420 554a 534f   ORJSON and UJSO
+00001fc0: 4e2a 2a3a 0a0a 6060 6073 6865 6c6c 0a24  N**:..```shell.$
+00001fd0: 2070 6970 2069 6e73 7461 6c6c 2065 736d   pip install esm
+00001fe0: 6572 616c 645b 656e 636f 6465 7273 5d0a  erald[encoders].
+00001ff0: 6060 600a 0a2a 2a49 6620 796f 7520 7761  ```..**If you wa
+00002000: 6e74 2074 6f20 7573 6520 7468 6520 6573  nt to use the es
+00002010: 6d65 7261 6c64 2074 6573 7469 6e67 2063  merald testing c
+00002020: 6c69 656e 742a 2a3a 0a0a 6060 6073 6865  lient**:..```she
+00002030: 6c6c 0a24 2070 6970 2069 6e73 7461 6c6c  ll.$ pip install
+00002040: 2065 736d 6572 616c 645b 7465 7374 5d0a   esmerald[test].
+00002050: 6060 600a 0a2a 2a49 6620 796f 7520 7761  ```..**If you wa
+00002060: 6e74 2074 6f20 7573 6520 7468 6520 6573  nt to use the es
+00002070: 6d65 7261 6c64 2073 6865 6c6c 2a2a 3a0a  merald shell**:.
+00002080: 0a4d 6f72 6520 5b64 6574 6169 6c73 5d28  .More [details](
+00002090: 6874 7470 733a 2f2f 6573 6d65 7261 6c64  https://esmerald
+000020a0: 2e64 6576 2f64 6972 6563 7469 7665 732f  .dev/directives/
+000020b0: 7368 656c 6c29 2061 626f 7574 2074 6869  shell) about thi
+000020c0: 7320 746f 7069 6320 5b69 6e20 7468 6520  s topic [in the 
+000020d0: 646f 6373 5d28 6874 7470 733a 2f2f 6573  docs](https://es
+000020e0: 6d65 7261 6c64 2e64 6576 2f64 6972 6563  merald.dev/direc
+000020f0: 7469 7665 732f 7368 656c 6c29 0a0a 6060  tives/shell)..``
+00002100: 6073 6865 6c6c 0a24 2070 6970 2069 6e73  `shell.$ pip ins
+00002110: 7461 6c6c 2065 736d 6572 616c 645b 6970  tall esmerald[ip
+00002120: 7974 686f 6e5d 2023 2064 6566 6175 6c74  ython] # default
+00002130: 2073 6865 6c6c 0a24 2070 6970 2069 6e73   shell.$ pip ins
+00002140: 7461 6c6c 2065 736d 6572 616c 645b 7074  tall esmerald[pt
+00002150: 7079 7468 6f6e 5d20 2320 7074 7079 7468  python] # ptpyth
+00002160: 6f6e 2073 6865 6c6c 0a60 6060 0a0a 2323  on shell.```..##
+00002170: 2320 5374 6172 7420 6120 7072 6f6a 6563  # Start a projec
+00002180: 7420 7573 696e 6720 6469 7265 6374 6976  t using directiv
+00002190: 6573 0a0a 2121 2120 5761 726e 696e 670a  es..!!! Warning.
+000021a0: 2020 2020 5468 6973 2069 7320 666f 7220      This is for 
+000021b0: 6d6f 7265 2061 6476 616e 6365 6420 7573  more advanced us
+000021c0: 6572 7320 7468 6174 2061 7265 2061 6c72  ers that are alr
+000021d0: 6561 6479 2063 6f6d 666f 7274 6162 6c65  eady comfortable
+000021e0: 2077 6974 6820 4573 6d65 7261 6c64 2028   with Esmerald (
+000021f0: 6f72 2050 7974 686f 6e20 696e 2067 656e  or Python in gen
+00002200: 6572 616c 290a 2020 2020 6f72 2066 6565  eral).    or fee
+00002210: 6c20 6c69 6b65 2069 7420 6973 206e 6f74  l like it is not
+00002220: 2061 2070 726f 626c 656d 2075 7369 6e67   a problem using
+00002230: 2074 6865 7365 2064 6972 6563 7469 7665   these directive
+00002240: 732e 2049 6620 796f 7520 646f 206e 6f74  s. If you do not
+00002250: 2066 6565 6c20 636f 6d66 6f72 7461 626c   feel comfortabl
+00002260: 6520 7965 7420 746f 2075 7365 2074 6869  e yet to use thi
+00002270: 732c 0a20 2020 2070 6c65 6173 6520 636f  s,.    please co
+00002280: 6e74 696e 7565 2072 6561 6469 6e67 2074  ntinue reading t
+00002290: 6865 2064 6f63 756d 656e 7461 7469 6f6e  he documentation
+000022a0: 2061 6e64 206c 6561 726e 696e 6720 6d6f   and learning mo
+000022b0: 7265 2061 626f 7574 2045 736d 6572 616c  re about Esmeral
+000022c0: 642e 0a0a 4966 2079 6f75 2077 6973 6820  d...If you wish 
+000022d0: 746f 2073 7461 7274 2061 6e20 4573 6d65  to start an Esme
+000022e0: 7261 6c64 2070 726f 6a65 6374 2077 6974  rald project wit
+000022f0: 6820 6120 6465 6661 756c 7420 7375 6767  h a default sugg
+00002300: 6573 7465 6420 7374 7275 6374 7572 652e  ested structure.
+00002310: 0a0a 6060 6073 6865 6c6c 0a65 736d 6572  ..```shell.esmer
+00002320: 616c 6420 6372 6561 7465 7072 6f6a 6563  ald createprojec
+00002330: 7420 3c59 4f55 522d 5052 4f4a 4543 542d  t <YOUR-PROJECT-
+00002340: 4e41 4d45 3e0a 6060 600a 0a54 6869 7320  NAME>.```..This 
+00002350: 7769 6c6c 2067 656e 6572 6174 6520 6120  will generate a 
+00002360: 7363 6166 666f 6c64 2066 6f72 2079 6f75  scaffold for you
+00002370: 7220 7072 6f6a 6563 7420 7769 7468 2073  r project with s
+00002380: 6f6d 6520 7072 652d 6465 6669 6e65 6420  ome pre-defined 
+00002390: 6669 6c65 7320 696e 2061 2073 696d 706c  files in a simpl
+000023a0: 6520 6661 7368 696f 6e2e 0a54 6869 7320  e fashion..This 
+000023b0: 7769 6c6c 2061 6c73 6f20 6765 6e65 7261  will also genera
+000023c0: 7465 2061 2066 696c 6520 666f 7220 7468  te a file for th
+000023d0: 6520 7465 7374 7320 7573 696e 6720 7468  e tests using th
+000023e0: 6520 4573 6d65 7261 6c64 5465 7374 436c  e EsmeraldTestCl
+000023f0: 6965 6e74 2c20 736f 206d 616b 6520 7375  ient, so make su
+00002400: 7265 2079 6f75 2072 756e 3a0a 0a60 6060  re you run:..```
+00002410: 7368 656c 6c0a 2420 7069 7020 696e 7374  shell.$ pip inst
+00002420: 616c 6c20 6573 6d65 7261 6c64 5b74 6573  all esmerald[tes
+00002430: 745d 0a60 6060 0a0a 4f72 2079 6f75 2063  t].```..Or you c
+00002440: 616e 2073 6b69 7020 7468 6973 2073 7465  an skip this ste
+00002450: 7020 6966 2079 6f75 2064 6f6e 2774 2077  p if you don't w
+00002460: 616e 7420 746f 2075 7365 2074 6865 2045  ant to use the E
+00002470: 736d 6572 616c 6454 6573 7443 6c69 656e  smeraldTestClien
+00002480: 742e 0a0a 596f 7520 6361 6e20 6669 6e64  t...You can find
+00002490: 205b 6d6f 7265 2069 6e66 6f72 6d61 7469   [more informati
+000024a0: 6f6e 5d28 6874 7470 733a 2f2f 6573 6d65  on](https://esme
+000024b0: 7261 6c64 2e64 6576 2f6d 616e 6167 656d  rald.dev/managem
+000024c0: 656e 742f 6469 7265 6374 6976 6573 2920  ent/directives) 
+000024d0: 6162 6f75 7420 7468 6973 2064 6972 6563  about this direc
+000024e0: 7469 7665 2061 6e64 2068 6f77 2074 6f0a  tive and how to.
+000024f0: 7573 6520 6974 2e0a 0a23 2320 4b65 7920  use it...## Key 
+00002500: 4665 6174 7572 6573 0a0a 2a20 2a2a 466c  Features..* **Fl
+00002510: 7569 6420 616e 6420 4661 7374 2a2a 3a20  uid and Fast**: 
+00002520: 5468 616e 6b73 2074 6f20 5374 6172 6c65  Thanks to Starle
+00002530: 7474 6520 616e 6420 5079 6461 6e74 6963  tte and Pydantic
+00002540: 2f6d 7367 7370 6563 2e0a 2a20 2a2a 4661  /msgspec..* **Fa
+00002550: 7374 2074 6f20 6465 7665 6c6f 702a 2a3a  st to develop**:
+00002560: 2054 6861 6e6b 7320 746f 2074 6865 2073   Thanks to the s
+00002570: 696d 706c 6963 6974 7920 6f66 2064 6573  implicity of des
+00002580: 6967 6e2c 2074 6865 2064 6576 656c 6f70  ign, the develop
+00002590: 6d65 6e74 2074 696d 6573 2063 616e 2062  ment times can b
+000025a0: 6520 7265 6475 6365 6420 6578 706f 6e65  e reduced expone
+000025b0: 6e74 6961 6c6c 792e 0a2a 202a 2a49 6e74  ntially..* **Int
+000025c0: 7569 7469 7665 2a2a 3a20 4966 2079 6f75  uitive**: If you
+000025d0: 2061 7265 2075 7365 6420 746f 2074 6865   are used to the
+000025e0: 206f 7468 6572 2066 7261 6d65 776f 726b   other framework
+000025f0: 732c 2045 736d 6572 616c 6420 6973 2061  s, Esmerald is a
+00002600: 206e 6f20 6272 6169 6e65 7220 746f 2064   no brainer to d
+00002610: 6576 656c 6f70 2e0a 2a20 2a2a 4561 7379  evelop..* **Easy
+00002620: 2a2a 3a20 4465 7665 6c6f 7065 6420 7769  **: Developed wi
+00002630: 7468 2064 6573 6967 6e20 696e 206d 696e  th design in min
+00002640: 6420 616e 6420 6561 7379 206c 6561 726e  d and easy learn
+00002650: 696e 672e 0a2a 202a 2a53 686f 7274 2a2a  ing..* **Short**
+00002660: 3a20 5769 7468 2074 6865 204f 4f50 2061  : With the OOP a
+00002670: 7661 696c 6162 6c65 206e 6174 6976 656c  vailable nativel
+00002680: 7920 7468 6572 6520 6973 206e 6f20 6e65  y there is no ne
+00002690: 6564 2066 6f72 2063 6f64 6520 6475 706c  ed for code dupl
+000026a0: 6963 6174 696f 6e2e 2053 4f4c 4944 2e0a  ication. SOLID..
+000026b0: 2a20 2a2a 5265 6164 792a 2a3a 2047 6574  * **Ready**: Get
+000026c0: 2079 6f75 7220 6170 706c 6963 6174 696f   your applicatio
+000026d0: 6e20 7570 2061 6e64 2072 756e 6e69 6e67  n up and running
+000026e0: 2077 6974 6820 7072 6f64 7563 7469 6f6e   with production
+000026f0: 2d72 6561 6479 2063 6f64 652e 0a2a 202a  -ready code..* *
+00002700: 2a4f 4f50 2061 6e64 2046 756e 6374 696f  *OOP and Functio
+00002710: 6e61 6c2a 2a3a 2044 6573 6967 6e20 4150  nal**: Design AP
+00002720: 4973 2069 6e20 616e 7920 6465 7369 7265  Is in any desire
+00002730: 6420 7761 792e 204f 4f50 206f 7220 4675  d way. OOP or Fu
+00002740: 6e63 7469 6f6e 616c 2069 7320 6176 6169  nctional is avai
+00002750: 6c61 626c 652e 0a2a 202a 2a41 7379 6e63  lable..* **Async
+00002760: 2061 6e64 2053 796e 632a 2a3a 2044 6f20   and Sync**: Do 
+00002770: 796f 7520 7072 6566 6572 2073 796e 6320  you prefer sync 
+00002780: 6f72 2061 7379 6e63 3f20 596f 7520 6361  or async? You ca
+00002790: 6e20 6861 7665 2062 6f74 682e 0a2a 202a  n have both..* *
+000027a0: 2a4d 6964 646c 6577 6172 652a 2a3a 2041  *Middleware**: A
+000027b0: 7070 6c79 206d 6964 646c 6577 6172 6573  pply middlewares
+000027c0: 206f 6e20 7468 6520 6170 706c 6963 6174   on the applicat
+000027d0: 696f 6e20 6c65 7665 6c20 6f72 2041 5049  ion level or API
+000027e0: 206c 6576 656c 2e0a 2a20 2a2a 4578 6365   level..* **Exce
+000027f0: 7074 696f 6e20 4861 6e64 6c65 7273 2a2a  ption Handlers**
+00002800: 3a20 4170 706c 7920 6578 6365 7074 696f  : Apply exceptio
+00002810: 6e20 6861 6e64 6c65 7273 206f 6e20 616e  n handlers on an
+00002820: 7920 6465 7369 7265 6420 6c65 7665 6c2e  y desired level.
+00002830: 0a2a 202a 2a50 6572 6d69 7373 696f 6e73  .* **Permissions
+00002840: 2a2a 3a20 4170 706c 7920 7370 6563 6966  **: Apply specif
+00002850: 6963 2072 756c 6573 2061 6e64 2070 6572  ic rules and per
+00002860: 6d69 7373 696f 6e73 206f 6e20 6561 6368  missions on each
+00002870: 2041 5049 2e0a 2a20 2a2a 496e 7465 7263   API..* **Interc
+00002880: 6570 746f 7273 2a2a 3a20 496e 7465 7263  eptors**: Interc
+00002890: 6570 7420 7265 7175 6573 7473 2061 6e64  ept requests and
+000028a0: 2061 6464 206c 6f67 6963 2062 6566 6f72   add logic befor
+000028b0: 6520 7265 6163 6869 6e67 2074 6865 2065  e reaching the e
+000028c0: 6e64 706f 696e 742e 0a2a 202a 2a50 6c75  ndpoint..* **Plu
+000028d0: 6767 6162 6c65 732a 2a3a 2043 7265 6174  ggables**: Creat
+000028e0: 6520 706c 7567 696e 7320 666f 7220 4573  e plugins for Es
+000028f0: 6d65 7261 6c64 2061 6e64 2068 6f6f 6b20  merald and hook 
+00002900: 7468 656d 2069 6e74 6f20 616e 7920 6170  them into any ap
+00002910: 706c 6963 6174 696f 6e20 616e 642f 6f72  plication and/or
+00002920: 0a64 6973 7472 6962 7574 6520 7468 656d  .distribute them
+00002930: 2e0a 2a20 2a2a 4441 4f20 616e 6420 4173  ..* **DAO and As
+00002940: 796e 6344 414f 2a2a 3a20 4176 6f69 6420  yncDAO**: Avoid 
+00002950: 6461 7461 6261 7365 2063 616c 6c73 2064  database calls d
+00002960: 6972 6563 746c 7920 6672 6f6d 2074 6865  irectly from the
+00002970: 2041 5049 732e 2055 7365 2062 7573 696e   APIs. Use busin
+00002980: 6573 7320 6f62 6a65 6374 7320 696e 7374  ess objects inst
+00002990: 6561 642e 0a2a 202a 2a4f 524d 2053 7570  ead..* **ORM Sup
+000029a0: 706f 7274 2a2a 3a20 4e61 7469 7665 2073  port**: Native s
+000029b0: 7570 706f 7274 2066 6f72 205b 5361 6666  upport for [Saff
+000029c0: 6965 725d 5b73 6166 6669 6572 5f6f 726d  ier][saffier_orm
+000029d0: 5d20 616e 6420 5b45 6467 795d 5b65 6467  ] and [Edgy][edg
+000029e0: 795f 6f72 6d5d 2e0a 2a20 2a2a 4f44 4d20  y_orm]..* **ODM 
+000029f0: 5375 7070 6f72 742a 2a3a 204e 6174 6976  Support**: Nativ
+00002a00: 6520 7375 7070 6f72 7420 666f 7220 5b4d  e support for [M
+00002a10: 6f6e 676f 7a5d 5b6d 6f6e 676f 7a5f 6f64  ongoz][mongoz_od
+00002a20: 6d5d 2e0a 2a20 2a2a 4150 4956 6965 772a  m]..* **APIView*
+00002a30: 2a3a 2043 6c61 7373 2042 6173 6564 2065  *: Class Based e
+00002a40: 6e64 706f 696e 7473 2066 6f72 2079 6f75  ndpoints for you
+00002a50: 7220 6265 6c6f 7665 6420 4f4f 5020 6465  r beloved OOP de
+00002a60: 7369 676e 2e0a 2a20 2a2a 4a53 4f4e 2073  sign..* **JSON s
+00002a70: 6572 6961 6c69 7a61 7469 6f6e 2f64 6573  erialization/des
+00002a80: 6572 6961 6c69 7a61 7469 6f6e 2a2a 3a20  erialization**: 
+00002a90: 426f 7468 2055 4a53 4f4e 2061 6e64 204f  Both UJSON and O
+00002aa0: 524a 4f4e 2073 7570 706f 7274 2e0a 2a20  RJON support..* 
+00002ab0: 2a2a 4c69 6665 7370 616e 2a2a 3a20 5375  **Lifespan**: Su
+00002ac0: 7070 6f72 7420 666f 7220 7468 6520 6e65  pport for the ne
+00002ad0: 776c 7920 6c69 6665 7370 616e 2061 6e64  wly lifespan and
+00002ae0: 206f 6e5f 7374 6172 742f 6f6e 5f73 6875   on_start/on_shu
+00002af0: 7464 6f77 6e20 6576 656e 7473 2e0a 2a20  tdown events..* 
+00002b00: 2a2a 5363 6865 6475 6c65 722a 2a3a 2059  **Scheduler**: Y
+00002b10: 6573 2c20 7468 6174 2773 2072 6967 6874  es, that's right
+00002b20: 2c20 6974 2063 6f6d 6573 2077 6974 6820  , it comes with 
+00002b30: 6120 7363 6865 6475 6c65 7220 666f 7220  a scheduler for 
+00002b40: 7468 6f73 6520 6175 746f 6d61 7465 6420  those automated 
+00002b50: 7461 736b 732e 0a2a 202a 2a44 6570 656e  tasks..* **Depen
+00002b60: 6465 6e63 7920 496e 6a65 6374 696f 6e2a  dency Injection*
+00002b70: 2a3a 204c 696b 6520 616e 7920 6f74 6865  *: Like any othe
+00002b80: 7220 6772 6561 7420 6672 616d 6577 6f72  r great framewor
+00002b90: 6b20 6f75 7420 7468 6572 652e 0a2a 202a  k out there..* *
+00002ba0: 2a53 696d 706c 6963 6974 7920 6672 6f6d  *Simplicity from
+00002bb0: 2073 6574 7469 6e67 732a 2a3a 2059 6573   settings**: Yes
+00002bc0: 2c20 7765 2068 6176 6520 6120 7761 7920  , we have a way 
+00002bd0: 746f 206d 616b 6520 7468 6520 636f 6465  to make the code
+00002be0: 2065 7665 6e20 636c 6561 6e65 7220 6279   even cleaner by
+00002bf0: 2069 6e74 726f 6475 6369 6e67 2073 6574   introducing set
+00002c00: 7469 6e67 730a 6261 7365 6420 7379 7374  tings.based syst
+00002c10: 656d 732e 0a2a 202a 2a6d 7367 7370 6563  ems..* **msgspec
+00002c20: 2a2a 202d 2053 7570 706f 7274 2066 6f72  ** - Support for
+00002c30: 2060 6d73 6773 7065 6360 2e0a 0a23 2320   `msgspec`...## 
+00002c40: 5265 6c61 7469 6f6e 2074 6f20 5374 6172  Relation to Star
+00002c50: 6c65 7474 6520 616e 6420 6f74 6865 7220  lette and other 
+00002c60: 6672 616d 6577 6f72 6b73 0a0a 4573 6d65  frameworks..Esme
+00002c70: 7261 6c64 2075 7365 7320 5374 6172 6c65  rald uses Starle
+00002c80: 7474 6520 756e 6465 7220 7468 6520 686f  tte under the ho
+00002c90: 6f64 2e20 5468 6520 7265 6173 6f6e 2062  od. The reason b
+00002ca0: 6568 696e 6420 7468 6973 2064 6563 6973  ehind this decis
+00002cb0: 6f6e 2063 6f6d 6573 2077 6974 6820 7468  on comes with th
+00002cc0: 6520 6661 6374 2074 6861 7420 7065 7266  e fact that perf
+00002cd0: 6f72 6d61 6e63 6520 6973 2074 6865 7265  ormance is there
+00002ce0: 0a61 6e64 206e 6f20 6973 7375 6573 2077  .and no issues w
+00002cf0: 6974 6820 726f 7574 696e 672e 0a0a 4f6e  ith routing...On
+00002d00: 6365 2074 6865 2061 7070 6c69 6361 7469  ce the applicati
+00002d10: 6f6e 2069 7320 7570 2c20 616c 6c20 7468  on is up, all th
+00002d20: 6520 726f 7574 6573 2061 7265 206d 6f75  e routes are mou
+00002d30: 6e74 6564 2061 6e64 2074 6865 7265 666f  nted and therefo
+00002d40: 7265 2074 6865 2075 726c 2070 6174 6873  re the url paths
+00002d50: 2061 7265 2064 6566 696e 6564 2e0a 4573   are defined..Es
+00002d60: 6d65 7261 6c64 2065 6e63 6f75 7261 6765  merald encourage
+00002d70: 7320 7374 616e 6461 7264 2070 7261 6374  s standard pract
+00002d80: 6963 6573 2061 6e64 2064 6573 6967 6e20  ices and design 
+00002d90: 696e 206d 696e 6420 7768 6963 6820 6d65  in mind which me
+00002da0: 616e 7320 7468 6174 2061 6e79 2061 7070  ans that any app
+00002db0: 6c69 6361 7469 6f6e 2c20 6269 6720 6f72  lication, big or
+00002dc0: 2073 6d61 6c6c 2c0a 6375 7374 6f6d 206f   small,.custom o
+00002dd0: 7220 656e 7465 7270 7269 7365 2c20 6669  r enterprise, fi
+00002de0: 7473 2077 6974 6869 6e20 4573 6d65 7261  ts within Esmera
+00002df0: 6c64 2065 636f 7379 7374 656d 2077 6974  ld ecosystem wit
+00002e00: 686f 7574 2073 6361 6c61 6269 6c69 7479  hout scalability
+00002e10: 2069 7373 7565 732e 0a0a 2323 2053 6574   issues...## Set
+00002e20: 7469 6e67 730a 0a4c 696b 6520 6576 6572  tings..Like ever
+00002e30: 7920 6f74 6865 7220 6672 616d 6577 6f72  y other framewor
+00002e40: 6b2c 2077 6865 6e20 7374 6172 7469 6e67  k, when starting
+00002e50: 2061 6e20 6170 706c 6963 6174 696f 6e2c   an application,
+00002e60: 2061 206c 6f74 206f 6620 5b73 6574 7469   a lot of [setti
+00002e70: 6e67 735d 282e 2f61 7070 6c69 6361 7469  ngs](./applicati
+00002e80: 6f6e 2f73 6574 7469 6e67 732e 6d64 2920  on/settings.md) 
+00002e90: 6361 6e2f 6e65 6564 2074 6f20 6265 0a70  can/need to be.p
+00002ea0: 6173 7365 6420 746f 2074 6865 206d 6169  assed to the mai
+00002eb0: 6e20 6f62 6a65 6374 2061 6e64 2074 6869  n object and thi
+00002ec0: 7320 6361 6e20 6265 2076 6572 7920 6461  s can be very da
+00002ed0: 7574 696e 6720 616e 6420 7567 6c79 2074  uting and ugly t
+00002ee0: 6f20 6d61 696e 7461 696e 2061 6e64 2073  o maintain and s
+00002ef0: 6565 2e0a 0a45 736d 6572 616c 6420 636f  ee...Esmerald co
+00002f00: 6d65 7320 7769 7468 2074 6865 0a5b 7365  mes with the.[se
+00002f10: 7474 696e 6773 5d28 2e2f 6170 706c 6963  ttings](./applic
+00002f20: 6174 696f 6e2f 7365 7474 696e 6773 2e6d  ation/settings.m
+00002f30: 6429 2069 6e20 6d69 6e64 2e20 4120 7365  d) in mind. A se
+00002f40: 7420 6f66 2064 6566 6175 6c74 7320 7468  t of defaults th
+00002f50: 6174 2063 616e 2062 6520 6f76 6572 7269  at can be overri
+00002f60: 6464 656e 2062 7920 796f 7572 2076 6572  dden by your ver
+00002f70: 7920 6f77 6e20 7365 7474 696e 6773 0a6d  y own settings.m
+00002f80: 6f64 756c 6520 6275 7420 6e6f 7420 6c69  odule but not li
+00002f90: 6d69 7465 6420 746f 2069 742c 2061 7320  mited to it, as 
+00002fa0: 796f 7520 6361 6e20 7374 696c 6c20 7573  you can still us
+00002fb0: 6520 7468 6520 636c 6173 7369 6320 6170  e the classic ap
+00002fc0: 7072 6f61 6368 206f 6620 7061 7373 696e  proach of passin
+00002fd0: 6720 6576 6572 7974 6869 6e67 2069 6e74  g everything int
+00002fe0: 6f20 610a 4573 6d65 7261 6c64 2069 6e73  o a.Esmerald ins
+00002ff0: 7461 6e63 6520 6469 7265 6374 6c79 2077  tance directly w
+00003000: 6865 6e20 696e 7374 616e 7469 6174 696e  hen instantiatin
+00003010: 672e 0a0a 2a2a 4578 616d 706c 6520 6f66  g...**Example of
+00003020: 2063 6c61 7373 6963 2061 7070 726f 6163   classic approac
+00003030: 682a 2a3a 0a0a 6060 6070 7974 686f 6e0a  h**:..```python.
+00003040: 6672 6f6d 2065 7861 6d70 6c65 2069 6d70  from example imp
+00003050: 6f72 7420 4578 616d 706c 654f 626a 6563  ort ExampleObjec
+00003060: 740a 0a23 2045 7861 6d70 6c65 4f62 6a65  t..# ExampleObje
+00003070: 6374 2069 7320 616e 2069 6e73 7461 6e63  ct is an instanc
+00003080: 6520 6f66 2061 6e6f 7468 6572 2061 7070  e of another app
+00003090: 6c69 6361 7469 6f6e 0a23 2061 6e64 2069  lication.# and i
+000030a0: 7420 7365 7276 6573 206f 6e6c 7920 666f  t serves only fo
+000030b0: 7220 6578 616d 706c 650a 0a61 7070 203d  r example..app =
+000030c0: 2045 7861 6d70 6c65 4f62 6a65 6374 2873   ExampleObject(s
+000030d0: 6574 7469 6e67 5f6f 6e65 3d2e 2e2e 2c20  etting_one=..., 
+000030e0: 7365 7474 696e 675f 7477 6f3d 2e2e 2e2c  setting_two=...,
+000030f0: 2073 6574 7469 6e67 5f74 6872 6565 3d2e   setting_three=.
+00003100: 2e2e 290a 0a60 6060 0a0a 496e 7370 6972  ..)..```..Inspir
+00003110: 6564 2062 7920 7468 6520 6772 6561 7420  ed by the great 
+00003120: 5b44 6a61 6e67 6f5d 2868 7474 7073 3a2f  [Django](https:/
+00003130: 2f77 7777 2e64 6a61 6e67 6f70 726f 6a65  /www.djangoproje
+00003140: 6374 2e63 6f6d 2f29 2061 6e64 2075 7369  ct.com/) and usi
+00003150: 6e67 2070 7964 616e 7469 632c 2045 736d  ng pydantic, Esm
+00003160: 6572 616c 6420 6861 7320 6120 6465 6661  erald has a defa
+00003170: 756c 7420 6f62 6a65 6374 0a72 6561 6479  ult object.ready
+00003180: 2074 6f20 6265 2075 7365 6420 6f75 742d   to be used out-
+00003190: 6f66 2d74 6865 2d62 6f78 2e0a 0a2a 2a45  of-the-box...**E
+000031a0: 736d 6572 616c 642a 2a3a 0a0a 6060 6070  smerald**:..```p
+000031b0: 7974 686f 6e0a 6672 6f6d 2065 736d 6572  ython.from esmer
+000031c0: 616c 6420 696d 706f 7274 2045 736d 6572  ald import Esmer
+000031d0: 616c 640a 0a61 7070 203d 2045 736d 6572  ald..app = Esmer
+000031e0: 616c 6428 290a 0a60 6060 0a0a 416e 6420  ald()..```..And 
+000031f0: 7468 6174 2773 2069 7421 2041 6c6c 2074  that's it! All t
+00003200: 6865 2064 6566 6175 6c74 2073 6574 7469  he default setti
+00003210: 6e67 7320 6172 6520 6c6f 6164 6564 2120  ngs are loaded! 
+00003220: 5468 6973 2069 7320 7369 6d70 6c65 206f  This is simple o
+00003230: 6620 636f 7572 7365 2062 7574 2063 616e  f course but can
+00003240: 2079 6f75 206f 7665 7272 6964 650a 696e   you override.in
+00003250: 7369 6465 2074 6865 206f 626a 6563 7420  side the object 
+00003260: 6173 2077 656c 6c3f 2059 6573 210a 0a60  as well? Yes!..`
+00003270: 6060 7079 7468 6f6e 0a66 726f 6d20 6573  ``python.from es
+00003280: 6d65 7261 6c64 2069 6d70 6f72 7420 4573  merald import Es
+00003290: 6d65 7261 6c64 0a0a 6170 7020 3d20 4573  merald..app = Es
+000032a0: 6d65 7261 6c64 2861 7070 5f6e 616d 653d  merald(app_name=
+000032b0: 274d 7920 4170 7027 2c20 7469 746c 653d  'My App', title=
+000032c0: 274d 7920 7469 746c 6527 290a 0a60 6060  'My title')..```
+000032d0: 0a0a 5361 6d65 2061 7320 7468 6520 636c  ..Same as the cl
+000032e0: 6173 7369 6373 2e0a 0a53 6f20 686f 7720  assics...So how 
+000032f0: 646f 6573 2045 736d 6572 616c 6420 6b6e  does Esmerald kn
+00003300: 6f77 2061 626f 7574 2074 6865 2064 6566  ow about the def
+00003310: 6175 6c74 2073 6574 7469 6e67 733f 2045  ault settings? E
+00003320: 6e74 6572 7320 5b45 736d 6572 616c 6420  nters [Esmerald 
+00003330: 7365 7474 696e 6773 206d 6f64 756c 655d  settings module]
+00003340: 2823 6573 6d65 7261 6c64 2d73 6574 7469  (#esmerald-setti
+00003350: 6e67 732d 6d6f 6475 6c65 292e 0a0a 2323  ngs-module)...##
+00003360: 2320 4573 6d65 7261 6c64 2053 6574 7469  # Esmerald Setti
+00003370: 6e67 7320 4d6f 6475 6c65 0a0a 5468 6973  ngs Module..This
+00003380: 2069 7320 7468 6520 7761 7920 4573 6d65   is the way Esme
+00003390: 7261 6c64 2064 6566 6175 6c74 7320 7468  rald defaults th
+000033a0: 6520 7661 6c75 6573 2e20 5768 656e 2073  e values. When s
+000033b0: 7461 7274 696e 6720 616e 2061 7070 6c69  tarting an appli
+000033c0: 6361 7469 6f6e 2c20 7468 6520 7379 7374  cation, the syst
+000033d0: 656d 206c 6f6f 6b73 2066 6f72 2061 0a60  em looks for a.`
+000033e0: 4553 4d45 5241 4c44 5f53 4554 5449 4e47  ESMERALD_SETTING
+000033f0: 535f 4d4f 4455 4c45 6020 656e 7669 726f  S_MODULE` enviro
+00003400: 6e6d 656e 7420 7661 7269 6162 6c65 2e20  nment variable. 
+00003410: 4966 206e 6f20 7661 7269 6162 6c65 2069  If no variable i
+00003420: 7320 7375 7070 6c69 6564 2074 6865 6e20  s supplied then 
+00003430: 7468 6520 7379 7374 656d 2077 696c 6c20  the system will 
+00003440: 6465 6661 756c 7420 746f 0a60 4573 6d65  default to.`Esme
+00003450: 7261 6c64 4150 4953 6574 7469 6e67 7360  raldAPISettings`
+00003460: 2073 6574 7469 6e67 7320 616e 6420 7374   settings and st
+00003470: 6172 742e 0a0a 2323 2320 4375 7374 6f6d  art...### Custom
+00003480: 2053 6574 7469 6e67 730a 0a53 6570 6172   Settings..Separ
+00003490: 6174 696f 6e20 6f66 2073 6574 7469 6e67  ation of setting
+000034a0: 7320 6279 2065 6e76 6972 6f6d 6d65 6e74  s by enviromment
+000034b0: 2069 7320 6120 6d75 7374 2068 6176 6520   is a must have 
+000034c0: 7468 6573 6520 6461 7973 2061 6e64 2073  these days and s
+000034d0: 7461 7274 696e 6720 7769 7468 2064 6566  tarting with def
+000034e0: 6175 6c74 206f 6620 4573 6d65 7261 6c64  ault of Esmerald
+000034f0: 2077 696c 6c20 6e6f 7420 6265 0a65 6e6f   will not be.eno
+00003500: 7567 6820 666f 7220 616e 7920 6170 706c  ugh for any appl
+00003510: 6963 6174 696f 6e2e 0a0a 5468 6520 7365  ication...The se
+00003520: 7474 696e 6773 2061 7265 2070 7964 616e  ttings are pydan
+00003530: 7469 6320 7374 616e 6461 7264 2073 6574  tic standard set
+00003540: 7469 6e67 7320 616e 6420 7468 6572 6566  tings and theref
+00003550: 6f72 6520 636f 6d70 6174 6962 6c65 2077  ore compatible w
+00003560: 6974 6820 4573 6d65 7261 6c64 2e0a 5468  ith Esmerald..Th
+00003570: 6520 7379 7374 656d 2062 7269 6e67 7320  e system brings 
+00003580: 736f 6d65 2064 6566 6175 6c74 7320 7468  some defaults th
+00003590: 6174 2063 616e 2062 6520 7573 6564 206f  at can be used o
+000035a0: 7574 2d6f 662d 7468 652d 626f 7820 6275  ut-of-the-box bu
+000035b0: 7420 6974 2773 206e 6f74 206d 616e 6461  t it's not manda
+000035c0: 746f 7279 2074 6f20 6265 2075 7365 642e  tory to be used.
+000035d0: 0a54 6865 2065 6e76 6972 6f6e 6d65 6e74  .The environment
+000035e0: 2064 6566 6175 6c74 7320 746f 202a 2a70   defaults to **p
+000035f0: 726f 6475 6374 696f 6e2a 2a2e 0a0a 6060  roduction**...``
+00003600: 6070 7974 686f 6e0a 0a66 726f 6d20 6573  `python..from es
+00003610: 6d65 7261 6c64 2069 6d70 6f72 7420 4573  merald import Es
+00003620: 6d65 7261 6c64 4150 4953 6574 7469 6e67  meraldAPISetting
+00003630: 730a 6672 6f6d 2065 736d 6572 616c 642e  s.from esmerald.
+00003640: 636f 6e66 2e65 6e75 6d73 2069 6d70 6f72  conf.enums impor
+00003650: 7420 456e 7669 726f 6e6d 656e 7454 7970  t EnvironmentTyp
+00003660: 650a 0a63 6c61 7373 2044 6576 656c 6f70  e..class Develop
+00003670: 6d65 6e74 2845 736d 6572 616c 6441 5049  ment(EsmeraldAPI
+00003680: 5365 7474 696e 6773 293a 0a20 2020 2061  Settings):.    a
+00003690: 7070 5f6e 616d 653a 2073 7472 203d 2027  pp_name: str = '
+000036a0: 4d79 2061 7070 2069 6e20 6465 7627 0a20  My app in dev'. 
+000036b0: 2020 2065 6e76 6972 6f6e 6d65 6e74 3a20     environment: 
+000036c0: 7374 7220 3d20 456e 7669 726f 6e6d 656e  str = Environmen
+000036d0: 7454 7970 652e 4445 5645 4c4f 504d 454e  tType.DEVELOPMEN
+000036e0: 540a 0a60 6060 0a0a 2a2a 4c6f 6164 2074  T..```..**Load t
+000036f0: 6865 2073 6574 7469 6e67 7320 696e 746f  he settings into
+00003700: 2079 6f75 7220 4573 6d65 7261 6c64 2061   your Esmerald a
+00003710: 7070 6c69 6361 7469 6f6e 2a2a 3a0a 0a41  pplication**:..A
+00003720: 7373 756d 696e 6720 796f 7572 2045 736d  ssuming your Esm
+00003730: 6572 616c 6420 6170 7020 6973 2069 6e73  erald app is ins
+00003740: 6964 6520 616e 2060 7372 632f 6170 702e  ide an `src/app.
+00003750: 7079 602e 0a0a 6060 6063 6f6e 736f 6c65  py`...```console
+00003760: 0a0a 4553 4d45 5241 4c44 5f53 4554 5449  ..ESMERALD_SETTI
+00003770: 4e47 535f 4d4f 4455 4c45 3d27 6d79 6170  NGS_MODULE='myap
+00003780: 702e 7365 7474 696e 6773 2e44 6576 656c  p.settings.Devel
+00003790: 6f70 6d65 6e74 2720 7079 7468 6f6e 202d  opment' python -
+000037a0: 6d20 7372 632e 6170 702e 7079 0a0a 6060  m src.app.py..``
+000037b0: 600a 0a23 2320 4761 7465 7761 792c 2057  `..## Gateway, W
+000037c0: 6562 536f 636b 6574 4761 7465 7761 7920  ebSocketGateway 
+000037d0: 616e 6420 496e 636c 7564 650a 0a53 7461  and Include..Sta
+000037e0: 726c 6574 7465 206f 6666 6572 7320 7468  rlette offers th
+000037f0: 6520 526f 7574 6520 636c 6173 7365 7320  e Route classes 
+00003800: 666f 7220 7369 6d70 6c65 2070 6174 6820  for simple path 
+00003810: 6173 7369 676e 6d65 6e74 7320 6275 7420  assignments but 
+00003820: 7468 6973 2069 7320 616c 736f 2076 6572  this is also ver
+00003830: 7920 6c69 6d69 7469 6e67 2069 6620 736f  y limiting if so
+00003840: 6d65 7468 696e 6720 6d6f 7265 0a63 6f6d  mething more.com
+00003850: 706c 6578 2069 6e20 6d69 6e64 2e20 4573  plex in mind. Es
+00003860: 6d65 7261 6c64 2065 7874 656e 6473 2074  merald extends t
+00003870: 6861 7420 6675 6e63 7469 6f6e 616c 6974  hat functionalit
+00003880: 7920 616e 6420 6164 6473 2073 6f6d 6520  y and adds some 
+00003890: 6066 6c61 6972 6020 616e 6420 6c65 7665  `flair` and leve
+000038a0: 6c73 2075 7020 6279 2068 6176 696e 6720  ls up by having 
+000038b0: 7468 650a 4761 7465 7761 792c 2057 6562  the.Gateway, Web
+000038c0: 536f 636b 6574 4761 7465 7761 7920 616e  SocketGateway an
+000038d0: 6420 496e 636c 7564 652e 0a0a 5468 6f73  d Include...Thos
+000038e0: 6520 6172 6520 7370 6563 6961 6c20 6f62  e are special ob
+000038f0: 6a65 6374 7320 7468 6174 2061 6c6c 6f77  jects that allow
+00003900: 2061 6c6c 2074 6865 206d 6167 6963 206f   all the magic o
+00003910: 6620 4573 6d65 7261 6c64 2074 6f20 6861  f Esmerald to ha
+00003920: 7070 656e 2e0a 0a46 6f72 2061 2063 6c61  ppen...For a cla
+00003930: 7373 6963 2c20 6469 7265 6374 2c20 6f6e  ssic, direct, on
+00003940: 6520 6669 6c65 2073 696e 676c 6520 6170  e file single ap
+00003950: 7072 6f61 6368 2e0a 0a2a 2a49 6e20 6120  proach...**In a 
+00003960: 6e75 7473 6865 6c6c 2a2a 3a0a 0a60 6060  nutshell**:..```
+00003970: 7079 7468 6f6e 2074 6974 6c65 3d27 7372  python title='sr
+00003980: 632f 6170 702e 7079 270a 6672 6f6d 2065  c/app.py'.from e
+00003990: 736d 6572 616c 6420 696d 706f 7274 2045  smerald import E
+000039a0: 736d 6572 616c 642c 2067 6574 2c20 7374  smerald, get, st
+000039b0: 6174 7573 2c20 5265 7175 6573 742c 2055  atus, Request, U
+000039c0: 4a53 4f4e 5265 7370 6f6e 7365 2c20 4761  JSONResponse, Ga
+000039d0: 7465 7761 792c 2057 6562 536f 636b 6574  teway, WebSocket
+000039e0: 4761 7465 7761 792c 2057 6562 736f 636b  Gateway, Websock
+000039f0: 6574 0a0a 4067 6574 2873 7461 7475 735f  et..@get(status_
+00003a00: 636f 6465 3d73 7461 7475 732e 4854 5450  code=status.HTTP
+00003a10: 5f32 3030 5f4f 4b29 0a61 7379 6e63 2064  _200_OK).async d
+00003a20: 6566 2068 6f6d 6528 2920 2d3e 2055 4a53  ef home() -> UJS
+00003a30: 4f4e 5265 7370 6f6e 7365 3a0a 2020 2020  ONResponse:.    
+00003a40: 7265 7475 726e 2055 4a53 4f4e 5265 7370  return UJSONResp
+00003a50: 6f6e 7365 287b 0a20 2020 2020 2020 2022  onse({.        "
+00003a60: 6465 7461 696c 223a 2022 4865 6c6c 6f20  detail": "Hello 
+00003a70: 776f 726c 6422 0a20 2020 207d 290a 0a0a  world".    })...
+00003a80: 4067 6574 2829 0a61 7379 6e63 2064 6566  @get().async def
+00003a90: 2061 6e6f 7468 6572 2872 6571 7565 7374   another(request
+00003aa0: 3a20 5265 7175 6573 7429 202d 3e20 6469  : Request) -> di
+00003ab0: 6374 3a0a 2020 2020 7265 7475 726e 207b  ct:.    return {
+00003ac0: 0a20 2020 2020 2020 2022 6465 7461 696c  .        "detail
+00003ad0: 223a 2022 416e 6f74 6865 7220 776f 726c  ": "Another worl
+00003ae0: 6421 220a 2020 2020 7d0a 0a40 7765 6273  d!".    }..@webs
+00003af0: 6f63 6b65 7428 7061 7468 3d22 2f7b 7061  ocket(path="/{pa
+00003b00: 7468 5f70 6172 616d 3a73 7472 7d22 290a  th_param:str}").
+00003b10: 6173 796e 6320 6465 6620 776f 726c 645f  async def world_
+00003b20: 736f 636b 6574 2873 6f63 6b65 743a 2057  socket(socket: W
+00003b30: 6562 736f 636b 6574 2920 2d3e 204e 6f6e  ebsocket) -> Non
+00003b40: 653a 0a20 2020 2061 7761 6974 2073 6f63  e:.    await soc
+00003b50: 6b65 742e 6163 6365 7074 2829 0a20 2020  ket.accept().   
+00003b60: 206d 7367 203d 2061 7761 6974 2073 6f63   msg = await soc
+00003b70: 6b65 742e 7265 6365 6976 655f 6a73 6f6e  ket.receive_json
+00003b80: 2829 0a20 2020 2061 7373 6572 7420 6d73  ().    assert ms
+00003b90: 670a 2020 2020 6173 7365 7274 2073 6f63  g.    assert soc
+00003ba0: 6b65 740a 2020 2020 6177 6169 7420 736f  ket.    await so
+00003bb0: 636b 6574 2e63 6c6f 7365 2829 0a0a 0a61  cket.close()...a
+00003bc0: 7070 203d 2045 736d 6572 616c 6428 726f  pp = Esmerald(ro
+00003bd0: 7574 6573 3d5b 0a20 2020 2047 6174 6577  utes=[.    Gatew
+00003be0: 6179 2868 616e 646c 6572 3d68 6f6d 6529  ay(handler=home)
+00003bf0: 2c0a 2020 2020 4761 7465 7761 7928 6861  ,.    Gateway(ha
+00003c00: 6e64 6c65 723d 616e 6f74 6865 7229 2c0a  ndler=another),.
+00003c10: 2020 2020 5765 6253 6f63 6b65 7447 6174      WebSocketGat
+00003c20: 6577 6179 2868 616e 646c 6572 3d77 6f72  eway(handler=wor
+00003c30: 6c64 5f73 6f63 6b65 7429 2c0a 5d29 0a0a  ld_socket),.])..
+00003c40: 6060 600a 0a23 2320 4465 7369 676e 2069  ```..## Design i
+00003c50: 6e20 6d69 6e64 0a0a 476f 6f64 2064 6573  n mind..Good des
+00003c60: 6967 6e20 6973 2061 6c77 6179 7320 656e  ign is always en
+00003c70: 636f 7572 6167 6564 2061 6e64 2045 736d  couraged and Esm
+00003c80: 6572 616c 6420 616c 6c6f 7773 2063 6f6d  erald allows com
+00003c90: 706c 6578 2072 6f75 7469 6e67 206f 6e20  plex routing on 
+00003ca0: 616e 7920 6c65 7665 6c2e 0a0a 2323 2320  any level...### 
+00003cb0: 5468 6520 6861 6e64 6c65 7273 2028 7669  The handlers (vi
+00003cc0: 6577 7329 0a0a 6060 6070 7974 686f 6e20  ews)..```python 
+00003cd0: 7469 746c 653d 226d 7961 7070 2f61 6363  title="myapp/acc
+00003ce0: 6f75 6e74 732f 7669 6577 732e 7079 220a  ounts/views.py".
+00003cf0: 6672 6f6d 2065 736d 6572 616c 6420 696d  from esmerald im
+00003d00: 706f 7274 2067 6574 2c20 706f 7374 2c20  port get, post, 
+00003d10: 7075 742c 2073 7461 7475 732c 2077 6562  put, status, web
+00003d20: 736f 636b 6574 2c20 4150 4956 6965 772c  socket, APIView,
+00003d30: 2052 6571 7565 7374 2c20 4a53 4f4e 5265   Request, JSONRe
+00003d40: 7370 6f6e 7365 2c20 5265 7370 6f6e 7365  sponse, Response
+00003d50: 2c20 5765 6253 6f63 6b65 740a 6672 6f6d  , WebSocket.from
+00003d60: 2070 7964 616e 7469 6320 696d 706f 7274   pydantic import
+00003d70: 2042 6173 654d 6f64 656c 0a0a 0a63 6c61   BaseModel...cla
+00003d80: 7373 2050 726f 6475 6374 2842 6173 654d  ss Product(BaseM
+00003d90: 6f64 656c 293a 0a20 2020 206e 616d 653a  odel):.    name:
+00003da0: 2073 7472 0a20 2020 2073 6b75 3a20 7374   str.    sku: st
+00003db0: 720a 2020 2020 7072 6963 653a 2066 6c6f  r.    price: flo
+00003dc0: 6174 0a0a 0a40 7075 7428 272f 7072 6f64  at...@put('/prod
+00003dd0: 7563 742f 7b70 726f 6475 6374 5f69 647d  uct/{product_id}
+00003de0: 2729 0a64 6566 2075 7064 6174 655f 7072  ').def update_pr
+00003df0: 6f64 7563 7428 7072 6f64 7563 745f 6964  oduct(product_id
+00003e00: 3a20 696e 742c 2064 6174 613a 2050 726f  : int, data: Pro
+00003e10: 6475 6374 2920 2d3e 2064 6963 743a 0a20  duct) -> dict:. 
+00003e20: 2020 2072 6574 7572 6e20 7b22 7072 6f64     return {"prod
+00003e30: 7563 745f 6964 223a 2070 726f 6475 6374  uct_id": product
+00003e40: 5f69 642c 2022 7072 6f64 7563 745f 6e61  _id, "product_na
+00003e50: 6d65 223a 2070 726f 6475 6374 2e6e 616d  me": product.nam
+00003e60: 6520 7d0a 0a0a 4067 6574 2873 7461 7475  e }...@get(statu
+00003e70: 735f 636f 6465 3d73 7461 7475 732e 4854  s_code=status.HT
+00003e80: 5450 5f32 3030 5f4f 4b29 0a61 7379 6e63  TP_200_OK).async
+00003e90: 2064 6566 2068 6f6d 6528 2920 2d3e 204a   def home() -> J
+00003ea0: 534f 4e52 6573 706f 6e73 653a 0a20 2020  SONResponse:.   
+00003eb0: 2072 6574 7572 6e20 4a53 4f4e 5265 7370   return JSONResp
+00003ec0: 6f6e 7365 287b 0a20 2020 2020 2020 2022  onse({.        "
+00003ed0: 6465 7461 696c 223a 2022 4865 6c6c 6f20  detail": "Hello 
+00003ee0: 776f 726c 6422 0a20 2020 207d 290a 0a0a  world".    })...
+00003ef0: 4067 6574 2829 0a61 7379 6e63 2064 6566  @get().async def
+00003f00: 2061 6e6f 7468 6572 2872 6571 7565 7374   another(request
+00003f10: 3a20 5265 7175 6573 7429 202d 3e20 6469  : Request) -> di
+00003f20: 6374 3a0a 2020 2020 7265 7475 726e 207b  ct:.    return {
+00003f30: 0a20 2020 2020 2020 2022 6465 7461 696c  .        "detail
+00003f40: 223a 2022 416e 6f74 6865 7220 776f 726c  ": "Another worl
+00003f50: 6421 220a 2020 2020 7d0a 0a0a 4077 6562  d!".    }...@web
+00003f60: 736f 636b 6574 2870 6174 683d 222f 7b70  socket(path="/{p
+00003f70: 6174 685f 7061 7261 6d3a 7374 727d 2229  ath_param:str}")
+00003f80: 0a61 7379 6e63 2064 6566 2077 6f72 6c64  .async def world
+00003f90: 5f73 6f63 6b65 7428 736f 636b 6574 3a20  _socket(socket: 
+00003fa0: 5765 6273 6f63 6b65 7429 202d 3e20 4e6f  Websocket) -> No
+00003fb0: 6e65 3a0a 2020 2020 6177 6169 7420 736f  ne:.    await so
+00003fc0: 636b 6574 2e61 6363 6570 7428 290a 2020  cket.accept().  
+00003fd0: 2020 6d73 6720 3d20 6177 6169 7420 736f    msg = await so
+00003fe0: 636b 6574 2e72 6563 6569 7665 5f6a 736f  cket.receive_jso
+00003ff0: 6e28 290a 2020 2020 6173 7365 7274 206d  n().    assert m
+00004000: 7367 0a20 2020 2061 7373 6572 7420 736f  sg.    assert so
+00004010: 636b 6574 0a20 2020 2061 7761 6974 2073  cket.    await s
+00004020: 6f63 6b65 742e 636c 6f73 6528 290a 0a0a  ocket.close()...
+00004030: 636c 6173 7320 576f 726c 6428 4150 4956  class World(APIV
+00004040: 6965 7729 3a0a 0a20 2020 2040 6765 7428  iew):..    @get(
+00004050: 7061 7468 3d27 2f7b 7572 6c7d 2729 0a20  path='/{url}'). 
+00004060: 2020 2061 7379 6e63 2064 6566 2068 6f6d     async def hom
+00004070: 6528 7265 7175 6573 743a 2052 6571 7565  e(request: Reque
+00004080: 7374 2c20 7572 6c3a 2073 7472 2920 2d3e  st, url: str) ->
+00004090: 2052 6573 706f 6e73 653a 0a20 2020 2020   Response:.     
+000040a0: 2020 2072 6574 7572 6e20 5265 7370 6f6e     return Respon
+000040b0: 7365 2866 2255 524c 3a20 7b75 726c 7d22  se(f"URL: {url}"
+000040c0: 290a 0a20 2020 2040 706f 7374 2870 6174  )..    @post(pat
+000040d0: 683d 272f 7b75 726c 7d27 2c20 7374 6174  h='/{url}', stat
+000040e0: 7573 5f63 6f64 653d 7374 6174 7573 2e48  us_code=status.H
+000040f0: 5454 505f 3230 315f 4352 4541 5445 4429  TTP_201_CREATED)
+00004100: 0a20 2020 2061 7379 6e63 2064 6566 206d  .    async def m
+00004110: 6172 7328 7265 7175 6573 743a 2052 6571  ars(request: Req
+00004120: 7565 7374 2c20 7572 6c3a 2073 7472 2920  uest, url: str) 
+00004130: 2d3e 204a 534f 4e52 6573 706f 6e73 653a  -> JSONResponse:
+00004140: 0a20 2020 2020 2020 202e 2e2e 0a0a 2020  .        .....  
+00004150: 2020 4077 6562 736f 636b 6574 2870 6174    @websocket(pat
+00004160: 683d 222f 7b70 6174 685f 7061 7261 6d3a  h="/{path_param:
+00004170: 7374 727d 2229 0a20 2020 2061 7379 6e63  str}").    async
+00004180: 2064 6566 2070 6c75 746f 2873 656c 662c   def pluto(self,
+00004190: 2073 6f63 6b65 743a 2057 6562 736f 636b   socket: Websock
+000041a0: 6574 2920 2d3e 204e 6f6e 653a 0a20 2020  et) -> None:.   
+000041b0: 2020 2020 2061 7761 6974 2073 6f63 6b65       await socke
+000041c0: 742e 6163 6365 7074 2829 0a20 2020 2020  t.accept().     
+000041d0: 2020 206d 7367 203d 2061 7761 6974 2073     msg = await s
+000041e0: 6f63 6b65 742e 7265 6365 6976 655f 6a73  ocket.receive_js
+000041f0: 6f6e 2829 0a20 2020 2020 2020 2061 7373  on().        ass
+00004200: 6572 7420 6d73 670a 2020 2020 2020 2020  ert msg.        
+00004210: 6173 7365 7274 2073 6f63 6b65 740a 2020  assert socket.  
+00004220: 2020 2020 2020 6177 6169 7420 736f 636b        await sock
+00004230: 6574 2e63 6c6f 7365 2829 0a0a 0a60 6060  et.close()...```
+00004240: 0a0a 4966 2061 2060 7061 7468 6020 6973  ..If a `path` is
+00004250: 206e 6f74 2070 726f 7669 6465 642c 2064   not provided, d
+00004260: 6566 6175 6c74 7320 746f 2060 2f60 2e0a  efaults to `/`..
+00004270: 0a23 2323 2054 6865 2067 6174 6577 6179  .### The gateway
+00004280: 7320 2875 726c 7329 0a0a 6060 6070 7974  s (urls)..```pyt
+00004290: 686f 6e20 7469 746c 653d 226d 7961 7070  hon title="myapp
+000042a0: 2f61 6363 6f75 6e74 732f 7572 6c73 2e70  /accounts/urls.p
+000042b0: 7922 0a66 726f 6d20 6573 6d65 7261 6c64  y".from esmerald
+000042c0: 2069 6d70 6f72 7420 4761 7465 7761 792c   import Gateway,
+000042d0: 2057 6562 536f 636b 6574 4761 7465 7761   WebSocketGatewa
+000042e0: 790a 6672 6f6d 202e 7669 6577 7320 696d  y.from .views im
+000042f0: 706f 7274 2068 6f6d 652c 2061 6e6f 7468  port home, anoth
+00004300: 6572 2c20 776f 726c 645f 736f 636b 6574  er, world_socket
+00004310: 2c20 576f 726c 640a 0a72 6f75 7465 5f70  , World..route_p
+00004320: 6174 7465 726e 7320 3d20 5b0a 2020 2020  atterns = [.    
+00004330: 4761 7465 7761 7928 6861 6e64 6c65 723d  Gateway(handler=
+00004340: 7570 6461 7465 5f70 726f 6475 6374 292c  update_product),
+00004350: 0a20 2020 2047 6174 6577 6179 2868 616e  .    Gateway(han
+00004360: 646c 6572 3d68 6f6d 6529 2c0a 2020 2020  dler=home),.    
+00004370: 4761 7465 7761 7928 6861 6e64 6c65 723d  Gateway(handler=
+00004380: 616e 6f74 6865 7229 2c0a 2020 2020 4761  another),.    Ga
+00004390: 7465 7761 7928 6861 6e64 6c65 723d 576f  teway(handler=Wo
+000043a0: 726c 6429 2c0a 2020 2020 5765 6253 6f63  rld),.    WebSoc
+000043b0: 6b65 7447 6174 6577 6179 2868 616e 646c  ketGateway(handl
+000043c0: 6572 3d77 6f72 6c64 5f73 6f63 6b65 7429  er=world_socket)
+000043d0: 2c0a 5d0a 0a60 6060 0a0a 4966 2061 2060  ,.]..```..If a `
+000043e0: 7061 7468 6020 6973 206e 6f74 2070 726f  path` is not pro
+000043f0: 7669 6465 642c 2064 6566 6175 6c74 7320  vided, defaults 
+00004400: 746f 2060 2f60 2e0a 0a23 2323 2054 6865  to `/`...### The
+00004410: 2049 6e63 6c75 6465 0a0a 5468 6973 2069   Include..This i
+00004420: 7320 6120 7665 7279 2073 7065 6369 616c  s a very special
+00004430: 206f 626a 6563 7420 7468 6174 2061 6c6c   object that all
+00004440: 6f77 7320 7468 6520 696d 706f 7274 206f  ows the import o
+00004450: 6620 616e 7920 726f 7574 6520 6672 6f6d  f any route from
+00004460: 2061 6e79 7768 6572 6520 696e 2074 6865   anywhere in the
+00004470: 2061 7070 6c69 6361 7469 6f6e 2e0a 0a60   application...`
+00004480: 496e 636c 7564 6560 2061 6363 6570 7473  Include` accepts
+00004490: 2074 6865 2069 6d70 6f72 7420 7669 6120   the import via 
+000044a0: 606e 616d 6573 7061 6365 6020 6f72 2076  `namespace` or v
+000044b0: 6961 2060 726f 7574 6573 6020 6c69 7374  ia `routes` list
+000044c0: 2062 7574 206e 6f74 2062 6f74 682e 0a0a   but not both...
+000044d0: 5768 656e 2075 7369 6e67 2061 2060 6e61  When using a `na
+000044e0: 6d65 7370 6163 6560 2c20 7468 6520 6049  mespace`, the `I
+000044f0: 6e63 6c75 6465 6020 7769 6c6c 206c 6f6f  nclude` will loo
+00004500: 6b20 666f 7220 7468 6520 6465 6661 756c  k for the defaul
+00004510: 7420 6072 6f75 7465 5f70 6174 7465 726e  t `route_pattern
+00004520: 7360 206f 626a 6563 7420 6c69 7374 2069  s` object list i
+00004530: 6e20 7468 6520 696d 706f 7274 6564 0a6e  n the imported.n
+00004540: 616d 6573 7061 6365 2075 6e6c 6573 7320  amespace unless 
+00004550: 6120 6469 6666 6572 656e 7420 6070 6174  a different `pat
+00004560: 7465 726e 6020 6973 2073 7065 6369 6669  tern` is specifi
+00004570: 6564 2e0a 0a54 6865 2070 6174 7465 726e  ed...The pattern
+00004580: 206f 6e6c 7920 776f 726b 7320 6966 2074   only works if t
+00004590: 6865 2069 6d70 6f72 7473 2061 7265 2064  he imports are d
+000045a0: 6f6e 6520 7669 6120 606e 616d 6573 7061  one via `namespa
+000045b0: 6365 6020 616e 6420 6e6f 7420 7669 6120  ce` and not via 
+000045c0: 6072 6f75 7465 7360 2e0a 0a2a 2a49 6d70  `routes`...**Imp
+000045d0: 6f72 7469 6e67 2075 7369 6e67 206e 616d  orting using nam
+000045e0: 6573 7061 6365 2a2a 3a0a 0a60 6060 7079  espace**:..```py
+000045f0: 7468 6f6e 2074 6974 6c65 3d27 6d79 6170  thon title='myap
+00004600: 702f 7572 6c73 2e70 7927 0a66 726f 6d20  p/urls.py'.from 
+00004610: 6573 6d65 7261 6c64 2069 6d70 6f72 7420  esmerald import 
+00004620: 496e 636c 7564 650a 0a72 6f75 7465 5f70  Include..route_p
+00004630: 6174 7465 726e 7320 3d20 5b0a 2020 2020  atterns = [.    
+00004640: 496e 636c 7564 6528 6e61 6d65 7370 6163  Include(namespac
+00004650: 653d 276d 7961 7070 2e61 6363 6f75 6e74  e='myapp.account
+00004660: 732e 7572 6c73 2729 0a5d 0a0a 6060 600a  s.urls').]..```.
+00004670: 0a2a 2a49 6d70 6f72 7469 6e67 2075 7369  .**Importing usi
+00004680: 6e67 2072 6f75 7465 732a 2a3a 0a0a 6060  ng routes**:..``
+00004690: 6070 7974 686f 6e20 7469 746c 653d 2773  `python title='s
+000046a0: 7263 2f6d 7961 7070 2f75 726c 732e 7079  rc/myapp/urls.py
+000046b0: 270a 6672 6f6d 2065 736d 6572 616c 6420  '.from esmerald 
+000046c0: 696d 706f 7274 2049 6e63 6c75 6465 0a66  import Include.f
+000046d0: 726f 6d20 6d79 6170 702e 6163 636f 756e  rom myapp.accoun
+000046e0: 7473 2069 6d70 6f72 7420 7572 6c73 0a0a  ts import urls..
+000046f0: 726f 7574 655f 7061 7474 6572 6e73 203d  route_patterns =
+00004700: 205b 0a20 2020 2049 6e63 6c75 6465 2872   [.    Include(r
+00004710: 6f75 7465 733d 7572 6c73 2e72 6f75 7465  outes=urls.route
+00004720: 5f70 6174 7465 726e 7329 0a5d 0a0a 6060  _patterns).]..``
+00004730: 600a 0a49 6620 6120 6070 6174 6860 2069  `..If a `path` i
+00004740: 7320 6e6f 7420 7072 6f76 6964 6564 2c20  s not provided, 
+00004750: 6465 6661 756c 7473 2074 6f20 602f 602e  defaults to `/`.
+00004760: 0a0a 2323 2323 2055 7369 6e67 2061 2064  ..#### Using a d
+00004770: 6966 6665 7265 6e74 2070 6174 7465 726e  ifferent pattern
+00004780: 0a0a 6060 6070 7974 686f 6e20 7469 746c  ..```python titl
+00004790: 653d 2273 7263 2f6d 7961 7070 2f61 6363  e="src/myapp/acc
+000047a0: 6f75 6e74 732f 7572 6c73 2e70 7922 0a66  ounts/urls.py".f
+000047b0: 726f 6d20 6573 6d65 7261 6c64 2069 6d70  rom esmerald imp
+000047c0: 6f72 7420 4761 7465 7761 792c 2057 6562  ort Gateway, Web
+000047d0: 536f 636b 6574 4761 7465 7761 790a 6672  SocketGateway.fr
+000047e0: 6f6d 202e 7669 6577 7320 696d 706f 7274  om .views import
+000047f0: 2068 6f6d 652c 2061 6e6f 7468 6572 2c20   home, another, 
+00004800: 776f 726c 645f 736f 636b 6574 2c20 576f  world_socket, Wo
+00004810: 726c 640a 0a6d 795f 7572 6c73 203d 205b  rld..my_urls = [
+00004820: 0a20 2020 2047 6174 6577 6179 2868 616e  .    Gateway(han
+00004830: 646c 6572 3d75 7064 6174 655f 7072 6f64  dler=update_prod
+00004840: 7563 7429 2c0a 2020 2020 4761 7465 7761  uct),.    Gatewa
+00004850: 7928 6861 6e64 6c65 723d 686f 6d65 292c  y(handler=home),
+00004860: 0a20 2020 2047 6174 6577 6179 2868 616e  .    Gateway(han
+00004870: 646c 6572 3d61 6e6f 7468 6572 292c 0a20  dler=another),. 
+00004880: 2020 2047 6174 6577 6179 2868 616e 646c     Gateway(handl
+00004890: 6572 3d57 6f72 6c64 292c 0a20 2020 2057  er=World),.    W
+000048a0: 6562 536f 636b 6574 4761 7465 7761 7928  ebSocketGateway(
+000048b0: 6861 6e64 6c65 723d 776f 726c 645f 736f  handler=world_so
+000048c0: 636b 6574 292c 0a5d 0a0a 6060 600a 0a2a  cket),.]..```..*
+000048d0: 2a49 6d70 6f72 7469 6e67 2075 7369 6e67  *Importing using
+000048e0: 206e 616d 6573 7061 6365 2a2a 3a0a 0a60   namespace**:..`
+000048f0: 6060 7079 7468 6f6e 2074 6974 6c65 3d27  ``python title='
+00004900: 7372 632f 6d79 6170 702f 7572 6c73 2e70  src/myapp/urls.p
+00004910: 7927 0a66 726f 6d20 6573 6d65 7261 6c64  y'.from esmerald
+00004920: 2069 6d70 6f72 7420 496e 636c 7564 650a   import Include.
+00004930: 0a72 6f75 7465 5f70 6174 7465 726e 7320  .route_patterns 
+00004940: 3d20 5b0a 2020 2020 496e 636c 7564 6528  = [.    Include(
+00004950: 6e61 6d65 7370 6163 653d 276d 7961 7070  namespace='myapp
+00004960: 2e61 6363 6f75 6e74 732e 7572 6c73 272c  .accounts.urls',
+00004970: 2070 6174 7465 726e 3d27 6d79 5f75 726c   pattern='my_url
+00004980: 7327 290a 5d0a 0a60 6060 0a0a 2323 2049  s').]..```..## I
+00004990: 6e63 6c75 6465 2061 6e64 2045 736d 6572  nclude and Esmer
+000049a0: 616c 640a 0a54 6865 2060 496e 636c 7564  ald..The `Includ
+000049b0: 6560 2063 616e 2062 6520 7665 7279 2068  e` can be very h
+000049c0: 656c 7066 756c 206d 6f73 746c 7920 7768  elpful mostly wh
+000049d0: 656e 2074 6865 2067 6f61 6c20 6973 2074  en the goal is t
+000049e0: 6f20 6176 6f69 6420 6120 6c6f 7420 6f66  o avoid a lot of
+000049f0: 2069 6d70 6f72 7473 2061 6e64 206d 6173   imports and mas
+00004a00: 7369 7665 206c 6973 740a 6f66 206f 626a  sive list.of obj
+00004a10: 6563 7473 2074 6f20 6265 2070 6173 7365  ects to be passe
+00004a20: 6420 696e 746f 206f 6e65 2073 696e 676c  d into one singl
+00004a30: 6520 6f62 6a65 6374 2e20 5468 6973 2063  e object. This c
+00004a40: 616e 2062 6520 7061 7274 6963 756c 6172  an be particular
+00004a50: 7920 7573 6566 756c 2074 6f20 6d61 6b65  y useful to make
+00004a60: 2061 2045 736d 6572 616c 6420 696e 7374   a Esmerald inst
+00004a70: 616e 6365 2e0a 0a2a 2a45 7861 6d70 6c65  ance...**Example
+00004a80: 2a2a 3a0a 0a60 6060 7079 7468 6f6e 2074  **:..```python t
+00004a90: 6974 6c65 3d27 7372 632f 7572 6c73 2e70  itle='src/urls.p
+00004aa0: 7927 0a66 726f 6d20 6573 6d65 7261 6c64  y'.from esmerald
+00004ab0: 2069 6d70 6f72 7420 496e 636c 7564 650a   import Include.
+00004ac0: 0a72 6f75 7465 5f70 6174 7465 726e 7320  .route_patterns 
+00004ad0: 3d20 5b0a 2020 2020 496e 636c 7564 6528  = [.    Include(
+00004ae0: 6e61 6d65 7370 6163 653d 276d 7961 7070  namespace='myapp
+00004af0: 2e61 6363 6f75 6e74 732e 7572 6c73 272c  .accounts.urls',
+00004b00: 2070 6174 7465 726e 3d27 6d79 5f75 726c   pattern='my_url
+00004b10: 7327 290a 5d0a 0a60 6060 0a0a 6060 6070  s').]..```..```p
+00004b20: 7974 686f 6e20 7469 746c 653d 2773 7263  ython title='src
+00004b30: 2f61 7070 2e70 7927 0a66 726f 6d20 6573  /app.py'.from es
+00004b40: 6d65 7261 6c64 2069 6d70 6f72 7420 4573  merald import Es
+00004b50: 6d65 7261 6c64 2c20 496e 636c 7564 650a  merald, Include.
+00004b60: 0a61 7070 203d 2045 736d 6572 616c 6428  .app = Esmerald(
+00004b70: 726f 7574 6573 3d5b 496e 636c 7564 6528  routes=[Include(
+00004b80: 2773 7263 2e75 726c 7327 295d 290a 0a60  'src.urls')])..`
+00004b90: 6060 0a0a 2323 2052 756e 2074 6865 2061  ``..## Run the a
+00004ba0: 7070 6c69 6361 7469 6f6e 0a0a 4173 206d  pplication..As m
+00004bb0: 656e 7469 6f6e 6564 2062 6566 6f72 652c  entioned before,
+00004bc0: 2077 6520 7265 636f 6d6d 656e 6420 7576   we recommend uv
+00004bd0: 6963 6f72 6e20 666f 7220 7072 6f64 7563  icorn for produc
+00004be0: 7469 6f6e 2062 7574 2069 7427 7320 6e6f  tion but it's no
+00004bf0: 7420 6d61 6e64 6174 6f72 792e 0a0a 2a2a  t mandatory...**
+00004c00: 5573 696e 6720 7576 6963 6f72 6e2a 2a3a  Using uvicorn**:
+00004c10: 0a0a 6060 6073 6865 6c6c 0a75 7669 636f  ..```shell.uvico
+00004c20: 726e 2073 7263 3a61 7070 202d 2d72 656c  rn src:app --rel
+00004c30: 6f61 640a 0a49 4e46 4f3a 2020 2020 2055  oad..INFO:     U
+00004c40: 7669 636f 726e 2072 756e 6e69 6e67 206f  vicorn running o
+00004c50: 6e20 6874 7470 3a2f 2f31 3237 2e30 2e30  n http://127.0.0
+00004c60: 2e31 3a38 3030 3020 2850 7265 7373 2043  .1:8000 (Press C
+00004c70: 5452 4c2b 4320 746f 2071 7569 7429 0a49  TRL+C to quit).I
+00004c80: 4e46 4f3a 2020 2020 2053 7461 7274 6564  NFO:     Started
+00004c90: 2072 656c 6f61 6465 7220 7072 6f63 6573   reloader proces
+00004ca0: 7320 5b32 3837 3230 5d0a 494e 464f 3a20  s [28720].INFO: 
+00004cb0: 2020 2020 5374 6172 7465 6420 7365 7276      Started serv
+00004cc0: 6572 2070 726f 6365 7373 205b 3238 3732  er process [2872
+00004cd0: 325d 0a49 4e46 4f3a 2020 2020 2057 6169  2].INFO:     Wai
+00004ce0: 7469 6e67 2066 6f72 2061 7070 6c69 6361  ting for applica
+00004cf0: 7469 6f6e 2073 7461 7274 7570 2e0a 494e  tion startup..IN
+00004d00: 464f 3a20 2020 2020 4170 706c 6963 6174  FO:     Applicat
+00004d10: 696f 6e20 7374 6172 7475 7020 636f 6d70  ion startup comp
+00004d20: 6c65 7465 2e0a 6060 600a 0a23 2320 5275  lete..```..## Ru
+00004d30: 6e20 7468 6520 6170 706c 6963 6174 696f  n the applicatio
+00004d40: 6e20 7769 7468 2063 7573 746f 6d20 7365  n with custom se
+00004d50: 7474 696e 6773 0a0a 2a2a 5573 696e 6720  ttings..**Using 
+00004d60: 7576 6963 6f72 6e2a 2a3a 0a0a 6060 6073  uvicorn**:..```s
+00004d70: 6865 6c6c 0a45 534d 4552 414c 445f 5345  hell.ESMERALD_SE
+00004d80: 5454 494e 4753 5f4d 4f44 554c 453d 6d79  TTINGS_MODULE=my
+00004d90: 6170 702e 4170 7053 6574 7469 6e67 7320  app.AppSettings 
+00004da0: 7576 6963 6f72 6e20 7372 633a 6170 7020  uvicorn src:app 
+00004db0: 2d2d 7265 6c6f 6164 0a0a 494e 464f 3a20  --reload..INFO: 
+00004dc0: 2020 2020 5576 6963 6f72 6e20 7275 6e6e      Uvicorn runn
+00004dd0: 696e 6720 6f6e 2068 7474 703a 2f2f 3132  ing on http://12
+00004de0: 372e 302e 302e 313a 3830 3030 2028 5072  7.0.0.1:8000 (Pr
+00004df0: 6573 7320 4354 524c 2b43 2074 6f20 7175  ess CTRL+C to qu
+00004e00: 6974 290a 494e 464f 3a20 2020 2020 5374  it).INFO:     St
+00004e10: 6172 7465 6420 7265 6c6f 6164 6572 2070  arted reloader p
+00004e20: 726f 6365 7373 205b 3238 3732 305d 0a49  rocess [28720].I
+00004e30: 4e46 4f3a 2020 2020 2053 7461 7274 6564  NFO:     Started
+00004e40: 2073 6572 7665 7220 7072 6f63 6573 7320   server process 
+00004e50: 5b32 3837 3232 5d0a 494e 464f 3a20 2020  [28722].INFO:   
+00004e60: 2020 5761 6974 696e 6720 666f 7220 6170    Waiting for ap
+00004e70: 706c 6963 6174 696f 6e20 7374 6172 7475  plication startu
+00004e80: 702e 0a49 4e46 4f3a 2020 2020 2041 7070  p..INFO:     App
+00004e90: 6c69 6361 7469 6f6e 2073 7461 7274 7570  lication startup
+00004ea0: 2063 6f6d 706c 6574 652e 0a60 6060 0a0a   complete..```..
+00004eb0: 2323 204f 7065 6e41 5049 2064 6f63 756d  ## OpenAPI docum
+00004ec0: 656e 7461 7469 6f6e 0a0a 4573 6d65 7261  entation..Esmera
+00004ed0: 6c64 2061 6c73 6f20 636f 6d65 7320 7769  ld also comes wi
+00004ee0: 7468 204f 7065 6e41 5049 2064 6f63 7320  th OpenAPI docs 
+00004ef0: 696e 7465 6772 6174 6564 2e20 466f 7220  integrated. For 
+00004f00: 7468 6f73 6520 7573 6564 2074 6f20 7468  those used to th
+00004f10: 6174 2c20 7468 6973 2069 7320 726f 7567  at, this is roug
+00004f20: 686c 7920 7468 6520 7361 6d65 2061 6e64  hly the same and
+00004f30: 2074 6f20 6d61 6b65 2069 740a 6861 7070   to make it.happ
+00004f40: 656e 2c20 7468 6572 6520 7765 7265 2069  en, there were i
+00004f50: 6e73 7069 7261 7469 6f6e 7320 7468 6174  nspirations that
+00004f60: 2068 656c 7065 6420 4573 6d65 7261 6c64   helped Esmerald
+00004f70: 2067 6574 7469 6e67 2074 6865 7265 2066   getting there f
+00004f80: 6173 742e 0a0a 4573 6d65 7261 6c64 2073  ast...Esmerald s
+00004f90: 7461 7274 7320 6175 746f 6d61 7469 6361  tarts automatica
+00004fa0: 6c6c 7920 7468 6520 4f70 656e 4150 4920  lly the OpenAPI 
+00004fb0: 646f 6375 6d65 6e74 6174 696f 6e20 6279  documentation by
+00004fc0: 2069 6e6a 6563 7469 6e67 2074 6865 204f   injecting the O
+00004fd0: 7065 6e41 5049 436f 6e66 6967 2064 6566  penAPIConfig def
+00004fe0: 6175 6c74 2066 726f 6d0a 7468 6520 7365  ault from.the se
+00004ff0: 7474 696e 6773 2061 6e64 206d 616b 6573  ttings and makes
+00005000: 2053 7761 6767 6572 2c20 5265 446f 6320   Swagger, ReDoc 
+00005010: 616e 2053 746f 706c 6967 6874 2065 6c65  an Stoplight ele
+00005020: 6d65 6e74 7320 6176 6169 6c61 626c 6520  ments available 
+00005030: 746f 2079 6f75 206f 7574 206f 6620 7468  to you out of th
+00005040: 6520 626f 782e 0a0a 546f 2061 6363 6573  e box...To acces
+00005050: 7320 7468 6520 4f70 656e 4150 492c 2073  s the OpenAPI, s
+00005060: 696d 706c 7920 7374 6172 7420 796f 7572  imply start your
+00005070: 206c 6f63 616c 2064 6576 656c 6f70 6d65   local developme
+00005080: 6e74 2061 6e64 2061 6363 6573 733a 0a0a  nt and access:..
+00005090: 2a20 2a2a 5377 6167 6765 722a 2a20 2d20  * **Swagger** - 
+000050a0: 602f 646f 6373 2f73 7761 6767 6572 602e  `/docs/swagger`.
+000050b0: 0a2a 202a 2a52 6564 6f63 2a2a 202d 2060  .* **Redoc** - `
+000050c0: 2f64 6f63 732f 7265 646f 6360 2e0a 2a20  /docs/redoc`..* 
+000050d0: 2a2a 5374 6f70 6c69 6768 7420 456c 656d  **Stoplight Elem
+000050e0: 656e 7473 2a2a 202d 2060 2f64 6f63 732f  ents** - `/docs/
+000050f0: 656c 656d 656e 7473 602e 0a0a 5468 6572  elements`...Ther
+00005100: 6520 6172 6520 6d6f 7265 2064 6574 6169  e are more detai
+00005110: 6c73 2061 626f 7574 205b 686f 7720 746f  ls about [how to
+00005120: 2063 6f6e 6669 6775 7265 2074 6865 204f   configure the O
+00005130: 7065 6e41 5049 436f 6e66 6967 5d28 6874  penAPIConfig](ht
+00005140: 7470 733a 2f2f 6573 6d65 7261 6c64 2e64  tps://esmerald.d
+00005150: 6576 2f63 6f6e 6669 6775 7261 7469 6f6e  ev/configuration
+00005160: 732f 6f70 656e 6170 692f 636f 6e66 6967  s/openapi/config
+00005170: 290a 7769 7468 696e 2074 6865 2064 6f63  ).within the doc
+00005180: 756d 656e 7461 7469 6f6e 2e0a 0a54 6865  umentation...The
+00005190: 7265 2069 7320 616c 736f 2061 2067 6f6f  re is also a goo
+000051a0: 6420 6578 706c 616e 6174 696f 6e20 6f6e  d explanation on
+000051b0: 2068 6f77 2074 6f20 7573 6520 7468 6520   how to use the 
+000051c0: 5b4f 7065 6e41 5049 5265 7370 6f6e 7365  [OpenAPIResponse
+000051d0: 5d28 6874 7470 733a 2f2f 6573 6d65 7261  ](https://esmera
+000051e0: 6c64 2e64 6576 2f72 6573 706f 6e73 6573  ld.dev/responses
+000051f0: 236f 7065 6e61 7069 2d72 6573 706f 6e73  #openapi-respons
+00005200: 6573 290a 6173 2077 656c 6c2e 0a0a 2323  es).as well...##
+00005210: 204e 6f74 6573 0a0a 5468 6973 2069 7320   Notes..This is 
+00005220: 6a75 7374 2061 2076 6572 7920 6869 6768  just a very high
+00005230: 2d6c 6576 656c 2064 656d 6f6e 7374 7261  -level demonstra
+00005240: 7469 6f6e 206f 6620 686f 7720 746f 2073  tion of how to s
+00005250: 7461 7274 2071 7569 636b 6c79 2061 6e64  tart quickly and
+00005260: 2077 6861 7420 4573 6d65 7261 6c64 2063   what Esmerald c
+00005270: 616e 2064 6f2e 0a54 6865 7265 2061 7265  an do..There are
+00005280: 2070 6c65 6e74 7920 6d6f 7265 2074 6869   plenty more thi
+00005290: 6e67 7320 796f 7520 6361 6e20 646f 2077  ngs you can do w
+000052a0: 6974 6820 4573 6d65 7261 6c64 2e20 456e  ith Esmerald. En
+000052b0: 6a6f 7921 20f0 9f98 8a0a 0a23 2320 5370  joy! ......## Sp
+000052c0: 6f6e 736f 7273 0a0a 4375 7272 656e 746c  onsors..Currentl
+000052d0: 7920 7468 6572 6520 6172 6520 6e6f 2073  y there are no s
+000052e0: 706f 6e73 6f72 7320 6f66 2045 736d 6572  ponsors of Esmer
+000052f0: 616c 6420 6275 7420 796f 7520 6361 6e20  ald but you can 
+00005300: 6669 6e61 6e63 6961 6c6c 7920 6865 6c70  financially help
+00005310: 2061 6e64 2073 7570 706f 7274 2074 6865   and support the
+00005320: 2061 7574 686f 7220 7468 6f75 6768 0a5b   author though.[
+00005330: 4769 7448 7562 2073 706f 6e73 6f72 735d  GitHub sponsors]
+00005340: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00005350: 636f 6d2f 7370 6f6e 736f 7273 2f74 6172  com/sponsors/tar
+00005360: 7369 6c29 2061 6e64 2062 6563 6f6d 6520  sil) and become 
+00005370: 6120 2a2a 5370 6563 6961 6c20 6f6e 652a  a **Special one*
+00005380: 2a20 6f72 2061 202a 2a4c 6567 656e 642a  * or a **Legend*
+00005390: 2a2e 0a0a 5b73 6166 6669 6572 5f6f 726d  *...[saffier_orm
+000053a0: 5d3a 2068 7474 7073 3a2f 2f65 736d 6572  ]: https://esmer
+000053b0: 616c 642e 6465 762f 6461 7461 6261 7365  ald.dev/database
+000053c0: 732f 7361 6666 6965 722f 6d6f 7469 7661  s/saffier/motiva
+000053d0: 7469 6f6e 0a5b 6564 6779 5f6f 726d 5d3a  tion.[edgy_orm]:
+000053e0: 2068 7474 7073 3a2f 2f65 736d 6572 616c   https://esmeral
+000053f0: 642e 6465 762f 6461 7461 6261 7365 732f  d.dev/databases/
+00005400: 7361 6666 6965 722f 6d6f 7469 7661 7469  saffier/motivati
+00005410: 6f6e 0a5b 6d6f 6e67 6f7a 5f6f 646d 5d3a  on.[mongoz_odm]:
+00005420: 2068 7474 7073 3a2f 2f65 736d 6572 616c   https://esmeral
+00005430: 642e 6465 762f 6461 7461 6261 7365 732f  d.dev/databases/
+00005440: 6d6f 6e67 6f7a 2f6d 6f74 6976 6174 696f  mongoz/motivatio
+00005450: 6e0a                                     n.
```

