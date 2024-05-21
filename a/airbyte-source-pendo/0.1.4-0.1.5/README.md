# Comparing `tmp/airbyte_source_pendo-0.1.4.tar.gz` & `tmp/airbyte_source_pendo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_pendo-0.1.4.tar", max compression
+gzip compressed data, was "airbyte_source_pendo-0.1.5.tar", max compression
```

## Comparing `airbyte_source_pendo-0.1.4.tar` & `airbyte_source_pendo-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4478 2024-05-01 18:15:10.242268 airbyte_source_pendo-0.1.4/README.md
--rw-r--r--   0        0        0      737 2024-05-01 18:18:56.505369 airbyte_source_pendo-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      122 2024-05-01 18:15:10.242268 airbyte_source_pendo-0.1.4/source_pendo/__init__.py
--rw-r--r--   0        0        0   136461 2024-05-01 18:15:10.246268 airbyte_source_pendo-0.1.4/source_pendo/manifest.yaml
--rw-r--r--   0        0        0      227 2024-05-01 18:15:10.246268 airbyte_source_pendo-0.1.4/source_pendo/run.py
--rw-r--r--   0        0        0      474 2024-05-01 18:15:10.246268 airbyte_source_pendo-0.1.4/source_pendo/source.py
--rw-r--r--   0        0        0      310 2024-05-01 18:15:10.246268 airbyte_source_pendo-0.1.4/source_pendo/spec.yaml
--rw-r--r--   0        0        0     5179 1970-01-01 00:00:00.000000 airbyte_source_pendo-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     4488 2024-05-21 01:12:13.464731 airbyte_source_pendo-0.1.5/README.md
+-rw-r--r--   0        0        0      737 2024-05-21 01:16:22.170558 airbyte_source_pendo-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-21 01:12:13.464731 airbyte_source_pendo-0.1.5/source_pendo/__init__.py
+-rw-r--r--   0        0        0   121424 2024-05-21 01:12:13.464731 airbyte_source_pendo-0.1.5/source_pendo/manifest.yaml
+-rw-r--r--   0        0        0      227 2024-05-21 01:12:13.464731 airbyte_source_pendo-0.1.5/source_pendo/run.py
+-rw-r--r--   0        0        0      474 2024-05-21 01:12:13.464731 airbyte_source_pendo-0.1.5/source_pendo/source.py
+-rw-r--r--   0        0        0     5189 1970-01-01 00:00:00.000000 airbyte_source_pendo-0.1.5/PKG-INFO
```

### Comparing `airbyte_source_pendo-0.1.4/README.md` & `airbyte_source_pendo-0.1.5/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Pendo source connector
 
-
 This is the repository for the Pendo source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pendo).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/pendo)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pendo/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-pendo spec
 poetry run source-pendo check --config secrets/config.json
 poetry run source-pendo discover --config secrets/config.json
 poetry run source-pendo read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-pendo build
 ```
 
 An image will be available on your host with the tag `airbyte/source-pendo:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-pendo:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pendo:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pendo:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-pendo:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-pendo test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-pendo test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/pendo.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_pendo-0.1.4/pyproject.toml` & `airbyte_source_pendo-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.1.4"
+version = "0.1.5"
 name = "airbyte-source-pendo"
 description = "Source implementation for Pendo."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_pendo-0.1.4/source_pendo/manifest.yaml` & `airbyte_source_pendo-0.1.5/source_pendo/manifest.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,3588 +1,3520 @@
-version: 0.30.1
+version: 0.78.5
+
 type: DeclarativeSource
+
 check:
   type: CheckStream
   stream_names:
     - Account Metadata
+
+definitions:
+  streams:
+    Page:
+      type: DeclarativeStream
+      name: Page
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /page
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/Page"
+    Feature:
+      type: DeclarativeStream
+      name: Feature
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /feature
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/Feature"
+    Report:
+      type: DeclarativeStream
+      name: Report
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /report
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/Report"
+    Guide:
+      type: DeclarativeStream
+      name: Guide
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /guide
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/Guide"
+    Account Metadata:
+      type: DeclarativeStream
+      name: Account Metadata
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /metadata/schema/account
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/Account Metadata"
+    Visitor Metadata:
+      type: DeclarativeStream
+      name: Visitor Metadata
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /metadata/schema/visitor
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path: []
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/Visitor Metadata"
+  base_requester:
+    type: HttpRequester
+    url_base: https://app.pendo.io/api/v1
+    authenticator:
+      type: ApiKeyAuthenticator
+      api_token: "{{ config['api_key'] }}"
+      inject_into:
+        type: RequestOption
+        field_name: x-pendo-integration-key
+        inject_into: header
+
 streams:
-  - type: DeclarativeStream
-    name: Page
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
+  - $ref: "#/definitions/streams/Page"
+  - $ref: "#/definitions/streams/Feature"
+  - $ref: "#/definitions/streams/Report"
+  - $ref: "#/definitions/streams/Guide"
+  - $ref: "#/definitions/streams/Account Metadata"
+  - $ref: "#/definitions/streams/Visitor Metadata"
+
+spec:
+  type: Spec
+  connection_specification:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    required:
+      - api_key
+    properties:
+      api_key:
+        type: string
+        title: API Key
+        airbyte_secret: true
+        order: 0
+    additionalProperties: true
+
+metadata:
+  autoImportSchema:
+    Page: false
+    Feature: false
+    Report: false
+    Guide: false
+    Account Metadata: false
+    Visitor Metadata: false
+
+schemas:
+  Page:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      appId:
+        type: integer
+        description: The ID of the Pendo application to which the page belongs.
+      color:
+        type: string
+        description: The color associated with the page.
+      createdAt:
+        type: integer
+        description: The date and time when the page was created.
+      createdByUser:
         type: object
-        $schema: http://json-schema.org/schema#
+        description: Details about the user who created the page.
         properties:
-          id:
-            description: The unique ID of the page.
+          deletedAt:
+            type: integer
+            description: The date and time when the user was deleted.
+          first:
             type: string
-          kind:
-            description: The kind of page data.
+            description: The first name of the user.
+          hasLoggedIn:
+            type: boolean
+            description: Flag indicating if the user has logged in.
+          id:
             type: string
-          name:
-            description: The name of the page.
+            description: The unique ID of the user.
+          last:
             type: string
-          appId:
-            description: The ID of the Pendo application to which the page belongs.
+            description: The last name of the user.
+          lastLogin:
             type: integer
-          color:
-            description: The color associated with the page.
+            description: The date and time of the user's last login.
+          role:
+            type: integer
+            description: The role of the user.
+          userType:
             type: string
-          dirty:
-            description: Flag indicating if the page data is dirty or needs updating.
-            type: boolean
-          group:
-            description: Details about the group to which the page belongs.
-            type: object
-            properties:
-              id:
-                description: The unique ID of the group.
-                type: string
-              name:
-                description: The name of the group.
-                type: string
-              type:
-                description: The type of the group.
-                type: string
-              color:
-                description: The color associated with the group.
-                type: string
-              items:
-                description: An array of items belonging to the group.
-                type:
-                  - array
-                  - "null"
-              length:
-                description: The length of the group.
-                type: integer
-              createdAt:
-                description: The date and time when the group was created.
-                type: integer
-              description:
-                description: The description of the group.
-                type: string
-              createdByUser:
-                description: Details about the user who created the group.
-                type: object
-                properties:
-                  id:
-                    description: The unique ID of the user.
-                    type: string
-                  last:
-                    description: The last name of the user.
-                    type: string
-                  role:
-                    description: The role of the user.
-                    type: integer
-                  first:
-                    description: The first name of the user.
-                    type: string
-                  userType:
-                    description: The type of user.
-                    type: string
-                  username:
-                    description: The username of the user.
-                    type: string
-                  deletedAt:
-                    description: The date and time when the user was deleted.
-                    type: integer
-                  lastLogin:
-                    description: The date and time of the user's last login.
-                    type: integer
-                  visitorIds:
-                    description: An array of visitor IDs associated with the user.
-                    type: array
-                    items:
-                      description: An individual visitor ID.
-                      type: string
-                  hasLoggedIn:
-                    description: Flag indicating if the user has logged in.
-                    type: boolean
-              lastUpdatedAt:
-                description: The date and time of the last update to the group.
-                type: integer
-              lastUpdatedByUser:
-                description: Details about the user who last updated the group.
-                type: object
-                properties:
-                  id:
-                    description: The unique ID of the user.
-                    type: string
-                  last:
-                    description: The last name of the user.
-                    type: string
-                  role:
-                    description: The role of the user.
-                    type: integer
-                  first:
-                    description: The first name of the user.
-                    type: string
-                  userType:
-                    description: The type of user.
-                    type: string
-                  username:
-                    description: The username of the user.
-                    type: string
-                  lastLogin:
-                    description: The date and time of the user's last login.
-                    type: integer
-                  visitorIds:
-                    description: An array of visitor IDs associated with the user.
-                    type: array
-                    items:
-                      description: An individual visitor ID.
-                      type: string
-                  hasLoggedIn:
-                    description: Flag indicating if the user has logged in.
-                    type: boolean
-          rules:
-            description: Rules associated with the page.
+            description: The type of user.
+          username:
+            type: string
+            description: The username of the user.
+          visitorIds:
             type: array
+            description: An array of visitor IDs associated with the user.
             items:
-              description: Individual rule details.
-              type: object
-              properties:
-                rule:
-                  description: The rule definition.
-                  type: string
-                parsedRule:
-                  description: The parsed version of the rule.
-                  type: string
-                designerHint:
-                  description: The designer hint for the rule.
-                  type: string
-          createdAt:
-            description: The date and time when the page was created.
-            type: integer
-          rulesjson:
-            description: The JSON representation of rules associated with the page.
+              type: string
+              description: An individual visitor ID.
+      dailyMergeFirst:
+        type: integer
+        description: Placeholder for daily merge information.
+      dailyRollupFirst:
+        type: integer
+        description: Placeholder for daily rollup information.
+      dirty:
+        type: boolean
+        description: Flag indicating if the page data is dirty or needs updating.
+      group:
+        type: object
+        description: Details about the group to which the page belongs.
+        properties:
+          type:
             type: string
-          isCoreEvent:
-            description: Flag indicating if the page is a core event.
-            type: boolean
-          isAutoTagged:
-            description: Flag indicating if the page is automatically tagged.
-            type: boolean
-          validThrough:
-            description: The date until which the page data is valid.
+            description: The type of the group.
+          color:
+            type: string
+            description: The color associated with the group.
+          createdAt:
             type: integer
+            description: The date and time when the group was created.
           createdByUser:
-            description: Details about the user who created the page.
             type: object
+            description: Details about the user who created the group.
             properties:
+              deletedAt:
+                type: integer
+                description: The date and time when the user was deleted.
+              first:
+                type: string
+                description: The first name of the user.
+              hasLoggedIn:
+                type: boolean
+                description: Flag indicating if the user has logged in.
               id:
-                description: The unique ID of the user.
                 type: string
+                description: The unique ID of the user.
               last:
-                description: The last name of the user.
                 type: string
+                description: The last name of the user.
+              lastLogin:
+                type: integer
+                description: The date and time of the user's last login.
               role:
-                description: The role of the user.
                 type: integer
-              first:
-                description: The first name of the user.
-                type: string
+                description: The role of the user.
               userType:
-                description: The type of user.
                 type: string
+                description: The type of user.
               username:
-                description: The username of the user.
                 type: string
-              deletedAt:
-                description: The date and time when the user was deleted.
-                type: integer
-              lastLogin:
-                description: The date and time of the user's last login.
-                type: integer
+                description: The username of the user.
               visitorIds:
-                description: An array of visitor IDs associated with the user.
                 type: array
+                description: An array of visitor IDs associated with the user.
                 items:
-                  description: An individual visitor ID.
                   type: string
-              hasLoggedIn:
-                description: Flag indicating if the user has logged in.
-                type: boolean
-          lastUpdatedAt:
-            description: The date and time of the last update to the page.
-            type: integer
-          rootVersionId:
-            description: The ID of the root version of the page.
-            type: string
-          suggestedName:
-            description: The suggested name for the page.
+                  description: An individual visitor ID.
+          description:
             type: string
-          dailyMergeFirst:
-            description: Placeholder for daily merge information.
-            type: integer
-          stableVersionId:
-            description: The ID of the stable version of the page.
+            description: The description of the group.
+          id:
             type: string
-          dailyRollupFirst:
-            description: Placeholder for daily rollup information.
+            description: The unique ID of the group.
+          items:
+            type:
+              - array
+              - "null"
+            description: An array of items belonging to the group.
+          lastUpdatedAt:
             type: integer
+            description: The date and time of the last update to the group.
           lastUpdatedByUser:
-            description: Details about the user who last updated the page.
             type: object
+            description: Details about the user who last updated the group.
             properties:
+              first:
+                type: string
+                description: The first name of the user.
+              hasLoggedIn:
+                type: boolean
+                description: Flag indicating if the user has logged in.
               id:
-                description: The unique ID of the user.
                 type: string
+                description: The unique ID of the user.
               last:
-                description: The last name of the user.
                 type: string
+                description: The last name of the user.
+              lastLogin:
+                type: integer
+                description: The date and time of the user's last login.
               role:
-                description: The role of the user.
                 type: integer
-              first:
-                description: The first name of the user.
-                type: string
+                description: The role of the user.
               userType:
-                description: The type of user.
                 type: string
+                description: The type of user.
               username:
-                description: The username of the user.
                 type: string
-              deletedAt:
-                description: The date and time when the user was deleted.
-                type: integer
-              lastLogin:
-                description: The date and time of the user's last login.
-                type: integer
+                description: The username of the user.
               visitorIds:
-                description: An array of visitor IDs associated with the user.
                 type: array
+                description: An array of visitor IDs associated with the user.
                 items:
-                  description: An individual visitor ID.
                   type: string
-              hasLoggedIn:
-                description: Flag indicating if the user has logged in.
-                type: boolean
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://app.pendo.io/api/v1
-        path: /page
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        request_body_json: {}
-        authenticator:
-          type: ApiKeyAuthenticator
-          header: x-pendo-integration-key
-          api_token: "{{ config['api_key'] }}"
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: Feature
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
+                  description: An individual visitor ID.
+          length:
+            type: integer
+            description: The length of the group.
+          name:
+            type: string
+            description: The name of the group.
+      id:
+        type: string
+        description: The unique ID of the page.
+      isAutoTagged:
+        type: boolean
+        description: Flag indicating if the page is automatically tagged.
+      isCoreEvent:
+        type: boolean
+        description: Flag indicating if the page is a core event.
+      kind:
+        type: string
+        description: The kind of page data.
+      lastUpdatedAt:
+        type: integer
+        description: The date and time of the last update to the page.
+      lastUpdatedByUser:
         type: object
-        $schema: http://json-schema.org/schema#
+        description: Details about the user who last updated the page.
         properties:
+          deletedAt:
+            type: integer
+            description: The date and time when the user was deleted.
+          first:
+            type: string
+            description: The first name of the user.
+          hasLoggedIn:
+            type: boolean
+            description: Flag indicating if the user has logged in.
           id:
-            description: The unique identifier of the feature.
             type: string
-          kind:
-            description: The kind of feature.
+            description: The unique ID of the user.
+          last:
             type: string
-          name:
-            description: The name of the feature.
+            description: The last name of the user.
+          lastLogin:
+            type: integer
+            description: The date and time of the user's last login.
+          role:
+            type: integer
+            description: The role of the user.
+          userType:
+            type: string
+            description: The type of user.
+          username:
             type: string
