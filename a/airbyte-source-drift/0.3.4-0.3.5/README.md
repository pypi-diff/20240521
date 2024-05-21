# Comparing `tmp/airbyte_source_drift-0.3.4.tar.gz` & `tmp/airbyte_source_drift-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_drift-0.3.4.tar", max compression
+gzip compressed data, was "airbyte_source_drift-0.3.5.tar", max compression
```

## Comparing `airbyte_source_drift-0.3.4.tar` & `airbyte_source_drift-0.3.5.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4478 2024-05-03 13:48:10.000000 airbyte_source_drift-0.3.4/README.md
--rw-r--r--   0        0        0      708 2024-05-03 14:06:02.310621 airbyte_source_drift-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      122 2024-05-03 13:48:10.000000 airbyte_source_drift-0.3.4/source_drift/__init__.py
--rw-r--r--   0        0        0    13120 2024-05-03 13:48:10.000000 airbyte_source_drift-0.3.4/source_drift/manifest.yaml
--rw-r--r--   0        0        0      227 2024-05-03 13:48:10.000000 airbyte_source_drift-0.3.4/source_drift/run.py
--rw-r--r--   0        0        0      474 2024-05-03 13:48:10.000000 airbyte_source_drift-0.3.4/source_drift/source.py
--rw-r--r--   0        0        0     3204 2024-05-03 13:48:10.000000 airbyte_source_drift-0.3.4/source_drift/spec.yaml
--rw-r--r--   0        0        0     5177 1970-01-01 00:00:00.000000 airbyte_source_drift-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     4488 2024-05-21 01:13:27.383396 airbyte_source_drift-0.3.5/README.md
+-rw-r--r--   0        0        0      708 2024-05-21 01:17:48.954432 airbyte_source_drift-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-21 01:13:27.383396 airbyte_source_drift-0.3.5/source_drift/__init__.py
+-rw-r--r--   0        0        0    16585 2024-05-21 01:13:27.383396 airbyte_source_drift-0.3.5/source_drift/manifest.yaml
+-rw-r--r--   0        0        0      227 2024-05-21 01:13:27.383396 airbyte_source_drift-0.3.5/source_drift/run.py
+-rw-r--r--   0        0        0      474 2024-05-21 01:13:27.383396 airbyte_source_drift-0.3.5/source_drift/source.py
+-rw-r--r--   0        0        0     5187 1970-01-01 00:00:00.000000 airbyte_source_drift-0.3.5/PKG-INFO
```

### Comparing `airbyte_source_drift-0.3.4/README.md` & `airbyte_source_drift-0.3.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Drift source connector
 
-
 This is the repository for the Drift source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/drift).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/drift)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_drift/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-drift spec
 poetry run source-drift check --config secrets/config.json
 poetry run source-drift discover --config secrets/config.json
 poetry run source-drift read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-drift build
 ```
 
 An image will be available on your host with the tag `airbyte/source-drift:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-drift:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-drift:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-drift:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-drift:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-drift test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-drift test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/drift.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_drift-0.3.4/pyproject.toml` & `airbyte_source_drift-0.3.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.3.4"
+version = "0.3.5"
 name = "airbyte-source-drift"
 description = "Source implementation for Drift."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_drift-0.3.4/source_drift/manifest.yaml` & `airbyte_source_drift-0.3.5/source_drift/manifest.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -1,411 +1,549 @@
-version: "0.29.0"
+version: 0.78.5
 
-definitions:
-  selector:
-    type: RecordSelector
-    extractor:
-      type: DpathExtractor
-      field_path: ["data"]
+type: DeclarativeSource
+
+check:
+  type: CheckStream
+  stream_names:
+    - accounts
 
