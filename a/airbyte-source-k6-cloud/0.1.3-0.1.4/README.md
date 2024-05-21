# Comparing `tmp/airbyte_source_k6_cloud-0.1.3.tar.gz` & `tmp/airbyte_source_k6_cloud-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_k6_cloud-0.1.3.tar", max compression
+gzip compressed data, was "airbyte_source_k6_cloud-0.1.4.tar", max compression
```

## Comparing `airbyte_source_k6_cloud-0.1.3.tar` & `airbyte_source_k6_cloud-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4532 2024-05-01 18:49:32.119271 airbyte_source_k6_cloud-0.1.3/README.md
--rw-r--r--   0        0        0      755 2024-05-01 18:55:57.682630 airbyte_source_k6_cloud-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      126 2024-05-01 18:49:32.119271 airbyte_source_k6_cloud-0.1.3/source_k6_cloud/__init__.py
--rw-r--r--   0        0        0     6276 2024-05-01 18:49:32.119271 airbyte_source_k6_cloud-0.1.3/source_k6_cloud/manifest.yaml
--rw-r--r--   0        0        0      234 2024-05-01 18:49:32.119271 airbyte_source_k6_cloud-0.1.3/source_k6_cloud/run.py
--rw-r--r--   0        0        0      476 2024-05-01 18:49:32.119271 airbyte_source_k6_cloud-0.1.3/source_k6_cloud/source.py
--rw-r--r--   0        0        0      500 2024-05-01 18:49:32.119271 airbyte_source_k6_cloud-0.1.3/source_k6_cloud/spec.yaml
--rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 airbyte_source_k6_cloud-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4542 2024-05-21 00:47:43.000000 airbyte_source_k6_cloud-0.1.4/README.md
+-rw-r--r--   0        0        0      755 2024-05-21 01:15:33.514494 airbyte_source_k6_cloud-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-21 00:47:43.000000 airbyte_source_k6_cloud-0.1.4/source_k6_cloud/__init__.py
+-rw-r--r--   0        0        0     7156 2024-05-21 00:47:43.000000 airbyte_source_k6_cloud-0.1.4/source_k6_cloud/manifest.yaml
+-rw-r--r--   0        0        0      234 2024-05-21 00:47:43.000000 airbyte_source_k6_cloud-0.1.4/source_k6_cloud/run.py
+-rw-r--r--   0        0        0      476 2024-05-21 00:47:43.000000 airbyte_source_k6_cloud-0.1.4/source_k6_cloud/source.py
+-rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 airbyte_source_k6_cloud-0.1.4/PKG-INFO
```

### Comparing `airbyte_source_k6_cloud-0.1.3/README.md` & `airbyte_source_k6_cloud-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # K6-Cloud source connector
 
-
 This is the repository for the K6-Cloud source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/k6-cloud).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/k6-cloud)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_k6_cloud/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-k6-cloud spec
 poetry run source-k6-cloud check --config secrets/config.json
 poetry run source-k6-cloud discover --config secrets/config.json
 poetry run source-k6-cloud read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-k6-cloud build
 ```
 
 An image will be available on your host with the tag `airbyte/source-k6-cloud:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-k6-cloud:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-k6-cloud:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-k6-cloud:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-k6-cloud:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-k6-cloud test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-k6-cloud test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/k6-cloud.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_k6_cloud-0.1.3/pyproject.toml` & `airbyte_source_k6_cloud-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.1.3"
+version = "0.1.4"
 name = "airbyte-source-k6-cloud"
 description = "Source implementation for K6 Cloud."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_k6_cloud-0.1.3/source_k6_cloud/manifest.yaml` & `airbyte_source_k6_cloud-0.1.4/source_k6_cloud/manifest.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,393 +1,448 @@