-          appId:
-            description:
-              The unique identifier of the application to which the feature
-              belongs.
+            description: The username of the user.
+          visitorIds:
+            type: array
+            description: An array of visitor IDs associated with the user.
+            items:
+              type: string
+              description: An individual visitor ID.
+      name:
+        type: string
+        description: The name of the page.
+      rootVersionId:
+        type: string
+        description: The ID of the root version of the page.
+      rules:
+        type: array
+        description: Rules associated with the page.
+        items:
+          type: object
+          description: Individual rule details.
+          properties:
+            designerHint:
+              type: string
+              description: The designer hint for the rule.
+            parsedRule:
+              type: string
+              description: The parsed version of the rule.
+            rule:
+              type: string
+              description: The rule definition.
+      rulesjson:
+        type: string
+        description: The JSON representation of rules associated with the page.
+      stableVersionId:
+        type: string
+        description: The ID of the stable version of the page.
+      suggestedName:
+        type: string
+        description: The suggested name for the page.
+      validThrough:
+        type: integer
+        description: The date until which the page data is valid.
+    additionalProperties: true
+  Feature:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      appId:
+        type: integer
+        description: The unique identifier of the application to which the feature belongs.
+      appWide:
+        type: boolean
+        description: >-
+          Indicates whether the feature is applicable across the entire
+          application.
+      color:
+        type: string
+        description: The color associated with the feature for visual identification.
+      createdAt:
+        type: integer
+        description: The timestamp when the feature was created.
+      createdByUser:
+        type: object
+        description: Details of the user who created the feature.
+        properties:
+          deletedAt:
             type: integer
-          color:
-            description: The color associated with the feature for visual identification.
+            description: Timestamp when the user was deleted.
+          first:
             type: string
-          dirty:
-            description: Indicates if the feature is marked as 'dirty' for updates.
+            description: The first name of the user.
+          hasLoggedIn:
             type: boolean
-          group:
-            description: Details of the group to which the feature belongs.
-            type: object
-            properties:
-              id:
-                description: The unique identifier of the group.
-                type: string
-              name:
-                description: The name of the group.
-                type: string
-              type:
-                description: The type of the group.
-                type: string
-              color:
-                description: Color assigned to the group.
-                type: string
-              items:
-                description: Items included in the group.
-                type:
-                  - array
-                  - "null"
-              length:
-                description: The number of items in the group.
-                type: integer
-              createdAt:
-                description: Timestamp of group creation.
-                type: integer
-              description:
-                description: Description of the group.
-                type: string
-              createdByUser:
-                description: Details of the user who created the group.
-                type: object
-                properties:
-                  id:
-                    description: The unique identifier of the user.
-                    type: string
-                  last:
-                    description: The last name of the user.
-                    type: string
-                  role:
-                    description: The role of the user.
-                    type: integer
-                  first:
-                    description: The first name of the user.
-                    type: string
-                  userType:
-                    description: The type of user.
-                    type: string
-                  username:
-                    description: The username of the user.
-                    type: string
-                  deletedAt:
-                    description: Timestamp when the user was deleted.
-                    type: integer
-                  lastLogin:
-                    description: Timestamp of the user's last login.
-                    type: integer
-                  visitorIds:
-                    description: List of visitor identifiers associated with the user.
-                    type: array
-                    items:
-                      description: Unique identifier of a visitor.
-                      type: string
-                  hasLoggedIn:
-                    description: Flag indicating if the user has logged in.
-                    type: boolean
-              lastUpdatedAt:
-                description: Timestamp of the last group update.
-                type: integer
-              lastUpdatedByUser:
-                description: Details of the user who last updated the group.
-                type: object
-                properties:
-                  id:
-                    description: The unique identifier of the user.
-                    type: string
-                  last:
-                    description: The last name of the user.
-                    type: string
-                  role:
-                    description: The role of the user.
-                    type: integer
-                  first:
-                    description: The first name of the user.
-                    type: string
-                  userType:
-                    description: The type of user.
-                    type: string
-                  username:
-                    description: The username of the user.
-                    type: string
-                  lastLogin:
-                    description: Timestamp of the user's last login.
-                    type: integer
-                  visitorIds:
-                    description: List of visitor identifiers associated with the user.
-                    type: array
-                    items:
-                      description: Unique identifier of a visitor.
-                      type: string
-                  hasLoggedIn:
-                    description: Flag indicating if the user has logged in.
-                    type: boolean
-          pageId:
-            description: The unique identifier of the page associated with the feature.
+            description: Flag indicating if the user has logged in.
+          id:
             type: string
-          appWide:
-            description:
-              Indicates whether the feature is applicable across the entire
-              application.
-            type: boolean
-          createdAt:
-            description: The timestamp when the feature was created.
+            description: The unique identifier of the user.
+          last:
+            type: string
+            description: The last name of the user.
+          lastLogin:
             type: integer
-          isCoreEvent:
-            description: Indicates if the feature is a core event.
-            type: boolean
-          validThrough:
-            description: The timestamp until which the feature is valid.
+            description: Timestamp of the user's last login.
+          role:
             type: integer
+            description: The role of the user.
+          userType:
+            type: string
+            description: The type of user.
+          username:
+            type: string
+            description: The username of the user.
+          visitorIds:
+            type: array
+            description: List of visitor identifiers associated with the user.
+            items:
+              type: string
+              description: Unique identifier of a visitor.
+      createdDesignerVersion:
+        type: string
+        description: The version of the designer tool used during feature creation.
+      dailyMergeFirst:
+        type: integer
+        description: Timestamp of the first daily merge process for the feature.
+      dailyRollupFirst:
+        type: integer
+        description: Timestamp of the first daily rollup process for the feature.
+      dirty:
+        type: boolean
+        description: Indicates if the feature is marked as 'dirty' for updates.
+      elementInitialTag:
+        type: string
+        description: The initial tag associated with the feature element.
+      elementPathRules:
+        type: array
+        description: Rules defining the paths of elements associated with the feature.
+        items:
+          type: string
+          description: A specific path rule for element selection.
+      elementSelectionType:
+        type: string
+        description: Type of selection method used for elements.
+      eventPropertyConfigurations:
+        type: array
+        description: Configurations for event properties.
+        items:
+          type: object
+          description: Settings for a specific event property.
+          properties:
+            type:
+              type: string
+              description: The type of the property.
+            isActive:
+              type: boolean
+              description: Flag indicating if the property is active.
+            name:
+              type: string
+              description: The name of the property.
+            path:
+              type: string
+              description: The path associated with the property.
+            pattern:
+              type: string
+              description: Pattern used for property matching.
+            rule:
+              type: string
+              description: The rule applied to the property.
+            selector:
+              type: string
+              description: Selector for the property.
+      group:
+        type: object
+        description: Details of the group to which the feature belongs.
+        properties:
+          type:
+            type: string
+            description: The type of the group.
+          color:
+            type: string
+            description: Color assigned to the group.
+          createdAt:
+            type: integer
+            description: Timestamp of group creation.
           createdByUser:
-            description: Details of the user who created the feature.
             type: object
+            description: Details of the user who created the group.
             properties:
+              deletedAt:
+                type: integer
+                description: Timestamp when the user was deleted.
+              first:
+                type: string
+                description: The first name of the user.
+              hasLoggedIn:
+                type: boolean
+                description: Flag indicating if the user has logged in.
               id:
-                description: The unique identifier of the user.
                 type: string
+                description: The unique identifier of the user.
               last:
-                description: The last name of the user.
                 type: string
+                description: The last name of the user.
+              lastLogin:
+                type: integer
+                description: Timestamp of the user's last login.
               role:
-                description: The role of the user.
                 type: integer
-              first:
-                description: The first name of the user.
-                type: string
+                description: The role of the user.
               userType:
-                description: The type of user.
                 type: string
+                description: The type of user.
               username:
-                description: The username of the user.
                 type: string
-              deletedAt:
-                description: Timestamp when the user was deleted.
-                type: integer
-              lastLogin:
-                description: Timestamp of the user's last login.
-                type: integer
+                description: The username of the user.
               visitorIds:
-                description: List of visitor identifiers associated with the user.
                 type: array
+                description: List of visitor identifiers associated with the user.
                 items:
-                  description: Unique identifier of a visitor.
                   type: string
-              hasLoggedIn:
-                description: Flag indicating if the user has logged in.
-                type: boolean
-          lastUpdatedAt:
-            description: Timestamp of the last feature update.
-            type: integer
-          rootVersionId:
-            description: The unique identifier of the root version of the feature.
-            type: string
-          suggestedMatch:
-            description: Indicates if there is a suggested match for the feature.
+                  description: Unique identifier of a visitor.
+          description:
             type: string
-          dailyMergeFirst:
-            description: Timestamp of the first daily merge process for the feature.
-            type: integer
-          stableVersionId:
-            description: The unique identifier of the stable version of the feature.
+            description: Description of the group.
+          id:
             type: string
-          dailyRollupFirst:
-            description: Timestamp of the first daily rollup process for the feature.
+            description: The unique identifier of the group.
+          items:
+            type:
+              - array
+              - "null"
+            description: Items included in the group.
+          lastUpdatedAt:
             type: integer
-          elementPathRules:
-            description: Rules defining the paths of elements associated with the feature.
-            type: array
-            items:
-              description: A specific path rule for element selection.
-              type: string
-          elementInitialTag:
-            description: The initial tag associated with the feature element.
-            type: string
+            description: Timestamp of the last group update.
           lastUpdatedByUser:
-            description: Details of the user who last updated the feature.
             type: object
+            description: Details of the user who last updated the group.
             properties:
+              first:
+                type: string
+                description: The first name of the user.
+              hasLoggedIn:
+                type: boolean
+                description: Flag indicating if the user has logged in.
               id:
-                description: The unique identifier of the user.
                 type: string
+                description: The unique identifier of the user.
               last:
-                description: The last name of the user.
                 type: string
+                description: The last name of the user.
+              lastLogin:
+                type: integer
+                description: Timestamp of the user's last login.
               role:
-                description: The role of the user.
                 type: integer
-              first:
-                description: The first name of the user.
-                type: string
+                description: The role of the user.
               userType:
-                description: The type of user.
                 type: string
+                description: The type of user.
               username:
-                description: The username of the user.
                 type: string
-              deletedAt:
-                description: Timestamp when the user was deleted.
-                type: integer
-              lastLogin:
-                description: Timestamp of the user's last login.
-                type: integer
+                description: The username of the user.
               visitorIds:
-                description: List of visitor identifiers associated with the user.
                 type: array
+                description: List of visitor identifiers associated with the user.
                 items:
-                  description: Unique identifier of a visitor.
                   type: string
-              hasLoggedIn:
-                description: Flag indicating if the user has logged in.
-                type: boolean
-          elementSelectionType:
-            description: Type of selection method used for elements.
+                  description: Unique identifier of a visitor.
+          length:
+            type: integer
+            description: The number of items in the group.
+          name:
             type: string
-          createdDesignerVersion:
-            description: The version of the designer tool used during feature creation.
+            description: The name of the group.
+      id:
+        type: string
+        description: The unique identifier of the feature.
+      isCoreEvent:
+        type: boolean
+        description: Indicates if the feature is a core event.
+      kind:
+        type: string
+        description: The kind of feature.
+      lastUpdatedAt:
+        type: integer
+        description: Timestamp of the last feature update.
+      lastUpdatedByUser:
+        type: object
+        description: Details of the user who last updated the feature.
+        properties:
+          deletedAt:
+            type: integer
+            description: Timestamp when the user was deleted.
+          first:
+            type: string
+            description: The first name of the user.
+          hasLoggedIn:
+            type: boolean
+            description: Flag indicating if the user has logged in.
+          id:
+            type: string
+            description: The unique identifier of the user.
+          last:
+            type: string
+            description: The last name of the user.
+          lastLogin:
+            type: integer
+            description: Timestamp of the user's last login.
+          role:
+            type: integer
+            description: The role of the user.
+          userType:
+            type: string
+            description: The type of user.
+          username:
             type: string
-          eventPropertyConfigurations:
-            description: Configurations for event properties.
+            description: The username of the user.
+          visitorIds:
             type: array
+            description: List of visitor identifiers associated with the user.
+            items:
+              type: string
+              description: Unique identifier of a visitor.
+      name:
+        type: string
+        description: The name of the feature.
+      pageId:
+        type: string
+        description: The unique identifier of the page associated with the feature.
+      rootVersionId:
+        type: string
+        description: The unique identifier of the root version of the feature.
+      stableVersionId:
+        type: string
+        description: The unique identifier of the stable version of the feature.
+      suggestedMatch:
+        type: string
+        description: Indicates if there is a suggested match for the feature.
+      validThrough:
+        type: integer
+        description: The timestamp until which the feature is valid.
+    additionalProperties: true
+  Report:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      type:
+        type: string
+        description: The type or category of the report data.
+      aggregation:
+        type: object
+        description: Defines aggregations to be applied to the report data
+        properties:
+          fields:
+            type: array
+            description: List of fields to be aggregated
             items:
-              description: Settings for a specific event property.
               type: object
               properties:
-                name:
-                  description: The name of the property.
-                  type: string
-                path:
-                  description: The path associated with the property.
-                  type: string
-                rule:
-                  description: The rule applied to the property.
-                  type: string
                 type:
-                  description: The type of the property.
                   type: string
-                pattern:
-                  description: Pattern used for property matching.
+                  description: Data type of the field
+                field:
                   type: string
-                isActive:
-                  description: Flag indicating if the property is active.
-                  type: boolean
-                selector:
-                  description: Selector for the property.
+                  description: Name of the field to be aggregated
+                title:
                   type: string
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://app.pendo.io/api/v1
-        path: /feature
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        request_body_json: {}
-        authenticator:
-          type: ApiKeyAuthenticator
-          header: x-pendo-integration-key
-          api_token: "{{ config['api_key'] }}"
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: Report
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        type: object
-        $schema: http://json-schema.org/schema#
-        properties:
-          id:
-            description: Unique ID of the report
-            type: string
-          kind:
-            description: Kind of the report
-            type: string
-          name:
-            description: Name of the report
-            type: string
-          type:
-            description: The type or category of the report data.
-            type: string
-          level:
-            description: The level at which the report data is generated or accessed.
-            type: string
-          scope:
-            description: The scope or range of data to include in the report.
-            type: string
-          share:
-            description: Information about sharing settings or permissions for the report.
-            type: string
-          shared:
-            description: Flag indicating whether the report is shared with others.
-            type: boolean
-          target:
-            description: The target or audience for which the report is intended.
-            type: string
-          createdAt:
-            description: Timestamp when the report was created
-            type: integer
-          lastRunAt:
-            description: Timestamp of the last run of the report
-            type: integer
-          definition:
-            description: Definition of the report data structure
-            type: object
-            properties:
-              kind:
-                type: string
-              type:
-                type: string
-              config:
-                description: Configuration settings for the report
-                type: object
-                properties:
-                  appId:
-                    type:
-                      - integer
-                      - string
-                  pageId:
-                    type: string
-                  columns:
-                    description: Columns configuration
-                    type: array
-                    items:
+                  description: Title for the aggregated field
+          pipeline:
+            type: array
+            description: Defines the aggregation pipeline stages
+            items:
+              type: object
+              properties:
+                bulkExpand:
+                  type: object
+                  description: Stage to expand data for specified accounts or visitors
+                  properties:
+                    account:
                       type: object
+                      description: Details for expanding account data
                       properties:
-                        kind:
-                          type: string
-                        pageId:
-                          type: string
-                        pollId:
-                          type: string
-                        schema:
-                          type: string
-                        guideId:
-                          type: string
-                        disabled:
-                          type: boolean
-                        showIcon:
-                          type: boolean
-                        featureId:
-                          type: string
-                        fieldName:
-                          type: string
-                        immutable:
-                          type: boolean
-                        pollField:
-                          type: string
-                        columnName:
-                          type: string
-                        columnLabel:
+                        account:
                           type: string
-                        primaryKeys:
-                          type: array
-                          items:
-                            type: string
-                        functionName:
+                          description: Account ID
+                    visitor:
+                      type: object
+                      description: Details for expanding visitor data
+                      properties:
+                        visitor:
                           type: string
