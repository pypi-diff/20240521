# Comparing `tmp/linked_services-1.2.2.tar.gz` & `tmp/linked_services-1.2.3.tar.gz`

## Comparing `linked_services-1.2.2.tar` & `linked_services-1.2.3.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 linked_services-1.2.2/.coveragerc
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 linked_services-1.2.2/.flake8
--rw-r--r--   0        0        0    23011 2020-02-02 00:00:00.000000 linked_services-1.2.2/conftest.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 linked_services-1.2.2/mkdocs.yml
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 linked_services-1.2.2/.github/workflows/workflow.yml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 linked_services-1.2.2/.vscode/settings.json
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/index.md
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/css/custom.css
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/extending-scope/rest-frameworks.md
--rw-r--r--   0        0        0    16120 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/extending-service/http-clients.md
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/extending-service/rest-frameworks.md
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/getting-started/installation.md
--rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/getting-started/scopes.md
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/getting-started/services.md
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/getting-started/set-up.md
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 linked_services-1.2.2/docs/getting-started/views.md
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/manage.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/__about__.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/admin.py
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/apps.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/models.py
--rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/settings.py
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/actions.py
--rw-r--r--   0        0        0    14688 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/decorators.py
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/exceptions.py
--rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/i18n.py
--rw-r--r--   0        0        0    28163 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/service.py
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/settings.py
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/shorteners.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/core/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/__init__.py
--rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/actions.py
--rw-r--r--   0        0        0     2668 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/admin.py
--rw-r--r--   0        0        0    14519 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/models.py
--rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/receivers.py
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/service.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/signals.py
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/tasks.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/django/urls.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/management/commands/__init__.py
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/management/commands/first_party_webhooks.py
--rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/management/commands/get_first_party_ids.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/management/commands/sign_jwt.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/management/commands/sign_request.py
--rw-r--r--   0        0        0    13691 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/migrations/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/rest_framework/__init__.py
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/rest_framework/decorators.py
--rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/rest_framework/types.py
--rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/rest_framework/views.py
--rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templates/app-not-found.html
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templates/authorize.html
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templates/button.html
--rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templates/scopes.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templatetags/__init__.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templatetags/button.py
--rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 linked_services-1.2.2/src/linked_services/templatetags/scopes.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/__init__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/__init__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/actions/__init__.py
--rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/actions/test_acreate_user.py
--rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/actions/test_aget_user.py
--rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/actions/test_create_user.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/actions/test_get_user.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/tasks/__init__.py
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/tasks/test_check_credentials.py
--rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/tasks/test_first_party_webhooks.py
--rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/django/tasks/test_import_external_user.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/management/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/management/commands/__init__.py
--rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/management/commands/test_sign_jwt.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/management/commands/test_sign_request.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/rest_framework/__init__.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/rest_framework/views/__init__.py
--rw-r--r--   0        0        0    20163 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/rest_framework/views/test_authorize_view.py
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/__init__.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/argument_parser.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/create_models.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/exceptions.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/get_list.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/is_valid.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 linked_services-1.2.2/tests/utils/just_one.py
--rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 linked_services-1.2.2/.gitignore
--rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 linked_services-1.2.2/LICENSE.txt
--rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 linked_services-1.2.2/README.md
--rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 linked_services-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 linked_services-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 linked_services-1.2.3/.coveragerc
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 linked_services-1.2.3/.flake8
+-rw-r--r--   0        0        0    23011 2020-02-02 00:00:00.000000 linked_services-1.2.3/conftest.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 linked_services-1.2.3/mkdocs.yml
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 linked_services-1.2.3/.github/workflows/workflow.yml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 linked_services-1.2.3/.vscode/settings.json
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 linked_services-1.2.3/docs/index.md
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 linked_services-1.2.3/docs/css/custom.css
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 linked_services-1.2.3/docs/extending-scope/rest-frameworks.md
+-rw-r--r--   0        0        0    16120 2020-02-02 00:00:00.000000 linked_services-1.2.3/docs/extending-service/http-clients.md
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 linked_services-1.2.3/docs/extending-service/rest-frameworks.md
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 linked_services-1.2.3/docs/getting-started/installation.md
+-rw-r--r--   0        0        0     4739 2020-02-02 00:00:00.000000 linked_services-1.2.3/docs/getting-started/scopes.md
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 linked_services-1.2.3/docs/getting-started/services.md
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 linked_services-1.2.3/docs/getting-started/set-up.md
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 linked_services-1.2.3/docs/getting-started/views.md
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/manage.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/__about__.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/admin.py
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/apps.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/models.py
+-rw-r--r--   0        0        0     1985 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/settings.py
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/core/actions.py
+-rw-r--r--   0        0        0    14688 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/core/decorators.py
+-rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/core/exceptions.py
+-rw-r--r--   0        0        0     3133 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/core/i18n.py
+-rw-r--r--   0        0        0    28163 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/core/service.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/core/settings.py
+-rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/core/shorteners.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/core/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/django/__init__.py
+-rw-r--r--   0        0        0    12955 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/django/actions.py
+-rw-r--r--   0        0        0     2667 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/django/admin.py
+-rw-r--r--   0        0        0    14519 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/django/models.py
+-rw-r--r--   0        0        0     1479 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/django/receivers.py
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/django/service.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/django/signals.py
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/django/tasks.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/django/urls.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/management/commands/__init__.py
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/management/commands/first_party_webhooks.py
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/management/commands/get_first_party_ids.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/management/commands/sign_jwt.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/management/commands/sign_request.py
+-rw-r--r--   0        0        0    13691 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/migrations/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/rest_framework/__init__.py
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/rest_framework/decorators.py
+-rw-r--r--   0        0        0     1403 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/rest_framework/types.py
+-rw-r--r--   0        0        0     7899 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/rest_framework/views.py
+-rw-r--r--   0        0        0     1273 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/templates/app-not-found.html
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/templates/authorize.html
+-rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/templates/button.html
+-rw-r--r--   0        0        0     2441 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/templates/scopes.html
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/templatetags/__init__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/templatetags/button.py
+-rw-r--r--   0        0        0      688 2020-02-02 00:00:00.000000 linked_services-1.2.3/src/linked_services/templatetags/scopes.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/django/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/django/actions/__init__.py
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/django/actions/test_acreate_user.py
+-rw-r--r--   0        0        0     1805 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/django/actions/test_aget_user.py
+-rw-r--r--   0        0        0     3310 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/django/actions/test_create_user.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/django/actions/test_get_user.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/django/tasks/__init__.py
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/django/tasks/test_check_credentials.py
+-rw-r--r--   0        0        0     3781 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/django/tasks/test_first_party_webhooks.py
+-rw-r--r--   0        0        0     2897 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/django/tasks/test_import_external_user.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/management/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/management/commands/__init__.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/management/commands/test_sign_jwt.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/management/commands/test_sign_request.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/rest_framework/__init__.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/rest_framework/views/__init__.py
+-rw-r--r--   0        0        0    20163 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/rest_framework/views/test_authorize_view.py
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/utils/__init__.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/utils/argument_parser.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/utils/create_models.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/utils/exceptions.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/utils/get_list.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/utils/is_valid.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 linked_services-1.2.3/tests/utils/just_one.py
+-rw-r--r--   0        0        0     3267 2020-02-02 00:00:00.000000 linked_services-1.2.3/.gitignore
+-rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 linked_services-1.2.3/LICENSE.txt
+-rw-r--r--   0        0        0     1397 2020-02-02 00:00:00.000000 linked_services-1.2.3/README.md
+-rw-r--r--   0        0        0     3718 2020-02-02 00:00:00.000000 linked_services-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 linked_services-1.2.3/PKG-INFO
```

### Comparing `linked_services-1.2.2/conftest.py` & `linked_services-1.2.3/conftest.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/mkdocs.yml` & `linked_services-1.2.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/.github/workflows/workflow.yml` & `linked_services-1.2.3/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/docs/extending-scope/rest-frameworks.md` & `linked_services-1.2.3/docs/extending-scope/rest-frameworks.md`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/docs/extending-service/http-clients.md` & `linked_services-1.2.3/docs/extending-service/http-clients.md`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/docs/extending-service/rest-frameworks.md` & `linked_services-1.2.3/docs/extending-service/rest-frameworks.md`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/docs/getting-started/scopes.md` & `linked_services-1.2.3/docs/getting-started/scopes.md`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/docs/getting-started/services.md` & `linked_services-1.2.3/docs/getting-started/services.md`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/docs/getting-started/set-up.md` & `linked_services-1.2.3/docs/getting-started/set-up.md`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/docs/getting-started/views.md` & `linked_services-1.2.3/docs/getting-started/views.md`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/manage.py` & `linked_services-1.2.3/src/manage.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/settings.py` & `linked_services-1.2.3/src/linked_services/settings.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/core/actions.py` & `linked_services-1.2.3/src/linked_services/core/actions.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/core/decorators.py` & `linked_services-1.2.3/src/linked_services/core/decorators.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/core/exceptions.py` & `linked_services-1.2.3/src/linked_services/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/core/i18n.py` & `linked_services-1.2.3/src/linked_services/core/i18n.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/core/service.py` & `linked_services-1.2.3/src/linked_services/core/service.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/core/settings.py` & `linked_services-1.2.3/src/linked_services/core/settings.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/django/actions.py` & `linked_services-1.2.3/src/linked_services/django/actions.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/django/admin.py` & `linked_services-1.2.3/src/linked_services/django/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
     actions = []
 
 
 @admin.register(FirstPartyWebhookLog)
 class FirstPartyWebhookLogAdmin(admin.ModelAdmin):
     list_display = ("id", "app", "type", "user_id", "external_id", "url", "processed", "attempts", "status")
     search_fields = ["user_id", "external_id", "url", "app__name", "app__slug"]
-    list_filter = ["app", "admin", "processed", "status"]
+    list_filter = ["app", "type", "processed", "status"]
     actions = []
 
 
 @admin.register(FirstPartyCredentials)
 class FirstPartyCredentialsAdmin(admin.ModelAdmin):
     list_display = ("id", "user", "app")
     search_fields = ["user__username", "user__email", "user__first_name", "user__last_name", "app__name", "app__slug"]
```

