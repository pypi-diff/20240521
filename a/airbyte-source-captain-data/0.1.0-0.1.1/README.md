# Comparing `tmp/airbyte-source-captain-data-0.1.0.tar.gz` & `tmp/airbyte_source_captain_data-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-captain-data-0.1.0.tar", last modified: Tue Jan 30 14:43:05 2024, max compression
+gzip compressed data, was "airbyte_source_captain_data-0.1.1.tar", max compression
```

## Comparing `airbyte-source-captain-data-0.1.0.tar` & `airbyte_source_captain_data-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,11 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:43:05.153193 airbyte-source-captain-data-0.1.0/
--rw-r--r--   0 root         (0) root         (0)     4278 2024-01-30 14:43:05.153193 airbyte-source-captain-data-0.1.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4091 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:43:05.153193 airbyte-source-captain-data-0.1.0/airbyte_source_captain_data.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4278 2024-01-30 14:43:05.000000 airbyte-source-captain-data-0.1.0/airbyte_source_captain_data.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      807 2024-01-30 14:43:05.000000 airbyte-source-captain-data-0.1.0/airbyte_source_captain_data.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-01-30 14:43:05.000000 airbyte-source-captain-data-0.1.0/airbyte_source_captain_data.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2024-01-30 14:43:05.000000 airbyte-source-captain-data-0.1.0/airbyte_source_captain_data.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-01-30 14:43:05.000000 airbyte-source-captain-data-0.1.0/airbyte_source_captain_data.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-01-30 14:43:05.000000 airbyte-source-captain-data-0.1.0/airbyte_source_captain_data.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:43:05.153193 airbyte-source-captain-data-0.1.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      314 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1742 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)       67 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)       59 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)     4136 2024-01-30 14:43:05.157193 airbyte-source-captain-data-0.1.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      939 2024-01-30 14:43:03.000000 airbyte-source-captain-data-0.1.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:43:05.153193 airbyte-source-captain-data-0.1.0/source_captain_data/
--rw-r--r--   0 root         (0) root         (0)      134 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/source_captain_data/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4595 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/source_captain_data/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      246 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/source_captain_data/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-01-30 14:43:05.153193 airbyte-source-captain-data-0.1.0/source_captain_data/schemas/
--rw-r--r--   0 root         (0) root         (0)      400 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/source_captain_data/schemas/job_results.json
--rw-r--r--   0 root         (0) root         (0)     1213 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/source_captain_data/schemas/jobs.json
--rw-r--r--   0 root         (0) root         (0)      771 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/source_captain_data/schemas/workflows.json
--rw-r--r--   0 root         (0) root         (0)      680 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/source_captain_data/schemas/workspace.json
--rw-r--r--   0 root         (0) root         (0)      480 2024-01-30 14:29:13.000000 airbyte-source-captain-data-0.1.0/source_captain_data/source.py
+-rw-r--r--   0        0        0     4604 2024-05-21 04:51:07.000000 airbyte_source_captain_data-0.1.1/README.md
+-rw-r--r--   0        0        0      778 2024-05-21 05:32:17.011391 airbyte_source_captain_data-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      134 2024-05-21 04:51:07.000000 airbyte_source_captain_data-0.1.1/source_captain_data/__init__.py
+-rw-r--r--   0        0        0     4595 2024-05-21 04:51:07.000000 airbyte_source_captain_data-0.1.1/source_captain_data/manifest.yaml
+-rw-r--r--   0        0        0      246 2024-05-21 04:51:07.000000 airbyte_source_captain_data-0.1.1/source_captain_data/run.py
+-rw-r--r--   0        0        0      400 2024-05-21 04:51:07.000000 airbyte_source_captain_data-0.1.1/source_captain_data/schemas/job_results.json
+-rw-r--r--   0        0        0     1213 2024-05-21 04:51:07.000000 airbyte_source_captain_data-0.1.1/source_captain_data/schemas/jobs.json
+-rw-r--r--   0        0        0      771 2024-05-21 04:51:07.000000 airbyte_source_captain_data-0.1.1/source_captain_data/schemas/workflows.json
+-rw-r--r--   0        0        0      680 2024-05-21 04:51:07.000000 airbyte_source_captain_data-0.1.1/source_captain_data/schemas/workspace.json
+-rw-r--r--   0        0        0      480 2024-05-21 04:51:07.000000 airbyte_source_captain_data-0.1.1/source_captain_data/source.py
+-rw-r--r--   0        0        0     5325 1970-01-01 00:00:00.000000 airbyte_source_captain_data-0.1.1/PKG-INFO
```

### Comparing `airbyte-source-captain-data-0.1.0/PKG-INFO` & `airbyte_source_captain_data-0.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,70 +1,91 @@
-Metadata-Version: 2.1
-Name: airbyte-source-captain-data
-Version: 0.1.0
-Summary: Source implementation for Captain Data.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
+# Captain-Data source connector
 