-                  filters:
-                    type: array
-                  features:
-                    type: boolean
-                  segments:
-                    type: array
-                  maxLength:
-                    type: integer
-                  omitPages:
-                    type: boolean
-                  segmentId:
-                    type: string
-                  acrossApps:
-                    type: boolean
-                  maxInterval:
-                    type: integer
-                  trackEvents:
-                    type: boolean
-                  collapseDups:
-                    type: boolean
-                  predecessors:
-                    type: boolean
-                  uniqueVisitors:
-                    type: boolean
-                  selectedAccount:
-                    description: Selected account settings
-                    type: object
-                    properties:
-                      id:
-                        type: string
-                      text:
-                        type: string
-                      className:
-                        type: string
-              period:
-                type: string
-              history:
-                type: array
-              minimum:
-                type: integer
-              sources:
-                description: Data sources settings
-                type: object
-                properties:
-                  alls:
-                    type: array
-                    items:
-                      type: string
-              segments:
-                type: array
-                items:
-                  type: string
-              attribute:
-                type: string
-              generator:
-                type: string
-              graphType:
-                type: string
-              tableType:
-                type: string
-              dateRanges:
-                description: Date range settings for the report
-                type: object
-                properties:
-                  primaryDateRange:
-                    type: object
-                    properties:
-                      type:
-                        type: string
-                  secondaryDateRange:
-                    type: "null"
-                  useSecondaryDateRange:
-                    type: boolean
-              timeSeries:
-                description: Time series settings for the report data
-                type: object
-                properties:
-                  end:
-                    type: string
-                  type:
-                    type: string
-                  start:
-                    type: string
-                  primaryTimeSeries:
-                    type: object
-                    properties:
-                      count:
-                        type: integer
-                      first:
-                        type: integer
-                      period:
-                        type: string
-                  secondaryTimeSeries:
-                    type: "null"
-              singleSource:
-                description: Settings for a single data source
-                type: object
-                properties:
-                  id:
-                    type: string
-                  kind:
-                    type: string
-              multiSourceType:
-                type: string
-              singleSourceType:
-                type: string
-              isComparingSources:
-                type: boolean
-              isComparingSegments:
-                type: boolean
-          aggregation:
-            description: Defines aggregations to be applied to the report data
-            type: object
-            properties:
-              fields:
-                description: List of fields to be aggregated
-                type: array
-                items:
+                          description: Visitor ID
+                eval:
                   type: object
+                  description: Stage to evaluate specific fields
                   properties:
-                    type:
-                      description: Data type of the field
+                    account_auto_id:
                       type: string
-                    field:
-                      description: Name of the field to be aggregated
+                      description: Auto-generated ID for the account
+                    visitor_agent_age:
                       type: string
-                    title:
-                      description: Title for the aggregated field
+                      description: Age of the visitor's agent
+                    visitor_agent_language:
                       type: string
-              pipeline:
-                description: Defines the aggregation pipeline stages
-                type: array
-                items:
-                  type: object
-                  properties:
-                    eval:
-                      description: Stage to evaluate specific fields
+                      description: Language used by the visitor's agent
+                    visitor_auto_firstvisit:
+                      type: string
+                      description: Auto-generated first visit timestamp
+                fork:
+                  type: array
+                  description: Stage to fork the pipeline
+                  items:
+                    type: array
+                    items:
                       type: object
                       properties:
-                        account_auto_id:
-                          description: Auto-generated ID for the account
-                          type: string
-                        visitor_agent_age:
-                          description: Age of the visitor's agent
-                          type: string
-                        visitor_agent_language:
-                          description: Language used by the visitor's agent
-                          type: string
-                        visitor_auto_firstvisit:
-                          description: Auto-generated first visit timestamp
-                          type: string
-                    fork:
-                      description: Stage to fork the pipeline
-                      type: array
-                      items:
-                        type: array
-                        items:
+                        eval:
                           type: object
+                          description: Evaluate specific conditions
                           properties:
-                            eval:
-                              description: Evaluate specific conditions
-                              type: object
-                              properties:
-                                items:
-                                  type: string
-                            group:
-                              description: Group data based on specified conditions
-                              type: object
-                              properties:
-                                group:
-                                  type: array
-                                  items:
-                                    type: string
-                                fields:
-                                  description: Fields for grouping
-                                  type: array
-                                  items:
+                            items:
+                              type: string
+                        group:
+                          type: object
+                          description: Group data based on specified conditions
+                          properties:
+                            fields:
+                              type: array
+                              description: Fields for grouping
+                              items:
+                                type: object
+                                properties:
+                                  count:
                                     type: object
+                                    description: Count of grouped items
                                     properties:
                                       count:
+                                        type:
+                                          - "null"
+                                          - string
                                         description: Count of grouped items
-                                        type: object
-                                        properties:
-                                          count:
-                                            description: Count of grouped items
-                                            type:
-                                              - "null"
-                                              - string
-                            limit:
-                              type: integer
-                            treeify:
-                              description: Treeify data based on specified keys
-                              type: object
-                              properties:
-                                keySort:
-                                  description: Key to sort the data tree
-                                  type: boolean
-                                threshold:
-                                  description: Threshold for treeifying the data
-                                  type: number
-                    group:
-                      description: Group data based on specified conditions
-                      type: object
-                      properties:
-                        group:
-                          type: array
-                          items:
-                            type: string
-                        fields:
-                          description: Fields for grouping data
-                          type: array
-                          items:
+                            group:
+                              type: array
+                              items:
+                                type: string
+                        limit:
+                          type: integer
+                        treeify:
+                          type: object
+                          description: Treeify data based on specified keys
+                          properties:
+                            keySort:
+                              type: boolean
+                              description: Key to sort the data tree
+                            threshold:
+                              type: number
+                              description: Threshold for treeifying the data
+                group:
+                  type: object
+                  description: Group data based on specified conditions
+                  properties:
+                    fields:
+                      type: array
+                      description: Fields for grouping data
+                      items:
+                        type: object
+                        properties:
+                          path:
                             type: object
+                            description: Path settings for grouping data
                             properties:
                               path:
-                                description: Path settings for grouping data
                                 type: object
+                                description: Path settings for grouping data
                                 properties:
-                                  path:
-                                    description: Path settings for grouping data
-                                    type: object
-                                    properties:
-                                      pageId:
-                                        description: ID of the page
-                                        type: string
-                                      features:
-                                        description: Features to consider
-                                        type: boolean
-                                      maxLength:
-                                        description: Maximum length of data
-                                        type: integer
-                                      omitPages:
-                                        description: Pages to omit from grouping
-                                        type: boolean
-                                      maxInterval:
-                                        description: Maximum interval allowed
-                                        type: integer
-                                      trackEvents:
-                                        description: Events to track
-                                        type: boolean
-                                      collapseDups:
-                                        description: Collapse duplicate entries
-                                        type: boolean
-                                      predecessors:
-                                        description: Predecessors to consider
-                                        type: boolean
-                                      followAcrossSessions:
-                                        description: Follow data across sessions
-                                        type: boolean
-                    merge:
-                      description: Merge data based on specified fields and mappings
+                                  collapseDups:
+                                    type: boolean
+                                    description: Collapse duplicate entries
+                                  features:
+                                    type: boolean
+                                    description: Features to consider
+                                  followAcrossSessions:
+                                    type: boolean
+                                    description: Follow data across sessions
+                                  maxInterval:
+                                    type: integer
+                                    description: Maximum interval allowed
+                                  maxLength:
+                                    type: integer
+                                    description: Maximum length of data
+                                  omitPages:
+                                    type: boolean
+                                    description: Pages to omit from grouping
+                                  pageId:
+                                    type: string
+                                    description: ID of the page
+                                  predecessors:
+                                    type: boolean
+                                    description: Predecessors to consider
+                                  trackEvents:
+                                    type: boolean
+                                    description: Events to track
+                    group:
+                      type: array
+                      items:
+                        type: string
+                identified:
+                  type: string
+                merge:
+                  type: object
+                  description: Merge data based on specified fields and mappings
+                  properties:
+                    fields:
+                      type: array
+                      items:
+                        type: string
+                    mappings:
                       type: object
+                      additionalProperties: true
+                      description: Field mappings for merging data
                       properties:
-                        fields:
-                          type: array
-                          items:
+                        daysActive:
+                          type: string
+                        usageTrending:
+                          type: string
+                    pipeline:
+                      type: array
+                      description: Pipeline stages for merging
+                      items:
+                        type: object
+                        properties:
+                          cat:
+                            type: "null"
+                          eval:
+                            type: object
+                            description: Evaluate usage trending data
+                            properties:
+                              usageTrending:
+                                type: string
+                          filter:
                             type: string
-                        mappings:
-                          description: Field mappings for merging data
-                          type: object
-                          properties:
-                            daysActive:
-                              type: string
-                            usageTrending:
-                              type: string
-                          additionalProperties: true
-                        pipeline:
-                          description: Pipeline stages for merging
-                          type: array
-                          items:
+                          group:
+                            type: object
+                            description: Group data for merging
+                            properties:
+                              fields:
+                                type: array
+                                description: Fields for grouping
+                                items:
+                                  type: object
+                                  additionalProperties: true
+                                  properties:
+                                    daysActive:
+                                      type: object
+                                      description: Days active count
+                                      properties:
+                                        count:
+                                          type: string
+                                          description: Count of days active
+                              group:
+                                type: array
+                                items:
+                                  type: string
+                          identified:
+                            type: string
+                          join:
+                            type: object
+                            properties:
+                              fields:
+                                type: array
+                                items:
+                                  type: string
+                          segment:
                             type: object
+                            description: Segment ID for merging data
                             properties:
-                              cat:
-                                type: "null"
-                              eval:
-                                description: Evaluate usage trending data
+                              id:
+                                type: string
+                                description: Segment ID
+                          source:
+                            type: object
+                            description: Source settings for merging data
+                            properties:
+                              events:
                                 type: object
+                                description: Data events settings
                                 properties:
-                                  usageTrending:
+                                  appId:
+                                    type: string
+                                  blacklist:
                                     type: string
-                              join:
+                              featureEvents:
                                 type: object
+                                description: Feature events settings
                                 properties:
-                                  fields:
-                                    type: array
-                                    items:
-                                      type: string
-                              group:
-                                description: Group data for merging
+                                  blacklist:
+                                    type: string
+                                  featureId:
+                                    type: string
+                              guideEvents:
                                 type: object
+                                description: Guide events settings
                                 properties:
-                                  group:
-                                    type: array
-                                    items:
-                                      type: string
-                                  fields:
-                                    description: Fields for grouping
-                                    type: array
-                                    items:
-                                      type: object
-                                      properties:
-                                        daysActive:
-                                          description: Days active count
-                                          type: object
-                                          properties:
-                                            count:
-                                              description: Count of days active
-                                              type: string
-                                      additionalProperties: true
-                              spawn:
-                                description: Spawn data based on specified conditions
-                                type: array
-                                items:
-                                  type: array
-                                  items:
-                                    type: object
-                                    properties:
-                                      group:
-                                        description: Group data
-                                        type: object
-                                        properties:
-                                          group:
-                                            type: array
-                                            items:
-                                              type: string
-                                          fields:
-                                            description: Fields for grouping
-                                            type: array
-                                            items:
-                                              type: object
-                                              properties:
-                                                totalTime:
-                                                  description: Total time settings
-                                                  type: object
-                                                  properties:
-                                                    sum:
-                                                      type: string
-                                                prevTotalTime:
-                                                  description: Previous total time settings
-                                                  type: object
-                                                  properties:
-                                                    sum:
-                                                      type: string
-                                      source:
-                                        description: Data source settings
-                                        type: object
-                                        properties:
-                                          events:
-                                            description: Data events settings
-                                            type: object
-                                            properties:
-                                              appId:
-                                                type:
-                                                  - integer
-                                                  - string
-                                              blacklist:
-                                                type: string
-                                          timeSeries:
-                                            description: Time series settings
-                                            type: object
-                                            properties:
-                                              last:
-                                                type: string
-                                              first:
-                                                type: string
-                                              period:
-                                                type: string
-                                      identified:
-                                        type: string
-                              filter:
-                                type: string
-                              source:
-                                description: Source settings for merging data
+                                  blacklist:
+                                    type: string
+                                  guideId:
+                                    type: string
+                              pageEvents:
                                 type: object
+                                description: Page events settings
                                 properties:
-                                  events:
-                                    description: Data events settings
-                                    type: object
-                                    properties:
-                                      appId:
-                                        type: string
-                                      blacklist:
-                                        type: string
-                                  pollsSeen:
-                                    description: Settings for seen polls
-                                    type: object
-                                    properties:
-                                      pollId:
-                                        type: string
-                                      guideId:
-                                        type: string
-                                      blacklist:
-                                        type: string
-                                  pageEvents:
-                                    description: Page events settings
-                                    type: object
-                                    properties:
-                                      pageId:
-                                        type: string
-                                      blacklist:
-                                        type: string
-                                  timeSeries:
-                                    description: Time series settings
-                                    type: object
-                                    properties:
-                                      last:
-                                        type: string
-                                      first:
-                                        type: string
-                                      period:
-                                        type: string
-                                  guideEvents:
-                                    description: Guide events settings
-                                    type: object
-                                    properties:
-                                      guideId:
-                                        type: string
-                                      blacklist:
-                                        type: string
-                                  featureEvents:
-                                    description: Feature events settings
-                                    type: object
-                                    properties:
-                                      blacklist:
-                                        type: string
-                                      featureId:
-                                        type: string
-                                  pollsSeenEver:
-                                    description: Settings for seen polls across sessions
-                                    type: object
-                                    properties:
-                                      pollId:
-                                        type: string
-                                      guideId:
-                                        type: string
-                                      blacklist:
-                                        type: string
-                              switch:
-                                description: Switch response based on conditions
+                                  blacklist:
+                                    type: string
+                                  pageId:
+                                    type: string
+                              pollsSeen:
                                 type: object
+                                description: Settings for seen polls
                                 properties:
-                                  response:
-                                    description: Response settings
+                                  blacklist:
+                                    type: string
+                                  guideId:
+                                    type: string
+                                  pollId:
+                                    type: string
+                              pollsSeenEver:
+                                type: object
+                                description: Settings for seen polls across sessions
+                                properties:
+                                  blacklist:
+                                    type: string
+                                  guideId:
+                                    type: string
+                                  pollId:
+                                    type: string
+                              timeSeries:
+                                type: object
+                                description: Time series settings
+                                properties:
+                                  first:
+                                    type: string
+                                  last:
+                                    type: string
+                                  period:
+                                    type: string
+                          spawn:
+                            type: array
+                            description: Spawn data based on specified conditions
+                            items:
+                              type: array
+                              items:
+                                type: object
+                                properties:
+                                  group:
                                     type: object
+                                    description: Group data
                                     properties:
-                                      response:
+                                      fields:
                                         type: array
+                                        description: Fields for grouping
                                         items:
                                           type: object
                                           properties:
-                                            "==":
-                                              type: integer
-                                            value:
-                                              type: string
-                              segment:
-                                description: Segment ID for merging data
+                                            prevTotalTime:
+                                              type: object
+                                              description: Previous total time settings
+                                              properties:
+                                                sum:
+                                                  type: string
+                                            totalTime:
+                                              type: object
+                                              description: Total time settings
+                                              properties:
+                                                sum:
+                                                  type: string
+                                      group:
+                                        type: array
+                                        items:
+                                          type: string
+                                  identified:
+                                    type: string
+                                  source:
+                                    type: object
+                                    description: Data source settings
+                                    properties:
+                                      events:
+                                        type: object
+                                        description: Data events settings
+                                        properties:
+                                          appId:
+                                            type:
+                                              - integer
+                                              - string
+                                          blacklist:
+                                            type: string
+                                      timeSeries:
+                                        type: object
+                                        description: Time series settings
+                                        properties:
+                                          first:
+                                            type: string
+                                          last:
+                                            type: string
+                                          period:
+                                            type: string
+                          switch:
+                            type: object
+                            description: Switch response based on conditions
+                            properties:
+                              response:
                                 type: object
+                                description: Response settings
                                 properties:
-                                  id:
-                                    description: Segment ID
-                                    type: string
-                              identified:
-                                type: string
-                    select:
-                      description: Select fields for the report data
+                                  response:
+                                    type: array
+                                    items:
+                                      type: object
+                                      properties:
+                                        "==":
+                                          type: integer
+                                        value:
+                                          type: string
+                segment:
+                  type: object
+                  description: Segment ID for filtering data
+                  properties:
+                    id:
+                      type: string
+                      description: Segment ID
+                select:
+                  type: object
+                  additionalProperties: true
+                  description: Select fields for the report data
+                  properties:
+                    accountId:
+                      type: string
+                    account_auto_id:
+                      type: string
+                    daysActive:
+                      type: string
+                    usageTrending:
+                      type: string
+                    visitorId:
+                      type: string
+                    visitor_agent_age:
+                      type: string
+                    visitor_agent_language:
+                      type: string
+                    visitor_auto_firstvisit:
+                      type: string
+                source:
+                  type: object
+                  description: Source settings for the report data
+                  properties:
+                    events:
                       type: object
+                      description: Event settings
                       properties:
-                        accountId:
-                          type: string
-                        visitorId:
-                          type: string
-                        daysActive:
-                          type: string
-                        usageTrending:
-                          type: string
-                        account_auto_id:
-                          type: string
-                        visitor_agent_age:
-                          type: string
-                        visitor_agent_language:
-                          type: string
-                        visitor_auto_firstvisit:
+                        appId:
+                          type:
+                            - integer
+                            - string
+                        blacklist:
                           type: string
-                      additionalProperties: true
-                    source:
-                      description: Source settings for the report data
+                    singleEvents:
                       type: object
+                      description: Settings for single events
                       properties:
-                        events:
-                          description: Event settings
-                          type: object
-                          properties:
-                            appId:
-                              type:
-                                - integer
-                                - string
-                            blacklist:
-                              type: string
-                        timeSeries:
-                          description: Time series settings
-                          type: object
-                          properties:
-                            last:
-                              type: string
-                            count:
-                              type: integer
-                            first:
-                              type:
-                                - integer
-                                - string
-                            period:
-                              type: string
-                        singleEvents:
-                          description: Settings for single events
-                          type: object
-                          properties:
-                            appId:
-                              type: integer
-                            blacklist:
-                              type: string
-                            eventClass:
-                              type: array
-                              items:
-                                type: string
-                            reverseTime:
-                              type: boolean
-                    unwind:
-                      description: Unwind specified field
-                      type: object
-                      properties:
-                        field:
-                          description: Field to unwind
+                        appId:
+                          type: integer
+                        blacklist:
                           type: string
-                    segment:
-                      description: Segment ID for filtering data
+                        eventClass:
+                          type: array
+                          items:
+                            type: string
+                        reverseTime:
+                          type: boolean
+                    timeSeries:
                       type: object
+                      description: Time series settings
                       properties:
-                        id:
-                          description: Segment ID
+                        count:
+                          type: integer
+                        first:
+                          type:
+                            - integer
+                            - string
+                        last:
                           type: string
-                    bulkExpand:
-                      description: Stage to expand data for specified accounts or visitors
-                      type: object
-                      properties:
-                        account:
-                          description: Details for expanding account data
-                          type: object
-                          properties:
-                            account:
-                              description: Account ID
-                              type: string
-                        visitor:
-                          description: Details for expanding visitor data
-                          type: object
-                          properties:
-                            visitor:
-                              description: Visitor ID
-                              type: string
-                    identified:
+                        period:
+                          type: string
+                unwind:
+                  type: object
+                  description: Unwind specified field
+                  properties:
+                    field:
                       type: string
-          ownedByUser:
-            description: User who owns the report
-            type: object
-            properties:
-              id:
-                type: string
-              last:
-                type: string
-              role:
-                type: integer
-              first:
-                type: string
-              userType:
-                type: string
-              username:
-                type: string
-              hasLoggedIn:
-                type: boolean
-          createdByUser:
-            description: User who created the report
-            type: object
-            properties:
-              id:
-                type: string
-              last:
-                type: string
-              role:
-                type: integer
-              first:
-                type: string
-              userType:
-                type: string
-              username:
-                type: string
-              deletedAt:
-                type: integer
-              lastLogin:
-                type: integer
-              visitorIds:
-                type: array
-                items:
-                  type: string
-              hasLoggedIn:
-                type: boolean
-          lastUpdatedAt:
-            description: Timestamp of the last update of the report
-            type: integer
-          rootVersionId:
-            description: The identifier for the root version of the report.
-            type: string
-          stableVersionId:
-            description: The identifier for the stable version of the report.
-            type: string
-          lastSuccessRunAt:
-            description: Timestamp of the last successful run of the report
-            type: integer
-          lastSuccessRunObj:
-            description:
-              The object containing information about the last successful
-              run.
-            type: string
-          lastUpdatedByUser:
-            description: User who last updated the report
-            type: object
-            properties:
-              id:
-                type: string
-              last:
-                type: string
-              role:
-                type: integer
-              first:
-                type: string
-              userType:
-                type: string
-              username:
-                type: string
-              deletedAt:
-                type: integer
-              lastLogin:
-                type: integer
-              visitorIds:
-                type: array
-                items:
-                  type: string
-              hasLoggedIn:
-                type: boolean
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://app.pendo.io/api/v1
-        path: /report
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        request_body_json: {}
-        authenticator:
-          type: ApiKeyAuthenticator
-          header: x-pendo-integration-key
-          api_token: "{{ config['api_key'] }}"
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: Guide
-    primary_key:
-      - id
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
+                      description: Field to unwind
+      createdAt:
+        type: integer
+        description: Timestamp when the report was created
+      createdByUser:
         type: object
-        $schema: http://json-schema.org/schema#
+        description: User who created the report
         properties:
-          id:
-            description: Unique identifier of the guide.
+          deletedAt:
+            type: integer
+          first:
             type: string
-          kind:
-            description: Type or category of the guide.
+          hasLoggedIn:
+            type: boolean
+          id:
             type: string
-          name:
-            description: Name of the guide.
+          last:
             type: string
-          appId:
-            description:
-              The unique identifier of the application associated with the
-              guide data.
+          lastLogin:
             type: integer
-          polls:
-            description: Poll questions and related details for the guide.
-            type: array
-            items:
-              type: object
-              properties:
-                id:
-                  type: string
-                resetAt:
-                  type: integer
-                question:
-                  type: string
-                attributes:
-                  type: object
-                  properties:
-                    type:
-                      type: string
-                    display:
-                      type: string
-                    followUp:
-                      type: string
-                    leftLabel:
-                      type: string
-                    rightLabel:
-                      type: string
-                idResponses:
-                  type: object
-                  additionalProperties: true
-                numericResponses:
-                  type: array
-                  items:
-                    type: integer
-          state:
-            description: Current state of the guide.
+          role:
+            type: integer
+          userType:
             type: string
-          steps:
-            description: Steps or sequences within the guide.
+          username:
+            type: string
+          visitorIds:
             type: array
             items:
-              type: object
-              properties:
-                id:
-                  type: string
-                name:
-                  type: string
-                rank:
-                  type: integer
+              type: string
+      definition:
+        type: object
+        description: Definition of the report data structure
+        properties:
+          type:
+            type: string
+          attribute:
+            type: string
+          config:
+            type: object
+            description: Configuration settings for the report
+            properties:
+              acrossApps:
+                type: boolean
+              appId:
                 type:
-                  type: string
-                domUrl:
-                  type: string
-                pageId:
-                  type: string
-                guideId:
-                  type: string
-                pollIds:
-                  type: array
-                  items:
-                    type: string
-                resetAt:
-                  type: integer
-                launchUrl:
-                  type: string
-                attributes:
-                  description: Attributes and configurations for the step.
+                  - integer
+                  - string
+              collapseDups:
+                type: boolean
+              columns:
+                type: array
+                description: Columns configuration
+                items:
                   type: object
                   properties:
-                    id:
-                      type: string
-                    css:
-                      type: string
-                    html:
+                    columnLabel:
                       type: string
-                    type:
+                    columnName:
                       type: string
-                    color:
-                      type: string
-                    title:
-                      type: string
-                    width:
-                      type: integer
-                    device:
-                      description: Device-specific configurations for the step.
-                      type: object
-                      properties:
-                        iframe:
-                          type: boolean
-                        mobile:
-                          type: boolean
-                        desktop:
-                          type: boolean
-                    height:
-                      type: integer
-                    enabled:
-                      description: Indicates if the step is enabled.
+                    disabled:
                       type: boolean
-                    themeId:
+                    featureId:
                       type: string
-                    position:
+                    fieldName:
                       type: string
-                    template:
+                    functionName:
                       type: string
-                    layoutDir:
+                    guideId:
                       type: string
-                    variables:
-                      description: Variables and settings for the step.
-                      type: object
-                      properties:
-                        company:
-                          type: string
-                        followUpType:
-                          type: string
-                        successMessage:
-                          type: string
-                        followUpNeutral:
-                          type: string
-                        followUpPromoter:
-                          type: string
-                        followUpStandard:
-                          type: string
-                        followUpDetractor:
-                          type: string
-                        enableSuccessMessage:
-                          type: boolean
-                        receivesRecommendation:
-                          type: string
-                    autoHeight:
-                      description: Indicates if the guide height adjusts automatically.
+                    immutable:
                       type: boolean
-                    blockOutUI:
-                      description: UI blocking settings for the guide.
-                      type: object
-                      properties:
-                        enabled:
-                          type: boolean
-                        padding:
-                          type: object
-                          properties:
-                            top:
-                              type: integer
-                            left:
-                              type: integer
-                            right:
-                              type: integer
-                            bottom:
-                              type: integer
-                        additionalElements:
-                          type: string
-                    javascript:
-                      type: string
-                    guideCssUrl:
+                    kind:
                       type: string
-                    isAutoFocus:
-                      description: Indicates if autofocus is enabled on the step.
-                      type: boolean
-                    templateName:
+                    pageId:
                       type: string
-                    advanceActions:
-                      description:
-                        Actions to be performed when advancing to the next
-                        step.
-                      anyOf:
-                        - type: "null"
-                        - type: object
-                          properties:
-                            elementClick:
-                              type: boolean
-                            elementHover:
-                              type: boolean
-                    contentHostUrl:
+                    pollField:
                       type: string
-                    launcherBadgeUrl:
+                    pollId:
                       type: string
-                    elementSelectionType:
-                      description: Type of selection for elements on the step.
+                    primaryKeys:
+                      type: array
+                      items:
+                        type: string
+                    schema:
                       type: string
-                contentUrl:
-                  type: string
-                templateId:
-                  type: string
-                contentType:
-                  type: string
-                domJsonpUrl:
-                  type: string
-                contentUrlJs:
-                  type: string
-                regexUrlRule:
-                  type: string
-                advanceMethod:
-                  description: Method used to advance to the next step.
-                  type: string
-                contentUrlCss:
-                  type: string
-                lastUpdatedAt:
-                  type: integer
-                elementPathRule:
-                  type: string
-                buildingBlocksUrl:
-                  type: string
-                triggerElementPathRule:
-                  type: string
-                confirmationElementPathRule:
-                  type: string
-          appIds:
-            description:
-              An array of identifiers for multiple applications associated
-              with the guide data.
+                    showIcon:
+                      type: boolean
+              features:
+                type: boolean
+              filters:
+                type: array
+              maxInterval:
+                type: integer
+              maxLength:
+                type: integer
+              omitPages:
+                type: boolean
+              pageId:
+                type: string
+              predecessors:
+                type: boolean
+              segmentId:
+                type: string
+              segments:
+                type: array
+              selectedAccount:
+                type: object
+                description: Selected account settings
+                properties:
+                  className:
+                    type: string
+                  id:
+                    type: string
+                  text:
+                    type: string
+              trackEvents:
+                type: boolean
+              uniqueVisitors:
+                type: boolean
+          dateRanges:
+            type: object
+            description: Date range settings for the report
+            properties:
+              primaryDateRange:
+                type: object
+                properties:
+                  type:
+                    type: string
+              secondaryDateRange:
+                type: "null"
+              useSecondaryDateRange:
+                type: boolean
+          generator:
+            type: string
+          graphType:
+            type: string
+          history:
             type: array
-            items:
-              type: integer
-          resetAt:
-            description: Timestamp indicating when the guide is reset.
+          isComparingSegments:
+            type: boolean
+          isComparingSources:
+            type: boolean
+          kind:
+            type: string
+          minimum:
             type: integer
-          audience:
-            description: Audience details and criteria for targeting the guide.
+          multiSourceType:
+            type: string
+          period:
+            type: string
+          segments:
             type: array
             items:
-              type: object
-              properties:
-                eval:
-                  type: object
-                  properties:
-                    accountId:
-                      description: Unique identifier of the account for audience evaluation.
-                      type: string
-                filter:
-                  description: Filter criteria for defining the target audience.
-                  type: string
-                select:
-                  description: Selection criteria for the audience.
-                  type: object
-                  properties:
-                    visitorId:
-                      description: Visitor identifier for audience selection.
-                      type: string
-                source:
-                  description: Source details for the audience.
-                  type: object
-                  properties:
-                    visitors:
-                      anyOf:
-                        - type: "null"
-                        - type: object
-                          properties:
-                            identified:
-                              type: boolean
-                unwind:
-                  description: Criteria for unwinding audience data.
-                  type: object
-                  properties:
-                    field:
-                      type: string
-                    keepEmpty:
-                      type: boolean
-                segment:
-                  description: Segment details for audience targeting.
-                  type: object
-                  properties:
-                    id:
-                      description: Identifier of the audience segment.
-                      type: string
-                identified:
-                  description: Indicates if the audience is identified.
+              type: string
+          singleSource:
+            type: object
+            description: Settings for a single data source
+            properties:
+              id:
+                type: string
+              kind:
+                type: string
+          singleSourceType:
+            type: string
+          sources:
+            type: object
+            description: Data sources settings
+            properties:
+              alls:
+                type: array
+                items:
                   type: string
-          children:
-            description: Child guides associated with the main guide.
+          tableType:
+            type: string
+          timeSeries:
+            type: object
+            description: Time series settings for the report data
+            properties:
+              type:
+                type: string
+              end:
+                type: string
+              primaryTimeSeries:
+                type: object
+                properties:
+                  count:
+                    type: integer
+                  first:
+                    type: integer
+                  period:
+                    type: string
+              secondaryTimeSeries:
+                type: "null"
+              start:
+                type: string
+      id:
+        type: string
+        description: Unique ID of the report
+      kind:
+        type: string
+        description: Kind of the report
+      lastRunAt:
+        type: integer
+        description: Timestamp of the last run of the report
+      lastSuccessRunAt:
+        type: integer
+        description: Timestamp of the last successful run of the report
+      lastSuccessRunObj:
+        type: string
+        description: The object containing information about the last successful run.
+      lastUpdatedAt:
+        type: integer
+        description: Timestamp of the last update of the report
+      lastUpdatedByUser:
+        type: object
+        description: User who last updated the report
+        properties:
+          deletedAt:
+            type: integer
+          first:
+            type: string
+          hasLoggedIn:
+            type: boolean
+          id:
+            type: string
+          last:
+            type: string
+          lastLogin:
+            type: integer
+          role:
+            type: integer
+          userType:
+            type: string
+          username:
+            type: string
+          visitorIds:
             type: array
             items:
               type: string
-          isModule:
-            description: Indicates if the guide is a module.
+      level:
+        type: string
+        description: The level at which the report data is generated or accessed.
+      name:
+        type: string
+        description: Name of the report
+      ownedByUser:
+        type: object
+        description: User who owns the report
+        properties:
+          first:
+            type: string
+          hasLoggedIn:
             type: boolean
-          originId:
-            description: Original identifier of the guide.
+          id:
             type: string
-          createdAt:
-            description: Timestamp indicating when the guide was created.
+          last:
+            type: string
+          role:
             type: integer
