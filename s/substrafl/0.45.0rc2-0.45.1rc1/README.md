# Comparing `tmp/substrafl-0.45.0rc2.tar.gz` & `tmp/substrafl-0.45.1rc1.tar.gz`

## Comparing `substrafl-0.45.0rc2.tar` & `substrafl-0.45.1rc1.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/.flake8
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/.git-blame-ignore-revs
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/.readthedocs.yml
--rw-r--r--   0        0        0    42831 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/CHANGELOG.md
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/CONTRIBUTING.md
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/CONTRIBUTORS.md
--rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/Makefile
--rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/Substra-logo-colour.svg
--rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/Substra-logo-white.svg
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/skaffold.yaml
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/.github/CODEOWNERS
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/.github/ISSUE_TEMPLATE/bug_report.yaml
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/.github/workflows/main-check.yml
--rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/.github/workflows/publish.yml
--rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/.github/workflows/validate-pr.yml
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/.github/workflows/windows-subprocess-check.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/changes/.gitkeep
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/charts/substrafl/.helmignore
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/charts/substrafl/Chart.yaml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/charts/substrafl/values.yaml
--rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/charts/substrafl/templates/_helpers.tpl
--rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/charts/substrafl/templates/deployment.yaml
--rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docker/substrafl-tests/Dockerfile
--rwxr-xr-x   0        0        0      720 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/Makefile
--rwxr-xr-x   0        0        0     6276 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/conf.py
--rwxr-xr-x   0        0        0     1541 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/favicon.ico
--rwxr-xr-x   0        0        0       94 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/index.rst
--rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/requirements.txt
--rwxr-xr-x   0        0        0     1560 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/api/algorithms.rst
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/api/compute_plan_builder.rst
--rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/api/dependency.rst
--rwxr-xr-x   0        0        0      146 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/api/evaluation_strategy.rst
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/api/exceptions.rst
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/api/experiment.rst
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/api/index.rst
--rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/api/index_generator.rst
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/api/logger.rst
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/api/model_loading.rst
--rwxr-xr-x   0        0        0     1044 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/api/nodes.rst
--rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/api/remote.rst
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/api/strategies.rst
--rwxr-xr-x   0        0        0      591 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/static/download.svg
--rwxr-xr-x   0        0        0     1831 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/static/favicon.png
--rwxr-xr-x   0        0        0      801 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/static/fonts.css
--rwxr-xr-x   0        0        0   805454 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/static/logo.svg
--rwxr-xr-x   0        0        0     3405 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/static/owkin.css
--rwxr-xr-x   0        0        0     2009 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/static/sidebar.css
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/technical/index.rst
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/docs/technical/task_execution.rst
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/__init__.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/__version__.py
--rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/compute_plan_builder.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/constants.py
--rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/evaluation_strategy.py
--rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/exceptions.py
--rw-r--r--   0        0        0    21917 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/experiment.py
--rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/logger.py
--rw-r--r--   0        0        0    18190 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/model_loading.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/schemas.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/algorithms/__init__.py
--rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/algorithms/algo.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/algorithms/pytorch/__init__.py
--rw-r--r--   0        0        0    14979 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/algorithms/pytorch/torch_base_algo.py
--rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
--rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/algorithms/pytorch/torch_fed_pca_algo.py
--rw-r--r--   0        0        0    18388 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
--rw-r--r--   0        0        0    23633 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/algorithms/pytorch/torch_scaffold_algo.py
--rw-r--r--   0        0        0     8095 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/algorithms/pytorch/torch_single_organization_algo.py
--rw-r--r--   0        0        0    11241 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/algorithms/pytorch/weight_manager.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/dependency/__init__.py
--rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/dependency/constants.py
--rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/dependency/manage_dependencies.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/dependency/path_management.py
--rw-r--r--   0        0        0    11062 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/dependency/schemas.py
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/index_generator/__init__.py
--rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/index_generator/base.py
--rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/index_generator/np_index_generator.py
--rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/nodes/__init__.py
--rw-r--r--   0        0        0     9975 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/nodes/aggregation_node.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/nodes/protocol.py
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/nodes/schemas.py
--rw-r--r--   0        0        0     9512 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/nodes/test_data_node.py
--rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/nodes/train_data_node.py
--rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/nodes/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/nodes/references/__init__.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/nodes/references/local_state.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/nodes/references/shared_state.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/remote/__init__.py
--rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/remote/decorators.py
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/remote/operations.py
--rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/remote/remote_struct.py
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/remote/substratools_methods.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/remote/register/__init__.py
--rw-r--r--   0        0        0     9627 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/remote/register/register.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/remote/serializers/__init__.py
--rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/remote/serializers/pickle_serializer.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/remote/serializers/serializer.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/strategies/__init__.py
--rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/strategies/fed_avg.py
--rw-r--r--   0        0        0    16361 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/strategies/fed_pca.py
--rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/strategies/newton_raphson.py
--rw-r--r--   0        0        0    18428 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/strategies/scaffold.py
--rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/strategies/schemas.py
--rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/strategies/single_organization.py
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/substrafl/strategies/strategy.py
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/.gitignore
--rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/LICENSE
--rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/README.md
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/pyproject.toml
--rw-r--r--   0        0        0    19829 2020-02-02 00:00:00.000000 substrafl-0.45.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      562 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/.flake8
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/.readthedocs.yml
+-rw-r--r--   0        0        0    42942 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/CHANGELOG.md
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/CONTRIBUTORS.md
+-rw-r--r--   0        0        0     1783 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/Makefile
+-rw-r--r--   0        0        0     9601 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/Substra-logo-colour.svg
+-rw-r--r--   0        0        0     9585 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/Substra-logo-white.svg
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/skaffold.yaml
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/.github/CODEOWNERS
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/.github/ISSUE_TEMPLATE/bug_report.yaml
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0     2077 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/.github/workflows/main-check.yml
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     4616 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/.github/workflows/validate-pr.yml
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/.github/workflows/windows-subprocess-check.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/changes/.gitkeep
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/charts/substrafl/.helmignore
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/charts/substrafl/Chart.yaml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/charts/substrafl/values.yaml
+-rw-r--r--   0        0        0     1427 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/charts/substrafl/templates/_helpers.tpl
+-rw-r--r--   0        0        0     2817 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/charts/substrafl/templates/deployment.yaml
+-rw-r--r--   0        0        0     1185 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docker/substrafl-tests/Dockerfile
+-rwxr-xr-x   0        0        0      720 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/Makefile
+-rwxr-xr-x   0        0        0     6276 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/conf.py
+-rwxr-xr-x   0        0        0     1541 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/favicon.ico
+-rwxr-xr-x   0        0        0       94 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/index.rst
+-rwxr-xr-x   0        0        0      138 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/requirements.txt
+-rwxr-xr-x   0        0        0     1560 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/api/algorithms.rst
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/api/compute_plan_builder.rst
+-rwxr-xr-x   0        0        0      182 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/api/dependency.rst
+-rwxr-xr-x   0        0        0      146 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/api/evaluation_strategy.rst
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/api/exceptions.rst
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/api/experiment.rst
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/api/index.rst
+-rwxr-xr-x   0        0        0      297 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/api/index_generator.rst
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/api/logger.rst
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/api/model_loading.rst
+-rwxr-xr-x   0        0        0     1044 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/api/nodes.rst
+-rwxr-xr-x   0        0        0      730 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/api/remote.rst
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/api/strategies.rst
+-rwxr-xr-x   0        0        0      591 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/static/download.svg
+-rwxr-xr-x   0        0        0     1831 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/static/favicon.png
+-rwxr-xr-x   0        0        0      801 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/static/fonts.css
+-rwxr-xr-x   0        0        0   805454 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/static/logo.svg
+-rwxr-xr-x   0        0        0     3405 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/static/owkin.css
+-rwxr-xr-x   0        0        0     2009 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/static/sidebar.css
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/technical/index.rst
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/docs/technical/task_execution.rst
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/__init__.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/__version__.py
+-rw-r--r--   0        0        0     3203 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/compute_plan_builder.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/constants.py
+-rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/evaluation_strategy.py
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/exceptions.py
+-rw-r--r--   0        0        0    21917 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/experiment.py
+-rw-r--r--   0        0        0      788 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/logger.py
+-rw-r--r--   0        0        0    18190 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/model_loading.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/schemas.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/algorithms/__init__.py
+-rw-r--r--   0        0        0     5287 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/algorithms/algo.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/algorithms/pytorch/__init__.py
+-rw-r--r--   0        0        0    14979 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/algorithms/pytorch/torch_base_algo.py
+-rw-r--r--   0        0        0    10571 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py
+-rw-r--r--   0        0        0    13468 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py
+-rw-r--r--   0        0        0    18388 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py
+-rw-r--r--   0        0        0    23633 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py
+-rw-r--r--   0        0        0     8095 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py
+-rw-r--r--   0        0        0    11241 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/algorithms/pytorch/weight_manager.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/dependency/__init__.py
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/dependency/constants.py
+-rw-r--r--   0        0        0     8213 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/dependency/manage_dependencies.py
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/dependency/path_management.py
+-rw-r--r--   0        0        0    11062 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/dependency/schemas.py
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/index_generator/__init__.py
+-rw-r--r--   0        0        0     5403 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/index_generator/base.py
+-rw-r--r--   0        0        0     5777 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/index_generator/np_index_generator.py
+-rw-r--r--   0        0        0     1122 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/nodes/__init__.py
+-rw-r--r--   0        0        0     9975 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/nodes/aggregation_node.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/nodes/protocol.py
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/nodes/schemas.py
+-rw-r--r--   0        0        0     9512 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/nodes/test_data_node.py
+-rw-r--r--   0        0        0    16811 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/nodes/train_data_node.py
+-rw-r--r--   0        0        0     1178 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/nodes/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/nodes/references/__init__.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/nodes/references/local_state.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/nodes/references/shared_state.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/remote/__init__.py
+-rw-r--r--   0        0        0     5368 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/remote/decorators.py
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/remote/operations.py
+-rw-r--r--   0        0        0     4648 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/remote/remote_struct.py
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/remote/substratools_methods.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/remote/register/__init__.py
+-rw-r--r--   0        0        0     9627 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/remote/register/register.py
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/remote/serializers/__init__.py
+-rw-r--r--   0        0        0      803 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/remote/serializers/pickle_serializer.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/remote/serializers/serializer.py
+-rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/strategies/__init__.py
+-rw-r--r--   0        0        0    12706 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/strategies/fed_avg.py
+-rw-r--r--   0        0        0    16361 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/strategies/fed_pca.py
+-rw-r--r--   0        0        0    15789 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/strategies/newton_raphson.py
+-rw-r--r--   0        0        0    18428 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/strategies/scaffold.py
+-rw-r--r--   0        0        0     3818 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/strategies/schemas.py
+-rw-r--r--   0        0        0     7542 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/strategies/single_organization.py
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/substrafl/strategies/strategy.py
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/.gitignore
+-rw-r--r--   0        0        0    10762 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/LICENSE
+-rw-r--r--   0        0        0     6077 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/README.md
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/pyproject.toml
+-rw-r--r--   0        0        0    19829 2020-02-02 00:00:00.000000 substrafl-0.45.1rc1/PKG-INFO
```

### Comparing `substrafl-0.45.0rc2/.flake8` & `substrafl-0.45.1rc1/.flake8`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/.pre-commit-config.yaml` & `substrafl-0.45.1rc1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/CHANGELOG.md` & `substrafl-0.45.1rc1/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 <!-- towncrier release notes start -->
 
+## [0.45.1](https://github.com/Substra/substrafl/releases/tag/0.45.1) - 2024-05-21
+
+
+No significant changes.
+
+
 ## [0.45.0](https://github.com/Substra/substrafl/releases/tag/0.45.0) - 2024-03-27
 
 
 ### Added
 
 - - New CLI arguments to Camelyon benchmark (`--torch-gpu` and `--cp-name`) ([#201](https://github.com/Substra/substrafl/pull/201))
```