-  requester:
+definitions:
+  streams:
+    accounts:
+      type: DeclarativeStream
+      name: accounts
+      primary_key:
+        - ownerId
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /accounts
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - data
+              - accounts
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestPath
+          pagination_strategy:
+            type: CursorPagination
+            cursor_value: "{{ last_record['next'] }}"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/accounts"
+    conversations:
+      type: DeclarativeStream
+      name: conversations
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /conversations
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - data
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestPath
+          pagination_strategy:
+            type: CursorPagination
+            cursor_value: "{{ last_record['next'] }}"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/conversations"
+    users:
+      type: DeclarativeStream
+      name: users
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /users
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - data
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/users"
+    contacts:
+      type: DeclarativeStream
+      name: contacts
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /contacts
+          http_method: GET
+          request_parameters:
+            email: "{{ config['email'] }}"
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - data
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/contacts"
+    messages:
+      type: DeclarativeStream
+      name: messages
+      primary_key:
+        - id
+      retriever:
+        type: SimpleRetriever
+        requester:
+          $ref: "#/definitions/base_requester"
+          path: /conversations/{{ stream_partition.parent_id }}/messages
+          http_method: GET
+        record_selector:
+          type: RecordSelector
+          extractor:
+            type: DpathExtractor
+            field_path:
+              - data
+              - messages
+        paginator:
+          type: DefaultPaginator
+          page_token_option:
+            type: RequestPath
+          pagination_strategy:
+            type: CursorPagination
+            cursor_value: "{{ last_record['next'] }}"
+        partition_router:
+          - type: SubstreamPartitionRouter
+            parent_stream_configs:
+              - type: ParentStreamConfig
+                parent_key: id
+                partition_field: parent_id
+                stream:
+                  $ref: "#/definitions/streams/conversations"
+      schema_loader:
+        type: InlineSchemaLoader
+        schema:
+          $ref: "#/schemas/messages"
+  base_requester:
     type: HttpRequester
-    url_base: "https://driftapi.com"
-    http_method: "GET"
+    url_base: https://driftapi.com
     authenticator:
       type: BearerAuthenticator
       api_token: "{{ config['credentials']['access_token'] }}"
 
-  retriever:
-    type: SimpleRetriever
-    record_selector:
-      $ref: "#/definitions/selector"
-    paginator:
-      type: "NoPagination"
-    requester:
-      $ref: "#/definitions/requester"
-
-  base_stream:
-    type: DeclarativeStream
-    retriever:
-      $ref: "#/definitions/retriever"
-
-  base_paginator:
-    type: "DefaultPaginator"
-    pagination_strategy:
-      type: "CursorPagination"
-      cursor_value: "{{ last_record['next'] }}"
-    page_token_option:
-      type: "RequestPath"
-      field_name: "page_token"
-      inject_into: "request_parameter"
-
-  accounts_stream:
-    $ref: "#/definitions/base_stream"
-    retriever:
-      $ref: "#/definitions/retriever"
-      paginator:
-        $ref: "#/definitions/base_paginator"
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: ["data", "accounts"]
-    name: "accounts"
-    primary_key: "ownerId"
-    $parameters:
-      path: "/accounts"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
+streams:
+  - $ref: "#/definitions/streams/accounts"
+  - $ref: "#/definitions/streams/conversations"
+  - $ref: "#/definitions/streams/users"
+  - $ref: "#/definitions/streams/contacts"
+  - $ref: "#/definitions/streams/messages"
+
+spec:
+  type: Spec
+  connection_specification:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    required: []
+    properties:
+      credentials:
+        type: object
+        title: Authorization Method
+        oneOf:
+          - type: object
+            title: OAuth2.0
+            required:
+              - client_id
+              - client_secret
+              - access_token
+              - refresh_token
+            properties:
+              credentials:
+                type: string
+                const: oauth2.0
+                order: 0
+              client_id:
+                type: string
+                title: Client ID
+                description: The Client ID of your Drift developer application.
+                airbyte_secret: true
+              client_secret:
+                type: string
+                title: Client Secret
+                description: The Client Secret of your Drift developer application.
+                airbyte_secret: true
+              access_token:
+                type: string
+                title: Access Token
+                description: Access Token for making authenticated requests.
+                airbyte_secret: true
+              refresh_token:
+                type: string
+                title: Refresh Token
+                description: Refresh Token to renew the expired Access Token.
+                airbyte_secret: true
+          - type: object
+            title: Access Token
+            required:
+              - access_token
+            properties:
+              credentials:
+                type: string
+                const: access_token
+                order: 0
+              access_token:
+                type: string
+                title: Access Token
+                description: >-
+                  Drift Access Token. See the <a
+                  href="https://docs.airbyte.com/integrations/sources/drift">docs</a>
+                  for more information on how to generate this key.
+                airbyte_secret: true
+        order: 0
+      email:
+        type: string
+        description: Email used as parameter for contacts stream
+        title: Email parameter for contacts stream
+        default: test@test.com
+        order: 1
+    additionalProperties: true
+  advanced_auth:
+    auth_flow_type: oauth2.0
+    predicate_key:
+      - credentials
+      - credentials
+    predicate_value: oauth2.0
+    oauth_config_specification:
+      complete_oauth_output_specification:
         type: object
         properties:
-          ownerId:
-            description: The unique identifier of the account owner
-            type: integer
-          name:
-            description: The name of the account
+          access_token:
             type: string
-          domain:
-            description: The domain associated with the account
+            path_in_connector_config:
+              - credentials
+              - access_token
+          refresh_token:
+            type: string
+            path_in_connector_config:
+              - credentials
+              - refresh_token
+      complete_oauth_server_input_specification:
+        type: object
+        properties:
+          client_id:
             type: string
-          accountId:
-            description: The unique identifier for the account
+          client_secret:
             type: string
-          customProperties:
-            description: Additional custom properties for the account
-            type: array
-            items:
-              description: A custom property for the account
-              type: object
-              properties:
-                label:
-                  description: The label for a custom property
-                  type: string
-                name:
-                  description: The name of the custom property
-                  type: string
-                value:
-                  description: The value of the custom property
-                type:
-                  description: The type of the custom property
-                  type: string
-          deleted:
-            description: Indicates if the account has been deleted
-            type: boolean
-          createDateTime:
-            description: The date and time when the account was created
-            type: integer
-          updateDateTime:
-            description: The date and time when the account was last updated
-            type: integer
-          targeted:
-            description: Indicates if the account is a targeted account
-            type: boolean
-  conversations_stream:
-    $ref: "#/definitions/base_stream"
-    retriever:
-      $ref: "#/definitions/retriever"
-      paginator:
-        $ref: "#/definitions/base_paginator"
-    name: "conversations"
-    primary_key: "id"
-    $parameters:
-      path: "/conversations"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
+      complete_oauth_server_output_specification:
         type: object
         properties:
-          id:
-            description: The unique identifier of the conversation.
-            type: integer
-          participants:
-            description: List of participants involved in the conversation
-            type: array
-            items:
-              description: Details of the participants in the conversation.
-              type: integer
-          status:
-            description: The status of the conversation (e.g., open, closed, in progress).
+          client_id:
             type: string
-            enum:
-              - open
-              - closed
-              - pending
-              - bulk_sent
-          contactId:
-            description:
-              The unique identifier of the contact associated with the
-              conversation.
-            type: integer
-          inboxId:
-            description:
-              The unique identifier of the inbox where the conversation
-              belongs.
-            type: integer
-          createdAt:
-            description: The timestamp when the conversation was created.
-            type: integer
-          updatedAt:
-            description: The timestamp when the conversation was last updated.
-            type: integer
-          relatedPlaybookId:
-            description:
-              The unique identifier of the playbook related to the conversation,
-              if any.
+            path_in_connector_config:
+              - credentials
+              - client_id
+          client_secret:
+            type: string
+            path_in_connector_config:
+              - credentials
+              - client_secret
+
+metadata:
+  autoImportSchema:
+    accounts: false
+    conversations: false
+    users: false
+    contacts: false
+    messages: false
+
+schemas:
+  accounts:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    properties:
+      accountId:
+        type: string
+        description: The unique identifier for the account
+      createDateTime:
+        type: integer
+        description: The date and time when the account was created
+      customProperties:
+        type: array
+        description: Additional custom properties for the account
+        items:
+          type: object
+          description: A custom property for the account
+          properties:
             type:
-              - "null"
-              - string
-          conversationTags:
-            description: Tags associated with the conversation
-            type: array
-            items:
-              description: Properties of each conversation tag
-              type: object
-              properties:
-                color:
-                  type: string
-                  description: HEX value
-                name:
-                  description: The name of the tag associated with the conversation.
-                  type: string
-  users_stream:
-    $ref: "#/definitions/base_stream"
-    name: "users"
-    primary_key: "id"
-    $parameters:
-      path: "/users"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
+              type: string
+              description: The type of the custom property
+            label:
+              type: string
+              description: The label for a custom property
+            name:
+              type: string
+              description: The name of the custom property
+            value:
+              description: The value of the custom property
+      deleted:
+        type: boolean
+        description: Indicates if the account has been deleted
+      domain:
+        type: string
+        description: The domain associated with the account
+      name:
+        type: string
+        description: The name of the account
+      ownerId:
+        type: integer
+        description: The unique identifier of the account owner
+      targeted:
+        type: boolean
+        description: Indicates if the account is a targeted account
+      updateDateTime:
+        type: integer
+        description: The date and time when the account was last updated
+    additionalProperties: true
+  conversations:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    properties:
+      contactId:
+        type: integer
+        description: The unique identifier of the contact associated with the conversation.
+      conversationTags:
+        type: array
+        description: Tags associated with the conversation
+        items:
+          type: object
+          description: Properties of each conversation tag
+          properties:
+            color:
+              type: string
+              description: HEX value
+            name:
+              type: string
+              description: The name of the tag associated with the conversation.
+      createdAt:
+        type: integer
+        description: The timestamp when the conversation was created.
+      id:
+        type: integer
+        description: The unique identifier of the conversation.
+      inboxId:
+        type: integer
+        description: The unique identifier of the inbox where the conversation belongs.
+      participants:
+        type: array
+        description: List of participants involved in the conversation
+        items:
+          type: integer
+          description: Details of the participants in the conversation.
+      relatedPlaybookId:
+        type:
+          - "null"
+          - string
+        description: >-
+          The unique identifier of the playbook related to the conversation, if
+          any.
+      status:
+        type: string
+        description: The status of the conversation (e.g., open, closed, in progress).
+        enum:
+          - open
+          - closed
+          - pending
+          - bulk_sent
+      updatedAt:
+        type: integer
+        description: The timestamp when the conversation was last updated.
+    additionalProperties: true
+  users:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    properties:
+      alias:
+        type: string
+        description: User's alias used for identification.
+      availability:
+        type: string
+        description: User's availability status.
+      avatarUrl:
+        type: string
+        description: URL for the user's avatar image.
+      bot:
+        type: boolean
+        description: Flag indicating if the user is a bot.
+      createdAt:
+        type: integer
+        description: Timestamp when the user was created.
+      email:
+        type: string
+        description: User's email address.
+      id:
+        type: integer
+        description: Unique identifier for the user.
+      locale:
+        type: string
+        description: User's preferred language and region settings.
+      name:
+        type: string
+        description: User's full name.
+      orgId:
+        type: integer
+        description: Identifier for the organization the user belongs to.
+      phone:
+        type: string
+        description: User's phone number.
+      role:
+        type: string
+        description: User's role or permission level.
+      timeZone:
+        type: string
+        description: User's preferred time zone.
+      updatedAt:
+        type: integer
+        description: Timestamp when the user was last updated.
+      verified:
+        type: boolean
+        description: Flag indicating if the user's account is verified.
+    additionalProperties: true
+  contacts:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    properties:
+      attributes:
         type: object
+        description: Additional details of the contact
         properties:
-          id:
-            description: Unique identifier for the user.
-            type: integer
-          orgId:
-            description: Identifier for the organization the user belongs to.
-            type: integer
-          name:
-            description: User's full name.
-            type: string
-          alias:
-            description: User's alias used for identification.
-            type: string
           email:
-            description: User's email address.
-            type: string
-          phone:
-            description: User's phone number.
-            type: string
-          locale:
-            description: User's preferred language and region settings.
-            type: string
-          availability:
-            description: User's availability status.
-            type: string
-          role:
-            description: User's role or permission level.
-            type: string
-          timeZone:
-            description: User's preferred time zone.
-            type: string
-          avatarUrl:
-            description: URL for the user's avatar image.
             type: string
-          verified:
-            description: Flag indicating if the user's account is verified.
-            type: boolean
-          bot:
-            description: Flag indicating if the user is a bot.
-            type: boolean
-          createdAt:
-            description: Timestamp when the user was created.
-            type: integer
-          updatedAt:
-            description: Timestamp when the user was last updated.
-            type: integer
-  contacts_stream:
-    $ref: "#/definitions/base_stream"
-    $parameters:
-      name: "contacts"
-      primary_key: "id"
-      path: "/contacts"
-    retriever:
-      $ref: "#/definitions/retriever"
-      requester:
-        $ref: "#/definitions/requester"
-        request_parameters:
-          email: "{{ config['email'] }}"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
-        type: object
-        properties:
-          id:
-            description: Unique identifier for the contact
-            type: integer
+            description: Email address of the contact
+          events:
+            description: Events related to the contact
           name:
+            type: string
             description: Name of the contact
+          phone:
             type: string
-          attributes:
-            description: Additional details of the contact
-            type: object
-            properties:
-              name:
-                description: Name of the contact
-                type: string
-              email:
-                description: Email address of the contact
-                type: string
-              phone:
-                description: Phone number of the contact
-                type: string
-              tags:
-                description: Tags associated with the contact
-                type: array
-                items:
-                  description: Tag name
-                  type: string
-              events:
-                description: Events related to the contact
-              socialProfiles:
-                description: Social media profiles of the contact
-          createdAt:
-            description: Timestamp of when the contact was created
-            type: integer
-  messages_partition_router:
-    type: SubstreamPartitionRouter
-    parent_stream_configs:
-      - stream: "#/definitions/conversations_stream"
-        parent_key: "id"
-        partition_field: "parent_id"
-
-  messages_stream:
-    $ref: "#/definitions/base_stream"
-    $parameters:
-      name: "messages"
-      primary_key: "id"
-      path: "/conversations/{{ stream_partition.parent_id }}/messages"
-    retriever:
-      $ref: "#/definitions/retriever"
-      paginator:
-        $ref: "#/definitions/base_paginator"
-      record_selector:
-        type: RecordSelector
-        extractor:
-          type: DpathExtractor
-          field_path: ["data", "messages"]
-      partition_router:
-        $ref: "#/definitions/messages_partition_router"
-
-    schema_loader:
-      type: InlineSchemaLoader
-      schema:
-        $schema: http://json-schema.org/draft-07/schema#
+            description: Phone number of the contact
+          socialProfiles:
+            description: Social media profiles of the contact
+          tags:
+            type: array
+            description: Tags associated with the contact
+            items:
+              type: string
+              description: Tag name
+      createdAt:
+        type: integer
+        description: Timestamp of when the contact was created
+      id:
+        type: integer
+        description: Unique identifier for the contact
+      name:
+        type: string
+        description: Name of the contact
+    additionalProperties: true
+  messages:
+    type: object
+    $schema: http://json-schema.org/draft-07/schema#
+    properties:
+      type:
+        type: string
+        description: Type of message (e.g., text, image, file).
+      attributes:
         type: object
+        description: Additional attributes associated with the message.
+      author:
+        type: object
+        description: Details about the author of the message.
         properties:
-          id:
-            description: Unique identifier of the message.
-            type: integer
-          orgId:
-            description:
-              Unique identifier of the organization associated with the
-              message.
-            type: integer
-          body:
-            description: The main content/body of the message.
-            type: string
-          author:
-            description: Details about the author of the message.
-            type: object
-            properties:
-              type:
-                description: Type of the author (e.g., user, bot).
-                type: string
-                enum:
-                  - contact
-                  - user
-              id:
-                description: Unique identifier of the author.
-                type: integer
-              bot:
-                description: Boolean flag indicating if the author is a bot.
-                type: boolean
           type:
-            description: Type of message (e.g., text, image, file).
             type: string
-          conversationId:
-            description:
-              Unique identifier of the conversation associated with the
-              message.
-            type: integer
-          createdAt:
-            description: Timestamp indicating when the message was created.
+            description: Type of the author (e.g., user, bot).
+            enum:
+              - contact
+              - user
+          bot:
+            type: boolean
+            description: Boolean flag indicating if the author is a bot.
+          id:
             type: integer
-          buttons:
-            description: Action buttons associated with the message.
-            type: array
-            items:
+            description: Unique identifier of the author.
+      body:
+        type: string
+        description: The main content/body of the message.
+      buttons:
+        type: array
+        description: Action buttons associated with the message.
+        items:
+          type: object
+          properties:
+            type:
+              type: string
+              description: Type of button (e.g., call to action, link).
+            label:
+              type: string
+              description: Text label displayed on the button.
+            reaction:
               type: object
+              description: Reaction associated with the button click.
               properties:
-                label:
-                  description: Text label displayed on the button.
-                  type: string
-                value:
-                  description:
-                    Value associated with the button (e.g., URL, action
-                    name).
-                  type: string
                 type:
-                  description: Type of button (e.g., call to action, link).
                   type: string
-                style:
-                  description: Visual style of the button (e.g., primary, secondary).
+                  description: Type of reaction triggered (e.g., message, action).
+                message:
                   type: string
-                reaction:
-                  description: Reaction associated with the button click.
-                  type: object
-                  properties:
-                    type:
-                      description: Type of reaction triggered (e.g., message, action).
-                      type: string
-                    message:
-                      description: Message triggered by clicking the button.
-                      type: string
-          context:
-            description: Contextual information related to the message.
-            type: object
-            properties:
-              ip:
-                description: IP address associated with the message.
-                type: string
-              userAgent:
-                description: User agent information of the client device.
-                type: string
-          attributes:
-            description: Additional attributes associated with the message.
-            type: object
-streams:
-  - "#/definitions/accounts_stream"
-  - "#/definitions/conversations_stream"
-  - "#/definitions/users_stream"
-  - "#/definitions/contacts_stream"
-  - "#/definitions/messages_stream"
-
-check:
-  type: CheckStream
-  stream_names:
-    - "accounts"
-    - "conversations"
-    - "users"
-    - "contacts"
-    - "messages"
+                  description: Message triggered by clicking the button.
+            style:
+              type: string
+              description: Visual style of the button (e.g., primary, secondary).
+            value:
+              type: string
+              description: Value associated with the button (e.g., URL, action name).
+      context:
+        type: object
+        description: Contextual information related to the message.
+        properties:
+          ip:
+            type: string
+            description: IP address associated with the message.
+          userAgent:
+            type: string
+            description: User agent information of the client device.
+      conversationId:
+        type: integer
+        description: Unique identifier of the conversation associated with the message.
+      createdAt:
+        type: integer
+        description: Timestamp indicating when the message was created.
+      id:
+        type: integer
+        description: Unique identifier of the message.
+      orgId:
+        type: integer
+        description: Unique identifier of the organization associated with the message.
+    additionalProperties: true
```

### Comparing `airbyte_source_drift-0.3.4/PKG-INFO` & `airbyte_source_drift-0.3.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-drift
-Version: 0.3.4
+Version: 0.3.5
 Summary: Source implementation for Drift.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (>=0,<1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/drift
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Drift source connector
 
-
 This is the repository for the Drift source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/drift).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/drift)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_drift/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-drift spec
 poetry run source-drift check --config secrets/config.json
 poetry run source-drift discover --config secrets/config.json
 poetry run source-drift read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-drift build
 ```
 
 An image will be available on your host with the tag `airbyte/source-drift:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-drift:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-drift:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-drift:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-drift:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-drift test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-drift test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/drift.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

