# Comparing `tmp/edge-containers-cli-3.4.1.tar.gz` & `tmp/edge_containers_cli-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edge-containers-cli-3.4.1.tar", last modified: Thu Mar 28 14:47:22 2024, max compression
+gzip compressed data, was "edge_containers_cli-3.5.0.tar", last modified: Tue May 21 11:20:39 2024, max compression
```

## Comparing `edge-containers-cli-3.4.1.tar` & `edge_containers_cli-3.5.0.tar`

### file list

```diff
@@ -1,142 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.625185 edge-containers-cli-3.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.609185 edge-containers-cli-3.4.1/.devcontainer/
--rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.devcontainer/devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.613185 edge-containers-cli-3.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.605185 edge-containers-cli-3.4.1/.github/actions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.613185 edge-containers-cli-3.4.1/.github/actions/install_requirements/
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.github/actions/install_requirements/action.yml
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.613185 edge-containers-cli-3.4.1/.github/pages/
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.github/pages/index.html
--rwxr-xr-x   0 runner    (1001) docker     (127)     2753 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.github/pages/make_switcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.613185 edge-containers-cli-3.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.github/workflows/_check.yml
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.github/workflows/_dist.yml
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.github/workflows/_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.github/workflows/_release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.github/workflows/_sys_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.github/workflows/_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.github/workflows/_tox.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.613185 edge-containers-cli-3.4.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/.vscode/tasks.json
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-03-28 14:47:22.625185 edge-containers-cli-3.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/catalog-info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.613185 edge-containers-cli-3.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.613185 edge-containers-cli-3.4.1/docs/developer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.613185 edge-containers-cli-3.4.1/docs/developer/explanations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.613185 edge-containers-cli-3.4.1/docs/developer/explanations/decisions/
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/explanations/decisions.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.617185 edge-containers-cli-3.4.1/docs/developer/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/how-to/build-docs.rst
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/how-to/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/how-to/lint.rst
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/how-to/make-release.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/how-to/pin-requirements.rst
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/how-to/run-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/how-to/static-analysis.rst
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/how-to/test-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/how-to/update-tools.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.617185 edge-containers-cli-3.4.1/docs/developer/reference/
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/reference/standards.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.617185 edge-containers-cli-3.4.1/docs/developer/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/developer/tutorials/dev-install.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/genindex.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.617185 edge-containers-cli-3.4.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)    99678 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/images/dls-favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/images/dls-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.617185 edge-containers-cli-3.4.1/docs/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.617185 edge-containers-cli-3.4.1/docs/user/explanations/
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/user/explanations/docs-structure.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.617185 edge-containers-cli-3.4.1/docs/user/how-to/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/user/how-to/run-container.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/user/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.617185 edge-containers-cli-3.4.1/docs/user/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/user/reference/api.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.617185 edge-containers-cli-3.4.1/docs/user/tutorials/
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/docs/user/tutorials/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 14:47:22.625185 edge-containers-cli-3.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.609185 edge-containers-cli-3.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.617185 edge-containers-cli-3.4.1/src/edge_containers_cli/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-28 14:47:22.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4714 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/autocomplete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.621185 edge-containers-cli-3.4.1/src/edge_containers_cli/cmds/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/cmds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9229 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/cmds/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3596 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/cmds/helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7949 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/cmds/k8s_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/cmds/kubectl.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/cmds/local_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/git.py
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/globals.py
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/shell.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/src/edge_containers_cli/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.625185 edge-containers-cli-3.4.1/src/edge_containers_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15373 2024-03-28 14:47:22.000000 edge-containers-cli-3.4.1/src/edge_containers_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-03-28 14:47:22.000000 edge-containers-cli-3.4.1/src/edge_containers_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 14:47:22.000000 edge-containers-cli-3.4.1/src/edge_containers_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-28 14:47:22.000000 edge-containers-cli-3.4.1/src/edge_containers_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-28 14:47:22.000000 edge-containers-cli-3.4.1/src/edge_containers_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-28 14:47:22.000000 edge-containers-cli-3.4.1/src/edge_containers_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.621185 edge-containers-cli-3.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.621185 edge-containers-cli-3.4.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/autocomplete.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.621185 edge-containers-cli-3.4.1/tests/data/bl01t/
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.621185 edge-containers-cli-3.4.1/tests/data/bl01t/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.625185 edge-containers-cli-3.4.1/tests/data/bl01t/.github/workflows/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1253 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/.github/workflows/ci_verify.sh
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/.github/workflows/verify.yml
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     1874 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/environment.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.609185 edge-containers-cli-3.4.1/tests/data/bl01t/helm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.625185 edge-containers-cli-3.4.1/tests/data/bl01t/helm/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/helm/shared/Chart.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/helm/shared/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/helm/shared/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.609185 edge-containers-cli-3.4.1/tests/data/bl01t/include/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.625185 edge-containers-cli-3.4.1/tests/data/bl01t/include/iocs/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/include/iocs/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.625185 edge-containers-cli-3.4.1/tests/data/bl01t/include/iocs/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/include/iocs/templates/configmap.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.609185 edge-containers-cli-3.4.1/tests/data/bl01t/services/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.625185 edge-containers-cli-3.4.1/tests/data/bl01t/services/bl01t-ea-test-01/
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/services/bl01t-ea-test-01/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:22.625185 edge-containers-cli-3.4.1/tests/data/bl01t/services/bl01t-ea-test-01/config/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.db
--rw-r--r--   0 runner    (1001) docker     (127)      679 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/services/bl01t-ea-test-01/pretend_helm.tgz
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/services/bl01t-ea-test-01/values.yaml
--rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/bl01t/update-helm
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/ioc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/data/local.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/test_autocomplete.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2653 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/test_ioc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/test_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-28 14:47:18.000000 edge-containers-cli-3.4.1/tests/test_system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.006164 edge_containers_cli-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.986163 edge_containers_cli-3.5.0/.devcontainer/
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.devcontainer/devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.982164 edge_containers_cli-3.5.0/.github/actions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/.github/actions/install_requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/actions/install_requirements/action.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/.github/pages/
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/pages/index.html
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2753 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/pages/make_switcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_check.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_dist.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_sys_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/_tox.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/.vscode/tasks.json
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/catalog-info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     6545 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/docs/developer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/docs/developer/explanations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.990164 edge_containers_cli-3.5.0/docs/developer/explanations/decisions/
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/explanations/decisions/0001-record-architecture-decisions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/explanations/decisions.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/developer/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/build-docs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/lint.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/make-release.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2880 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/pin-requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/run-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/static-analysis.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/test-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/how-to/update-tools.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1404 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/developer/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/reference/standards.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/developer/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/developer/tutorials/dev-install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/genindex.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    99678 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/images/dls-favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/images/dls-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/user/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/user/explanations/
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/user/explanations/docs-structure.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/user/how-to/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/user/how-to/run-container.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/user/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/user/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/user/reference/api.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.994164 edge_containers_cli-3.5.0/docs/user/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/docs/user/tutorials/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:20:39.006164 edge_containers_cli-3.5.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.986163 edge_containers_cli-3.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.998164 edge_containers_cli-3.5.0/src/edge_containers_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4732 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/autocomplete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.998164 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8651 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7856 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/k8s_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/kubectl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9713 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/local_commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8601 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/monitor.tcss
+-rw-r--r--   0 runner    (1001) docker     (127)     4678 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/globals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/shell.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/src/edge_containers_cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15396 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-21 11:20:38.000000 edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.998164 edge_containers_cli-3.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5932 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.998164 edge_containers_cli-3.5.0/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/autocomplete.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/.github/workflows/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1253 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/.github/workflows/ci_verify.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/.github/workflows/verify.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11359 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1874 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/environment.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.986163 edge_containers_cli-3.5.0/tests/data/bl01t/helm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/helm/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/helm/shared/Chart.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/helm/shared/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/helm/shared/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.986163 edge_containers_cli-3.5.0/tests/data/bl01t/include/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/include/iocs/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/include/iocs/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/include/iocs/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/include/iocs/templates/configmap.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:38.986163 edge_containers_cli-3.5.0/tests/data/bl01t/services/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:39.002164 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.db
+-rw-r--r--   0 runner    (1001) docker     (127)      679 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/pretend_helm.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/values.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (127)      491 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/bl01t/update-helm
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/ioc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5112 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/data/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/test_autocomplete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/test_ioc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/test_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-05-21 11:20:34.000000 edge_containers_cli-3.5.0/tests/test_system.py
```

### Comparing `edge-containers-cli-3.4.1/.devcontainer/devcontainer.json` & `edge_containers_cli-3.5.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/.github/CONTRIBUTING.md` & `edge_containers_cli-3.5.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/.github/actions/install_requirements/action.yml` & `edge_containers_cli-3.5.0/.github/actions/install_requirements/action.yml`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/.github/dependabot.yml` & `edge_containers_cli-3.5.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/.github/pages/make_switcher.py` & `edge_containers_cli-3.5.0/.github/pages/make_switcher.py`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/.github/workflows/_check.yml` & `edge_containers_cli-3.5.0/.github/workflows/_check.yml`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/.github/workflows/_dist.yml` & `edge_containers_cli-3.5.0/.github/workflows/_dist.yml`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/.github/workflows/_release.yml` & `edge_containers_cli-3.5.0/.github/workflows/_release.yml`

 * *Files 15% similar despite different names*

```diff
@@ -19,14 +19,14 @@
             zip -r docs.zip $GITHUB_REF_NAME
             rm -rf $GITHUB_REF_NAME
           fi
 
       - name: Create GitHub Release
         # We pin to the SHA, not the tag, for security reasons.
         # https://docs.github.com/en/actions/learn-github-actions/security-hardening-for-github-actions#using-third-party-actions