### Comparing `substrafl-0.45.0rc2/CONTRIBUTORS.md` & `substrafl-0.45.1rc1/CONTRIBUTORS.md`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/Makefile` & `substrafl-0.45.1rc1/Makefile`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/Substra-logo-colour.svg` & `substrafl-0.45.1rc1/Substra-logo-colour.svg`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/Substra-logo-white.svg` & `substrafl-0.45.1rc1/Substra-logo-white.svg`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/.github/PULL_REQUEST_TEMPLATE.md` & `substrafl-0.45.1rc1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/.github/ISSUE_TEMPLATE/bug_report.yaml` & `substrafl-0.45.1rc1/.github/ISSUE_TEMPLATE/bug_report.yaml`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/.github/ISSUE_TEMPLATE/config.yml` & `substrafl-0.45.1rc1/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/.github/workflows/main-check.yml` & `substrafl-0.45.1rc1/.github/workflows/main-check.yml`

 * *Files 10% similar despite different names*

```diff
@@ -11,39 +11,39 @@
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-22.04]
         python: ["3.9", "3.10", "3.11"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           path: substrafl
 
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
 
       - name: Free disk space
         run: |
           # Based on https://github.com/actions/runner-images/issues/2840#issuecomment-790492173
           sudo rm -rf /usr/share/dotnet
           sudo rm -rf /usr/local/lib/android
           sudo rm -rf /opt/ghc
           sudo rm -rf "/usr/local/share/boost"
           sudo rm -rf "$AGENT_TOOLSDIRECTORY"
 
       - name: Checkout pyconfig from a private repos
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           repository: substra/substra-tools
           path: substratools
 
       - name: Checkout pyconfig from a private repos
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           repository: substra/substra
           path: substra
 
       - uses: actions/cache@v3.0.8
         id: cache
         with:
```