-          attributes:
-            description: Additional attributes and configurations for the guide.
-            type: object
-            properties:
-              dom:
-                description: DOM behavior settings for the guide.
-                type: object
+          userType:
+            type: string
+          username:
+            type: string
+      rootVersionId:
+        type: string
+        description: The identifier for the root version of the report.
+      scope:
+        type: string
+        description: The scope or range of data to include in the report.
+      share:
+        type: string
+        description: Information about sharing settings or permissions for the report.
+      shared:
+        type: boolean
+        description: Flag indicating whether the report is shared with others.
+      stableVersionId:
+        type: string
+        description: The identifier for the stable version of the report.
+      target:
+        type: string
+        description: The target or audience for which the report is intended.
+    additionalProperties: true
+  Guide:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      appId:
+        type: integer
+        description: >-
+          The unique identifier of the application associated with the guide
+          data.
+      appIds:
+        type: array
+        description: >-
+          An array of identifiers for multiple applications associated with the
+          guide data.
+        items:
+          type: integer
+      attributes:
+        type: object
+        description: Additional attributes and configurations for the guide.
+        properties:
+          type:
+            type: string
+            description: Type of guide.
+          activation:
+            anyOf:
+              - type: "null"
+              - type: object
                 properties:
-                  isOnlyShowOnce:
-                    description: Indicates if the guide should be shown only once.
-                    type: boolean
-                  showGuideOnlyOnElementClick:
-                    description:
-                      Specifies if the guide is triggered by clicking on
-                      an element.
+                  event:
+                    type: array
+                    items:
+                      type: string
+                  inheritStepOne:
                     type: boolean
-              type:
-                description: Type of guide.
-                type: string
-              badge:
-                description: Badge details associated with the guide.
-                anyOf:
-                  - type: "null"
-                  - type: object
+                  selector:
+                    type: string
+            description: Information related to guide activation.
+          badge:
+            anyOf:
+              - type: "null"
+              - type: object
+                properties:
+                  bbJson:
+                    type: object
                     properties:
-                      name:
-                        type: string
-                      color:
+                      actions:
+                        type: array
+                      id:
                         type: string
-                      width:
-                        type: integer
-                      bbJson:
+                      layoutId:
+                        type: "null"
+                      properties:
+                        type: array
+                        items:
+                          type: object
+                          properties:
+                            type:
+                              type: string
+                            name:
+                              type: string
+                            value:
+                              type:
+                                - integer
+                                - string
+                      templateName:
+                        type: "null"
+                      uiMetadata:
                         type: object
                         properties:
-                          id:
+                          name:
                             type: string
-                          web:
+                          wizard:
                             type: object
                             properties:
-                              type:
-                                type: string
-                              domId:
-                                type: string
-                              layout:
-                                type: string
-                              ariaLabel:
-                                type: string
-                              domClasses:
-                                type: array
-                              semanticTag:
-                                type: string
-                              ariaExpanded:
-                                type: string
-                              pseudoStyles:
-                                type: array
-                              translationId:
-                                type: string
-                          views:
-                            type: array
-                            items:
+                              defaultActions:
+                                type: object
+                              defaultValues:
+                                type: object
+                      views:
+                        type: array
+                        items:
+                          type: object
+                          properties:
+                            actions:
+                              type: array
+                            id:
+                              type: string
+                            layoutId:
+                              type: "null"
+                            properties:
+                              type: array
+                              items:
+                                type: object
+                                properties:
+                                  type:
+                                    type: string
+                                  name:
+                                    type: string
+                                  value:
+                                    type:
+                                      - integer
+                                      - string
+                            templateName:
+                              type: "null"
+                            uiMetadata:
                               type: object
                               properties:
-                                id:
+                                name:
                                   type: string
-                                web:
+                                wizard:
                                   type: object
                                   properties:
-                                    type:
-                                      type: string
-                                    domId:
-                                      type: string
-                                    altText:
-                                      type: string
-                                    wrapper:
+                                    defaultActions:
                                       type: object
-                                      properties:
-                                        type:
-                                          type: string
-                                        props:
-                                          type: object
-                                          properties:
-                                            id:
-                                              type: string
-                                            class:
-                                              type: string
-                                            data-img-id:
-                                              type: string
-                                        children:
-                                          type: array
-                                    domClasses:
-                                      type: array
-                                    semanticTag:
-                                      type: string
-                                    pseudoStyles:
-                                      type: array
-                                    translationId:
-                                      type: string
-                                views:
-                                  type: array
-                                widget:
+                                    defaultValues:
+                                      type: object
+                            views:
+                              type: array
+                            web:
+                              type: object
+                              properties:
+                                type:
+                                  type: string
+                                altText:
                                   type: string
-                                actions:
+                                domClasses:
                                   type: array
-                                layoutId:
-                                  type: "null"
-                                properties:
+                                domId:
+                                  type: string
+                                pseudoStyles:
                                   type: array
-                                  items:
-                                    type: object
-                                    properties:
-                                      name:
-                                        type: string
-                                      type:
-                                        type: string
-                                      value:
-                                        type:
-                                          - integer
-                                          - string
-                                uiMetadata:
+                                semanticTag:
+                                  type: string
+                                translationId:
+                                  type: string
+                                wrapper:
                                   type: object
                                   properties:
-                                    name:
+                                    type:
                                       type: string
-                                    wizard:
+                                    children:
+                                      type: array
+                                    props:
                                       type: object
                                       properties:
-                                        defaultValues:
-                                          type: object
-                                        defaultActions:
-                                          type: object
-                                templateName:
-                                  type: "null"
-                          widget:
-                            type: string
-                          actions:
-                            type: array
-                          layoutId:
-                            type: "null"
-                          properties:
-                            type: array
-                            items:
-                              type: object
-                              properties:
-                                name:
-                                  type: string
-                                type:
-                                  type: string
-                                value:
-                                  type:
-                                    - integer
-                                    - string
-                          uiMetadata:
-                            type: object
-                            properties:
-                              name:
-                                type: string
-                              wizard:
-                                type: object
-                                properties:
-                                  defaultValues:
-                                    type: object
-                                  defaultActions:
-                                    type: object
-                          templateName:
-                            type: "null"
-                      height:
-                        type: integer
-                      domJson:
+                                        class:
+                                          type: string
+                                        data-img-id:
+                                          type: string
+                                        id:
+                                          type: string
+                            widget:
+                              type: string
+                      web:
                         type: object
                         properties:
                           type:
                             type: string
-                          props:
-                            type: object
-                            properties:
-                              id:
-                                type: string
-                              type:
-                                type: string
-                              class:
-                                type: string
-                              style:
+                          ariaExpanded:
+                            type: string
+                          ariaLabel:
+                            type: string
+                          domClasses:
+                            type: array
+                          domId:
+                            type: string
+                          layout:
+                            type: string
+                          pseudoStyles:
+                            type: array
+                          semanticTag:
+                            type: string
+                          translationId:
+                            type: string
+                      widget:
+                        type: string
+                  color:
+                    type: string
+                  domJson:
+                    type: object
+                    properties:
+                      type:
+                        type: string
+                      children:
+                        type: array
+                        items:
+                          type: object
+                          properties:
+                            type:
+                              type: string
+                            children:
+                              type: array
+                              items:
                                 type: object
                                 properties:
-                                  top:
-                                    type: string
-                                  left:
-                                    type: string
-                                  float:
-                                    type: string
-                                  right:
-                                    type: string
-                                  width:
-                                    type: string
-                                  border:
-                                    type: string
-                                  bottom:
-                                    type: string
-                                  height:
-                                    type: string
-                                  display:
-                                    type: string
-                                  z-index:
-                                    type: integer
-                                  position:
-                                    type: string
-                                  font-size:
-                                    type: string
-                                  min-width:
-                                    type: string
-                                  background:
-                                    type: string
-                                  box-shadow:
-                                    type: string
-                                  margin-top:
-                                    type: string
-                                  min-height:
-                                    type: string
-                                  line-height:
-                                    type: integer
-                                  margin-left:
-                                    type: string
-                                  padding-top:
-                                    type: string
-                                  margin-right:
-                                    type: string
-                                  padding-left:
-                                    type: string
-                                  border-radius:
-                                    type: string
-                                  margin-bottom:
-                                    type: string
-                                  padding-right:
-                                    type: string
-                                  padding-bottom:
-                                    type: string
-                                  vertical-align:
+                                  type:
                                     type: string
-                              aria-label:
-                                type: string
-                              data-layout:
-                                type: string
-                              aria-expanded:
-                                type: string
-                          children:
-                            type: array
-                            items:
+                                  props:
+                                    type: object
+                                    properties:
+                                      type:
+                                        type: string
+                                      alt:
+                                        type: string
+                                      class:
+                                        type: string
+                                      data-_pendo-image-1:
+                                        type: string
+                                      id:
+                                        type: string
+                                      src:
+                                        type: string
+                                      style:
+                                        type: object
+                                        properties:
+                                          border:
+                                            type: string
+                                          box-shadow:
+                                            type: string
+                                          display:
+                                            type: string
+                                          float:
+                                            type: string
+                                          height:
+                                            type: string
+                                          line-height:
+                                            type: integer
+                                          margin:
+                                            type: string
+                                          padding:
+                                            type: string
+                                          vertical-align:
+                                            type: string
+                                          width:
+                                            type: string
+                            css:
+                              type: array
+                            props:
                               type: object
                               properties:
-                                css:
-                                  type: array
                                 type:
                                   type: string
-                                props:
+                                alt:
+                                  type: string
+                                class:
+                                  type: string
+                                data-_pendo-image-1:
+                                  type: string
+                                data-_pendo-image-wrapper-1:
+                                  type: string
+                                data-img-id:
+                                  type: string
+                                id:
+                                  type: string
+                                scoped:
+                                  type: string
+                                src:
+                                  type: string
+                                style:
                                   type: object
                                   properties:
-                                    id:
+                                    border:
                                       type: string
-                                    alt:
+                                    box-shadow:
                                       type: string
-                                    src:
+                                    display:
                                       type: string
-                                    type:
+                                    float:
                                       type: string
-                                    class:
+                                    height:
                                       type: string
-                                    style:
-                                      type: object
-                                      properties:
-                                        float:
-                                          type: string
-                                        width:
-                                          type: string
-                                        border:
-                                          type: string
-                                        height:
-                                          type: string
-                                        margin:
-                                          type: string
-                                        display:
-                                          type: string
-                                        padding:
-                                          type: string
-                                        box-shadow:
-                                          type: string
-                                        line-height:
-                                          type: integer
-                                        vertical-align:
-                                          type: string
-                                    scoped:
+                                    line-height:
+                                      type: integer
+                                    margin:
                                       type: string
-                                    data-img-id:
+                                    padding:
                                       type: string
-                                    data-_pendo-image-1:
+                                    vertical-align:
                                       type: string
-                                    data-_pendo-image-wrapper-1:
+                                    width:
                                       type: string
-                                children:
-                                  type: array
-                                  items:
-                                    type: object
-                                    properties:
-                                      type:
-                                        type: string
-                                      props:
-                                        type: object
-                                        properties:
-                                          id:
-                                            type: string
-                                          alt:
-                                            type: string
-                                          src:
-                                            type: string
-                                          type:
-                                            type: string
-                                          class:
-                                            type: string
-                                          style:
-                                            type: object
-                                            properties:
-                                              float:
-                                                type: string
-                                              width:
-                                                type: string
-                                              border:
-                                                type: string
-                                              height:
-                                                type: string
-                                              margin:
-                                                type: string
-                                              display:
-                                                type: string
-                                              padding:
-                                                type: string
-                                              box-shadow:
-                                                type: string
-                                              line-height:
-                                                type: integer
-                                              vertical-align:
-                                                type: string
-                                          data-_pendo-image-1:
-                                            type: string
-                      offsets:
+                      props:
                         type: object
                         properties:
-                          top:
-                            type: integer
-                          left:
-                            type: integer
-                          right:
-                            type: integer
-                      imageUrl:
-                        type: string
-                      position:
-                        type: string
-                      isOnlyShowOnce:
-                        type: boolean
-                      showGuideOnBadgeHover:
-                        type: boolean
-                      showBadgeOnlyOnElementHover:
-                        type: boolean
-              dates:
-                description: Date configurations for different locales.
-                type: object
-                properties:
-                  es:
-                    type: string
-                  ja:
-                    type: string
-                  en-US:
-                    type: string
-              email:
-                description:
-                  Configuration details for email notifications related to
-                  the guide.
-                type: boolean
-              device:
-                description: Device-specific details for the guide.
-                type: object
-                properties:
-                  type:
-                    description: Type of device the guide is optimized for.
-                    type: string
-              capping:
-                description: Capping rules for guide impressions.
-                type: object
-                properties:
-                  maxImpressions:
-                    description:
-                      Maximum number of times the guide is allowed to be
-                      displayed.
-                    type: integer
-                  maxSessionImpressions:
-                    description:
-                      Maximum number of times the guide can be displayed
-                      in a single session.
+                          type:
+                            type: string
+                          aria-expanded:
+                            type: string
+                          aria-label:
+                            type: string
+                          class:
+                            type: string
+                          data-layout:
+                            type: string
+                          id:
+                            type: string
+                          style:
+                            type: object
+                            properties:
+                              background:
+                                type: string
+                              border:
+                                type: string
+                              border-radius:
+                                type: string
+                              bottom:
+                                type: string
+                              box-shadow:
+                                type: string
+                              display:
+                                type: string
+                              float:
+                                type: string
+                              font-size:
+                                type: string
+                              height:
+                                type: string
+                              left:
+                                type: string
+                              line-height:
+                                type: integer
+                              margin-bottom:
+                                type: string
+                              margin-left:
+                                type: string
+                              margin-right:
+                                type: string
+                              margin-top:
+                                type: string
+                              min-height:
+                                type: string
+                              min-width:
+                                type: string
+                              padding-bottom:
+                                type: string
+                              padding-left:
+                                type: string
+                              padding-right:
+                                type: string
+                              padding-top:
+                                type: string
+                              position:
+                                type: string
+                              right:
+                                type: string
+                              top:
+                                type: string
+                              vertical-align:
+                                type: string
+                              width:
+                                type: string
+                              z-index:
+                                type: integer
+                  height:
                     type: integer
-              priority:
-                description: Priority level of the guide.
-                type: integer
-              activation:
-                description: Information related to guide activation.
-                anyOf:
-                  - type: "null"
-                  - type: object
-                    properties:
-                      event:
-                        type: array
-                        items:
-                          type: string
-                      selector:
-                        type: string
-                      inheritStepOne:
-                        type: boolean
-              isAnnouncement:
-                description: Indicates if the guide is an announcement.
-                type: boolean
-              resourceCenter:
-                description: Details related to the resource center integration.
-                type: object
-                properties:
-                  children:
-                    type: array
-                    items:
-                      type: string
-                  isModule:
-                    type: boolean
-                  moduleId:
+                  imageUrl:
                     type: string
-                  originId:
-                    type: string
-                  homeViewId:
-                    type: string
-                  isTopLevel:
+                  isOnlyShowOnce:
                     type: boolean
-                  integrationName:
-                    type: string
-                  integrationProvider:
-                    type: string
-              notificationBubble:
-                description: Styling details for the notification bubble.
-                type: object
-                properties:
-                  color:
+                  name:
                     type: string
-                  font-family:
+                  offsets:
+                    type: object
+                    properties:
+                      left:
+                        type: integer
+                      right:
+                        type: integer
+                      top:
+                        type: integer
+                  position:
                     type: string
-                  font-weight:
+                  showBadgeOnlyOnElementHover:
+                    type: boolean
+                  showGuideOnBadgeHover:
+                    type: boolean
+                  width:
                     type: integer
-                  background-color:
-                    type: string
-              elementSelectionType:
-                description: Type of selection for guide elements.
+            description: Badge details associated with the guide.
+          capping:
+            type: object
+            description: Capping rules for guide impressions.
+            properties:
+              maxImpressions:
+                type: integer
+                description: Maximum number of times the guide is allowed to be displayed.
+              maxSessionImpressions:
+                type: integer
+                description: >-
+                  Maximum number of times the guide can be displayed in a single
+                  session.
+          dates:
+            type: object
+            description: Date configurations for different locales.
+            properties:
+              en-US:
                 type: string
-              sharedServiceVersion:
-                description: Version of the shared service used by the guide.
+              es:
                 type: string