-        uses: softprops/action-gh-release@9d7c94cfd0a1f3ed45544c887983e9fa900f0564 # v0.1.15
+        uses: softprops/action-gh-release@69320dbe05506a9a39fc8ae11030b214ec2d1f87 # v0.1.15
         with:
           prerelease: ${{ contains(github.ref_name, 'a') || contains(github.ref_name, 'b') || contains(github.ref_name, 'rc') }}
           files: "*"
           generate_release_notes: true
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `edge-containers-cli-3.4.1/.github/workflows/_sys_test.yml` & `edge_containers_cli-3.5.0/.github/workflows/_sys_test.yml`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/.github/workflows/_test.yml` & `edge_containers_cli-3.5.0/.github/workflows/_test.yml`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/.github/workflows/ci.yml` & `edge_containers_cli-3.5.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/.gitignore` & `edge_containers_cli-3.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/.pre-commit-config.yaml` & `edge_containers_cli-3.5.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-yaml
       - id: check-merge-conflict
 
   - repo: local
     hooks:
```

### Comparing `edge-containers-cli-3.4.1/.vscode/launch.json` & `edge_containers_cli-3.5.0/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/LICENSE` & `edge_containers_cli-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/PKG-INFO` & `edge_containers_cli-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-containers-cli
-Version: 3.4.1
+Version: 3.5.0
 Summary: CLI for deploying and managing epics containers IOCs and services
 Author-email: Giles Knap <giles.knap@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -216,14 +216,15 @@
 License-File: LICENSE
 Requires-Dist: natsort
 Requires-Dist: typer[all]
 Requires-Dist: requests
 Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2
 Requires-Dist: polars
+Requires-Dist: textual
 Provides-Extra: dev
 Requires-Dist: copier; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
```

### Comparing `edge-containers-cli-3.4.1/README.md` & `edge_containers_cli-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/conf.py` & `edge_containers_cli-3.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst` & `edge_containers_cli-3.5.0/docs/developer/explanations/decisions/0002-switched-to-pip-skeleton.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/developer/explanations/decisions.rst` & `edge_containers_cli-3.5.0/docs/developer/explanations/decisions.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/developer/how-to/build-docs.rst` & `edge_containers_cli-3.5.0/docs/developer/how-to/build-docs.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/developer/how-to/lint.rst` & `edge_containers_cli-3.5.0/docs/developer/how-to/lint.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/developer/how-to/make-release.rst` & `edge_containers_cli-3.5.0/docs/developer/how-to/make-release.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/developer/how-to/pin-requirements.rst` & `edge_containers_cli-3.5.0/docs/developer/how-to/pin-requirements.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/developer/how-to/test-container.rst` & `edge_containers_cli-3.5.0/docs/developer/how-to/test-container.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/developer/how-to/update-tools.rst` & `edge_containers_cli-3.5.0/docs/developer/how-to/update-tools.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/developer/index.rst` & `edge_containers_cli-3.5.0/docs/developer/index.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/developer/reference/standards.rst` & `edge_containers_cli-3.5.0/docs/developer/reference/standards.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/developer/tutorials/dev-install.rst` & `edge_containers_cli-3.5.0/docs/developer/tutorials/dev-install.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/images/dls-favicon.ico` & `edge_containers_cli-3.5.0/docs/images/dls-favicon.ico`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/images/dls-logo.svg` & `edge_containers_cli-3.5.0/docs/images/dls-logo.svg`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/index.rst` & `edge_containers_cli-3.5.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/user/explanations/docs-structure.rst` & `edge_containers_cli-3.5.0/docs/user/explanations/docs-structure.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/user/index.rst` & `edge_containers_cli-3.5.0/docs/user/index.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/docs/user/tutorials/installation.rst` & `edge_containers_cli-3.5.0/docs/user/tutorials/installation.rst`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/pyproject.toml` & `edge_containers_cli-3.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 dependencies = [
     "natsort",
     "typer[all]",
     "requests",
     "ruamel.yaml",
     "jinja2",
     "polars",
+    "textual",
 ]
 
 dynamic = ["version"]
 license.file = "LICENSE"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `edge-containers-cli-3.4.1/src/edge_containers_cli/__main__.py` & `edge_containers_cli-3.5.0/src/edge_containers_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/src/edge_containers_cli/autocomplete.py` & `edge_containers_cli-3.5.0/src/edge_containers_cli/autocomplete.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 import typer
 
 import edge_containers_cli.globals as globals
 import edge_containers_cli.shell as shell
 from edge_containers_cli.cmds.k8s_commands import check_namespace
 from edge_containers_cli.docker import Docker