-# Captain Data Source
 
-This is the repository for the Captain Data configuration based source connector.
+This is the repository for the Captain-Data source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/captain-data).
 
+## Local development
 
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
+
+
+### Create credentials
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/captain-data)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_captain_data/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source captain-data test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-captain-data spec
+poetry run source-captain-data check --config secrets/config.json
+poetry run source-captain-data discover --config secrets/config.json
+poetry run source-captain-data read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-captain-data build
 ```
 
-An image will be built with the tag `airbyte/source-captain-data:dev`.
+An image will be available on your host with the tag `airbyte/source-captain-data:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-captain-data:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-captain-data:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-captain-data:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-captain-data:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-captain-data:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-captain-data test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-captain-data test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/captain-data.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/captain-data.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-captain-data-0.1.0/airbyte_source_captain_data.egg-info/PKG-INFO` & `airbyte_source_captain_data-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,110 @@
 Metadata-Version: 2.1
 Name: airbyte-source-captain-data
-Version: 0.1.0
+Version: 0.1.1
 Summary: Source implementation for Captain Data.
+Home-page: https://airbyte.com
+License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (==1.0.0)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/captain-data
+Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
 
-# Captain Data Source
+# Captain-Data source connector
 
-This is the repository for the Captain Data configuration based source connector.
+
+This is the repository for the Captain-Data source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/captain-data).
 
+## Local development
+
+### Prerequisites
+* Python (~=3.9)
+* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
+
+
+### Installing the connector
+From this connector directory, run:
+```bash
+poetry install --with dev
+```
 
+
+### Create credentials
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/captain-data)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_captain_data/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
-See `integration_tests/sample_config.json` for a sample config file.
+See `sample_files/sample_config.json` for a sample config file.
 
-**If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source captain-data test creds`
-and place them into `secrets/config.json`.
 
+### Locally running the connector
+```
+poetry run source-captain-data spec
+poetry run source-captain-data check --config secrets/config.json
+poetry run source-captain-data discover --config secrets/config.json
+poetry run source-captain-data read --config secrets/config.json --catalog sample_files/configured_catalog.json
+```
 
+### Running unit tests
+To run unit tests locally, from the connector directory run:
+```
+poetry run pytest unit_tests
+```
 
-**Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
+### Building the docker image
+1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
+2. Run the following command to build the docker image:
 ```bash
 airbyte-ci connectors --name=source-captain-data build
 ```
 
-An image will be built with the tag `airbyte/source-captain-data:dev`.
+An image will be available on your host with the tag `airbyte/source-captain-data:dev`.
 
-**Via `docker build`:**
-```bash
-docker build -t airbyte/source-captain-data:dev .
-```
 
+### Running as a docker container
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-captain-data:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-captain-data:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-captain-data:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-captain-data:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+### Running our CI test suite
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-captain-data test
 ```
 
-Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
+### Customizing acceptance Tests
+Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
-All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
-We split dependencies between two groups, dependencies that are:
-* required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
-* required for the testing need to go to `TEST_REQUIREMENTS` list
+### Dependency Management
+All of your dependencies should be managed via Poetry. 
+To add a new dependency, run:
+```bash
+poetry add <package-name>
+```
+
+Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
+## Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-captain-data test`
-2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
+    - bump the `dockerImageTag` value in in `metadata.yaml`
+    - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
-4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/captain-data.md`).
+4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/captain-data.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte-source-captain-data-0.1.0/source_captain_data/manifest.yaml` & `airbyte_source_captain_data-0.1.1/source_captain_data/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte-source-captain-data-0.1.0/source_captain_data/schemas/jobs.json` & `airbyte_source_captain_data-0.1.1/source_captain_data/schemas/jobs.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-captain-data-0.1.0/source_captain_data/schemas/workflows.json` & `airbyte_source_captain_data-0.1.1/source_captain_data/schemas/workflows.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-captain-data-0.1.0/source_captain_data/schemas/workspace.json` & `airbyte_source_captain_data-0.1.1/source_captain_data/schemas/workspace.json`

 * *Files identical despite different names*