-              overrideAutoThrottling:
-                description: Flag to override automatic throttle settings.
-                type: boolean
-          conversion:
-            description: Conversion settings and configurations.
+              ja:
+                type: string
+          device:
             type: object
+            description: Device-specific details for the guide.
             properties:
-              itemId:
-                description: Identifier of the item associated with the conversion.
-                type: string
-              itemType:
-                description: Type of item that triggers the conversion.
+              type:
                 type: string
-              attributionWindow:
-                description: Time window for attributing conversions to the guide.
-                type: integer
-          editorType:
-            description: Type of editor used to create the guide.
-            type: string
-          emailState:
-            description: State of email notifications for the guide.
-            type: string
-          experiment:
-            description: Details of experiment settings for the guide.
+                description: Type of device the guide is optimized for.
+          dom:
             type: object
+            description: DOM behavior settings for the guide.
             properties:
-              endTime:
-                type: integer
-              groupSize:
-                type: integer
-              startTime:
-                type: integer
-              notificationDuration:
-                type: integer
-          isTopLevel:
-            description: Specifies if the guide is at the top level.
-            type: boolean
-          isTraining:
-            description: Indicates if the guide is for training purposes.
-            type: boolean
-          recurrence:
-            description: Recurrence settings for the guide.
-            type: integer
-          showsAfter:
-            description: Time duration after which the guide is displayed.
-            type: integer
-          description:
-            description: Description of the guide.
+              isOnlyShowOnce:
+                type: boolean
+                description: Indicates if the guide should be shown only once.
+              showGuideOnlyOnElementClick:
+                type: boolean
+                description: Specifies if the guide is triggered by clicking on an element.
+          elementSelectionType:
             type: string
-          isMultiStep:
-            description: Flag to indicate if the guide has multiple steps.
+            description: Type of selection for guide elements.
+          email:
             type: boolean
-          publishedAt:
-            description: Timestamp indicating when the guide was published.
-            type: integer
-          launchMethod:
-            description: Method used to launch the guide.
-            type: string
-          createdByUser:
-            description: Details of the user who created the guide.
+            description: >-
+              Configuration details for email notifications related to the
+              guide.
+          isAnnouncement:
+            type: boolean
+            description: Indicates if the guide is an announcement.
+          notificationBubble:
             type: object
+            description: Styling details for the notification bubble.
             properties:
-              id:
+              background-color:
                 type: string
-              last:
-                type: string
-              role:
-                type: integer
-              first:
-                type: string
-              userType:
+              color:
                 type: string
-              username:
+              font-family:
                 type: string
-              deletedAt:
+              font-weight:
                 type: integer
-              lastLogin:
-                type: integer
-              visitorIds:
+          overrideAutoThrottling:
+            type: boolean
+            description: Flag to override automatic throttle settings.
+          priority:
+            type: integer
+            description: Priority level of the guide.
+          resourceCenter:
+            type: object
+            description: Details related to the resource center integration.
+            properties:
+              children:
                 type: array
                 items:
                   type: string
-              hasLoggedIn:
+              homeViewId:
+                type: string
+              integrationName:
+                type: string
+              integrationProvider:
+                type: string
+              isModule:
                 type: boolean
-          lastUpdatedAt:
-            description: Timestamp indicating the last update time for the guide.
+              isTopLevel:
+                type: boolean
+              moduleId:
+                type: string
+              originId:
+                type: string
+          sharedServiceVersion:
+            type: string
+            description: Version of the shared service used by the guide.
+      audience:
+        type: array
+        description: Audience details and criteria for targeting the guide.
+        items:
+          type: object
+          properties:
+            eval:
+              type: object
+              properties:
+                accountId:
+                  type: string
+                  description: Unique identifier of the account for audience evaluation.
+            filter:
+              type: string
+              description: Filter criteria for defining the target audience.
+            identified:
+              type: string
+              description: Indicates if the audience is identified.
+            segment:
+              type: object
+              description: Segment details for audience targeting.
+              properties:
+                id:
+                  type: string
+                  description: Identifier of the audience segment.
+            select:
+              type: object
+              description: Selection criteria for the audience.
+              properties:
+                visitorId:
+                  type: string
+                  description: Visitor identifier for audience selection.
+            source:
+              type: object
+              description: Source details for the audience.
+              properties:
+                visitors:
+                  anyOf:
+                    - type: "null"
+                    - type: object
+                      properties:
+                        identified:
+                          type: boolean
+            unwind:
+              type: object
+              description: Criteria for unwinding audience data.
+              properties:
+                field:
+                  type: string
+                keepEmpty:
+                  type: boolean
+      audienceUiHint:
+        type: object
+        description: Provides hints on the intended audience for displaying the guide.
+        properties:
+          filters:
+            type: array
+            description: UI hints related to audience filters.
+            items:
+              type: object
+              properties:
+                type:
+                  type: string
+                $valid:
+                  type: boolean
+                elementType:
+                  type: string
+                field:
+                  type: string
+                group:
+                  type: string
+                id:
+                  type: string
+                key:
+                  type: string
+                kind:
+                  type: string
+                name:
+                  type: string
+                operator:
+                  type: string
+                schema:
+                  type: string
+                segmentId:
+                  type: string
+                value:
+                  type:
+                    - integer
+                    - string
+      authoredLanguage:
+        type: string
+        description: Language in which the guide is authored.
+      children:
+        type: array
+        description: Child guides associated with the main guide.
+        items:
+          type: string
+      conversion:
+        type: object
+        description: Conversion settings and configurations.
+        properties:
+          attributionWindow:
+            type: integer
+            description: Time window for attributing conversions to the guide.
+          itemId:
+            type: string
+            description: Identifier of the item associated with the conversion.
+          itemType:
+            type: string
+            description: Type of item that triggers the conversion.
+      createdAt:
+        type: integer
+        description: Timestamp indicating when the guide was created.
+      createdByUser:
+        type: object
+        description: Details of the user who created the guide.
+        properties:
+          deletedAt:
             type: integer
-          publishedEver:
-            description: Indicates if the guide has ever been published.
+          first:
+            type: string
+          hasLoggedIn:
             type: boolean
-          rootVersionId:
-            description: Identifier of the root version of the guide.
+          id:
             type: string
-          audienceUiHint:
-            description:
-              Provides hints on the intended audience for displaying the
-              guide.
-            type: object
-            properties:
-              filters:
-                description: UI hints related to audience filters.
-                type: array
-                items:
+          last:
+            type: string
+          lastLogin:
+            type: integer
+          role:
+            type: integer
+          userType:
+            type: string
+          username:
+            type: string
+          visitorIds:
+            type: array
+            items:
+              type: string
+      currentFirstEligibleToBeSeenAt:
+        type: integer
+        description: Timestamp for the first eligibility of the guide to be shown.
+      description:
+        type: string
+        description: Description of the guide.
+      editorType:
+        type: string
+        description: Type of editor used to create the guide.
+      emailConfiguration:
+        type: object
+        description: Configuration details for email notifications related to the guide.
+        properties:
+          emailMetadataPropertyName:
+            type: string
+          subject:
+            type: string
+      emailState:
+        type: string
+        description: State of email notifications for the guide.
+      experiment:
+        type: object
+        description: Details of experiment settings for the guide.
+        properties:
+          endTime:
+            type: integer
+          groupSize:
+            type: integer
+          notificationDuration:
+            type: integer
+          startTime:
+            type: integer
+      id:
+        type: string
+        description: Unique identifier of the guide.
+      isModule:
+        type: boolean
+        description: Indicates if the guide is a module.
+      isMultiStep:
+        type: boolean
+        description: Flag to indicate if the guide has multiple steps.
+      isTopLevel:
+        type: boolean
+        description: Specifies if the guide is at the top level.
+      isTraining:
+        type: boolean
+        description: Indicates if the guide is for training purposes.
+      kind:
+        type: string
+        description: Type or category of the guide.
+      lastUpdatedAt:
+        type: integer
+        description: Timestamp indicating the last update time for the guide.
+      lastUpdatedByUser:
+        type: object
+        description: Details of the user who last updated the guide.
+        properties:
+          deletedAt:
+            type: integer
+          first:
+            type: string
+          hasLoggedIn:
+            type: boolean
+          id:
+            type: string
+          last:
+            type: string
+          lastLogin:
+            type: integer
+          role:
+            type: integer
+          userType:
+            type: string
+          username:
+            type: string
+          visitorIds:
+            type: array
+            items:
+              type: string
+      launchMethod:
+        type: string
+        description: Method used to launch the guide.
+      minAgentVersion:
+        type: string
+        description: Minimum agent version required for guide compatibility.
+      name:
+        type: string
+        description: Name of the guide.
+      originId:
+        type: string
+        description: Original identifier of the guide.
+      polls:
+        type: array
+        description: Poll questions and related details for the guide.
+        items:
+          type: object
+          properties:
+            attributes:
+              type: object
+              properties:
+                type:
+                  type: string
+                display:
+                  type: string
+                followUp:
+                  type: string
+                leftLabel:
+                  type: string
+                rightLabel:
+                  type: string
+            id:
+              type: string
+            idResponses:
+              type: object
+              additionalProperties: true
+            numericResponses:
+              type: array
+              items:
+                type: integer
+            question:
+              type: string
+            resetAt:
+              type: integer
+      publishedAt:
+        type: integer
+        description: Timestamp indicating when the guide was published.
+      publishedEver:
+        type: boolean
+        description: Indicates if the guide has ever been published.
+      recurrence:
+        type: integer
+        description: Recurrence settings for the guide.
+      recurrenceEligibilityWindow:
+        type: integer
+        description: Time window for recurrence eligibility.
+      resetAt:
+        type: integer
+        description: Timestamp indicating when the guide is reset.
+      resourceCenterId:
+        type: string
+        description: Identifier of the resource center associated with the guide.
+      rootVersionId:
+        type: string
+        description: Identifier of the root version of the guide.
+      showsAfter:
+        type: integer
+        description: Time duration after which the guide is displayed.
+      stableVersionId:
+        type: string
+        description: Identifier of the stable version of the guide.
+      state:
+        type: string
+        description: Current state of the guide.
+      steps:
+        type: array
+        description: Steps or sequences within the guide.
+        items:
+          type: object
+          properties:
+            type:
+              type: string
+            advanceMethod:
+              type: string
+              description: Method used to advance to the next step.
+            attributes:
+              type: object
+              description: Attributes and configurations for the step.
+              properties:
+                type:
+                  type: string
+                advanceActions:
+                  anyOf:
+                    - type: "null"
+                    - type: object
+                      properties:
+                        elementClick:
+                          type: boolean
+                        elementHover:
+                          type: boolean
+                  description: Actions to be performed when advancing to the next step.
+                autoHeight:
+                  type: boolean
+                  description: Indicates if the guide height adjusts automatically.
+                blockOutUI:
                   type: object
+                  description: UI blocking settings for the guide.
                   properties:
-                    id:
-                      type: string
-                    key:
+                    additionalElements:
                       type: string
-                    kind:
-                      type: string
-                    name:
+                    enabled:
+                      type: boolean
+                    padding:
+                      type: object
+                      properties:
+                        bottom:
+                          type: integer
+                        left:
+                          type: integer
+                        right:
+                          type: integer
+                        top:
+                          type: integer
+                color:
+                  type: string
+                contentHostUrl:
+                  type: string
+                css:
+                  type: string
+                device:
+                  type: object
+                  description: Device-specific configurations for the step.
+                  properties:
+                    desktop:
+                      type: boolean
+                    iframe:
+                      type: boolean
+                    mobile:
+                      type: boolean
+                elementSelectionType:
+                  type: string
+                  description: Type of selection for elements on the step.
+                enabled:
+                  type: boolean
+                  description: Indicates if the step is enabled.
+                guideCssUrl:
+                  type: string
+                height:
+                  type: integer
+                html:
+                  type: string
+                id:
+                  type: string
+                isAutoFocus:
+                  type: boolean
+                  description: Indicates if autofocus is enabled on the step.
+                javascript:
+                  type: string
+                launcherBadgeUrl:
+                  type: string
+                layoutDir:
+                  type: string
+                position:
+                  type: string
+                template:
+                  type: string
+                templateName:
+                  type: string
+                themeId:
+                  type: string
+                title:
+                  type: string
+                variables:
+                  type: object
+                  description: Variables and settings for the step.
+                  properties:
+                    company:
                       type: string
-                    type:
+                    enableSuccessMessage:
+                      type: boolean
+                    followUpDetractor:
                       type: string
-                    field:
+                    followUpNeutral:
                       type: string
-                    group:
+                    followUpPromoter:
                       type: string
-                    value:
-                      type:
-                        - integer
-                        - string
-                    $valid:
-                      type: boolean
-                    schema:
+                    followUpStandard:
                       type: string
-                    operator:
+                    followUpType:
                       type: string
-                    segmentId:
+                    receivesRecommendation:
                       type: string
-                    elementType:
+                    successMessage:
                       type: string
-          minAgentVersion:
-            description: Minimum agent version required for guide compatibility.
-            type: string
-          stableVersionId:
-            description: Identifier of the stable version of the guide.
-            type: string
-          authoredLanguage:
-            description: Language in which the guide is authored.
-            type: string
-          resourceCenterId:
-            description: Identifier of the resource center associated with the guide.
-            type: string
-          lastUpdatedByUser:
-            description: Details of the user who last updated the guide.
+                width:
+                  type: integer
+            buildingBlocksUrl:
+              type: string
+            confirmationElementPathRule:
+              type: string
+            contentType:
+              type: string
+            contentUrl:
+              type: string
+            contentUrlCss:
+              type: string
+            contentUrlJs:
+              type: string
+            domJsonpUrl:
+              type: string
+            domUrl:
+              type: string
+            elementPathRule:
+              type: string
+            guideId:
+              type: string
+            id:
+              type: string
+            lastUpdatedAt:
+              type: integer
+            launchUrl:
+              type: string
+            name:
+              type: string
+            pageId:
+              type: string
+            pollIds:
+              type: array
+              items:
+                type: string
+            rank:
+              type: integer
+            regexUrlRule:
+              type: string
+            resetAt:
+              type: integer
+            templateId:
+              type: string
+            triggerElementPathRule:
+              type: string
+    additionalProperties: true
+  Account Metadata:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      agent:
+        type: object
+        description: Information related to the agent associated with the account.
+        properties:
+          id:
             type: object
+            description: The unique identifier of the agent.
             properties:
-              id:
+              Dirty:
+                type: boolean
+                description: Flag indicating if the data is dirty or not.
+              DisplayName:
                 type: string
-              last:
+                description: Display name of the ID.
+              ElementFormat:
                 type: string
-              role:
-                type: integer
-              first:
+                description: Format of the element.
+              ElementType:
                 type: string
-              userType:
+                description: Type of the element.
+              Type:
                 type: string
-              username:
+                description: Type of the ID.
+              isCalculated:
+                type: boolean
+                description: Flag indicating if the ID is calculated or not.
+              isDeleted:
+                type: boolean
+                description: Flag indicating if the ID is deleted or not.
+              isHidden:
+                type: boolean
+                description: Flag indicating if the ID is hidden or not.
+              isPerApp:
+                type: boolean
+                description: Flag indicating if the ID is specific to an app or not.
+              isPromoted:
+                type: boolean
+                description: Flag indicating if the ID is promoted or not.
+              neverIndex:
+                type: boolean
+                description: Flag indicating if the ID should never be indexed.
+          name:
+            type: object
+            description: The name of the agent.
+            properties:
+              Dirty:
+                type: boolean
+                description: Flag indicating if the data is dirty or not.
+              DisplayName:
                 type: string