-from edge_containers_cli.git import create_svc_graph
+from edge_containers_cli.git import create_version_map
 from edge_containers_cli.logging import log
 from edge_containers_cli.utils import cleanup_temp
 
 
 def url_encode(in_string: str) -> str:
     return urllib.parse.quote(in_string, safe="")  # type: ignore
 
@@ -42,22 +42,22 @@
             with open(cache_path) as f:
                 read_dict = json.load(f)
 
     return read_dict
 
 
 def fetch_service_graph(beamline_repo: str) -> dict:
-    svc_graph = read_cached_dict(url_encode(beamline_repo), globals.IOC_CACHE)
-    if not svc_graph:
+    version_map = read_cached_dict(url_encode(beamline_repo), globals.IOC_CACHE)
+    if not version_map:
         tmp_dir = Path(tempfile.mkdtemp())
-        svc_graph = create_svc_graph(beamline_repo, tmp_dir)
-        cache_dict(url_encode(beamline_repo), globals.IOC_CACHE, svc_graph)
+        version_map = create_version_map(beamline_repo, tmp_dir)
+        cache_dict(url_encode(beamline_repo), globals.IOC_CACHE, version_map)
         cleanup_temp(tmp_dir)
 
-    return svc_graph
+    return version_map
 
 
 def avail_services(ctx: typer.Context) -> list[str]:
     params = ctx.parent.params  # type: ignore
     services_repo = params["repo"] or globals.EC_SERVICES_REPO
 
     # This block prevents getting a stack trace during autocompletion
@@ -73,16 +73,16 @@
 def avail_versions(ctx: typer.Context) -> list[str]:
     params = ctx.parent.params  # type: ignore
     beamline_repo = params["repo"] or globals.EC_SERVICES_REPO
     service_name = ctx.params["service_name"]
 
     # This block prevents getting a stack trace during autocompletion
     try:
-        svc_graph = fetch_service_graph(beamline_repo)
-        svc_versions = svc_graph[service_name]
+        version_map = fetch_service_graph(beamline_repo)
+        svc_versions = version_map[service_name]
         return svc_versions
     except KeyError:
         log.error("IOC not found")
         return [" "]
     except typer.Exit:
         return [" "]
     except CalledProcessError:
```

### Comparing `edge-containers-cli-3.4.1/src/edge_containers_cli/cmds/cli.py` & `edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,79 +11,106 @@
     avail_services,
     avail_versions,
     force_plain_completion,
     running_svc,
 )
 from edge_containers_cli.cmds.k8s_commands import K8sCommands
 from edge_containers_cli.cmds.local_commands import LocalCommands
-from edge_containers_cli.git import create_svc_graph
+from edge_containers_cli.cmds.monitor import MonitorApp
+from edge_containers_cli.git import create_version_map
+from edge_containers_cli.globals import EC_K8S_NAMESPACE
 from edge_containers_cli.logging import log
 from edge_containers_cli.utils import cleanup_temp, drop_path
 
-cli = typer.Typer(pretty_exceptions_show_locals=False)
+
+class ErrorHandlingTyper(typer.Typer):
+    def __call__(self, *args, **kwargs):
+        try:
+            super().__call__(*args, **kwargs)
+        except NotImplementedError:
+            typer.echo("This function is not available for the current namespace")
+
+
+cli = ErrorHandlingTyper(pretty_exceptions_show_locals=False)
+
+
+def commands(ctx):
+    """
+    Construct the appropriate Commands class for the local or K8S namespace
+    """
+    if ctx.obj.namespace == globals.LOCAL_NAMESPACE:
+        commands = LocalCommands(ctx.obj)
+    else:
+        commands = K8sCommands(ctx.obj)
+
+    return commands
 
 
 @cli.command()
 def ps(
     ctx: typer.Context,
     all: bool = typer.Option(
         False, "-a", "--all", help="list stopped IOCs/services as well as running ones"
     ),
     wide: bool = typer.Option(
         False, "--wide", "-w", help="use a wide format with additional fields"
     ),
 ):
     """List the IOCs/services running in the current namespace"""
-    if ctx.obj.namespace == globals.LOCAL_NAMESPACE:
-        LocalCommands(ctx.obj).ps(all, wide)
-    else:
-        K8sCommands(ctx.obj).ps(all, wide)
+    commands(ctx).ps(all, wide)
+
+
+@cli.command()
+def monitor(
+    ctx: typer.Context,
+    all: bool = typer.Option(
+        False, "-a", "--all", help="list stopped IOCs/services as well as running ones"
+    ),
+):
+    """Open IOC monitor TUI."""
+    cmds = commands(ctx)
+    app = MonitorApp(EC_K8S_NAMESPACE, cmds, all)
+    app.run()
 
 
 @cli.command()
 def env(
     ctx: typer.Context,
     verbose: bool = typer.Option(
         False, "-v", "--verbose", help="show all relevant environment variables"
     ),
 ):
     """List all relevant environment variables"""
-    LocalCommands(ctx.obj).environment(verbose == verbose)
+    commands(ctx).environment(verbose == verbose)
 
 
 @cli.command()
 def attach(
     ctx: typer.Context,
     service_name: str = typer.Argument(
         ..., help="Name of the IOC/service to attach to", autocompletion=running_svc
     ),
 ):
     """
     Attach to the console of a live service
     """
-    if ctx.obj.namespace == globals.LOCAL_NAMESPACE:
-        LocalCommands(ctx.obj, service_name).attach()
-    else:
-        K8sCommands(ctx.obj, service_name).attach()
+    commands(ctx).attach(service_name)
 
 
 @cli.command()
 def delete(
     ctx: typer.Context,
     service_name: str = typer.Argument(
         ..., help="Name of the IOC/service to delete", autocompletion=all_svc
     ),
 ):
     """
     Remove a helm deployment from the cluster
     """
-    if ctx.obj.namespace == globals.LOCAL_NAMESPACE:
-        LocalCommands(ctx.obj, service_name).delete()
-    else:
-        K8sCommands(ctx.obj, service_name).delete()
+    commands(ctx).delete(service_name)
 
 
 @cli.command()
 def template(
     ctx: typer.Context,
     svc_instance: Path = typer.Argument(
         ...,
@@ -95,18 +122,15 @@
     ),  # noqa: B008
     args: str = typer.Option("", help="Additional args for helm, 'must be quoted'"),
 ):
     """
     print out the helm template generated from a local service instance
     """
     args = f"{args} --debug"