### Comparing `linked_services-1.2.2/src/linked_services/django/models.py` & `linked_services-1.2.3/src/linked_services/django/models.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/django/receivers.py` & `linked_services-1.2.3/src/linked_services/django/receivers.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/django/service.py` & `linked_services-1.2.3/src/linked_services/django/service.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/django/tasks.py` & `linked_services-1.2.3/src/linked_services/django/tasks.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/management/commands/first_party_webhooks.py` & `linked_services-1.2.3/src/linked_services/management/commands/first_party_webhooks.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/management/commands/get_first_party_ids.py` & `linked_services-1.2.3/src/linked_services/management/commands/get_first_party_ids.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/management/commands/sign_jwt.py` & `linked_services-1.2.3/src/linked_services/management/commands/sign_jwt.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/management/commands/sign_request.py` & `linked_services-1.2.3/src/linked_services/management/commands/sign_request.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/migrations/0001_initial.py` & `linked_services-1.2.3/src/linked_services/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/rest_framework/types.py` & `linked_services-1.2.3/src/linked_services/rest_framework/types.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/rest_framework/views.py` & `linked_services-1.2.3/src/linked_services/rest_framework/views.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/templates/app-not-found.html` & `linked_services-1.2.3/src/linked_services/templates/app-not-found.html`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/templates/authorize.html` & `linked_services-1.2.3/src/linked_services/templates/authorize.html`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/templates/scopes.html` & `linked_services-1.2.3/src/linked_services/templates/scopes.html`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/src/linked_services/templatetags/scopes.py` & `linked_services-1.2.3/src/linked_services/templatetags/scopes.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/tests/django/actions/test_acreate_user.py` & `linked_services-1.2.3/tests/django/actions/test_acreate_user.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/tests/django/actions/test_aget_user.py` & `linked_services-1.2.3/tests/django/actions/test_aget_user.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/tests/django/actions/test_create_user.py` & `linked_services-1.2.3/tests/django/actions/test_create_user.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/tests/django/actions/test_get_user.py` & `linked_services-1.2.3/tests/django/actions/test_get_user.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/tests/django/tasks/test_check_credentials.py` & `linked_services-1.2.3/tests/django/tasks/test_check_credentials.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/tests/django/tasks/test_first_party_webhooks.py` & `linked_services-1.2.3/tests/django/tasks/test_first_party_webhooks.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/tests/django/tasks/test_import_external_user.py` & `linked_services-1.2.3/tests/django/tasks/test_import_external_user.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/tests/management/commands/test_sign_jwt.py` & `linked_services-1.2.3/tests/management/commands/test_sign_jwt.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/tests/management/commands/test_sign_request.py` & `linked_services-1.2.3/tests/management/commands/test_sign_request.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/tests/rest_framework/views/test_authorize_view.py` & `linked_services-1.2.3/tests/rest_framework/views/test_authorize_view.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/tests/utils/argument_parser.py` & `linked_services-1.2.3/tests/utils/argument_parser.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/tests/utils/create_models.py` & `linked_services-1.2.3/tests/utils/create_models.py`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/.gitignore` & `linked_services-1.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/LICENSE.txt` & `linked_services-1.2.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/README.md` & `linked_services-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/pyproject.toml` & `linked_services-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `linked_services-1.2.2/PKG-INFO` & `linked_services-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: linked-services
-Version: 1.2.2
+Version: 1.2.3
 Project-URL: Documentation, https://breatheco-de.github.io/linked-services-django-plugin/
 Project-URL: Issues, https://github.com/breatheco-de/linked-services-django-plugin/issues
 Project-URL: Source, https://github.com/breatheco-de/linked-services-django-plugin
 Author-email: jefer94 <jdefreitaspinto@gmail.com>
 License-Expression: LGPL-3.0-or-later
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
```