-              deletedAt:
-                type: integer
-              lastLogin:
-                type: integer
-              visitorIds:
+                description: Display name of the agent's name.
+              ElementFormat:
+                type: string
+                description: Format of the element.
+              ElementType:
+                type: string
+                description: Type of the element.
+              Type:
+                type: string
+                description: Type of the agent's name.
+              isCalculated:
+                type: boolean
+                description: Flag indicating if the agent's name is calculated or not.
+              isDeleted:
+                type: boolean
+                description: Flag indicating if the agent's name is deleted or not.
+              isHidden:
+                type: boolean
+                description: Flag indicating if the agent's name is hidden or not.
+              isPerApp:
+                type: boolean
+                description: >-
+                  Flag indicating if the agent's name is specific to an app or
+                  not.
+              isPromoted:
+                type: boolean
+                description: Flag indicating if the agent's name is promoted or not.
+              neverIndex:
+                type: boolean
+                description: Flag indicating if the agent's name should never be indexed.
+              sample:
+                type: string
+                description: Sample data for the agent's name.
+          size:
+            type: object
+            description: The size of the agent.
+            properties:
+              Dirty:
+                type: boolean
+                description: Flag indicating if the data is dirty or not.
+              DisplayName:
+                type: string
+                description: Display name of the agent's size.
+              ElementFormat:
+                type: string
+                description: Format of the element.
+              ElementType:
+                type: string
+                description: Type of the element.
+              Type:
+                type: string
+                description: Type of the agent's size.
+              isCalculated:
+                type: boolean
+                description: Flag indicating if the agent's size is calculated or not.
+              isDeleted:
+                type: boolean
+                description: Flag indicating if the agent's size is deleted or not.
+              isHidden:
+                type: boolean
+                description: Flag indicating if the agent's size is hidden or not.
+              isPerApp:
+                type: boolean
+                description: >-
+                  Flag indicating if the agent's size is specific to an app or
+                  not.
+              isPromoted:
+                type: boolean
+                description: Flag indicating if the agent's size is promoted or not.
+              neverIndex:
+                type: boolean
+                description: Flag indicating if the agent's size should never be indexed.
+              sample:
+                type: string
+                description: Sample data for the agent's size.
+          tier:
+            type: object
+            description: The tier of the agent.
+            properties:
+              Dirty:
+                type: boolean
+                description: Flag indicating if the data is dirty or not.
+              DisplayName:
+                type: string
+                description: Display name of the agent's tier.
+              ElementFormat:
+                type: string
+                description: Format of the element.
+              ElementType:
+                type: string
+                description: Type of the element.
+              Type:
+                type: string
+                description: Type of the agent's tier.
+              isCalculated:
+                type: boolean
+                description: Flag indicating if the agent's tier is calculated or not.
+              isDeleted:
+                type: boolean
+                description: Flag indicating if the agent's tier is deleted or not.
+              isHidden:
+                type: boolean
+                description: Flag indicating if the agent's tier is hidden or not.
+              isPerApp:
+                type: boolean
+                description: >-
+                  Flag indicating if the agent's tier is specific to an app or
+                  not.
+              isPromoted:
+                type: boolean
+                description: Flag indicating if the agent's tier is promoted or not.
+              neverIndex:
+                type: boolean
+                description: Flag indicating if the agent's tier should never be indexed.
+              sample:
+                type: string
+                description: Sample data for the agent's tier.
+          timezone:
+            type: object
+            description: The timezone of the agent.
+            properties:
+              Dirty:
+                type: boolean
+                description: Flag indicating if the data is dirty or not.
+              DisplayName:
+                type: string
+                description: Display name of the agent's timezone.
+              ElementFormat:
+                type: string
+                description: Format of the element.
+              ElementType:
+                type: string
+                description: Type of the element.
+              Type:
+                type: string
+                description: Type of the agent's timezone.
+              isCalculated:
+                type: boolean
+                description: Flag indicating if the agent's timezone is calculated or not.
+              isDeleted:
+                type: boolean
+                description: Flag indicating if the agent's timezone is deleted or not.
+              isHidden:
+                type: boolean
+                description: Flag indicating if the agent's timezone is hidden or not.
+              isPerApp:
+                type: boolean
+                description: >-
+                  Flag indicating if the agent's timezone is specific to an app
+                  or not.
+              isPromoted:
+                type: boolean
+                description: Flag indicating if the agent's timezone is promoted or not.
+              neverIndex:
+                type: boolean
+                description: >-
+                  Flag indicating if the agent's timezone should never be
+                  indexed.
+              sample:
+                type: string
+                description: Sample data for the agent's timezone.
+      auto:
+        type: object
+        description: Automatic data related to visits.
+        properties:
+          firstvisit:
+            type: object
+            description: The timestamp of the first visit.
+            properties:
+              Dirty:
+                type: boolean
+                description: Flag indicating if the data is dirty or not.
+              DisplayName:
+                type: string
+                description: Display name of the first visit.
+              ElementFormat:
+                type: string
+                description: Format of the element.
+              ElementType:
+                type: string
+                description: Type of the element.
+              Type:
+                type: string
+                description: Type of the first visit.
+              isCalculated:
+                type: boolean
+                description: Flag indicating if the first visit is calculated or not.
+              isDeleted:
+                type: boolean
+                description: Flag indicating if the first visit is deleted or not.
+              isHidden:
+                type: boolean
+                description: Flag indicating if the first visit is hidden or not.
+              isPerApp:
+                type: boolean
+                description: >-
+                  Flag indicating if the first visit is specific to an app or
+                  not.
+              isPromoted:
+                type: boolean
+                description: Flag indicating if the first visit is promoted or not.
+              neverIndex:
+                type: boolean
+                description: Flag indicating if the first visit should never be indexed.
+          id:
+            type: object
+            description: The unique identifier of the visit.
+            properties:
+              Dirty:
+                type: boolean
+                description: Flag indicating if the data is dirty or not.
+              DisplayName:
+                type: string
+                description: Display name of the auto ID.
+              ElementFormat:
+                type: string
+                description: Format of the element.
+              ElementType:
+                type: string
+                description: Type of the element.
+              Type:
+                type: string
+                description: Type of the auto ID.
+              isCalculated:
+                type: boolean
+                description: Flag indicating if the auto ID is calculated or not.
+              isDeleted:
+                type: boolean
+                description: Flag indicating if the auto ID is deleted or not.
+              isHidden:
+                type: boolean
+                description: Flag indicating if the auto ID is hidden or not.
+              isPerApp:
+                type: boolean
+                description: Flag indicating if the auto ID is specific to an app or not.
+              isPromoted:
+                type: boolean
+                description: Flag indicating if the auto ID is promoted or not.
+              neverIndex:
+                type: boolean
+                description: Flag indicating if the auto ID should never be indexed.
+          lastvisit:
+            type: object
+            description: The timestamp of the last visit.
+            properties:
+              Dirty:
+                type: boolean
+                description: Flag indicating if the data is dirty or not.
+              DisplayName:
+                type: string
+                description: Display name of the last visit.
+              ElementFormat:
+                type: string
+                description: Format of the element.
+              ElementType:
+                type: string
+                description: Type of the element.
+              Type:
+                type: string
+                description: Type of the last visit.
+              isCalculated:
+                type: boolean
+                description: Flag indicating if the last visit is calculated or not.
+              isDeleted:
+                type: boolean
+                description: Flag indicating if the last visit is deleted or not.
+              isHidden:
+                type: boolean
+                description: Flag indicating if the last visit is hidden or not.
+              isPerApp:
+                type: boolean
+                description: >-
+                  Flag indicating if the last visit is specific to an app or
+                  not.
+              isPromoted:
+                type: boolean
+                description: Flag indicating if the last visit is promoted or not.
+              neverIndex:
+                type: boolean
+                description: Flag indicating if the last visit should never be indexed.
+      pendo:
+        type: object
+        description: Pendo-specific metadata.
+        properties:
+          blacklistguides:
+            type: object
+            description: List of guides that are blacklisted.
+            properties:
+              Dirty:
+                type: boolean
+                description: Flag indicating if the data is dirty or not.
+              DisplayName:
+                type: string
+                description: Display name of the blacklisted guides.
+              ElementFormat:
+                type: string
+                description: Format of the element.
+              ElementType:
+                type: string
+                description: Type of the element.
+              Type:
+                type: string
+                description: Type of the blacklisted guides.
+              isCalculated:
+                type: boolean
+                description: >-
+                  Flag indicating if the blacklisted guides are calculated or
+                  not.
+              isDeleted:
+                type: boolean
+                description: Flag indicating if the blacklisted guides are deleted or not.
+              isHidden:
+                type: boolean
+                description: Flag indicating if the blacklisted guides are hidden or not.
+              isPerApp:
+                type: boolean
+                description: >-
+                  Flag indicating if the blacklisted guides are specific to an
+                  app or not.
+              isPromoted:
+                type: boolean
+                description: Flag indicating if the blacklisted guides are promoted or not.
+              neverIndex:
+                type: boolean
+                description: >-
+                  Flag indicating if the blacklisted guides should never be
+                  indexed.
+          donotprocess:
+            type: object
+            description: >-
+              Flag indicating whether the account metadata should not be
+              processed.
+            properties:
+              Dirty:
+                type: boolean
+                description: Flag indicating if the data is dirty or not.
+              DisplayName:
+                type: string
+                description: Display name of the data not to process.
+              ElementFormat:
+                type: string
+                description: Format of the element.
+              ElementType:
+                type: string
+                description: Type of the element.
+              Type:
+                type: string
+                description: Type of the data not to process.
+              isCalculated:
+                type: boolean
+                description: >-
+                  Flag indicating if the data not to process is calculated or
+                  not.
+              isDeleted:
+                type: boolean
+                description: Flag indicating if the data not to process is deleted or not.
+              isHidden:
+                type: boolean
+                description: Flag indicating if the data not to process is hidden or not.
+              isPerApp:
+                type: boolean
+                description: >-
+                  Flag indicating if the data not to process is specific to an
+                  app or not.
+              isPromoted:
+                type: boolean
+                description: Flag indicating if the data not to process is promoted or not.
+              neverIndex:
+                type: boolean
+                description: >-
+                  Flag indicating if the data not to process should never be
+                  indexed.
+    additionalProperties: true
+  Visitor Metadata:
+    type: object
+    $schema: http://json-schema.org/schema#
+    properties:
+      agent:
+        type: object
+        description: Information about the agent accessing the visitor metadata
+        properties:
+          age:
+            type: object
+            description: The age of the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+              sample:
+                type: string
+          country:
+            type: object
+            description: The country of the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+              sample:
+                type: string
+          displayname:
+            type: object
+            description: The display name of the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+              sample:
+                type: string
+          email:
+            type: object
+            description: The email address of the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+              sample:
+                type: string
+          firstname:
+            type: object
+            description: The first name of the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+              sample:
+                type: string
+          gender:
+            type: object
+            description: The gender of the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+              sample:
+                type: string
+          language:
+            type: object
+            description: The language preference of the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+              sample:
+                type: string
+          loccomplete:
+            type: object
+            description: The location completeness flag for the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+              sample:
+                type: string
+          name:
+            type: object
+            description: The name of the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+              sample:
+                type: string
+          role:
+            type: object
+            description: The role of the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+              sample:
+                type: string
+          tags:
+            type: object
+            description: Tags associated with the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+              sample:
                 type: array
                 items:
                   type: string
-              hasLoggedIn:
+      auto:
+        type: object
+        description: Automatically generated metadata
+        properties:
+          accountid:
+            type: object
+            description: The account ID associated with the visitor
+            properties:
+              Dirty:
                 type: boolean
-          emailConfiguration:
-            description:
-              Configuration details for email notifications related to the
-              guide.
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+          accountids:
             type: object
+            description: List of account IDs associated with the visitor
             properties:
-              subject:
+              Dirty:
+                type: boolean
+              DisplayName:
                 type: string
-              emailMetadataPropertyName:
+              ElementFormat:
                 type: string
-          recurrenceEligibilityWindow:
-            description: Time window for recurrence eligibility.
-            type: integer
-          currentFirstEligibleToBeSeenAt:
-            description: Timestamp for the first eligibility of the guide to be shown.
-            type: integer
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://app.pendo.io/api/v1
-        path: /guide
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        request_body_json: {}
-        authenticator:
-          type: ApiKeyAuthenticator
-          header: x-pendo-integration-key
-          api_token: "{{ config['api_key'] }}"
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: Account Metadata
-    primary_key: []
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
-        properties:
-          agent:
-            description: Information related to the agent associated with the account.
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+          firstvisit:
+            type: object
+            description: Timestamp of the first visit of the visitor
             properties:
-              id:
-                description: The unique identifier of the agent.
-                properties:
-                  Dirty:
-                    description: Flag indicating if the data is dirty or not.
-                    type: boolean
-                  DisplayName:
-                    description: Display name of the ID.
-                    type: string
-                  ElementFormat:
-                    description: Format of the element.
-                    type: string
-                  ElementType:
-                    description: Type of the element.
-                    type: string
-                  Type:
-                    description: Type of the ID.
-                    type: string
-                  isCalculated:
-                    description: Flag indicating if the ID is calculated or not.
-                    type: boolean
-                  isDeleted:
-                    description: Flag indicating if the ID is deleted or not.
-                    type: boolean
-                  isHidden:
-                    description: Flag indicating if the ID is hidden or not.
-                    type: boolean
-                  isPerApp:
-                    description:
-                      Flag indicating if the ID is specific to an app or
-                      not.
-                    type: boolean
-                  isPromoted:
-                    description: Flag indicating if the ID is promoted or not.
-                    type: boolean
-                  neverIndex:
-                    description: Flag indicating if the ID should never be indexed.
-                    type: boolean
-                type: object
-              name:
-                description: The name of the agent.
-                properties:
-                  Dirty:
-                    description: Flag indicating if the data is dirty or not.
-                    type: boolean
-                  DisplayName:
-                    description: Display name of the agent's name.
-                    type: string
-                  ElementFormat:
-                    description: Format of the element.
-                    type: string
-                  ElementType:
-                    description: Type of the element.
-                    type: string
-                  Type:
-                    description: Type of the agent's name.
-                    type: string
-                  isCalculated:
-                    description:
-                      Flag indicating if the agent's name is calculated or
-                      not.
-                    type: boolean
-                  isDeleted:
-                    description: Flag indicating if the agent's name is deleted or not.
-                    type: boolean
-                  isHidden:
-                    description: Flag indicating if the agent's name is hidden or not.
-                    type: boolean
-                  isPerApp:
-                    description:
-                      Flag indicating if the agent's name is specific to
-                      an app or not.
-                    type: boolean
-                  isPromoted:
-                    description:
-                      Flag indicating if the agent's name is promoted or
-                      not.
-                    type: boolean
-                  neverIndex:
-                    description:
-                      Flag indicating if the agent's name should never be
-                      indexed.
-                    type: boolean
-                  sample:
-                    description: Sample data for the agent's name.
-                    type: string
-                type: object
-              size:
-                description: The size of the agent.
-                properties:
-                  Dirty:
-                    description: Flag indicating if the data is dirty or not.
-                    type: boolean
-                  DisplayName:
-                    description: Display name of the agent's size.
-                    type: string
-                  ElementFormat:
-                    description: Format of the element.
-                    type: string
-                  ElementType:
-                    description: Type of the element.
-                    type: string
-                  Type:
-                    description: Type of the agent's size.
-                    type: string
-                  isCalculated:
-                    description:
-                      Flag indicating if the agent's size is calculated or
-                      not.
-                    type: boolean
-                  isDeleted:
-                    description: Flag indicating if the agent's size is deleted or not.
-                    type: boolean
-                  isHidden:
-                    description: Flag indicating if the agent's size is hidden or not.
-                    type: boolean
-                  isPerApp:
-                    description:
-                      Flag indicating if the agent's size is specific to
-                      an app or not.
-                    type: boolean
-                  isPromoted:
-                    description:
-                      Flag indicating if the agent's size is promoted or
-                      not.
-                    type: boolean
-                  neverIndex:
-                    description:
-                      Flag indicating if the agent's size should never be
-                      indexed.
-                    type: boolean
-                  sample:
-                    description: Sample data for the agent's size.
-                    type: string
-                type: object
-              tier:
-                description: The tier of the agent.
-                properties:
-                  Dirty:
-                    description: Flag indicating if the data is dirty or not.
-                    type: boolean
-                  DisplayName:
-                    description: Display name of the agent's tier.
-                    type: string
-                  ElementFormat:
-                    description: Format of the element.
-                    type: string
-                  ElementType:
-                    description: Type of the element.
-                    type: string
-                  Type:
-                    description: Type of the agent's tier.
-                    type: string
-                  isCalculated:
-                    description:
-                      Flag indicating if the agent's tier is calculated or
-                      not.
-                    type: boolean
-                  isDeleted:
-                    description: Flag indicating if the agent's tier is deleted or not.
-                    type: boolean
-                  isHidden:
-                    description: Flag indicating if the agent's tier is hidden or not.
-                    type: boolean
-                  isPerApp:
-                    description:
-                      Flag indicating if the agent's tier is specific to
-                      an app or not.
-                    type: boolean
-                  isPromoted:
-                    description:
-                      Flag indicating if the agent's tier is promoted or
-                      not.
-                    type: boolean
-                  neverIndex:
-                    description:
-                      Flag indicating if the agent's tier should never be
-                      indexed.
-                    type: boolean
-                  sample:
-                    description: Sample data for the agent's tier.
-                    type: string
-                type: object
-              timezone:
-                description: The timezone of the agent.
-                properties:
-                  Dirty:
-                    description: Flag indicating if the data is dirty or not.
-                    type: boolean
-                  DisplayName:
-                    description: Display name of the agent's timezone.
-                    type: string
-                  ElementFormat:
-                    description: Format of the element.
-                    type: string
-                  ElementType:
-                    description: Type of the element.
-                    type: string
-                  Type:
-                    description: Type of the agent's timezone.
-                    type: string
-                  isCalculated:
-                    description:
-                      Flag indicating if the agent's timezone is calculated
-                      or not.
-                    type: boolean
-                  isDeleted:
-                    description:
-                      Flag indicating if the agent's timezone is deleted
-                      or not.
-                    type: boolean
-                  isHidden:
-                    description:
-                      Flag indicating if the agent's timezone is hidden or
-                      not.
-                    type: boolean
-                  isPerApp:
-                    description:
-                      Flag indicating if the agent's timezone is specific
-                      to an app or not.
-                    type: boolean
-                  isPromoted:
-                    description:
-                      Flag indicating if the agent's timezone is promoted
-                      or not.
-                    type: boolean
-                  neverIndex:
-                    description:
-                      Flag indicating if the agent's timezone should never
-                      be indexed.
-                    type: boolean
-                  sample:
-                    description: Sample data for the agent's timezone.
-                    type: string
-                type: object
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+          id:
             type: object