-    if ctx.obj.namespace == globals.LOCAL_NAMESPACE:
-        typer.echo("Not applicable to local deployments")
-    else:
-        K8sCommands(ctx.obj).template(svc_instance, args)
+    commands(ctx).template(svc_instance, args)
 
 
 @cli.command()
 def deploy_local(
     ctx: typer.Context,
     svc_instance: Path = typer.Argument(
         ...,
@@ -119,19 +143,15 @@
     yes: bool = typer.Option(False, "-y", "--yes", help="Skip confirmation prompt"),
     wait: bool = typer.Option(False, "--wait", help="Waits for readiness"),
     args: str = typer.Option("", help="Additional args for helm, 'must be quoted'"),
 ):
     """
     Deploy a local IOC/service helm chart directly to the cluster with dated beta version
     """
-    if ctx.obj.namespace == globals.LOCAL_NAMESPACE:
-        LocalCommands(ctx.obj).deploy_local(svc_instance, yes, args)
-    else:
-        args = args if not wait else args + " --wait"
-        K8sCommands(ctx.obj).deploy_local(svc_instance, yes, args)
+    commands(ctx).deploy_local(svc_instance, yes, args)
 
 
 @cli.command()
 def deploy(
     ctx: typer.Context,
     service_name: str = typer.Argument(
         ..., help="Name of the IOC/service to deploy", autocompletion=avail_services
@@ -145,35 +165,30 @@
     args: str = typer.Option(
         "", help="Additional args for helm or docker, 'must be quoted'"
     ),
 ):
     """
     Pull an IOC/service helm chart version from the domain repo and deploy it to the cluster
     """
+    args = args if not wait else args + " --wait"
     service_name = drop_path(service_name)
-    if ctx.obj.namespace == globals.LOCAL_NAMESPACE:
-        LocalCommands(ctx.obj, service_name).deploy(service_name, version, args)
-    else:
-        args = args if not wait else args + " --wait"
-        K8sCommands(ctx.obj, service_name, check=False).deploy(
-            service_name, version, args
-        )
+    commands(ctx).deploy(service_name, version, args)
 
 
 @cli.command()
 def list(
     ctx: typer.Context,
 ):
     """List all IOCs/services available in the helm registry"""
     tmp_dir = Path(tempfile.mkdtemp())
-    svc_graph = create_svc_graph(ctx.obj.beamline_repo, tmp_dir)
-    svc_list = natsorted(svc_graph.keys())
-    log.debug(f"svc_graph = {svc_graph}")
+    version_map = create_version_map(ctx.obj.beamline_repo, tmp_dir)
+    svc_list = natsorted(version_map.keys())
+    log.debug(f"version_map = {version_map}")
 
-    versions = [natsorted(svc_graph[svc])[-1] for svc in svc_list]
+    versions = [natsorted(version_map[svc])[-1] for svc in svc_list]
     services_df = polars.from_dict({"name": svc_list, "version": versions})
     print(services_df)
 
     cleanup_temp(tmp_dir)
 
 
 @cli.command()
@@ -181,17 +196,17 @@
     ctx: typer.Context,
     service_name: str = typer.Argument(
         ..., help="Name of the IOC/service to inspect", autocompletion=avail_services
     ),
 ):
     """List all versions of the IOC/service available in the helm registry"""
     tmp_dir = Path(tempfile.mkdtemp())
-    svc_graph = create_svc_graph(ctx.obj.beamline_repo, tmp_dir)
+    version_map = create_version_map(ctx.obj.beamline_repo, tmp_dir)
     try:
-        svc_list = svc_graph[service_name]
+        svc_list = version_map[service_name]
     except KeyError:
         svc_list = []
 
     sorted_list = natsorted(svc_list)[::-1]
     services_df = polars.from_dict({"version": sorted_list})
     print(services_df)
 
@@ -204,30 +219,28 @@
     service_name: str = typer.Argument(
         ...,
         help="Name of the IOC/service container to run in",
         autocompletion=running_svc,
     ),
 ):
     """Execute a bash prompt in a running container"""
-    if ctx.obj.namespace == globals.LOCAL_NAMESPACE:
-        LocalCommands(ctx.obj, service_name).exec()
-    else:
-        K8sCommands(ctx.obj, service_name).exec()
+    commands(ctx).exec(service_name)
 
 
 @cli.command()
 def log_history(
+    ctx: typer.Context,
     service_name: str = typer.Argument(
         ...,
         help="Name of the IOC/service to inspect",
         autocompletion=all_svc,
     ),
 ):
     """Open historical logs for an IOC/service"""
-    K8sCommands(None, service_name).log_history()
+    commands(ctx).log_history(service_name)
 
 
 @cli.command()
 def logs(
     ctx: typer.Context,
     service_name: str = typer.Argument(
         ..., help="Name of the IOC/service to inspect", autocompletion=running_svc
@@ -237,63 +250,51 @@
         "--previous",
         "-p",
         help="Show log from the previous instance of the IOC/service",
     ),
     follow: bool = typer.Option(False, "--follow", "-f", help="Follow the log stream"),
 ):
     """Show logs for current and previous instances of an IOC/service"""
-    if ctx.obj.namespace == globals.LOCAL_NAMESPACE:
-        LocalCommands(ctx.obj, service_name).logs(prev, follow)
-    else:
-        K8sCommands(ctx.obj, service_name).logs(prev, follow)
+    commands(ctx).logs(service_name, prev, follow)
 
 
 @cli.command()
 def restart(
     ctx: typer.Context,
     service_name: str = typer.Argument(
         ..., help="Name of the container to restart", autocompletion=running_svc
     ),
 ):
     """Restart an IOC/service"""
-    if ctx.obj.namespace == globals.LOCAL_NAMESPACE:
-        LocalCommands(ctx.obj, service_name).restart()
-    else:
-        K8sCommands(ctx.obj, service_name).restart()
+    commands(ctx).restart(service_name)
 
 
 @cli.command()
 def start(
     ctx: typer.Context,
     service_name: str = typer.Argument(
         ..., help="Name of the IOC/service container to start", autocompletion=all_svc
     ),
 ):
     """Start an IOC/service"""
     log.debug("Starting IOC/service with LOCAL={ctx.obj.namespace == " "}")
-    if ctx.obj.namespace == globals.LOCAL_NAMESPACE:
-        LocalCommands(ctx.obj, service_name).start()
-    else:
-        K8sCommands(ctx.obj, service_name).start()
+    commands(ctx).start(service_name)
 
 
 @cli.command()
 def stop(
     ctx: typer.Context,
     service_name: str = typer.Argument(
         ...,
         help="Name of the IOC/service container to stop",
         autocompletion=running_svc,
     ),
 ):
     """Stop an IOC/service"""