### Comparing `substrafl-0.45.0rc2/.github/workflows/validate-pr.yml` & `substrafl-0.45.1rc1/.github/workflows/validate-pr.yml`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,19 @@
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [ubuntu-22.04]
         python: ["3.9", "3.10", "3.11"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           path: substrafl
 
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
 
       - uses: actions/cache@v3.0.8
         id: cache
         with:
           path: ${{ env.pythonLocation }}
@@ -36,20 +36,20 @@
           pip install --upgrade pytest black flake8 pre-commit
 
       - name: Code conventions
         run: |
           cd substrafl
           pre-commit run --all-files
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           repository: substra/substra-tools
           path: substratools
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           repository: substra/substra
           path: substra
 
       - name: Install package
         run: |
           pip install --upgrade -e substrafl[dev]
@@ -66,32 +66,32 @@
         with:
           name: coverage
           path: substrafl/htmlcov
 
   pr-validation-docs:
     runs-on: ubuntu-22.04
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v5
         with:
           python-version: "3.10"
 
       - uses: actions/cache@v3.0.8
         id: cache
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-${{ env.pythonLocation }}-pip-${{ hashFiles('substrafl/pyproject.toml') }}-${{ hashFiles  ('substrafl/docs/requirements.txt') }}-${{ hashFiles('substrafl/benchmark/camelyon/requirements.txt') }}
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           repository: substra/substra
           path: substra
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           repository: substra/substra-tools
           path: substratools
 
       - name: Install Dependencies
         run: |
           pip install --upgrade ./substra
@@ -103,28 +103,28 @@
         run: |
           cd docs
           make clean html
 
   benchmark:
     runs-on: ubuntu-22.04
     steps:
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v5
         with:
           python-version: 3.11
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           path: substrafl
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           repository: substra/substra-tools
           path: substratools
 
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           repository: substra/substra
           path: substra
 
       - uses: actions/cache@v3.0.8
         id: cache
         with:
```

### Comparing `substrafl-0.45.0rc2/.github/workflows/windows-subprocess-check.yml` & `substrafl-0.45.1rc1/.github/workflows/windows-subprocess-check.yml`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 name: windows-subprocess-check
 on:
   push:
     branches:
       - main
-
 jobs:
   pr-validation:
     name: test-${{ matrix.os }}-py-${{ matrix.python }}
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
         os: [windows-latest]
         python: ["3.9", "3.10", "3.11"]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           path: substrafl
 
-      - uses: actions/setup-python@v3
+      - uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python }}
 
       - name: Checkout pyconfig from a private repos
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           repository: substra/substra-tools
           path: substratools
 
       - name: Checkout pyconfig from a private repos
-        uses: actions/checkout@v3
+        uses: actions/checkout@v4
         with:
           repository: substra/substra
           path: substra
 
       - uses: actions/cache@v3.0.8
         id: cache
         with:
           path: ${{ env.pythonLocation }}
           key: ${{ runner.os }}-${{ env.pythonLocation }}-pip-${{ hashFiles('substrafl/pyproject.toml') }}-${{ hashFiles  ('substrafl/docs/requirements.txt') }}-${{ hashFiles('substrafl/benchmark/camelyon/requirements.txt') }}
 
       - name: Install package
         run: |
-          pip install --upgrade -e substrafl[dev]
+          pip install --upgrade -e "substrafl[dev]"
           pip install --upgrade -e substra
           pip install --upgrade -e substratools
 
       - name: Run the subprocess tests
         run: |
           cd substrafl
           make COV_OPTIONS="--cov=substrafl --cov-append --cov-report=html:htmlcov" test-subprocess
```

### Comparing `substrafl-0.45.0rc2/charts/substrafl/values.yaml` & `substrafl-0.45.1rc1/charts/substrafl/values.yaml`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/charts/substrafl/templates/_helpers.tpl` & `substrafl-0.45.1rc1/charts/substrafl/templates/_helpers.tpl`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/charts/substrafl/templates/deployment.yaml` & `substrafl-0.45.1rc1/charts/substrafl/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docker/substrafl-tests/Dockerfile` & `substrafl-0.45.1rc1/docker/substrafl-tests/Dockerfile`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/Makefile` & `substrafl-0.45.1rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/conf.py` & `substrafl-0.45.1rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/favicon.ico` & `substrafl-0.45.1rc1/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/api/algorithms.rst` & `substrafl-0.45.1rc1/docs/api/algorithms.rst`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/api/nodes.rst` & `substrafl-0.45.1rc1/docs/api/nodes.rst`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/api/remote.rst` & `substrafl-0.45.1rc1/docs/api/remote.rst`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/api/strategies.rst` & `substrafl-0.45.1rc1/docs/api/strategies.rst`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/static/download.svg` & `substrafl-0.45.1rc1/docs/static/download.svg`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/static/favicon.png` & `substrafl-0.45.1rc1/docs/static/favicon.png`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/static/fonts.css` & `substrafl-0.45.1rc1/docs/static/fonts.css`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/static/logo.svg` & `substrafl-0.45.1rc1/docs/static/logo.svg`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/static/owkin.css` & `substrafl-0.45.1rc1/docs/static/owkin.css`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/static/sidebar.css` & `substrafl-0.45.1rc1/docs/static/sidebar.css`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/docs/technical/task_execution.rst` & `substrafl-0.45.1rc1/docs/technical/task_execution.rst`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/__init__.py` & `substrafl-0.45.1rc1/substrafl/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/compute_plan_builder.py` & `substrafl-0.45.1rc1/substrafl/compute_plan_builder.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/evaluation_strategy.py` & `substrafl-0.45.1rc1/substrafl/evaluation_strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/exceptions.py` & `substrafl-0.45.1rc1/substrafl/exceptions.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/experiment.py` & `substrafl-0.45.1rc1/substrafl/experiment.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/logger.py` & `substrafl-0.45.1rc1/substrafl/logger.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/model_loading.py` & `substrafl-0.45.1rc1/substrafl/model_loading.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/algorithms/algo.py` & `substrafl-0.45.1rc1/substrafl/algorithms/algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/algorithms/pytorch/__init__.py` & `substrafl-0.45.1rc1/substrafl/algorithms/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/algorithms/pytorch/torch_base_algo.py` & `substrafl-0.45.1rc1/substrafl/algorithms/pytorch/torch_base_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/algorithms/pytorch/torch_fed_avg_algo.py` & `substrafl-0.45.1rc1/substrafl/algorithms/pytorch/torch_fed_avg_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/algorithms/pytorch/torch_fed_pca_algo.py` & `substrafl-0.45.1rc1/substrafl/algorithms/pytorch/torch_fed_pca_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py` & `substrafl-0.45.1rc1/substrafl/algorithms/pytorch/torch_newton_raphson_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/algorithms/pytorch/torch_scaffold_algo.py` & `substrafl-0.45.1rc1/substrafl/algorithms/pytorch/torch_scaffold_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/algorithms/pytorch/torch_single_organization_algo.py` & `substrafl-0.45.1rc1/substrafl/algorithms/pytorch/torch_single_organization_algo.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/algorithms/pytorch/weight_manager.py` & `substrafl-0.45.1rc1/substrafl/algorithms/pytorch/weight_manager.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/dependency/constants.py` & `substrafl-0.45.1rc1/substrafl/dependency/constants.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/dependency/manage_dependencies.py` & `substrafl-0.45.1rc1/substrafl/dependency/manage_dependencies.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/dependency/path_management.py` & `substrafl-0.45.1rc1/substrafl/dependency/path_management.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/dependency/schemas.py` & `substrafl-0.45.1rc1/substrafl/dependency/schemas.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/index_generator/base.py` & `substrafl-0.45.1rc1/substrafl/index_generator/base.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/index_generator/np_index_generator.py` & `substrafl-0.45.1rc1/substrafl/index_generator/np_index_generator.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/nodes/__init__.py` & `substrafl-0.45.1rc1/substrafl/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/nodes/aggregation_node.py` & `substrafl-0.45.1rc1/substrafl/nodes/aggregation_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/nodes/protocol.py` & `substrafl-0.45.1rc1/substrafl/nodes/protocol.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/nodes/schemas.py` & `substrafl-0.45.1rc1/substrafl/nodes/schemas.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/nodes/test_data_node.py` & `substrafl-0.45.1rc1/substrafl/nodes/test_data_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/nodes/train_data_node.py` & `substrafl-0.45.1rc1/substrafl/nodes/train_data_node.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/nodes/utils.py` & `substrafl-0.45.1rc1/substrafl/nodes/utils.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/remote/decorators.py` & `substrafl-0.45.1rc1/substrafl/remote/decorators.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/remote/operations.py` & `substrafl-0.45.1rc1/substrafl/remote/operations.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/remote/remote_struct.py` & `substrafl-0.45.1rc1/substrafl/remote/remote_struct.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/remote/substratools_methods.py` & `substrafl-0.45.1rc1/substrafl/remote/substratools_methods.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/remote/register/register.py` & `substrafl-0.45.1rc1/substrafl/remote/register/register.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/remote/serializers/pickle_serializer.py` & `substrafl-0.45.1rc1/substrafl/remote/serializers/pickle_serializer.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/strategies/fed_avg.py` & `substrafl-0.45.1rc1/substrafl/strategies/fed_avg.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/strategies/fed_pca.py` & `substrafl-0.45.1rc1/substrafl/strategies/fed_pca.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/strategies/newton_raphson.py` & `substrafl-0.45.1rc1/substrafl/strategies/newton_raphson.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/strategies/scaffold.py` & `substrafl-0.45.1rc1/substrafl/strategies/scaffold.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/strategies/schemas.py` & `substrafl-0.45.1rc1/substrafl/strategies/schemas.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/strategies/single_organization.py` & `substrafl-0.45.1rc1/substrafl/strategies/single_organization.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/substrafl/strategies/strategy.py` & `substrafl-0.45.1rc1/substrafl/strategies/strategy.py`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/.gitignore` & `substrafl-0.45.1rc1/.gitignore`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/LICENSE` & `substrafl-0.45.1rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/README.md` & `substrafl-0.45.1rc1/README.md`

 * *Files identical despite different names*

### Comparing `substrafl-0.45.0rc2/pyproject.toml` & `substrafl-0.45.1rc1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,16 +17,16 @@
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version"]
 readme = "README.md"
 dependencies = [
     "numpy>=1.24",
     "cloudpickle>=1.6.0",
-    "substra~=0.52.0rc1",
-    "substratools~=0.21.3rc1",
+    "substra~=0.52.1rc1",
+    "substratools~=0.21.4rc1",
     "pydantic>=2.3.0,<3.0",
     "pip>=21.2",
     "tqdm",
     "wheel",
     "six",
     "packaging",
     "pip-tools",
```

### Comparing `substrafl-0.45.0rc2/PKG-INFO` & `substrafl-0.45.1rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: substrafl
-Version: 0.45.0rc2
+Version: 0.45.1rc1
 Summary: A high-level federated learning Python library to run     federated learning experiments at scale on a Substra network
 Project-URL: Documentation, https://docs.substra.org/en/stable/
 Project-URL: Repository, https://github.com/Substra/substrafl
 Project-URL: Changelog, https://github.com/Substra/substrafl/blob/main/CHANGELOG.md
 Author: Owkin, Inc.
 License: 
                                          Apache License
@@ -207,16 +207,16 @@
 Requires-Dist: cloudpickle>=1.6.0
 Requires-Dist: numpy>=1.24
 Requires-Dist: packaging
 Requires-Dist: pip-tools
 Requires-Dist: pip>=21.2
 Requires-Dist: pydantic<3.0,>=2.3.0
 Requires-Dist: six
-Requires-Dist: substratools~=0.21.3rc1
-Requires-Dist: substra~=0.52.0rc1
+Requires-Dist: substratools~=0.21.4rc1
+Requires-Dist: substra~=0.52.1rc1
 Requires-Dist: tqdm
 Requires-Dist: wheel
 Provides-Extra: dev
 Requires-Dist: docker; extra == 'dev'
 Requires-Dist: nbmake>=1.4.3; extra == 'dev'
 Requires-Dist: pre-commit>=2.13.0; extra == 'dev'
 Requires-Dist: pytest-cov>=2.12.0; extra == 'dev'
```