-00000000: 7665 7273 696f 6e3a 2022 302e 3239 2e30  version: "0.29.0
-00000010: 220a 0a64 6566 696e 6974 696f 6e73 3a0a  "..definitions:.
-00000020: 2020 7365 6c65 6374 6f72 3a0a 2020 2020    selector:.    
-00000030: 6578 7472 6163 746f 723a 0a20 2020 2020  extractor:.     
-00000040: 2066 6965 6c64 5f70 6174 683a 0a20 2020   field_path:.   
-00000050: 2020 2020 202d 2022 7b7b 2070 6172 616d       - "{{ param
-00000060: 6574 6572 735b 276e 616d 6527 5d20 7d7d  eters['name'] }}
-00000070: 220a 2020 7265 7175 6573 7465 723a 0a20  ".  requester:. 
-00000080: 2020 2075 726c 5f62 6173 653a 2022 6874     url_base: "ht
-00000090: 7470 733a 2f2f 6170 692e 6b36 2e69 6f22  tps://api.k6.io"
-000000a0: 0a20 2020 2068 7474 705f 6d65 7468 6f64  .    http_method
-000000b0: 3a20 2247 4554 220a 2020 2020 6175 7468  : "GET".    auth
-000000c0: 656e 7469 6361 746f 723a 0a20 2020 2020  enticator:.     
-000000d0: 2074 7970 653a 2042 6561 7265 7241 7574   type: BearerAut
-000000e0: 6865 6e74 6963 6174 6f72 0a20 2020 2020  henticator.     
-000000f0: 2061 7069 5f74 6f6b 656e 3a20 227b 7b20   api_token: "{{ 
-00000100: 636f 6e66 6967 5b27 6170 695f 746f 6b65  config['api_toke
-00000110: 6e27 5d20 7d7d 220a 0a20 2069 6e63 7265  n'] }}"..  incre
-00000120: 6d65 6e74 5f70 6167 696e 6174 6f72 3a0a  ment_paginator:.
-00000130: 2020 2020 7479 7065 3a20 2244 6566 6175      type: "Defau
-00000140: 6c74 5061 6769 6e61 746f 7222 0a20 2020  ltPaginator".   
-00000150: 2070 6167 696e 6174 696f 6e5f 7374 7261   pagination_stra
-00000160: 7465 6779 3a0a 2020 2020 2020 7479 7065  tegy:.      type
-00000170: 3a20 2250 6167 6549 6e63 7265 6d65 6e74  : "PageIncrement
-00000180: 220a 2020 2020 2020 7061 6765 5f73 697a  ".      page_siz
-00000190: 653a 2033 320a 2020 2020 7061 6765 5f74  e: 32.    page_t
-000001a0: 6f6b 656e 5f6f 7074 696f 6e3a 0a20 2020  oken_option:.   
-000001b0: 2020 2074 7970 653a 2052 6571 7565 7374     type: Request
-000001c0: 4f70 7469 6f6e 0a20 2020 2020 2069 6e6a  Option.      inj
-000001d0: 6563 745f 696e 746f 3a20 2272 6571 7565  ect_into: "reque
-000001e0: 7374 5f70 6172 616d 6574 6572 220a 2020  st_parameter".  
-000001f0: 2020 2020 6669 656c 645f 6e61 6d65 3a20      field_name: 
-00000200: 2270 6167 6522 0a20 2020 2070 6167 655f  "page".    page_
-00000210: 7369 7a65 5f6f 7074 696f 6e3a 0a20 2020  size_option:.   
-00000220: 2020 2069 6e6a 6563 745f 696e 746f 3a20     inject_into: 
-00000230: 2262 6f64 795f 6461 7461 220a 2020 2020  "body_data".    
-00000240: 2020 6669 656c 645f 6e61 6d65 3a20 2270    field_name: "p
-00000250: 6167 655f 7369 7a65 220a 2020 7265 7472  age_size".  retr
-00000260: 6965 7665 723a 0a20 2020 2072 6563 6f72  iever:.    recor
-00000270: 645f 7365 6c65 6374 6f72 3a0a 2020 2020  d_selector:.    
-00000280: 2020 2472 6566 3a20 2223 2f64 6566 696e    $ref: "#/defin
-00000290: 6974 696f 6e73 2f73 656c 6563 746f 7222  itions/selector"
-000002a0: 0a20 2020 2070 6167 696e 6174 6f72 3a0a  .    paginator:.
-000002b0: 2020 2020 2020 2472 6566 3a20 2223 2f64        $ref: "#/d
-000002c0: 6566 696e 6974 696f 6e73 2f69 6e63 7265  efinitions/incre
-000002d0: 6d65 6e74 5f70 6167 696e 6174 6f72 220a  ment_paginator".
-000002e0: 2020 2020 7265 7175 6573 7465 723a 0a20      requester:. 
-000002f0: 2020 2020 2024 7265 663a 2022 232f 6465       $ref: "#/de
-00000300: 6669 6e69 7469 6f6e 732f 7265 7175 6573  finitions/reques
-00000310: 7465 7222 0a20 2062 6173 655f 7374 7265  ter".  base_stre
-00000320: 616d 3a0a 2020 2020 7265 7472 6965 7665  am:.    retrieve
-00000330: 723a 0a20 2020 2020 2024 7265 663a 2022  r:.      $ref: "
-00000340: 232f 6465 6669 6e69 7469 6f6e 732f 7265  #/definitions/re
-00000350: 7472 6965 7665 7222 0a20 206f 7267 616e  triever".  organ
-00000360: 697a 6174 696f 6e73 5f73 7472 6561 6d3a  izations_stream:
-00000370: 0a20 2020 2024 7265 663a 2022 232f 6465  .    $ref: "#/de
-00000380: 6669 6e69 7469 6f6e 732f 6261 7365 5f73  finitions/base_s
-00000390: 7472 6561 6d22 0a20 2020 2072 6574 7269  tream".    retri
-000003a0: 6576 6572 3a0a 2020 2020 2020 7265 636f  ever:.      reco
-000003b0: 7264 5f73 656c 6563 746f 723a 0a20 2020  rd_selector:.   
-000003c0: 2020 2020 2024 7265 663a 2022 232f 6465       $ref: "#/de
-000003d0: 6669 6e69 7469 6f6e 732f 7365 6c65 6374  finitions/select
-000003e0: 6f72 220a 2020 2020 2020 7061 6769 6e61  or".      pagina
-000003f0: 746f 723a 0a20 2020 2020 2020 2074 7970  tor:.        typ
-00000400: 653a 204e 6f50 6167 696e 6174 696f 6e0a  e: NoPagination.
-00000410: 2020 2020 2020 7265 7175 6573 7465 723a        requester:
-00000420: 0a20 2020 2020 2020 2024 7265 663a 2022  .        $ref: "
-00000430: 232f 6465 6669 6e69 7469 6f6e 732f 7265  #/definitions/re
-00000440: 7175 6573 7465 7222 0a20 2020 2024 7061  quester".    $pa
-00000450: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-00000460: 6e61 6d65 3a20 226f 7267 616e 697a 6174  name: "organizat
-00000470: 696f 6e73 220a 2020 2020 2020 7072 696d  ions".      prim
-00000480: 6172 795f 6b65 793a 2022 6964 220a 2020  ary_key: "id".  
-00000490: 2020 2020 7061 7468 3a20 222f 7633 2f6f      path: "/v3/o
-000004a0: 7267 616e 697a 6174 696f 6e73 220a 2020  rganizations".  
-000004b0: 2020 7363 6865 6d61 5f6c 6f61 6465 723a    schema_loader:
-000004c0: 0a20 2020 2020 2074 7970 653a 2049 6e6c  .      type: Inl
-000004d0: 696e 6553 6368 656d 614c 6f61 6465 720a  ineSchemaLoader.
-000004e0: 2020 2020 2020 7363 6865 6d61 3a0a 2020        schema:.  
-000004f0: 2020 2020 2020 2473 6368 656d 613a 2068        $schema: h
-00000500: 7474 703a 2f2f 6a73 6f6e 2d73 6368 656d  ttp://json-schem
-00000510: 612e 6f72 672f 6472 6166 742d 3037 2f73  a.org/draft-07/s
-00000520: 6368 656d 6123 0a20 2020 2020 2020 2074  chema#.        t
-00000530: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
-00000540: 2020 2020 7072 6f70 6572 7469 6573 3a0a      properties:.
-00000550: 2020 2020 2020 2020 2020 6964 3a0a 2020            id:.  
-00000560: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00000570: 7074 696f 6e3a 2054 6865 2075 6e69 7175  ption: The uniqu
-00000580: 6520 6964 656e 7469 6669 6572 2066 6f72  e identifier for
-00000590: 2074 6865 206f 7267 616e 697a 6174 696f   the organizatio
-000005a0: 6e2e 0a20 2020 2020 2020 2020 2020 2074  n..            t
-000005b0: 7970 653a 2069 6e74 6567 6572 0a20 2020  ype: integer.   
-000005c0: 2020 2020 2020 206e 616d 653a 0a20 2020         name:.   
-000005d0: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-000005e0: 7469 6f6e 3a20 5468 6520 6e61 6d65 206f  tion: The name o
-000005f0: 6620 7468 6520 6f72 6761 6e69 7a61 7469  f the organizati
-00000600: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-00000610: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
-00000620: 2020 2020 2020 206f 776e 6572 5f69 643a         owner_id:
-00000630: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00000640: 6372 6970 7469 6f6e 3a20 5468 6520 7573  cription: The us
-00000650: 6572 2049 4420 6f66 2074 6865 206f 776e  er ID of the own
-00000660: 6572 206f 7220 6372 6561 746f 7220 6f66  er or creator of
-00000670: 2074 6865 206f 7267 616e 697a 6174 696f   the organizatio
-00000680: 6e2e 0a20 2020 2020 2020 2020 2020 2074  n..            t
-00000690: 7970 653a 2069 6e74 6567 6572 0a20 2020  ype: integer.   
-000006a0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-000006b0: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
-000006c0: 6465 7363 7269 7074 696f 6e3a 2041 2074  description: A t
-000006d0: 6578 7475 616c 2064 6573 6372 6970 7469  extual descripti
-000006e0: 6f6e 206f 7220 6465 7461 696c 7320 6162  on or details ab
-000006f0: 6f75 7420 7468 6520 6f72 6761 6e69 7a61  out the organiza
-00000700: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
-00000710: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-00000720: 2020 2020 2020 2020 2062 696c 6c69 6e67           billing
-00000730: 5f61 6464 7265 7373 3a0a 2020 2020 2020  _address:.      
-00000740: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00000750: 6e3a 2054 6865 2062 696c 6c69 6e67 2061  n: The billing a
-00000760: 6464 7265 7373 206f 6620 7468 6520 6f72  ddress of the or
-00000770: 6761 6e69 7a61 7469 6f6e 2e0a 2020 2020  ganization..    
-00000780: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
-00000790: 7269 6e67 0a20 2020 2020 2020 2020 2062  ring.          b
-000007a0: 696c 6c69 6e67 5f63 6f75 6e74 7279 3a0a  illing_country:.
-000007b0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
-000007c0: 7269 7074 696f 6e3a 2054 6865 2063 6f75  ription: The cou
-000007d0: 6e74 7279 2061 7373 6f63 6961 7465 6420  ntry associated 
-000007e0: 7769 7468 2074 6865 2062 696c 6c69 6e67  with the billing
-000007f0: 2061 6464 7265 7373 206f 6620 7468 6520   address of the 
-00000800: 6f72 6761 6e69 7a61 7469 6f6e 2e0a 2020  organization..  
-00000810: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-00000820: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-00000830: 2062 696c 6c69 6e67 5f65 6d61 696c 3a0a   billing_email:.
-00000840: 2020 2020 2020 2020 2020 2020 6465 7363              desc
-00000850: 7269 7074 696f 6e3a 2054 6865 2062 696c  ription: The bil
-00000860: 6c69 6e67 2065 6d61 696c 2061 6464 7265  ling email addre
-00000870: 7373 2066 6f72 2074 6865 206f 7267 616e  ss for the organ
-00000880: 697a 6174 696f 6e2e 0a20 2020 2020 2020  ization..       
-00000890: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-000008a0: 670a 2020 2020 2020 2020 2020 7661 745f  g.          vat_
-000008b0: 6e75 6d62 6572 3a0a 2020 2020 2020 2020  number:.        
-000008c0: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-000008d0: 2056 616c 7565 2d61 6464 6564 2074 6178   Value-added tax
-000008e0: 2028 5641 5429 206e 756d 6265 7220 666f   (VAT) number fo
-000008f0: 7220 7468 6520 6f72 6761 6e69 7a61 7469  r the organizati
-00000900: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-00000910: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
-00000920: 2020 2020 2020 2063 7265 6174 6564 3a0a         created:.
-00000930: 2020 2020 2020 2020 2020 2020 6465 7363              desc
-00000940: 7269 7074 696f 6e3a 2054 6865 2074 696d  ription: The tim
-00000950: 6573 7461 6d70 2077 6865 6e20 7468 6520  estamp when the 
-00000960: 6f72 6761 6e69 7a61 7469 6f6e 2077 6173  organization was
-00000970: 2063 7265 6174 6564 2e0a 2020 2020 2020   created..      
-00000980: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
-00000990: 6e67 0a20 2020 2020 2020 2020 2075 7064  ng.          upd
-000009a0: 6174 6564 3a0a 2020 2020 2020 2020 2020  ated:.          
-000009b0: 2020 6465 7363 7269 7074 696f 6e3a 2054    description: T
-000009c0: 6865 2074 696d 6573 7461 6d70 2077 6865  he timestamp whe
-000009d0: 6e20 7468 6520 6f72 6761 6e69 7a61 7469  n the organizati
-000009e0: 6f6e 2064 6174 6120 7761 7320 6c61 7374  on data was last
-000009f0: 2075 7064 6174 6564 2e0a 2020 2020 2020   updated..      
-00000a00: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
-00000a10: 6e67 0a20 2020 2020 2020 2020 2069 735f  ng.          is_
-00000a20: 6465 6661 756c 743a 0a20 2020 2020 2020  default:.       
-00000a30: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-00000a40: 3a20 496e 6469 6361 7465 7320 6966 2074  : Indicates if t
-00000a50: 6865 206f 7267 616e 697a 6174 696f 6e20  he organization 
-00000a60: 6973 2073 6574 2061 7320 7468 6520 6465  is set as the de
-00000a70: 6661 756c 7420 6f72 6761 6e69 7a61 7469  fault organizati
-00000a80: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-00000a90: 7479 7065 3a20 626f 6f6c 6561 6e0a 2020  type: boolean.  
-00000aa0: 2020 2020 2020 2020 6973 5f73 616d 6c5f          is_saml_
-00000ab0: 6f72 673a 0a20 2020 2020 2020 2020 2020  org:.           
-00000ac0: 2064 6573 6372 6970 7469 6f6e 3a20 466c   description: Fl
-00000ad0: 6167 2073 686f 7769 6e67 2069 6620 7468  ag showing if th
-00000ae0: 6520 6f72 6761 6e69 7a61 7469 6f6e 2075  e organization u
-00000af0: 7365 7320 5341 4d4c 2066 6f72 2061 7574  ses SAML for aut
-00000b00: 6865 6e74 6963 6174 696f 6e2e 0a20 2020  hentication..   
-00000b10: 2020 2020 2020 2020 2074 7970 653a 2062           type: b
-00000b20: 6f6f 6c65 616e 0a20 206f 7267 616e 697a  oolean.  organiz
-00000b30: 6174 696f 6e73 5f70 6172 7469 7469 6f6e  ations_partition
-00000b40: 5f72 6f75 7465 723a 0a20 2020 2074 7970  _router:.    typ
-00000b50: 653a 2053 7562 7374 7265 616d 5061 7274  e: SubstreamPart
-00000b60: 6974 696f 6e52 6f75 7465 720a 2020 2020  itionRouter.    
-00000b70: 7061 7265 6e74 5f73 7472 6561 6d5f 636f  parent_stream_co
-00000b80: 6e66 6967 733a 0a20 2020 2020 202d 2073  nfigs:.      - s
-00000b90: 7472 6561 6d3a 2022 232f 6465 6669 6e69  tream: "#/defini
-00000ba0: 7469 6f6e 732f 6f72 6761 6e69 7a61 7469  tions/organizati
-00000bb0: 6f6e 735f 7374 7265 616d 220a 2020 2020  ons_stream".    
-00000bc0: 2020 2020 7061 7265 6e74 5f6b 6579 3a20      parent_key: 
-00000bd0: 6964 0a20 2020 2020 2020 2070 6172 7469  id.        parti
-00000be0: 7469 6f6e 5f66 6965 6c64 3a20 6964 0a20  tion_field: id. 
-00000bf0: 2070 726f 6a65 6374 735f 7374 7265 616d   projects_stream
-00000c00: 3a0a 2020 2020 2472 6566 3a20 2223 2f64  :.    $ref: "#/d
-00000c10: 6566 696e 6974 696f 6e73 2f62 6173 655f  efinitions/base_
-00000c20: 7374 7265 616d 220a 2020 2020 7479 7065  stream".    type
-00000c30: 3a20 4465 636c 6172 6174 6976 6553 7472  : DeclarativeStr
-00000c40: 6561 6d0a 2020 2020 2470 6172 616d 6574  eam.    $paramet
-00000c50: 6572 733a 0a20 2020 2020 206e 616d 653a  ers:.      name:
-00000c60: 2022 7072 6f6a 6563 7473 220a 2020 2020   "projects".    
-00000c70: 7265 7472 6965 7665 723a 0a20 2020 2020  retriever:.     
-00000c80: 2024 7265 663a 2022 232f 6465 6669 6e69   $ref: "#/defini
-00000c90: 7469 6f6e 732f 7265 7472 6965 7665 7222  tions/retriever"
-00000ca0: 0a20 2020 2020 2072 6571 7565 7374 6572  .      requester
-00000cb0: 3a0a 2020 2020 2020 2020 2472 6566 3a20  :.        $ref: 
-00000cc0: 2223 2f64 6566 696e 6974 696f 6e73 2f72  "#/definitions/r
-00000cd0: 6571 7565 7374 6572 220a 2020 2020 2020  equester".      
-00000ce0: 2020 7061 7468 3a20 222f 7633 2f6f 7267    path: "/v3/org
-00000cf0: 616e 697a 6174 696f 6e73 2f7b 7b20 7374  anizations/{{ st
-00000d00: 7265 616d 5f73 6c69 6365 2e69 6420 7d7d  ream_slice.id }}
-00000d10: 2f70 726f 6a65 6374 7322 0a20 2020 2020  /projects".     
-00000d20: 2070 6172 7469 7469 6f6e 5f72 6f75 7465   partition_route
-00000d30: 723a 0a20 2020 2020 2020 2024 7265 663a  r:.        $ref:
-00000d40: 2022 232f 6465 6669 6e69 7469 6f6e 732f   "#/definitions/
-00000d50: 6f72 6761 6e69 7a61 7469 6f6e 735f 7061  organizations_pa
-00000d60: 7274 6974 696f 6e5f 726f 7574 6572 220a  rtition_router".
-00000d70: 2020 2020 2020 7265 636f 7264 5f73 656c        record_sel
-00000d80: 6563 746f 723a 0a20 2020 2020 2020 2024  ector:.        $
-00000d90: 7265 663a 2022 232f 6465 6669 6e69 7469  ref: "#/definiti
-00000da0: 6f6e 732f 7365 6c65 6374 6f72 220a 2020  ons/selector".  
-00000db0: 2020 7363 6865 6d61 5f6c 6f61 6465 723a    schema_loader:
-00000dc0: 0a20 2020 2020 2074 7970 653a 2049 6e6c  .      type: Inl
-00000dd0: 696e 6553 6368 656d 614c 6f61 6465 720a  ineSchemaLoader.
-00000de0: 2020 2020 2020 7363 6865 6d61 3a0a 2020        schema:.  
-00000df0: 2020 2020 2020 2473 6368 656d 613a 2068        $schema: h
-00000e00: 7474 703a 2f2f 6a73 6f6e 2d73 6368 656d  ttp://json-schem
-00000e10: 612e 6f72 672f 6472 6166 742d 3037 2f73  a.org/draft-07/s
-00000e20: 6368 656d 6123 0a20 2020 2020 2020 2074  chema#.        t
-00000e30: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
-00000e40: 2020 2020 7072 6f70 6572 7469 6573 3a0a      properties:.
-00000e50: 2020 2020 2020 2020 2020 6964 3a0a 2020            id:.  
-00000e60: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00000e70: 7074 696f 6e3a 2054 6865 2075 6e69 7175  ption: The uniqu
-00000e80: 6520 6964 656e 7469 6669 6572 2066 6f72  e identifier for
-00000e90: 2074 6865 2070 726f 6a65 6374 0a20 2020   the project.   
-00000ea0: 2020 2020 2020 2020 2074 7970 653a 2069           type: i
-00000eb0: 6e74 6567 6572 0a20 2020 2020 2020 2020  nteger.         
-00000ec0: 206e 616d 653a 0a20 2020 2020 2020 2020   name:.         
-00000ed0: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-00000ee0: 5468 6520 6e61 6d65 206f 6620 7468 6520  The name of the 
-00000ef0: 7072 6f6a 6563 740a 2020 2020 2020 2020  project.        
-00000f00: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-00000f10: 0a20 2020 2020 2020 2020 2064 6573 6372  .          descr
-00000f20: 6970 7469 6f6e 3a0a 2020 2020 2020 2020  iption:.        
-00000f30: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-00000f40: 2041 2073 686f 7274 2064 6573 6372 6970   A short descrip
-00000f50: 7469 6f6e 206f 6620 7468 6520 7072 6f6a  tion of the proj
-00000f60: 6563 740a 2020 2020 2020 2020 2020 2020  ect.            
-00000f70: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
-00000f80: 2020 2020 2020 206f 7267 616e 697a 6174         organizat
-00000f90: 696f 6e5f 6964 3a0a 2020 2020 2020 2020  ion_id:.        
-00000fa0: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-00000fb0: 0a20 2020 2020 2020 2020 2020 2020 2054  .              T
-00000fc0: 6865 2075 6e69 7175 6520 6964 656e 7469  he unique identi
-00000fd0: 6669 6572 206f 6620 7468 6520 6f72 6761  fier of the orga
-00000fe0: 6e69 7a61 7469 6f6e 2074 6865 2070 726f  nization the pro
-00000ff0: 6a65 6374 2062 656c 6f6e 6773 0a20 2020  ject belongs.   
-00001000: 2020 2020 2020 2020 2020 2074 6f0a 2020             to.  
-00001010: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-00001020: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
-00001030: 2020 6372 6561 7465 643a 0a20 2020 2020    created:.     
-00001040: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00001050: 6f6e 3a20 5468 6520 7469 6d65 7374 616d  on: The timestam
-00001060: 7020 7768 656e 2074 6865 2070 726f 6a65  p when the proje
-00001070: 6374 2077 6173 2063 7265 6174 6564 0a20  ct was created. 
-00001080: 2020 2020 2020 2020 2020 2074 7970 653a             type:
-00001090: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-000010a0: 2020 7570 6461 7465 643a 0a20 2020 2020    updated:.     
-000010b0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-000010c0: 6f6e 3a20 5468 6520 7469 6d65 7374 616d  on: The timestam
-000010d0: 7020 7768 656e 2074 6865 2070 726f 6a65  p when the proje
-000010e0: 6374 2077 6173 206c 6173 7420 7570 6461  ct was last upda
-000010f0: 7465 640a 2020 2020 2020 2020 2020 2020  ted.            
-00001100: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
-00001110: 2020 2020 2020 2069 735f 6465 6661 756c         is_defaul
-00001120: 743a 0a20 2020 2020 2020 2020 2020 2064  t:.            d
-00001130: 6573 6372 6970 7469 6f6e 3a20 4120 666c  escription: A fl
-00001140: 6167 2069 6e64 6963 6174 696e 6720 6966  ag indicating if
-00001150: 2074 6865 2070 726f 6a65 6374 2069 7320   the project is 
-00001160: 7468 6520 6465 6661 756c 7420 6f6e 650a  the default one.
-00001170: 2020 2020 2020 2020 2020 2020 7479 7065              type
-00001180: 3a20 626f 6f6c 6561 6e0a 2020 7465 7374  : boolean.  test
-00001190: 735f 7374 7265 616d 3a0a 2020 2020 2472  s_stream:.    $r
-000011a0: 6566 3a20 2223 2f64 6566 696e 6974 696f  ef: "#/definitio
-000011b0: 6e73 2f62 6173 655f 7374 7265 616d 220a  ns/base_stream".
-000011c0: 2020 2020 7265 7472 6965 7665 723a 0a20      retriever:. 
-000011d0: 2020 2020 2072 6563 6f72 645f 7365 6c65       record_sele
-000011e0: 6374 6f72 3a0a 2020 2020 2020 2020 2472  ctor:.        $r
-000011f0: 6566 3a20 2223 2f64 6566 696e 6974 696f  ef: "#/definitio
-00001200: 6e73 2f73 656c 6563 746f 7222 0a20 2020  ns/selector".   
-00001210: 2020 2070 6167 696e 6174 6f72 3a0a 2020     paginator:.  
-00001220: 2020 2020 2020 2472 6566 3a20 2223 2f64        $ref: "#/d
-00001230: 6566 696e 6974 696f 6e73 2f69 6e63 7265  efinitions/incre
-00001240: 6d65 6e74 5f70 6167 696e 6174 6f72 220a  ment_paginator".
-00001250: 2020 2020 2020 7265 7175 6573 7465 723a        requester:
-00001260: 0a20 2020 2020 2020 2024 7265 663a 2022  .        $ref: "
-00001270: 232f 6465 6669 6e69 7469 6f6e 732f 7265  #/definitions/re
-00001280: 7175 6573 7465 7222 0a20 2020 2024 7061  quester".    $pa
-00001290: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
-000012a0: 6e61 6d65 3a20 226b 362d 7465 7374 7322  name: "k6-tests"
-000012b0: 0a20 2020 2020 2070 7269 6d61 7279 5f6b  .      primary_k
-000012c0: 6579 3a20 2269 6422 0a20 2020 2020 2070  ey: "id".      p
-000012d0: 6174 683a 2022 6c6f 6164 7465 7374 732f  ath: "loadtests/
-000012e0: 7632 2f74 6573 7473 220a 0a20 2020 2073  v2/tests"..    s
-000012f0: 6368 656d 615f 6c6f 6164 6572 3a0a 2020  chema_loader:.  
-00001300: 2020 2020 7479 7065 3a20 496e 6c69 6e65      type: Inline
-00001310: 5363 6865 6d61 4c6f 6164 6572 0a20 2020  SchemaLoader.   
-00001320: 2020 2073 6368 656d 613a 0a20 2020 2020     schema:.     
-00001330: 2020 2024 7363 6865 6d61 3a20 6874 7470     $schema: http
-00001340: 3a2f 2f6a 736f 6e2d 7363 6865 6d61 2e6f  ://json-schema.o
-00001350: 7267 2f64 7261 6674 2d30 372f 7363 6865  rg/draft-07/sche
-00001360: 6d61 230a 2020 2020 2020 2020 7479 7065  ma#.        type
-00001370: 3a20 6f62 6a65 6374 0a20 2020 2020 2020  : object.       
-00001380: 2070 726f 7065 7274 6965 733a 0a20 2020   properties:.   
-00001390: 2020 2020 2020 2069 643a 0a20 2020 2020         id:.     
-000013a0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-000013b0: 6f6e 3a20 556e 6971 7565 2069 6465 6e74  on: Unique ident
-000013c0: 6966 6965 7220 666f 7220 7468 6520 6b36  ifier for the k6
-000013d0: 2074 6573 742e 0a20 2020 2020 2020 2020   test..         
-000013e0: 2020 2074 7970 653a 2069 6e74 6567 6572     type: integer
-000013f0: 0a20 2020 2020 2020 2020 2070 726f 6a65  .          proje
-00001400: 6374 5f69 643a 0a20 2020 2020 2020 2020  ct_id:.         
-00001410: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-00001420: 4964 656e 7469 6669 6572 2066 6f72 2074  Identifier for t
-00001430: 6865 2070 726f 6a65 6374 2074 6f20 7768  he project to wh
-00001440: 6963 6820 7468 6973 206b 3620 7465 7374  ich this k6 test
-00001450: 2062 656c 6f6e 6773 2e0a 2020 2020 2020   belongs..      
-00001460: 2020 2020 2020 7479 7065 3a20 696e 7465        type: inte
-00001470: 6765 720a 2020 2020 2020 2020 2020 7573  ger.          us
-00001480: 6572 5f69 643a 0a20 2020 2020 2020 2020  er_id:.         
-00001490: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-000014a0: 4964 656e 7469 6669 6572 206f 6620 7468  Identifier of th
-000014b0: 6520 7573 6572 2077 686f 206f 776e 7320  e user who owns 
-000014c0: 7468 6973 206b 3620 7465 7374 2e0a 2020  this k6 test..  
-000014d0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-000014e0: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
-000014f0: 2020 6e61 6d65 3a0a 2020 2020 2020 2020    name:.        
-00001500: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-00001510: 204e 616d 6520 6f66 2074 6865 206b 3620   Name of the k6 
-00001520: 7465 7374 2e0a 2020 2020 2020 2020 2020  test..          
-00001530: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-00001540: 2020 2020 2020 2020 2063 7265 6174 6564           created
-00001550: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-00001560: 7363 7269 7074 696f 6e3a 2044 6174 6520  scription: Date 
-00001570: 616e 6420 7469 6d65 2077 6865 6e20 7468  and time when th
-00001580: 6520 6b36 2074 6573 7420 7761 7320 6372  e k6 test was cr
-00001590: 6561 7465 642e 0a20 2020 2020 2020 2020  eated..         
-000015a0: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
-000015b0: 2020 2020 2020 2020 2020 7570 6461 7465            update
-000015c0: 643a 0a20 2020 2020 2020 2020 2020 2064  d:.            d
-000015d0: 6573 6372 6970 7469 6f6e 3a20 4461 7465  escription: Date
-000015e0: 2061 6e64 2074 696d 6520 7768 656e 2074   and time when t
-000015f0: 6865 206b 3620 7465 7374 2077 6173 206c  he k6 test was l
-00001600: 6173 7420 7570 6461 7465 642e 0a20 2020  ast updated..   
-00001610: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
-00001620: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
-00001630: 6c61 7374 5f74 6573 745f 7275 6e5f 6964  last_test_run_id
-00001640: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-00001650: 7363 7269 7074 696f 6e3a 0a20 2020 2020  scription:.     
-00001660: 2020 2020 2020 2020 2049 6465 6e74 6966           Identif
-00001670: 6965 7220 666f 7220 7468 6520 6c61 7374  ier for the last
-00001680: 2074 6573 7420 7275 6e20 6173 736f 6369   test run associ
-00001690: 6174 6564 2077 6974 6820 7468 6973 206b  ated with this k
-000016a0: 360a 2020 2020 2020 2020 2020 2020 2020  6.              
-000016b0: 7465 7374 2e0a 2020 2020 2020 2020 2020  test..          
-000016c0: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-000016d0: 2020 2020 2020 2020 2074 6573 745f 7275           test_ru
-000016e0: 6e5f 6964 733a 0a20 2020 2020 2020 2020  n_ids:.         
-000016f0: 2020 2064 6573 6372 6970 7469 6f6e 3a0a     description:.
-00001700: 2020 2020 2020 2020 2020 2020 2020 4c69                Li
-00001710: 7374 206f 6620 6964 656e 7469 6669 6572  st of identifier
-00001720: 7320 666f 7220 616c 6c20 7465 7374 2072  s for all test r
-00001730: 756e 7320 6173 736f 6369 6174 6564 2077  uns associated w
-00001740: 6974 6820 7468 6973 0a20 2020 2020 2020  ith this.       
-00001750: 2020 2020 2020 206b 3620 7465 7374 2e0a         k6 test..
-00001760: 2020 2020 2020 2020 2020 2020 7479 7065              type
-00001770: 3a20 6172 7261 790a 2020 2020 2020 2020  : array.        
-00001780: 2020 7363 7269 7074 3a0a 2020 2020 2020    script:.      
-00001790: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-000017a0: 6e3a 2054 6865 2073 6372 6970 7420 636f  n: The script co
-000017b0: 6e74 656e 7420 6f66 2074 6865 206b 3620  ntent of the k6 
-000017c0: 7465 7374 2e0a 2020 2020 2020 2020 2020  test..          
-000017d0: 2020 7479 7065 3a20 7374 7269 6e67 0a73    type: string.s
-000017e0: 7472 6561 6d73 3a0a 2020 2d20 2223 2f64  treams:.  - "#/d
-000017f0: 6566 696e 6974 696f 6e73 2f6f 7267 616e  efinitions/organ
-00001800: 697a 6174 696f 6e73 5f73 7472 6561 6d22  izations_stream"
-00001810: 0a20 202d 2022 232f 6465 6669 6e69 7469  .  - "#/definiti
-00001820: 6f6e 732f 7072 6f6a 6563 7473 5f73 7472  ons/projects_str
-00001830: 6561 6d22 0a20 202d 2022 232f 6465 6669  eam".  - "#/defi
-00001840: 6e69 7469 6f6e 732f 7465 7374 735f 7374  nitions/tests_st
-00001850: 7265 616d 220a 0a63 6865 636b 3a0a 2020  ream"..check:.  
-00001860: 7374 7265 616d 5f6e 616d 6573 3a0a 2020  stream_names:.  
-00001870: 2020 2d20 226f 7267 616e 697a 6174 696f    - "organizatio
-00001880: 6e73 220a                                ns".
+00000000: 7665 7273 696f 6e3a 2030 2e37 382e 350a  version: 0.78.5.
+00000010: 0a74 7970 653a 2044 6563 6c61 7261 7469  .type: Declarati
+00000020: 7665 536f 7572 6365 0a0a 6368 6563 6b3a  veSource..check:
+00000030: 0a20 2074 7970 653a 2043 6865 636b 5374  .  type: CheckSt
+00000040: 7265 616d 0a20 2073 7472 6561 6d5f 6e61  ream.  stream_na
+00000050: 6d65 733a 0a20 2020 202d 206f 7267 616e  mes:.    - organ
+00000060: 697a 6174 696f 6e73 0a0a 6465 6669 6e69  izations..defini
+00000070: 7469 6f6e 733a 0a20 2073 7472 6561 6d73  tions:.  streams
+00000080: 3a0a 2020 2020 6f72 6761 6e69 7a61 7469  :.    organizati
+00000090: 6f6e 733a 0a20 2020 2020 2074 7970 653a  ons:.      type:
+000000a0: 2044 6563 6c61 7261 7469 7665 5374 7265   DeclarativeStre
+000000b0: 616d 0a20 2020 2020 206e 616d 653a 206f  am.      name: o
+000000c0: 7267 616e 697a 6174 696f 6e73 0a20 2020  rganizations.   
+000000d0: 2020 2070 7269 6d61 7279 5f6b 6579 3a0a     primary_key:.
+000000e0: 2020 2020 2020 2020 2d20 6964 0a20 2020          - id.   
+000000f0: 2020 2072 6574 7269 6576 6572 3a0a 2020     retriever:.  
+00000100: 2020 2020 2020 7479 7065 3a20 5369 6d70        type: Simp
+00000110: 6c65 5265 7472 6965 7665 720a 2020 2020  leRetriever.    
+00000120: 2020 2020 7265 7175 6573 7465 723a 0a20      requester:. 
+00000130: 2020 2020 2020 2020 2024 7265 663a 2022           $ref: "
+00000140: 232f 6465 6669 6e69 7469 6f6e 732f 6261  #/definitions/ba
+00000150: 7365 5f72 6571 7565 7374 6572 220a 2020  se_requester".  
+00000160: 2020 2020 2020 2020 7061 7468 3a20 2f76          path: /v
+00000170: 332f 6f72 6761 6e69 7a61 7469 6f6e 730a  3/organizations.
+00000180: 2020 2020 2020 2020 2020 6874 7470 5f6d            http_m
+00000190: 6574 686f 643a 2047 4554 0a20 2020 2020  ethod: GET.     
+000001a0: 2020 2072 6563 6f72 645f 7365 6c65 6374     record_select
+000001b0: 6f72 3a0a 2020 2020 2020 2020 2020 7479  or:.          ty
+000001c0: 7065 3a20 5265 636f 7264 5365 6c65 6374  pe: RecordSelect
+000001d0: 6f72 0a20 2020 2020 2020 2020 2065 7874  or.          ext
+000001e0: 7261 6374 6f72 3a0a 2020 2020 2020 2020  ractor:.        
+000001f0: 2020 2020 7479 7065 3a20 4470 6174 6845      type: DpathE
+00000200: 7874 7261 6374 6f72 0a20 2020 2020 2020  xtractor.       
+00000210: 2020 2020 2066 6965 6c64 5f70 6174 683a       field_path:
+00000220: 0a20 2020 2020 2020 2020 2020 2020 202d  .              -
+00000230: 206f 7267 616e 697a 6174 696f 6e73 0a20   organizations. 
+00000240: 2020 2020 2073 6368 656d 615f 6c6f 6164       schema_load
+00000250: 6572 3a0a 2020 2020 2020 2020 7479 7065  er:.        type
+00000260: 3a20 496e 6c69 6e65 5363 6865 6d61 4c6f  : InlineSchemaLo
+00000270: 6164 6572 0a20 2020 2020 2020 2073 6368  ader.        sch
+00000280: 656d 613a 0a20 2020 2020 2020 2020 2024  ema:.          $
+00000290: 7265 663a 2022 232f 7363 6865 6d61 732f  ref: "#/schemas/
+000002a0: 6f72 6761 6e69 7a61 7469 6f6e 7322 0a20  organizations". 
+000002b0: 2020 2070 726f 6a65 6374 733a 0a20 2020     projects:.   
+000002c0: 2020 2074 7970 653a 2044 6563 6c61 7261     type: Declara
+000002d0: 7469 7665 5374 7265 616d 0a20 2020 2020  tiveStream.     
+000002e0: 206e 616d 653a 2070 726f 6a65 6374 730a   name: projects.
+000002f0: 2020 2020 2020 7265 7472 6965 7665 723a        retriever:
+00000300: 0a20 2020 2020 2020 2074 7970 653a 2053  .        type: S
+00000310: 696d 706c 6552 6574 7269 6576 6572 0a20  impleRetriever. 
+00000320: 2020 2020 2020 2072 6571 7565 7374 6572         requester
+00000330: 3a0a 2020 2020 2020 2020 2020 2472 6566  :.          $ref
+00000340: 3a20 2223 2f64 6566 696e 6974 696f 6e73  : "#/definitions
+00000350: 2f62 6173 655f 7265 7175 6573 7465 7222  /base_requester"
+00000360: 0a20 2020 2020 2020 2020 2070 6174 683a  .          path:
+00000370: 202f 7633 2f6f 7267 616e 697a 6174 696f   /v3/organizatio
+00000380: 6e73 2f7b 7b20 7374 7265 616d 5f73 6c69  ns/{{ stream_sli
+00000390: 6365 2e69 6420 7d7d 2f70 726f 6a65 6374  ce.id }}/project
+000003a0: 730a 2020 2020 2020 2020 2020 6874 7470  s.          http
+000003b0: 5f6d 6574 686f 643a 2047 4554 0a20 2020  _method: GET.   
+000003c0: 2020 2020 2072 6563 6f72 645f 7365 6c65       record_sele
+000003d0: 6374 6f72 3a0a 2020 2020 2020 2020 2020  ctor:.          
+000003e0: 7479 7065 3a20 5265 636f 7264 5365 6c65  type: RecordSele
+000003f0: 6374 6f72 0a20 2020 2020 2020 2020 2065  ctor.          e
+00000400: 7874 7261 6374 6f72 3a0a 2020 2020 2020  xtractor:.      
+00000410: 2020 2020 2020 7479 7065 3a20 4470 6174        type: Dpat
+00000420: 6845 7874 7261 6374 6f72 0a20 2020 2020  hExtractor.     
+00000430: 2020 2020 2020 2066 6965 6c64 5f70 6174         field_pat
+00000440: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
+00000450: 202d 2070 726f 6a65 6374 730a 2020 2020   - projects.    
+00000460: 2020 2020 7061 6769 6e61 746f 723a 0a20      paginator:. 
+00000470: 2020 2020 2020 2020 2074 7970 653a 2044           type: D
+00000480: 6566 6175 6c74 5061 6769 6e61 746f 720a  efaultPaginator.
+00000490: 2020 2020 2020 2020 2020 7061 6765 5f74            page_t
+000004a0: 6f6b 656e 5f6f 7074 696f 6e3a 0a20 2020  oken_option:.   
+000004b0: 2020 2020 2020 2020 2074 7970 653a 2052           type: R
+000004c0: 6571 7565 7374 4f70 7469 6f6e 0a20 2020  equestOption.   
+000004d0: 2020 2020 2020 2020 2069 6e6a 6563 745f           inject_
+000004e0: 696e 746f 3a20 7265 7175 6573 745f 7061  into: request_pa
+000004f0: 7261 6d65 7465 720a 2020 2020 2020 2020  rameter.        
+00000500: 2020 2020 6669 656c 645f 6e61 6d65 3a20      field_name: 
+00000510: 7061 6765 0a20 2020 2020 2020 2020 2070  page.          p
+00000520: 6167 655f 7369 7a65 5f6f 7074 696f 6e3a  age_size_option:
+00000530: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
+00000540: 653a 2052 6571 7565 7374 4f70 7469 6f6e  e: RequestOption
+00000550: 0a20 2020 2020 2020 2020 2020 2069 6e6a  .            inj
+00000560: 6563 745f 696e 746f 3a20 626f 6479 5f64  ect_into: body_d
+00000570: 6174 610a 2020 2020 2020 2020 2020 2020  ata.            
+00000580: 6669 656c 645f 6e61 6d65 3a20 7061 6765  field_name: page
+00000590: 5f73 697a 650a 2020 2020 2020 2020 2020  _size.          
+000005a0: 7061 6769 6e61 7469 6f6e 5f73 7472 6174  pagination_strat
+000005b0: 6567 793a 0a20 2020 2020 2020 2020 2020  egy:.           
+000005c0: 2074 7970 653a 2050 6167 6549 6e63 7265   type: PageIncre
+000005d0: 6d65 6e74 0a20 2020 2020 2020 2020 2020  ment.           
+000005e0: 2070 6167 655f 7369 7a65 3a20 3332 0a20   page_size: 32. 
+000005f0: 2020 2020 2020 2070 6172 7469 7469 6f6e         partition
+00000600: 5f72 6f75 7465 723a 0a20 2020 2020 2020  _router:.       
+00000610: 2020 202d 2074 7970 653a 2053 7562 7374     - type: Subst
+00000620: 7265 616d 5061 7274 6974 696f 6e52 6f75  reamPartitionRou
+00000630: 7465 720a 2020 2020 2020 2020 2020 2020  ter.            
+00000640: 7061 7265 6e74 5f73 7472 6561 6d5f 636f  parent_stream_co
+00000650: 6e66 6967 733a 0a20 2020 2020 2020 2020  nfigs:.         
+00000660: 2020 2020 202d 2074 7970 653a 2050 6172       - type: Par
+00000670: 656e 7453 7472 6561 6d43 6f6e 6669 670a  entStreamConfig.
+00000680: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000690: 7061 7265 6e74 5f6b 6579 3a20 6964 0a20  parent_key: id. 
+000006a0: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+000006b0: 6172 7469 7469 6f6e 5f66 6965 6c64 3a20  artition_field: 
+000006c0: 6964 0a20 2020 2020 2020 2020 2020 2020  id.             
+000006d0: 2020 2073 7472 6561 6d3a 0a20 2020 2020     stream:.     
+000006e0: 2020 2020 2020 2020 2020 2020 2024 7265               $re
+000006f0: 663a 2022 232f 6465 6669 6e69 7469 6f6e  f: "#/definition
+00000700: 732f 7374 7265 616d 732f 6f72 6761 6e69  s/streams/organi
+00000710: 7a61 7469 6f6e 7322 0a20 2020 2020 2073  zations".      s
+00000720: 6368 656d 615f 6c6f 6164 6572 3a0a 2020  chema_loader:.  
+00000730: 2020 2020 2020 7479 7065 3a20 496e 6c69        type: Inli
+00000740: 6e65 5363 6865 6d61 4c6f 6164 6572 0a20  neSchemaLoader. 
+00000750: 2020 2020 2020 2073 6368 656d 613a 0a20         schema:. 
+00000760: 2020 2020 2020 2020 2024 7265 663a 2022           $ref: "
+00000770: 232f 7363 6865 6d61 732f 7072 6f6a 6563  #/schemas/projec
+00000780: 7473 220a 2020 2020 6b36 2d74 6573 7473  ts".    k6-tests
+00000790: 3a0a 2020 2020 2020 7479 7065 3a20 4465  :.      type: De
+000007a0: 636c 6172 6174 6976 6553 7472 6561 6d0a  clarativeStream.
+000007b0: 2020 2020 2020 6e61 6d65 3a20 6b36 2d74        name: k6-t
+000007c0: 6573 7473 0a20 2020 2020 2070 7269 6d61  ests.      prima
+000007d0: 7279 5f6b 6579 3a0a 2020 2020 2020 2020  ry_key:.        
+000007e0: 2d20 6964 0a20 2020 2020 2072 6574 7269  - id.      retri
+000007f0: 6576 6572 3a0a 2020 2020 2020 2020 7479  ever:.        ty
+00000800: 7065 3a20 5369 6d70 6c65 5265 7472 6965  pe: SimpleRetrie
+00000810: 7665 720a 2020 2020 2020 2020 7265 7175  ver.        requ
+00000820: 6573 7465 723a 0a20 2020 2020 2020 2020  ester:.         
+00000830: 2024 7265 663a 2022 232f 6465 6669 6e69   $ref: "#/defini
+00000840: 7469 6f6e 732f 6261 7365 5f72 6571 7565  tions/base_reque
+00000850: 7374 6572 220a 2020 2020 2020 2020 2020  ster".          
+00000860: 7061 7468 3a20 6c6f 6164 7465 7374 732f  path: loadtests/
+00000870: 7632 2f74 6573 7473 0a20 2020 2020 2020  v2/tests.       
+00000880: 2020 2068 7474 705f 6d65 7468 6f64 3a20     http_method: 
+00000890: 4745 540a 2020 2020 2020 2020 7265 636f  GET.        reco
+000008a0: 7264 5f73 656c 6563 746f 723a 0a20 2020  rd_selector:.   
+000008b0: 2020 2020 2020 2074 7970 653a 2052 6563         type: Rec
+000008c0: 6f72 6453 656c 6563 746f 720a 2020 2020  ordSelector.    
+000008d0: 2020 2020 2020 6578 7472 6163 746f 723a        extractor:
+000008e0: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
+000008f0: 653a 2044 7061 7468 4578 7472 6163 746f  e: DpathExtracto
+00000900: 720a 2020 2020 2020 2020 2020 2020 6669  r.            fi
+00000910: 656c 645f 7061 7468 3a0a 2020 2020 2020  eld_path:.      
+00000920: 2020 2020 2020 2020 2d20 6b36 2d74 6573          - k6-tes
+00000930: 7473 0a20 2020 2020 2020 2070 6167 696e  ts.        pagin
+00000940: 6174 6f72 3a0a 2020 2020 2020 2020 2020  ator:.          
+00000950: 7479 7065 3a20 4465 6661 756c 7450 6167  type: DefaultPag
+00000960: 696e 6174 6f72 0a20 2020 2020 2020 2020  inator.         
+00000970: 2070 6167 655f 746f 6b65 6e5f 6f70 7469   page_token_opti
+00000980: 6f6e 3a0a 2020 2020 2020 2020 2020 2020  on:.            
+00000990: 7479 7065 3a20 5265 7175 6573 744f 7074  type: RequestOpt
+000009a0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
+000009b0: 696e 6a65 6374 5f69 6e74 6f3a 2072 6571  inject_into: req
+000009c0: 7565 7374 5f70 6172 616d 6574 6572 0a20  uest_parameter. 
+000009d0: 2020 2020 2020 2020 2020 2066 6965 6c64             field
+000009e0: 5f6e 616d 653a 2070 6167 650a 2020 2020  _name: page.    
+000009f0: 2020 2020 2020 7061 6765 5f73 697a 655f        page_size_
+00000a00: 6f70 7469 6f6e 3a0a 2020 2020 2020 2020  option:.        
+00000a10: 2020 2020 7479 7065 3a20 5265 7175 6573      type: Reques
+00000a20: 744f 7074 696f 6e0a 2020 2020 2020 2020  tOption.        
+00000a30: 2020 2020 696e 6a65 6374 5f69 6e74 6f3a      inject_into:
+00000a40: 2062 6f64 795f 6461 7461 0a20 2020 2020   body_data.     
+00000a50: 2020 2020 2020 2066 6965 6c64 5f6e 616d         field_nam
+00000a60: 653a 2070 6167 655f 7369 7a65 0a20 2020  e: page_size.   
+00000a70: 2020 2020 2020 2070 6167 696e 6174 696f         paginatio
+00000a80: 6e5f 7374 7261 7465 6779 3a0a 2020 2020  n_strategy:.    
+00000a90: 2020 2020 2020 2020 7479 7065 3a20 5061          type: Pa
+00000aa0: 6765 496e 6372 656d 656e 740a 2020 2020  geIncrement.    
+00000ab0: 2020 2020 2020 2020 7061 6765 5f73 697a          page_siz
+00000ac0: 653a 2033 320a 2020 2020 2020 7363 6865  e: 32.      sche
+00000ad0: 6d61 5f6c 6f61 6465 723a 0a20 2020 2020  ma_loader:.     
+00000ae0: 2020 2074 7970 653a 2049 6e6c 696e 6553     type: InlineS
+00000af0: 6368 656d 614c 6f61 6465 720a 2020 2020  chemaLoader.    
+00000b00: 2020 2020 7363 6865 6d61 3a0a 2020 2020      schema:.    
+00000b10: 2020 2020 2020 2472 6566 3a20 2223 2f73        $ref: "#/s
+00000b20: 6368 656d 6173 2f6b 362d 7465 7374 7322  chemas/k6-tests"
+00000b30: 0a20 2062 6173 655f 7265 7175 6573 7465  .  base_requeste
+00000b40: 723a 0a20 2020 2074 7970 653a 2048 7474  r:.    type: Htt
+00000b50: 7052 6571 7565 7374 6572 0a20 2020 2075  pRequester.    u
+00000b60: 726c 5f62 6173 653a 2068 7474 7073 3a2f  rl_base: https:/
+00000b70: 2f61 7069 2e6b 362e 696f 0a20 2020 2061  /api.k6.io.    a
+00000b80: 7574 6865 6e74 6963 6174 6f72 3a0a 2020  uthenticator:.  
+00000b90: 2020 2020 7479 7065 3a20 4265 6172 6572      type: Bearer
+00000ba0: 4175 7468 656e 7469 6361 746f 720a 2020  Authenticator.  
+00000bb0: 2020 2020 6170 695f 746f 6b65 6e3a 2022      api_token: "
+00000bc0: 7b7b 2063 6f6e 6669 675b 2761 7069 5f74  {{ config['api_t
+00000bd0: 6f6b 656e 275d 207d 7d22 0a0a 7374 7265  oken'] }}"..stre
+00000be0: 616d 733a 0a20 202d 2024 7265 663a 2022  ams:.  - $ref: "
+00000bf0: 232f 6465 6669 6e69 7469 6f6e 732f 7374  #/definitions/st
+00000c00: 7265 616d 732f 6f72 6761 6e69 7a61 7469  reams/organizati
+00000c10: 6f6e 7322 0a20 202d 2024 7265 663a 2022  ons".  - $ref: "
+00000c20: 232f 6465 6669 6e69 7469 6f6e 732f 7374  #/definitions/st
+00000c30: 7265 616d 732f 7072 6f6a 6563 7473 220a  reams/projects".
+00000c40: 2020 2d20 2472 6566 3a20 2223 2f64 6566    - $ref: "#/def
+00000c50: 696e 6974 696f 6e73 2f73 7472 6561 6d73  initions/streams
+00000c60: 2f6b 362d 7465 7374 7322 0a0a 7370 6563  /k6-tests"..spec
+00000c70: 3a0a 2020 7479 7065 3a20 5370 6563 0a20  :.  type: Spec. 
+00000c80: 2063 6f6e 6e65 6374 696f 6e5f 7370 6563   connection_spec
+00000c90: 6966 6963 6174 696f 6e3a 0a20 2020 2074  ification:.    t
+00000ca0: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
+00000cb0: 2473 6368 656d 613a 2068 7474 703a 2f2f  $schema: http://
+00000cc0: 6a73 6f6e 2d73 6368 656d 612e 6f72 672f  json-schema.org/
+00000cd0: 6472 6166 742d 3037 2f73 6368 656d 6123  draft-07/schema#
+00000ce0: 0a20 2020 2072 6571 7569 7265 643a 0a20  .    required:. 
+00000cf0: 2020 2020 202d 2061 7069 5f74 6f6b 656e       - api_token
+00000d00: 0a20 2020 2070 726f 7065 7274 6965 733a  .    properties:
+00000d10: 0a20 2020 2020 2061 7069 5f74 6f6b 656e  .      api_token
+00000d20: 3a0a 2020 2020 2020 2020 7479 7065 3a20  :.        type: 
+00000d30: 7374 7269 6e67 0a20 2020 2020 2020 2074  string.        t
+00000d40: 6974 6c65 3a20 4170 6920 546f 6b65 6e0a  itle: Api Token.
+00000d50: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00000d60: 696f 6e3a 203e 2d0a 2020 2020 2020 2020  ion: >-.        
+00000d70: 2020 596f 7572 2041 5049 2054 6f6b 656e    Your API Token
+00000d80: 2e20 5365 6520 3c61 0a20 2020 2020 2020  . See <a.       
+00000d90: 2020 2068 7265 663d 2268 7474 7073 3a2f     href="https:/
+00000da0: 2f6b 362e 696f 2f64 6f63 732f 636c 6f75  /k6.io/docs/clou
+00000db0: 642f 696e 7465 6772 6174 696f 6e73 2f74  d/integrations/t
+00000dc0: 6f6b 656e 2f22 3e68 6572 653c 2f61 3e2e  oken/">here</a>.
+00000dd0: 2054 6865 206b 6579 0a20 2020 2020 2020   The key.       
+00000de0: 2020 2069 7320 6361 7365 2073 656e 7369     is case sensi
+00000df0: 7469 7665 2e0a 2020 2020 2020 2020 6169  tive..        ai
+00000e00: 7262 7974 655f 7365 6372 6574 3a20 7472  rbyte_secret: tr
+00000e10: 7565 0a20 2020 2020 2020 206f 7264 6572  ue.        order
+00000e20: 3a20 300a 2020 2020 6164 6469 7469 6f6e  : 0.    addition
+00000e30: 616c 5072 6f70 6572 7469 6573 3a20 7472  alProperties: tr
+00000e40: 7565 0a0a 6d65 7461 6461 7461 3a0a 2020  ue..metadata:.  
+00000e50: 6175 746f 496d 706f 7274 5363 6865 6d61  autoImportSchema
+00000e60: 3a0a 2020 2020 6f72 6761 6e69 7a61 7469  :.    organizati
+00000e70: 6f6e 733a 2066 616c 7365 0a20 2020 2070  ons: false.    p
+00000e80: 726f 6a65 6374 733a 2066 616c 7365 0a20  rojects: false. 
+00000e90: 2020 206b 362d 7465 7374 733a 2066 616c     k6-tests: fal
+00000ea0: 7365 0a0a 7363 6865 6d61 733a 0a20 206f  se..schemas:.  o
+00000eb0: 7267 616e 697a 6174 696f 6e73 3a0a 2020  rganizations:.  
+00000ec0: 2020 7479 7065 3a20 6f62 6a65 6374 0a20    type: object. 
+00000ed0: 2020 2024 7363 6865 6d61 3a20 6874 7470     $schema: http
+00000ee0: 3a2f 2f6a 736f 6e2d 7363 6865 6d61 2e6f  ://json-schema.o
+00000ef0: 7267 2f64 7261 6674 2d30 372f 7363 6865  rg/draft-07/sche
+00000f00: 6d61 230a 2020 2020 7072 6f70 6572 7469  ma#.    properti
+00000f10: 6573 3a0a 2020 2020 2020 6269 6c6c 696e  es:.      billin
+00000f20: 675f 6164 6472 6573 733a 0a20 2020 2020  g_address:.     
+00000f30: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
+00000f40: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00000f50: 696f 6e3a 2054 6865 2062 696c 6c69 6e67  ion: The billing
+00000f60: 2061 6464 7265 7373 206f 6620 7468 6520   address of the 
+00000f70: 6f72 6761 6e69 7a61 7469 6f6e 2e0a 2020  organization..  
+00000f80: 2020 2020 6269 6c6c 696e 675f 636f 756e      billing_coun
+00000f90: 7472 793a 0a20 2020 2020 2020 2074 7970  try:.        typ
+00000fa0: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
+00000fb0: 2020 6465 7363 7269 7074 696f 6e3a 2054    description: T
+00000fc0: 6865 2063 6f75 6e74 7279 2061 7373 6f63  he country assoc
+00000fd0: 6961 7465 6420 7769 7468 2074 6865 2062  iated with the b
+00000fe0: 696c 6c69 6e67 2061 6464 7265 7373 206f  illing address o
+00000ff0: 6620 7468 6520 6f72 6761 6e69 7a61 7469  f the organizati
+00001000: 6f6e 2e0a 2020 2020 2020 6269 6c6c 696e  on..      billin
+00001010: 675f 656d 6169 6c3a 0a20 2020 2020 2020  g_email:.       
+00001020: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
+00001030: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00001040: 6e3a 2054 6865 2062 696c 6c69 6e67 2065  n: The billing e
+00001050: 6d61 696c 2061 6464 7265 7373 2066 6f72  mail address for
+00001060: 2074 6865 206f 7267 616e 697a 6174 696f   the organizatio
+00001070: 6e2e 0a20 2020 2020 2063 7265 6174 6564  n..      created
+00001080: 3a0a 2020 2020 2020 2020 7479 7065 3a20  :.        type: 
+00001090: 7374 7269 6e67 0a20 2020 2020 2020 2064  string.        d
+000010a0: 6573 6372 6970 7469 6f6e 3a20 5468 6520  escription: The 
+000010b0: 7469 6d65 7374 616d 7020 7768 656e 2074  timestamp when t
+000010c0: 6865 206f 7267 616e 697a 6174 696f 6e20  he organization 
+000010d0: 7761 7320 6372 6561 7465 642e 0a20 2020  was created..   
+000010e0: 2020 2064 6573 6372 6970 7469 6f6e 3a0a     description:.
+000010f0: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
+00001100: 7269 6e67 0a20 2020 2020 2020 2064 6573  ring.        des
+00001110: 6372 6970 7469 6f6e 3a20 4120 7465 7874  cription: A text
+00001120: 7561 6c20 6465 7363 7269 7074 696f 6e20  ual description 
+00001130: 6f72 2064 6574 6169 6c73 2061 626f 7574  or details about
+00001140: 2074 6865 206f 7267 616e 697a 6174 696f   the organizatio
+00001150: 6e2e 0a20 2020 2020 2069 643a 0a20 2020  n..      id:.   
+00001160: 2020 2020 2074 7970 653a 2069 6e74 6567       type: integ
+00001170: 6572 0a20 2020 2020 2020 2064 6573 6372  er.        descr
+00001180: 6970 7469 6f6e 3a20 5468 6520 756e 6971  iption: The uniq
+00001190: 7565 2069 6465 6e74 6966 6965 7220 666f  ue identifier fo
+000011a0: 7220 7468 6520 6f72 6761 6e69 7a61 7469  r the organizati
+000011b0: 6f6e 2e0a 2020 2020 2020 6973 5f64 6566  on..      is_def
+000011c0: 6175 6c74 3a0a 2020 2020 2020 2020 7479  ault:.        ty
+000011d0: 7065 3a20 626f 6f6c 6561 6e0a 2020 2020  pe: boolean.    
+000011e0: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+000011f0: 2049 6e64 6963 6174 6573 2069 6620 7468   Indicates if th
+00001200: 6520 6f72 6761 6e69 7a61 7469 6f6e 2069  e organization i
+00001210: 7320 7365 7420 6173 2074 6865 2064 6566  s set as the def
+00001220: 6175 6c74 206f 7267 616e 697a 6174 696f  ault organizatio
+00001230: 6e2e 0a20 2020 2020 2069 735f 7361 6d6c  n..      is_saml
+00001240: 5f6f 7267 3a0a 2020 2020 2020 2020 7479  _org:.        ty
+00001250: 7065 3a20 626f 6f6c 6561 6e0a 2020 2020  pe: boolean.    
+00001260: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00001270: 2046 6c61 6720 7368 6f77 696e 6720 6966   Flag showing if
+00001280: 2074 6865 206f 7267 616e 697a 6174 696f   the organizatio
+00001290: 6e20 7573 6573 2053 414d 4c20 666f 7220  n uses SAML for 
+000012a0: 6175 7468 656e 7469 6361 7469 6f6e 2e0a  authentication..
+000012b0: 2020 2020 2020 6e61 6d65 3a0a 2020 2020        name:.    
+000012c0: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+000012d0: 0a20 2020 2020 2020 2064 6573 6372 6970  .        descrip
+000012e0: 7469 6f6e 3a20 5468 6520 6e61 6d65 206f  tion: The name o
+000012f0: 6620 7468 6520 6f72 6761 6e69 7a61 7469  f the organizati
+00001300: 6f6e 2e0a 2020 2020 2020 6f77 6e65 725f  on..      owner_
+00001310: 6964 3a0a 2020 2020 2020 2020 7479 7065  id:.        type
+00001320: 3a20 696e 7465 6765 720a 2020 2020 2020  : integer.      
+00001330: 2020 6465 7363 7269 7074 696f 6e3a 2054    description: T
+00001340: 6865 2075 7365 7220 4944 206f 6620 7468  he user ID of th
+00001350: 6520 6f77 6e65 7220 6f72 2063 7265 6174  e owner or creat
+00001360: 6f72 206f 6620 7468 6520 6f72 6761 6e69  or of the organi
+00001370: 7a61 7469 6f6e 2e0a 2020 2020 2020 7570  zation..      up
+00001380: 6461 7465 643a 0a20 2020 2020 2020 2074  dated:.        t
+00001390: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
+000013a0: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+000013b0: 2054 6865 2074 696d 6573 7461 6d70 2077   The timestamp w
+000013c0: 6865 6e20 7468 6520 6f72 6761 6e69 7a61  hen the organiza
+000013d0: 7469 6f6e 2064 6174 6120 7761 7320 6c61  tion data was la
+000013e0: 7374 2075 7064 6174 6564 2e0a 2020 2020  st updated..    
+000013f0: 2020 7661 745f 6e75 6d62 6572 3a0a 2020    vat_number:.  
+00001400: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+00001410: 6e67 0a20 2020 2020 2020 2064 6573 6372  ng.        descr
+00001420: 6970 7469 6f6e 3a20 5661 6c75 652d 6164  iption: Value-ad
+00001430: 6465 6420 7461 7820 2856 4154 2920 6e75  ded tax (VAT) nu
+00001440: 6d62 6572 2066 6f72 2074 6865 206f 7267  mber for the org
+00001450: 616e 697a 6174 696f 6e2e 0a20 2020 2061  anization..    a
+00001460: 6464 6974 696f 6e61 6c50 726f 7065 7274  dditionalPropert
+00001470: 6965 733a 2074 7275 650a 2020 7072 6f6a  ies: true.  proj
+00001480: 6563 7473 3a0a 2020 2020 7479 7065 3a20  ects:.    type: 
+00001490: 6f62 6a65 6374 0a20 2020 2024 7363 6865  object.    $sche
+000014a0: 6d61 3a20 6874 7470 3a2f 2f6a 736f 6e2d  ma: http://json-
+000014b0: 7363 6865 6d61 2e6f 7267 2f64 7261 6674  schema.org/draft
+000014c0: 2d30 372f 7363 6865 6d61 230a 2020 2020  -07/schema#.    
+000014d0: 7072 6f70 6572 7469 6573 3a0a 2020 2020  properties:.    
+000014e0: 2020 6372 6561 7465 643a 0a20 2020 2020    created:.     
+000014f0: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
+00001500: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00001510: 696f 6e3a 2054 6865 2074 696d 6573 7461  ion: The timesta
+00001520: 6d70 2077 6865 6e20 7468 6520 7072 6f6a  mp when the proj
+00001530: 6563 7420 7761 7320 6372 6561 7465 640a  ect was created.
+00001540: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00001550: 6e3a 0a20 2020 2020 2020 2074 7970 653a  n:.        type:
+00001560: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00001570: 6465 7363 7269 7074 696f 6e3a 2041 2073  description: A s
+00001580: 686f 7274 2064 6573 6372 6970 7469 6f6e  hort description
+00001590: 206f 6620 7468 6520 7072 6f6a 6563 740a   of the project.
+000015a0: 2020 2020 2020 6964 3a0a 2020 2020 2020        id:.      
+000015b0: 2020 7479 7065 3a20 696e 7465 6765 720a    type: integer.
+000015c0: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+000015d0: 696f 6e3a 2054 6865 2075 6e69 7175 6520  ion: The unique 
+000015e0: 6964 656e 7469 6669 6572 2066 6f72 2074  identifier for t
+000015f0: 6865 2070 726f 6a65 6374 0a20 2020 2020  he project.     
+00001600: 2069 735f 6465 6661 756c 743a 0a20 2020   is_default:.   
+00001610: 2020 2020 2074 7970 653a 2062 6f6f 6c65       type: boole
+00001620: 616e 0a20 2020 2020 2020 2064 6573 6372  an.        descr
+00001630: 6970 7469 6f6e 3a20 4120 666c 6167 2069  iption: A flag i
+00001640: 6e64 6963 6174 696e 6720 6966 2074 6865  ndicating if the
+00001650: 2070 726f 6a65 6374 2069 7320 7468 6520   project is the 
+00001660: 6465 6661 756c 7420 6f6e 650a 2020 2020  default one.    
+00001670: 2020 6e61 6d65 3a0a 2020 2020 2020 2020    name:.        
+00001680: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
+00001690: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+000016a0: 3a20 5468 6520 6e61 6d65 206f 6620 7468  : The name of th
+000016b0: 6520 7072 6f6a 6563 740a 2020 2020 2020  e project.      
+000016c0: 6f72 6761 6e69 7a61 7469 6f6e 5f69 643a  organization_id:
+000016d0: 0a20 2020 2020 2020 2074 7970 653a 2069  .        type: i
+000016e0: 6e74 6567 6572 0a20 2020 2020 2020 2064  nteger.        d
+000016f0: 6573 6372 6970 7469 6f6e 3a20 5468 6520  escription: The 
+00001700: 756e 6971 7565 2069 6465 6e74 6966 6965  unique identifie
+00001710: 7220 6f66 2074 6865 206f 7267 616e 697a  r of the organiz
+00001720: 6174 696f 6e20 7468 6520 7072 6f6a 6563  ation the projec
+00001730: 7420 6265 6c6f 6e67 7320 746f 0a20 2020  t belongs to.   
+00001740: 2020 2075 7064 6174 6564 3a0a 2020 2020     updated:.    
+00001750: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+00001760: 0a20 2020 2020 2020 2064 6573 6372 6970  .        descrip
+00001770: 7469 6f6e 3a20 5468 6520 7469 6d65 7374  tion: The timest
+00001780: 616d 7020 7768 656e 2074 6865 2070 726f  amp when the pro
+00001790: 6a65 6374 2077 6173 206c 6173 7420 7570  ject was last up
+000017a0: 6461 7465 640a 2020 2020 6164 6469 7469  dated.    additi
+000017b0: 6f6e 616c 5072 6f70 6572 7469 6573 3a20  onalProperties: 
+000017c0: 7472 7565 0a20 206b 362d 7465 7374 733a  true.  k6-tests:
+000017d0: 0a20 2020 2074 7970 653a 206f 626a 6563  .    type: objec
+000017e0: 740a 2020 2020 2473 6368 656d 613a 2068  t.    $schema: h
+000017f0: 7474 703a 2f2f 6a73 6f6e 2d73 6368 656d  ttp://json-schem
+00001800: 612e 6f72 672f 6472 6166 742d 3037 2f73  a.org/draft-07/s
+00001810: 6368 656d 6123 0a20 2020 2070 726f 7065  chema#.    prope
+00001820: 7274 6965 733a 0a20 2020 2020 2063 7265  rties:.      cre
+00001830: 6174 6564 3a0a 2020 2020 2020 2020 7479  ated:.        ty
+00001840: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
+00001850: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
+00001860: 4461 7465 2061 6e64 2074 696d 6520 7768  Date and time wh
+00001870: 656e 2074 6865 206b 3620 7465 7374 2077  en the k6 test w
+00001880: 6173 2063 7265 6174 6564 2e0a 2020 2020  as created..    
+00001890: 2020 6964 3a0a 2020 2020 2020 2020 7479    id:.        ty
+000018a0: 7065 3a20 696e 7465 6765 720a 2020 2020  pe: integer.    
+000018b0: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+000018c0: 2055 6e69 7175 6520 6964 656e 7469 6669   Unique identifi
+000018d0: 6572 2066 6f72 2074 6865 206b 3620 7465  er for the k6 te
+000018e0: 7374 2e0a 2020 2020 2020 6c61 7374 5f74  st..      last_t
+000018f0: 6573 745f 7275 6e5f 6964 3a0a 2020 2020  est_run_id:.    
+00001900: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+00001910: 0a20 2020 2020 2020 2064 6573 6372 6970  .        descrip
+00001920: 7469 6f6e 3a20 4964 656e 7469 6669 6572  tion: Identifier
+00001930: 2066 6f72 2074 6865 206c 6173 7420 7465   for the last te
+00001940: 7374 2072 756e 2061 7373 6f63 6961 7465  st run associate
+00001950: 6420 7769 7468 2074 6869 7320 6b36 2074  d with this k6 t
+00001960: 6573 742e 0a20 2020 2020 206e 616d 653a  est..      name:
+00001970: 0a20 2020 2020 2020 2074 7970 653a 2073  .        type: s
+00001980: 7472 696e 670a 2020 2020 2020 2020 6465  tring.        de
+00001990: 7363 7269 7074 696f 6e3a 204e 616d 6520  scription: Name 
+000019a0: 6f66 2074 6865 206b 3620 7465 7374 2e0a  of the k6 test..
+000019b0: 2020 2020 2020 7072 6f6a 6563 745f 6964        project_id
+000019c0: 3a0a 2020 2020 2020 2020 7479 7065 3a20  :.        type: 
+000019d0: 696e 7465 6765 720a 2020 2020 2020 2020  integer.        
+000019e0: 6465 7363 7269 7074 696f 6e3a 2049 6465  description: Ide
+000019f0: 6e74 6966 6965 7220 666f 7220 7468 6520  ntifier for the 
+00001a00: 7072 6f6a 6563 7420 746f 2077 6869 6368  project to which
+00001a10: 2074 6869 7320 6b36 2074 6573 7420 6265   this k6 test be
+00001a20: 6c6f 6e67 732e 0a20 2020 2020 2073 6372  longs..      scr
+00001a30: 6970 743a 0a20 2020 2020 2020 2074 7970  ipt:.        typ
+00001a40: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
+00001a50: 2020 6465 7363 7269 7074 696f 6e3a 2054    description: T
+00001a60: 6865 2073 6372 6970 7420 636f 6e74 656e  he script conten
+00001a70: 7420 6f66 2074 6865 206b 3620 7465 7374  t of the k6 test
+00001a80: 2e0a 2020 2020 2020 7465 7374 5f72 756e  ..      test_run
+00001a90: 5f69 6473 3a0a 2020 2020 2020 2020 7479  _ids:.        ty
+00001aa0: 7065 3a20 6172 7261 790a 2020 2020 2020  pe: array.      
+00001ab0: 2020 6465 7363 7269 7074 696f 6e3a 204c    description: L
+00001ac0: 6973 7420 6f66 2069 6465 6e74 6966 6965  ist of identifie
+00001ad0: 7273 2066 6f72 2061 6c6c 2074 6573 7420  rs for all test 
+00001ae0: 7275 6e73 2061 7373 6f63 6961 7465 6420  runs associated 
+00001af0: 7769 7468 2074 6869 7320 6b36 2074 6573  with this k6 tes
+00001b00: 742e 0a20 2020 2020 2075 7064 6174 6564  t..      updated
+00001b10: 3a0a 2020 2020 2020 2020 7479 7065 3a20  :.        type: 
+00001b20: 7374 7269 6e67 0a20 2020 2020 2020 2064  string.        d
+00001b30: 6573 6372 6970 7469 6f6e 3a20 4461 7465  escription: Date
+00001b40: 2061 6e64 2074 696d 6520 7768 656e 2074   and time when t
+00001b50: 6865 206b 3620 7465 7374 2077 6173 206c  he k6 test was l
+00001b60: 6173 7420 7570 6461 7465 642e 0a20 2020  ast updated..   
+00001b70: 2020 2075 7365 725f 6964 3a0a 2020 2020     user_id:.    
+00001b80: 2020 2020 7479 7065 3a20 696e 7465 6765      type: intege
+00001b90: 720a 2020 2020 2020 2020 6465 7363 7269  r.        descri
+00001ba0: 7074 696f 6e3a 2049 6465 6e74 6966 6965  ption: Identifie
+00001bb0: 7220 6f66 2074 6865 2075 7365 7220 7768  r of the user wh
+00001bc0: 6f20 6f77 6e73 2074 6869 7320 6b36 2074  o owns this k6 t
+00001bd0: 6573 742e 0a20 2020 2061 6464 6974 696f  est..    additio
+00001be0: 6e61 6c50 726f 7065 7274 6965 733a 2074  nalProperties: t
+00001bf0: 7275 650a                                rue.
```

### Comparing `airbyte_source_k6_cloud-0.1.3/PKG-INFO` & `airbyte_source_k6_cloud-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-k6-cloud
-Version: 0.1.3
+Version: 0.1.4
 Summary: Source implementation for K6 Cloud.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/k6-cloud
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # K6-Cloud source connector
 
-
 This is the repository for the K6-Cloud source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/k6-cloud).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/k6-cloud)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_k6_cloud/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-k6-cloud spec
 poetry run source-k6-cloud check --config secrets/config.json
 poetry run source-k6-cloud discover --config secrets/config.json
 poetry run source-k6-cloud read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-k6-cloud build
 ```
 
 An image will be available on your host with the tag `airbyte/source-k6-cloud:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-k6-cloud:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-k6-cloud:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-k6-cloud:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-k6-cloud:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-k6-cloud test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-k6-cloud test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/k6-cloud.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