-    if ctx.obj.namespace == globals.LOCAL_NAMESPACE:
-        LocalCommands(ctx.obj, service_name).stop()
-    else:
-        K8sCommands(ctx.obj, service_name).stop()
+    commands(ctx).stop(service_name)
 
 
 @cli.command()
 def validate(
     ctx: typer.Context,
     svc_instance: Path = typer.Argument(
         ...,
```

### Comparing `edge-containers-cli-3.4.1/src/edge_containers_cli/cmds/helm.py` & `edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/helm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import tempfile
 from pathlib import Path
 from typing import Optional
 
 import typer
+from ruamel.yaml import YAML
 
 import edge_containers_cli.globals as globals
 import edge_containers_cli.shell as shell
 from edge_containers_cli.utils import (
     chdir,
     check_instance_path,
     cleanup_temp,
@@ -88,23 +89,27 @@
 
         # package up the charts to get the appVersion set
         for chart in chart_paths:
             shell.run_command(f"helm dependency update {chart}", interactive=False)
 
         with chdir(service_folder):
             shell.run_command(
-                f"helm dependency update {service_folder}; "
-                f"helm package {service_folder} --app-version {self.version}",
+                f"helm package {service_folder} -u --app-version {self.version}",
                 interactive=False,
             )
-            # find the packaged chart
-            chart_file = list(service_folder.glob("*.tgz"))[0]
+
+            # Determine package name
+            with open("Chart.yaml") as fp:
+                chart_yaml = YAML(typ="safe").load(fp)
+            package_path = (
+                service_folder / f'{chart_yaml["name"]}-{chart_yaml["version"]}.tgz'
+            )
 
         # use helm to install the chart
-        self._install(chart_file)
+        self._install(package_path)
 
     def _install(self, helm_chart: Path):
         """
         Execute helm install command
         """
 
         helm_cmd = "template" if self.template else "upgrade --install"
```

### Comparing `edge-containers-cli-3.4.1/src/edge_containers_cli/cmds/k8s_commands.py` & `edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/k8s_commands.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 implements commands for deploying and managing service instances in the k8s cluster.
 
 Relies on the Helm class for deployment aspects.
 """
 
-import webbrowser
 from datetime import datetime
 from io import StringIO
 from pathlib import Path
 from typing import Optional
 
 import polars
 import typer
 
 import edge_containers_cli.globals as globals
 import edge_containers_cli.shell as shell
+from edge_containers_cli.cmds.commands import Commands
 from edge_containers_cli.cmds.helm import Helm
 from edge_containers_cli.cmds.kubectl import jsonpath_deploy_info, jsonpath_pod_info
 from edge_containers_cli.logging import log
 
 
 def check_service(service_name: str, namespace: str) -> str:
     """
@@ -55,51 +55,43 @@
             f"~/.kube/config or change EC_K8S_NAMESPACE"
         )
         raise typer.Exit(1)
 
     log.info("domain = %s", namespace)
 
 
-class K8sCommands:
+class K8sCommands(Commands):
     """
     A class for implementing the Kubernetes based commands
     """
 
     def __init__(
         self,
-        ctx: Optional[globals.Context],
-        service_name: str = "",
-        check: bool = True,
+        ctx: globals.Context,
+        # check: bool = True,
     ):
-        self.namespace: str = ""
-        self.beamline_repo: str = ""
-        # TODO isnt ctx always set??
-        if ctx is not None:
-            namespace = ctx.namespace
-            check_namespace(namespace)
-            if service_name != "" and check:
-                self.fullname = check_service(service_name, namespace)
-            self.namespace = namespace
-            self.beamline_repo = ctx.beamline_repo
-        self.service_name: str = service_name
+        super().__init__(ctx)
+        check_namespace(self.namespace)
 
-    def attach(self):
+    def attach(self, service_name):
+        fullname = check_service(service_name, self.namespace)
         shell.run_command(
-            f"kubectl -it -n {self.namespace} attach {self.fullname}",
+            f"kubectl -it -n {self.namespace} attach {fullname}",
             interactive=True,
         )
 
-    def delete(self):
+    def delete(self, service_name):
+        check_service(service_name, self.namespace)
         if not typer.confirm(
-            f"This will remove all versions of {self.service_name} "
+            f"This will remove all versions of {service_name} "
             "from the cluster. Are you sure ?"
         ):
             raise typer.Abort()
 
-        shell.run_command(f"helm delete -n {self.namespace} {self.service_name}")
+        shell.run_command(f"helm delete -n {self.namespace} {service_name}")
 
     def template(self, svc_instance: Path, args: str):
         datetime.strftime(datetime.now(), "%Y.%-m.%-d-b%-H.%-M")
 
         service_name = svc_instance.name.lower()
 
         chart = Helm(
@@ -123,56 +115,45 @@
             service_name,
             args,
             version,
             repo=self.beamline_repo,
         )
         chart.deploy()
 
-    def exec(self):
-        shell.run_command(
-            f"kubectl -it -n {self.namespace} exec {self.fullname} -- bash"
-        )
-
-    def log_history(self):
-        if not globals.EC_LOG_URL:
-            log.error("EC_LOG_URL environment not set")
-            raise typer.Exit(1)
-
-        url = globals.EC_LOG_URL.format(service_name=self.service_name)
-        webbrowser.open(url)
+    def exec(self, service_name):
+        fullname = check_service(service_name, self.namespace)
+        shell.run_command(f"kubectl -it -n {self.namespace} exec {fullname} -- bash")
 
-    def logs(self, prev: bool, follow: bool):
+    def logs(self, service_name: str, prev: bool, follow: bool):
+        fullname = check_service(service_name, self.namespace)
         previous = "-p" if prev else ""
         fol = "-f" if follow else ""
 
         shell.run_command(
-            f"kubectl -n {self.namespace} logs {self.fullname} {previous} {fol}"
+            f"kubectl -n {self.namespace} logs {fullname} {previous} {fol}"
         )
 
-    def restart(self):
+    def restart(self, service_name):
+        check_service(service_name, self.namespace)
         pod_name = shell.run_command(
-            f"kubectl get -n {self.namespace} pod -l app={self.service_name} -o name",
+            f"kubectl get -n {self.namespace} pod -l app={service_name} -o name",
             interactive=False,
         )
         shell.run_command(f"kubectl delete -n {self.namespace} {pod_name}")
 
-    def start(self):
-        shell.run_command(
-            f"kubectl scale -n {self.namespace} {self.fullname} --replicas=1"
-        )
+    def start(self, service_name):
+        fullname = check_service(service_name, self.namespace)
+        shell.run_command(f"kubectl scale -n {self.namespace} {fullname} --replicas=1")
 
-    def stop(self):
+    def stop(self, service_name):
+        fullname = check_service(service_name, self.namespace)
         """Stop an IOC"""
-        shell.run_command(
-            f"kubectl scale -n {self.namespace} {self.fullname} --replicas=0 "
-        )
-
-    def ps(self, all: bool, wide: bool):
-        """List all IOCs and Services in the current namespace"""
+        shell.run_command(f"kubectl scale -n {self.namespace} {fullname} --replicas=0 ")
 
+    def get_services(self, all: bool) -> polars.DataFrame:
         services_df = polars.DataFrame()
 
         # Gives all services (running & not running) and their image
         for resource in ["deployment", "statefulset"]:
             kubectl_res = shell.run_command(
                 f"kubectl get {resource} -n {self.namespace} {jsonpath_deploy_info}",
                 interactive=False,
@@ -228,11 +209,16 @@
         # Arrange columns
         services_df = services_df.select(
             ["name", "version", "running", "restarts", "deployed", "image"]
         )
         if not all:
             services_df = services_df.filter(polars.col("running").eq(True))
             log.debug(services_df)
+        return services_df
+
+    def ps(self, all: bool, wide: bool):
+        """List all IOCs and Services in the current namespace"""
+        services_df = self.get_services(all)
         if not wide:
             services_df.drop_in_place("image")
             log.debug(services_df)
         print(services_df)
```

### Comparing `edge-containers-cli-3.4.1/src/edge_containers_cli/cmds/local_commands.py` & `edge_containers_cli-3.5.0/src/edge_containers_cli/cmds/local_commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,72 +11,63 @@
 
 import json
 import re
 import tempfile
 from datetime import datetime
 from io import StringIO
 from pathlib import Path
-from typing import Optional
 
 import polars
 import requests
 import typer
 
 import edge_containers_cli.globals as globals
 import edge_containers_cli.shell as shell
-from edge_containers_cli.cmds.k8s_commands import check_namespace
+from edge_containers_cli.cmds.commands import Commands
 from edge_containers_cli.docker import Docker
 from edge_containers_cli.logging import log
 from edge_containers_cli.shell import check_services_repo
 from edge_containers_cli.utils import (
     check_instance_path,
     cleanup_temp,
     generic_ioc_from_image,
     get_instance_image_name,
     local_version,
 )
 
 
-class LocalCommands:
+class LocalCommands(Commands):
     """
     A class for implementing the ioc command namespace for local docker/podman
     """
 
     def __init__(
         self,
-        ctx: Optional[globals.Context],
-        service_name: str = "",
+        ctx: globals.Context,
         with_docker: bool = True,
     ):
-        self.namespace = ""
-        self.beamline_repo: str = ""
-        if ctx is not None:
-            self.beamline_repo = ctx.beamline_repo
-            self.namespace = ctx.namespace
-
-        self.service_name: str = service_name
-
         self.tmp = Path(tempfile.mkdtemp())
-        self.ioc_folder = self.tmp / "services" / service_name
+        self.ioc_folder = self.tmp / "services"
         self.docker = Docker(check=with_docker)
+        super().__init__(ctx)
 
     def __del__(self):
         if hasattr(self, "tmp"):
             cleanup_temp(self.tmp)
 
-    def attach(self):
-        self.docker.attach(self.service_name)
+    def attach(self, service_name):
+        self.docker.attach(service_name)
 
-    def delete(self):
+    def delete(self, service_name):
         if not typer.confirm(
-            f"This will remove the IOC container {self.service_name} "
+            f"This will remove the IOC container {service_name} "
             "from the this server. Are you sure ?"
         ):
             raise typer.Abort()
-        self.docker.remove(self.service_name)
+        self.docker.remove(service_name)
 
     def _do_deploy(self, ioc_instance: Path, version: str, args: str):
         service_name, _ = check_instance_path(ioc_instance)
 
         image = get_instance_image_name(ioc_instance)
         log.debug(f"deploying {ioc_instance} with image {image}")
         config = ioc_instance / globals.CONFIG_FOLDER
@@ -113,60 +104,60 @@
         shell.run_command(f"{self.docker.docker} {cmd} --name {service_name} {image}")
         if not self.docker.is_running(service_name, retry=5):
             typer.echo(
                 f"Failed to start {service_name} please try 'ec ioc logs {service_name}'"
             )
             raise typer.Exit(1)
 
-    def deploy_local(self, ioc_instance: Path, yes: bool, args: str):
+    def deploy_local(self, svc_instance: Path, yes: bool, args: str):
         """
         Use a local copy of an ioc instance definition to deploy a temporary
         version of the IOC to the local docker instance
         """
         version = local_version()
         if not yes:
             typer.echo(
                 f"Deploy TEMPORARY version {version} "
-                f"from {ioc_instance} to the local docker instance"
+                f"from {svc_instance} to the local docker instance"
             )
             if not typer.confirm("Are you sure ?"):
                 raise typer.Abort()
-        self._do_deploy(ioc_instance, version, args)
+        self._do_deploy(svc_instance, version, args)
 
     def deploy(self, service_name: str, version: str, args: str):
         """
         deploy a tagged version of an ioc from a remote repo
         """
 
         check_services_repo(self.beamline_repo)
 
         shell.run_command(
             f"git clone {self.beamline_repo} {self.tmp} --depth=1 "
             f"--single-branch --branch={version}",
             interactive=False,
         )
 
-        self._do_deploy(self.ioc_folder, version, args)
+        self._do_deploy(self.ioc_folder / service_name, version, args)
 
-    def exec(self):
-        self.docker.exec(self.service_name, "bash", args="-it")
+    def exec(self, service_name):
+        self.docker.exec(service_name, "bash", args="-it")
 
-    def logs(self, prev: bool, follow: bool):
-        self.docker.logs(self.service_name, prev, follow)
+    def logs(self, service_name: str, prev: bool, follow: bool):
+        self.docker.logs(service_name, prev, follow)
 
-    def restart(self):
-        shell.run_command(f"{self.docker.docker} restart {self.service_name}")
+    def restart(self, service_name: str):
+        shell.run_command(f"{self.docker.docker} restart {service_name}")
 
-    def start(self):
-        shell.run_command(f"{self.docker.docker} start {self.service_name}")
+    def start(self, service_name: str):
+        shell.run_command(f"{self.docker.docker} start {service_name}")
 
-    def stop(self):
-        shell.run_command(f"{self.docker.docker} stop {self.service_name}")
+    def stop(self, service_name: str):
+        shell.run_command(f"{self.docker.docker} stop {service_name}")
 
-    def ps(self, all: bool, wide: bool):
+    def get_services(self, all: bool) -> polars.DataFrame:
         all_arg = " --all" if all else ""
 
         # List services
         avail_services = shell.run_command(
             f"{self.docker.docker} ps{all_arg} -q --filter label=is_IOC=true",
             interactive=False,
         )
@@ -204,15 +195,18 @@
                     "deployed": datetime.strptime(
                         service["Created"].split(".")[0], "%Y-%m-%dT%H:%M:%S"
                     ),
                     "image": service["Config"]["Image"],
                 }
             )
         log.debug(select_data)
+        return polars.DataFrame(select_data)
 
+    def ps(self, all: bool, wide: bool):
+        select_data = self.get_services(all)
         services_df = polars.DataFrame(select_data)
         if not wide:
             services_df.drop_in_place("image")
         print(services_df)
 
     def validate_instance(self, ioc_instance: Path):
         check_instance_path(ioc_instance)
@@ -268,22 +262,7 @@
         shell.run_command(
             f"{self.docker.docker} manifest inspect {image}", interactive=False
         )
 
         cleanup_temp(tmp)
 
         typer.echo(f"{ioc_instance} validated successfully")
-
-    def environment(self, verbose: bool):
-        """
-        declare the environment settings for ec
-        """
-        ns = self.namespace
-
-        if ns == globals.LOCAL_NAMESPACE:
-            typer.echo("ioc commands deploy to the local docker/podman instance")
-        else:
-            check_namespace(ns)
-            typer.echo(f"ioc commands deploy to the {ns} namespace the K8S cluster")
-
-        typer.echo("\nEC environment variables:")
-        shell.run_command("env | grep '^EC_'", interactive=False, show=True)
```

### Comparing `edge-containers-cli-3.4.1/src/edge_containers_cli/docker.py` & `edge_containers_cli-3.5.0/src/edge_containers_cli/docker.py`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/src/edge_containers_cli/globals.py` & `edge_containers_cli-3.5.0/src/edge_containers_cli/globals.py`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/src/edge_containers_cli/logging.py` & `edge_containers_cli-3.5.0/src/edge_containers_cli/logging.py`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/src/edge_containers_cli/shell.py` & `edge_containers_cli-3.5.0/src/edge_containers_cli/shell.py`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/src/edge_containers_cli/utils.py` & `edge_containers_cli-3.5.0/src/edge_containers_cli/utils.py`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/src/edge_containers_cli.egg-info/PKG-INFO` & `edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edge-containers-cli
-Version: 3.4.1
+Version: 3.5.0
 Summary: CLI for deploying and managing epics containers IOCs and services
 Author-email: Giles Knap <giles.knap@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -216,14 +216,15 @@
 License-File: LICENSE
 Requires-Dist: natsort
 Requires-Dist: typer[all]
 Requires-Dist: requests
 Requires-Dist: ruamel.yaml
 Requires-Dist: jinja2
 Requires-Dist: polars
+Requires-Dist: textual
 Provides-Extra: dev
 Requires-Dist: copier; extra == "dev"
 Requires-Dist: pipdeptree; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: pyright; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
```

### Comparing `edge-containers-cli-3.4.1/src/edge_containers_cli.egg-info/SOURCES.txt` & `edge_containers_cli-3.5.0/src/edge_containers_cli.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -63,18 +63,21 @@
 src/edge_containers_cli.egg-info/SOURCES.txt
 src/edge_containers_cli.egg-info/dependency_links.txt
 src/edge_containers_cli.egg-info/entry_points.txt
 src/edge_containers_cli.egg-info/requires.txt
 src/edge_containers_cli.egg-info/top_level.txt
 src/edge_containers_cli/cmds/__init__.py
 src/edge_containers_cli/cmds/cli.py
+src/edge_containers_cli/cmds/commands.py
 src/edge_containers_cli/cmds/helm.py
 src/edge_containers_cli/cmds/k8s_commands.py
 src/edge_containers_cli/cmds/kubectl.py
 src/edge_containers_cli/cmds/local_commands.py
+src/edge_containers_cli/cmds/monitor.py
+src/edge_containers_cli/cmds/monitor.tcss
 tests/__init__.py
 tests/conftest.py
 tests/test_autocomplete.py
 tests/test_cli.py
 tests/test_ioc.py
 tests/test_local.py
 tests/test_system.py
```

### Comparing `edge-containers-cli-3.4.1/tests/conftest.py` & `edge_containers_cli-3.5.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/tests/data/autocomplete.yaml` & `edge_containers_cli-3.5.0/tests/data/autocomplete.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -38,14 +38,18 @@
     rsp: |
       1.0
       2.0
   - cmd: git ls-tree -r 1.0 --name-only
     rsp: bl01t-ea-test-01
   - cmd: git diff --name-only 1.0 2.0
     rsp: bl01t-ea-test-01
+  - cmd: git ls-tree 2.0 -r | grep 120000
+    rsp: 120000 blob test services/bl01t-ea-test-01/Chart.yaml
+  - cmd: git cat-file -p test
+    rsp: ../../include/iocs/templates
 
 running_iocs:
   - cmd: kubectl get namespace bl01t -o name
     rsp: namespace/bl01t
   - cmd: kubectl -n bl01t get pod -o custom-columns=IOC_NAME:metadata
     rsp: NAME, bl01t-ea-test-01
```

### Comparing `edge-containers-cli-3.4.1/tests/data/bl01t/.github/workflows/ci_verify.sh` & `edge_containers_cli-3.5.0/tests/data/bl01t/.github/workflows/ci_verify.sh`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/tests/data/bl01t/LICENSE` & `edge_containers_cli-3.5.0/tests/data/bl01t/LICENSE`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/tests/data/bl01t/README.md` & `edge_containers_cli-3.5.0/tests/data/bl01t/README.md`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/tests/data/bl01t/environment.sh` & `edge_containers_cli-3.5.0/tests/data/bl01t/environment.sh`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/tests/data/bl01t/helm/shared/README.md` & `edge_containers_cli-3.5.0/tests/data/bl01t/helm/shared/README.md`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/tests/data/bl01t/helm/shared/values.yaml` & `edge_containers_cli-3.5.0/tests/data/bl01t/helm/shared/values.yaml`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/tests/data/bl01t/include/iocs/Chart.yaml` & `edge_containers_cli-3.5.0/tests/data/bl01t/include/iocs/Chart.yaml`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/tests/data/bl01t/services/bl01t-ea-test-01/Chart.yaml` & `edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/Chart.yaml`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.db` & `edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.db`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.yaml` & `edge_containers_cli-3.5.0/tests/data/bl01t/services/bl01t-ea-test-01/config/ioc.yaml`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/tests/data/ioc.yaml` & `edge_containers_cli-3.5.0/tests/data/ioc.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,73 +1,80 @@
 checks:
   - cmd: kubectl get namespace bl01t -o name
     rsp: namespace/bl01t
   - cmd: kubectl get statefulset -o name -n bl01t bl01t-ea-test-01 --ignore-not-found
     rsp: statefulset/bl01t-ea-test-01
 
+svc_check:
+  - cmd: kubectl get namespace bl01t -o name
+    rsp: namespace/bl01t
+
 attach:
   - cmd: kubectl -it -n bl01t attach statefulset/bl01t-ea-test-01
     rsp: True
 
 delete:
   - cmd: helm delete -n bl01t bl01t-ea-test-01
     rsp: True
 
 template:
   - cmd: 'helm dependency update .*\/tests\/data\/bl01t\/services\/bl01t-ea-test-01\/..\/..\/helm\/shared'
     rsp: ""
-  - cmd: 'helm dependency update .*\/tests\/data\/bl01t\/services\/bl01t-ea-test-01\; helm package .*\/tests\/data\/bl01t\/services\/bl01t-ea-test-01 --app-version .*'
+  - cmd: 'helm package .*\/tests\/data\/bl01t\/services\/bl01t-ea-test-01 -u --app-version .*'
     rsp: ""
-  - cmd: 'bash -c "helm template bl01t-ea-test-01 .*pretend_helm.tgz --namespace bl01t  --debug'
+  - cmd: 'bash -c "helm template bl01t-ea-test-01 .*\.tgz --namespace bl01t  --debug *'
     rsp: |
       # Source: bl01t-ea-test-01/templates/configmap.yaml
       apiVersion: v1
       ...
 
 deploy_local:
   - cmd: 'helm dependency update .*\/tests\/data\/bl01t\/services\/bl01t-ea-test-01\/..\/..\/helm\/shared'
     rsp: ""
-  - cmd: 'helm dependency update .*\/tests\/data\/bl01t\/services\/bl01t-ea-test-01\; helm package .*\/tests\/data\/bl01t\/services\/bl01t-ea-test-01 --app-version .*'
+  - cmd: 'helm package .*\/tests\/data\/bl01t\/services\/bl01t-ea-test-01 -u --app-version .*'
     rsp: ""
-  - cmd: 'bash -c "helm upgrade --install bl01t-ea-test-01 .*pretend_helm.tgz --namespace bl01t'
+  - cmd: 'bash -c "helm upgrade --install bl01t-ea-test-01 .*\.tgz --namespace bl01t *'
     rsp: ""
 
 deploy:
   - cmd: kubectl get namespace bl01t -o name
     rsp: namespace/bl01t
   - cmd: git clone https://github.com/epics-containers/bl01t /tmp/ec_tests --depth=1 --single-branch --branch=2.0
     rsp: ""
-  - cmd: helm dependency update /tmp/ec_tests/services/bl01t-ea-test-01; helm package /tmp/ec_tests/services/bl01t-ea-test-01 --app-version 2.0
+  - cmd: helm package /tmp/ec_tests/services/bl01t-ea-test-01 -u --app-version 2.0
     rsp: ""
-  - cmd: 'bash -c "helm upgrade --install bl01t-ea-test-01 .*pretend_helm.tgz --namespace bl01t.*'
+  - cmd: 'bash -c "helm upgrade --install bl01t-ea-test-01 .*\.tgz --namespace bl01t *'
     rsp: ""
 
 instances:
   - cmd: git clone https://github.com/epics-containers/bl01t /tmp/.*
     rsp: Cloning into /tmp/xxxx...
   - cmd: git tag
     rsp: |
       1.0
       2.0
   - cmd: git ls-tree -r 1.0 --name-only
     rsp: bl01t-ea-test-01
   - cmd: git diff --name-only 1.0 2.0
     rsp: bl01t-ea-test-01
+  - cmd: git ls-tree 2.0 -r | grep 120000
+    rsp: 120000 blob test services/bl01t-ea-test-01/Chart.yaml
+  - cmd: git cat-file -p test
+    rsp: ../../include/iocs/templates
 
 exec:
   - cmd: kubectl -it -n bl01t exec statefulset/bl01t-ea-test-01 -- bash
     rsp: True
 
 exec2:
   - cmd: kubectl -it -n bl01t exec statefulset/bl01t-ea-test-01 -- bash
     rsp: True
 
 log_history:
-  - cmd:
-      "https://graylog2.diamond.ac.uk/search?rangetype=relative&fields=message\
+  - cmd: "https://graylog2.diamond.ac.uk/search?rangetype=relative&fields=message\
       %2Csource&width=1489&highlightMessage=&relative=172800&q=pod_name%3A\
       bl01t-ea-test-01*"
     rsp: True
 
 logs:
   - cmd: kubectl -n bl01t logs statefulset/bl01t-ea-test-01
     rsp: True
```

### Comparing `edge-containers-cli-3.4.1/tests/data/local.yaml` & `edge_containers_cli-3.5.0/tests/data/local.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -26,17 +26,18 @@
     rsp: bl01t-ea-test-01-config
   - cmd: docker volume create bl01t-ea-test-01_config
     rsp: bl01t-ea-test-01-config
   - cmd: docker rm -f busybox
     rsp: ""
   - cmd: docker container create --name busybox -v bl01t-ea-test-01_config:/copyto busybox
     rsp: ""
-  - cmd: docker cp {data}/bl01t/services/bl01t-ea-test-01/config/ioc.db busybox:copyto
+  # order of globbing of files may be non-deterministic so use ioc.*
+  - cmd: docker cp {data}/bl01t/services/bl01t-ea-test-01/config/ioc.* busybox:copyto
     rsp: ""
-  - cmd: docker cp {data}/bl01t/services/bl01t-ea-test-01/config/ioc.yaml busybox:copyto
+  - cmd: docker cp {data}/bl01t/services/bl01t-ea-test-01/config/ioc.* busybox:copyto
     rsp: ""
   - cmd: docker rm -f busybox
     rsp: ""
   - cmd: docker run -dit --net host --restart unless-stopped -l is_IOC=true -l version=.* -v bl01t-ea-test-01_config:\/epics\/ioc\/config\/  --name bl01t-ea-test-01 ghcr.io\/epics-containers\/ioc-adsimdetector-runtime:2024.4.1
     rsp: True
   - cmd: docker ps -f name=bl01t-ea-test-01 --format .*
     rsp: bl01t-ea-test-01
@@ -52,17 +53,18 @@
     rsp: bl01t-ea-test-01-config
   - cmd: docker volume create bl01t-ea-test-01_config
     rsp: bl01t-ea-test-01-config
   - cmd: docker rm -f busybox
     rsp: ""
   - cmd: docker container create --name busybox -v bl01t-ea-test-01_config:/copyto busybox
     rsp: ""
-  - cmd: docker cp /tmp/ec_tests/services/bl01t-ea-test-01/config/ioc.db busybox:copyto
+  # order of globbing of files may be non-deterministic so use ioc.*
+  - cmd: docker cp /tmp/ec_tests/services/bl01t-ea-test-01/config/ioc.* busybox:copyto
     rsp: ""
-  - cmd: docker cp /tmp/ec_tests/services/bl01t-ea-test-01/config/ioc.yaml busybox:copyto
+  - cmd: docker cp /tmp/ec_tests/services/bl01t-ea-test-01/config/ioc.* busybox:copyto
     rsp: ""
   - cmd: docker rm -f busybox
     rsp: ""
   - cmd: docker run -dit --net host --restart unless-stopped -l is_IOC=true -l version=2.0 -v bl01t-ea-test-01_config:/epics/ioc/config/  --name bl01t-ea-test-01 ghcr.io/epics-containers/ioc-adsimdetector-runtime:2024.4.1
     rsp: True
   - cmd: docker ps -f name=bl01t-ea-test-01 --format .*
     rsp: bl01t-ea-test-01
@@ -74,14 +76,18 @@
     rsp: |
       1.0
       2.0
   - cmd: git ls-tree -r 1.0 --name-only
     rsp: bl01t-ea-test-01
   - cmd: git diff --name-only 1.0 2.0
     rsp: bl01t-ea-test-01
+  - cmd: git ls-tree 2.0 -r | grep 120000
+    rsp: 120000 blob test services/bl01t-ea-test-01/Chart.yaml
+  - cmd: git cat-file -p test
+    rsp: ../../include/iocs/templates
 
 exec:
   - cmd: docker ps -f name=bl01t-ea-test-01 --format .*
     rsp: bl01t-ea-test-01
   - cmd: docker exec -it bl01t-ea-test-01 bash -c "bash"
     rsp: True
```

### Comparing `edge-containers-cli-3.4.1/tests/test_autocomplete.py` & `edge_containers_cli-3.5.0/tests/test_autocomplete.py`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/tests/test_ioc.py` & `edge_containers_cli-3.5.0/tests/test_ioc.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 def test_exec(mock_run, ioc):
     mock_run.set_seq(ioc.checks + ioc.exec)
     mock_run.run_cli("exec bl01t-ea-test-01")
 
 
 def test_log_history(mock_run, ioc):
-    mock_run.set_seq(ioc.log_history)
+    mock_run.set_seq(ioc.svc_check + ioc.log_history)
     mock_run.run_cli("log-history bl01t-ea-test-01")
 
 
 def test_logs(mock_run, ioc):
     mock_run.set_seq(ioc.checks + ioc.logs)
     mock_run.run_cli("logs bl01t-ea-test-01")
```

### Comparing `edge-containers-cli-3.4.1/tests/test_local.py` & `edge_containers_cli-3.5.0/tests/test_local.py`

 * *Files identical despite different names*

### Comparing `edge-containers-cli-3.4.1/tests/test_system.py` & `edge_containers_cli-3.5.0/tests/test_system.py`

 * *Files identical despite different names*