-          auto:
-            description: Automatic data related to visits.
+            description: Unique identifier of the visitor
             properties:
-              firstvisit:
-                description: The timestamp of the first visit.
-                properties:
-                  Dirty:
-                    description: Flag indicating if the data is dirty or not.
-                    type: boolean
-                  DisplayName:
-                    description: Display name of the first visit.
-                    type: string
-                  ElementFormat:
-                    description: Format of the element.
-                    type: string
-                  ElementType:
-                    description: Type of the element.
-                    type: string
-                  Type:
-                    description: Type of the first visit.
-                    type: string
-                  isCalculated:
-                    description:
-                      Flag indicating if the first visit is calculated or
-                      not.
-                    type: boolean
-                  isDeleted:
-                    description: Flag indicating if the first visit is deleted or not.
-                    type: boolean
-                  isHidden:
-                    description: Flag indicating if the first visit is hidden or not.
-                    type: boolean
-                  isPerApp:
-                    description:
-                      Flag indicating if the first visit is specific to an
-                      app or not.
-                    type: boolean
-                  isPromoted:
-                    description: Flag indicating if the first visit is promoted or not.
-                    type: boolean
-                  neverIndex:
-                    description:
-                      Flag indicating if the first visit should never be
-                      indexed.
-                    type: boolean
-                type: object
-              id:
-                description: The unique identifier of the visit.
-                properties:
-                  Dirty:
-                    description: Flag indicating if the data is dirty or not.
-                    type: boolean
-                  DisplayName:
-                    description: Display name of the auto ID.
-                    type: string
-                  ElementFormat:
-                    description: Format of the element.
-                    type: string
-                  ElementType:
-                    description: Type of the element.
-                    type: string
-                  Type:
-                    description: Type of the auto ID.
-                    type: string
-                  isCalculated:
-                    description: Flag indicating if the auto ID is calculated or not.
-                    type: boolean
-                  isDeleted:
-                    description: Flag indicating if the auto ID is deleted or not.
-                    type: boolean
-                  isHidden:
-                    description: Flag indicating if the auto ID is hidden or not.
-                    type: boolean
-                  isPerApp:
-                    description:
-                      Flag indicating if the auto ID is specific to an app
-                      or not.
-                    type: boolean
-                  isPromoted:
-                    description: Flag indicating if the auto ID is promoted or not.
-                    type: boolean
-                  neverIndex:
-                    description: Flag indicating if the auto ID should never be indexed.
-                    type: boolean
-                type: object
-              lastvisit:
-                description: The timestamp of the last visit.
-                properties:
-                  Dirty:
-                    description: Flag indicating if the data is dirty or not.
-                    type: boolean
-                  DisplayName:
-                    description: Display name of the last visit.
-                    type: string
-                  ElementFormat:
-                    description: Format of the element.
-                    type: string
-                  ElementType:
-                    description: Type of the element.
-                    type: string
-                  Type:
-                    description: Type of the last visit.
-                    type: string
-                  isCalculated:
-                    description:
-                      Flag indicating if the last visit is calculated or
-                      not.
-                    type: boolean
-                  isDeleted:
-                    description: Flag indicating if the last visit is deleted or not.
-                    type: boolean
-                  isHidden:
-                    description: Flag indicating if the last visit is hidden or not.
-                    type: boolean
-                  isPerApp:
-                    description:
-                      Flag indicating if the last visit is specific to an
-                      app or not.
-                    type: boolean
-                  isPromoted:
-                    description: Flag indicating if the last visit is promoted or not.
-                    type: boolean
-                  neverIndex:
-                    description: Flag indicating if the last visit should never be indexed.
-                    type: boolean
-                type: object
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+          lastbrowsername:
             type: object
-          pendo:
-            description: Pendo-specific metadata.
+            description: Name of the last browser used by the visitor
             properties:
-              blacklistguides:
-                description: List of guides that are blacklisted.
-                properties:
-                  Dirty:
-                    description: Flag indicating if the data is dirty or not.
-                    type: boolean
-                  DisplayName:
-                    description: Display name of the blacklisted guides.
-                    type: string
-                  ElementFormat:
-                    description: Format of the element.
-                    type: string
-                  ElementType:
-                    description: Type of the element.
-                    type: string
-                  Type:
-                    description: Type of the blacklisted guides.
-                    type: string
-                  isCalculated:
-                    description:
-                      Flag indicating if the blacklisted guides are calculated
-                      or not.
-                    type: boolean
-                  isDeleted:
-                    description:
-                      Flag indicating if the blacklisted guides are deleted
-                      or not.
-                    type: boolean
-                  isHidden:
-                    description:
-                      Flag indicating if the blacklisted guides are hidden
-                      or not.
-                    type: boolean
-                  isPerApp:
-                    description:
-                      Flag indicating if the blacklisted guides are specific
-                      to an app or not.
-                    type: boolean
-                  isPromoted:
-                    description:
-                      Flag indicating if the blacklisted guides are promoted
-                      or not.
-                    type: boolean
-                  neverIndex:
-                    description:
-                      Flag indicating if the blacklisted guides should never
-                      be indexed.
-                    type: boolean
-                type: object
-              donotprocess:
-                description:
-                  Flag indicating whether the account metadata should not
-                  be processed.
-                properties:
-                  Dirty:
-                    description: Flag indicating if the data is dirty or not.
-                    type: boolean
-                  DisplayName:
-                    description: Display name of the data not to process.
-                    type: string
-                  ElementFormat:
-                    description: Format of the element.
-                    type: string
-                  ElementType:
-                    description: Type of the element.
-                    type: string
-                  Type:
-                    description: Type of the data not to process.
-                    type: string
-                  isCalculated:
-                    description:
-                      Flag indicating if the data not to process is calculated
-                      or not.
-                    type: boolean
-                  isDeleted:
-                    description:
-                      Flag indicating if the data not to process is deleted
-                      or not.
-                    type: boolean
-                  isHidden:
-                    description:
-                      Flag indicating if the data not to process is hidden
-                      or not.
-                    type: boolean
-                  isPerApp:
-                    description:
-                      Flag indicating if the data not to process is specific
-                      to an app or not.
-                    type: boolean
-                  isPromoted:
-                    description:
-                      Flag indicating if the data not to process is promoted
-                      or not.
-                    type: boolean
-                  neverIndex:
-                    description:
-                      Flag indicating if the data not to process should never
-                      be indexed.
-                    type: boolean
-                type: object
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+          lastbrowserversion:
             type: object
+            description: Version of the last browser used by the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+          lastoperatingsystem:
+            type: object
+            description: Operating system of the last device used by the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+          lastservername:
+            type: object
+            description: Last known server name for the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+          lastvisit:
+            type: object
+            description: Timestamp of the last visit of the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+      custom:
         type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://app.pendo.io/api/v1
-        path: /metadata/schema/account
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        request_body_json: {}
-        authenticator:
-          type: ApiKeyAuthenticator
-          header: x-pendo-integration-key
-          api_token: "{{ config['api_key'] }}"
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-  - type: DeclarativeStream
-    name: Visitor Metadata
-    primary_key: []
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/schema#
+        description: Custom metadata provided by the user
         properties:
-          agent:
-            description: Information about the agent accessing the visitor metadata
+          practicumtest:
+            type: object
+            description: Flag for practicum test status
             properties:
-              age:
-                description: The age of the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                  sample:
-                    type: string
-                type: object
-              country:
-                description: The country of the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                  sample:
-                    type: string
-                type: object
-              displayname:
-                description: The display name of the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                  sample:
-                    type: string
-                type: object
-              email:
-                description: The email address of the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                  sample:
-                    type: string
-                type: object
-              firstname:
-                description: The first name of the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                  sample:
-                    type: string
-                type: object
-              gender:
-                description: The gender of the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                  sample:
-                    type: string
-                type: object
-              language:
-                description: The language preference of the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                  sample:
-                    type: string
-                type: object
-              loccomplete:
-                description: The location completeness flag for the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                  sample:
-                    type: string
-                type: object
-              name:
-                description: The name of the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                  sample:
-                    type: string
-                type: object
-              role:
-                description: The role of the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                  sample:
-                    type: string
-                type: object
-              tags:
-                description: Tags associated with the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                  sample:
-                    items:
-                      type: string
-                    type: array
-                type: object
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+          rmlsurveytest:
             type: object
-          auto:
-            description: Automatically generated metadata
+            description: Flag for RML survey test status
             properties:
-              accountid:
-                description: The account ID associated with the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
-              accountids:
-                description: List of account IDs associated with the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
-              firstvisit:
-                description: Timestamp of the first visit of the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
-              id:
-                description: Unique identifier of the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
-              lastbrowsername:
-                description: Name of the last browser used by the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
-              lastbrowserversion:
-                description: Version of the last browser used by the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
-              lastoperatingsystem:
-                description: Operating system of the last device used by the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
-              lastservername:
-                description: Last known server name for the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
-              lastvisit:
-                description: Timestamp of the last visit of the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+          special:
             type: object
-          custom:
-            description: Custom metadata provided by the user
+            description: Special custom field for the visitor
             properties:
-              practicumtest:
-                description: Flag for practicum test status
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
-              rmlsurveytest:
-                description: Flag for RML survey test status
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
-              special:
-                description: Special custom field for the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+      pendo:
+        type: object
+        description: Specific Pendo related metadata
+        properties:
+          blacklistguides:
             type: object
-          pendo:
-            description: Specific Pendo related metadata
+            description: Flag to blacklist certain guides for the visitor
             properties:
-              blacklistguides:
-                description: Flag to blacklist certain guides for the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
-              designerenabled:
-                description:
-                  Flag to indicate whether the designer is enabled for the
-                  visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
-              donotprocess:
-                description:
-                  Flag to indicate whether certain processes should not be
-                  carried out for the visitor
-                properties:
-                  Dirty:
-                    type: boolean
-                  DisplayName:
-                    type: string
-                  ElementFormat:
-                    type: string
-                  ElementType:
-                    type: string
-                  Type:
-                    type: string
-                  isCalculated:
-                    type: boolean
-                  isDeleted:
-                    type: boolean
-                  isHidden:
-                    type: boolean
-                  isPerApp:
-                    type: boolean
-                  isPromoted:
-                    type: boolean
-                  neverIndex:
-                    type: boolean
-                type: object
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+          designerenabled:
             type: object
-        type: object
-    retriever:
-      type: SimpleRetriever
-      requester:
-        type: HttpRequester
-        url_base: https://app.pendo.io/api/v1
-        path: /metadata/schema/visitor
-        http_method: GET
-        request_parameters: {}
-        request_headers: {}
-        request_body_json: {}
-        authenticator:
-          type: ApiKeyAuthenticator
-          header: x-pendo-integration-key
-          api_token: "{{ config['api_key'] }}"
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: []
-      paginator:
-        type: NoPagination
-spec:
-  connection_specification:
-    $schema: http://json-schema.org/draft-07/schema#
-    type: object
-    required:
-      - api_key
-    properties:
-      api_key:
-        type: string
-        title: API Key
-        airbyte_secret: true
+            description: Flag to indicate whether the designer is enabled for the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
+          donotprocess:
+            type: object
+            description: >-
+              Flag to indicate whether certain processes should not be carried
+              out for the visitor
+            properties:
+              Dirty:
+                type: boolean
+              DisplayName:
+                type: string
+              ElementFormat:
+                type: string
+              ElementType:
+                type: string
+              Type:
+                type: string
+              isCalculated:
+                type: boolean
+              isDeleted:
+                type: boolean
+              isHidden:
+                type: boolean
+              isPerApp:
+                type: boolean
+              isPromoted:
+                type: boolean
+              neverIndex:
+                type: boolean
     additionalProperties: true
-  documentation_url: https://docs.airbyte.com/integrations/sources/pendo
-  type: Spec
```

### Comparing `airbyte_source_pendo-0.1.4/PKG-INFO` & `airbyte_source_pendo-0.1.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-pendo
-Version: 0.1.4
+Version: 0.1.5
 Summary: Source implementation for Pendo.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/pendo
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Pendo source connector
 
-
 This is the repository for the Pendo source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/pendo).
 
 ## Local development
 
 ### Prerequisites
-* Python (~=3.9)
-* Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
+- Python (~=3.9)
+- Poetry (~=1.7) - installation instructions [here](https://python-poetry.org/docs/#installation)
 
 ### Installing the connector
+
 From this connector directory, run:
+
 ```bash
 poetry install --with dev
 ```
 
-
 ### Create credentials
+
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/pendo)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_pendo/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-pendo spec
 poetry run source-pendo check --config secrets/config.json
 poetry run source-pendo discover --config secrets/config.json
 poetry run source-pendo read --config secrets/config.json --catalog sample_files/configured_catalog.json
 ```
 
 ### Running unit tests
+
 To run unit tests locally, from the connector directory run:
+
 ```
 poetry run pytest unit_tests
 ```
 
 ### Building the docker image
+
 1. Install [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md)
 2. Run the following command to build the docker image:
+
 ```bash
 airbyte-ci connectors --name=source-pendo build
 ```
 
 An image will be available on your host with the tag `airbyte/source-pendo:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-pendo:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pendo:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-pendo:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-pendo:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-pendo test
 ```
 
 ### Customizing acceptance Tests
+
 Customize `acceptance-test-config.yml` file to configure acceptance tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
 ### Dependency Management
-All of your dependencies should be managed via Poetry. 
+
+All of your dependencies should be managed via Poetry.
 To add a new dependency, run:
+
 ```bash
 poetry add <package-name>
 ```
 
 Please commit the changes to `pyproject.toml` and `poetry.lock` files.
 
 ## Publishing a new version of the connector
+
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
+
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-pendo test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/pendo.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

