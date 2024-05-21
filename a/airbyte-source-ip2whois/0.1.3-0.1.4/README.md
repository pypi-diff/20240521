# Comparing `tmp/airbyte_source_ip2whois-0.1.3.tar.gz` & `tmp/airbyte_source_ip2whois-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_ip2whois-0.1.3.tar", max compression
+gzip compressed data, was "airbyte_source_ip2whois-0.1.4.tar", max compression
```

## Comparing `airbyte_source_ip2whois-0.1.3.tar` & `airbyte_source_ip2whois-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     4532 2024-05-01 18:49:11.737083 airbyte_source_ip2whois-0.1.3/README.md
--rw-r--r--   0        0        0      755 2024-05-01 18:54:00.061348 airbyte_source_ip2whois-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      128 2024-05-01 18:49:11.737083 airbyte_source_ip2whois-0.1.3/source_ip2whois/__init__.py
--rw-r--r--   0        0        0     9224 2024-05-01 18:49:11.737083 airbyte_source_ip2whois-0.1.3/source_ip2whois/manifest.yaml
--rw-r--r--   0        0        0      236 2024-05-01 18:49:11.737083 airbyte_source_ip2whois-0.1.3/source_ip2whois/run.py
--rw-r--r--   0        0        0      477 2024-05-01 18:49:11.737083 airbyte_source_ip2whois-0.1.3/source_ip2whois/source.py
--rw-r--r--   0        0        0      660 2024-05-01 18:49:11.737083 airbyte_source_ip2whois-0.1.3/source_ip2whois/spec.yaml
--rw-r--r--   0        0        0     5242 1970-01-01 00:00:00.000000 airbyte_source_ip2whois-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     4542 2024-05-21 00:49:18.000000 airbyte_source_ip2whois-0.1.4/README.md
+-rw-r--r--   0        0        0      755 2024-05-21 01:15:49.207786 airbyte_source_ip2whois-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      128 2024-05-21 00:49:18.000000 airbyte_source_ip2whois-0.1.4/source_ip2whois/__init__.py
+-rw-r--r--   0        0        0     9062 2024-05-21 00:49:18.000000 airbyte_source_ip2whois-0.1.4/source_ip2whois/manifest.yaml
+-rw-r--r--   0        0        0      236 2024-05-21 00:49:18.000000 airbyte_source_ip2whois-0.1.4/source_ip2whois/run.py
+-rw-r--r--   0        0        0      477 2024-05-21 00:49:18.000000 airbyte_source_ip2whois-0.1.4/source_ip2whois/source.py
+-rw-r--r--   0        0        0     5252 1970-01-01 00:00:00.000000 airbyte_source_ip2whois-0.1.4/PKG-INFO
```

### Comparing `airbyte_source_ip2whois-0.1.3/README.md` & `airbyte_source_ip2whois-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,91 +1,104 @@
 # Ip2Whois source connector
 
-
 This is the repository for the Ip2Whois source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/ip2whois).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/ip2whois)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_ip2whois/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-ip2whois spec
 poetry run source-ip2whois check --config secrets/config.json
 poetry run source-ip2whois discover --config secrets/config.json
 poetry run source-ip2whois read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-ip2whois build
 ```
 
 An image will be available on your host with the tag `airbyte/source-ip2whois:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-ip2whois:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-ip2whois:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-ip2whois:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-ip2whois:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-ip2whois test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-ip2whois test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/ip2whois.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
-8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
```

### Comparing `airbyte_source_ip2whois-0.1.3/pyproject.toml` & `airbyte_source_ip2whois-0.1.4/pyproject.toml`

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
 name = "airbyte-source-ip2whois"
 description = "Source implementation for Ip2whois."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_ip2whois-0.1.3/source_ip2whois/manifest.yaml` & `airbyte_source_ip2whois-0.1.4/source_ip2whois/manifest.yaml`

 * *Files 17% similar despite different names*

```diff
@@ -1,577 +1,567 @@
-00000000: 7665 7273 696f 6e3a 2022 302e 3239 2e30  version: "0.29.0
-00000010: 220a 0a64 6566 696e 6974 696f 6e73 3a0a  "..definitions:.
-00000020: 2020 7365 6c65 6374 6f72 3a0a 2020 2020    selector:.    
-00000030: 6578 7472 6163 746f 723a 0a20 2020 2020  extractor:.     
-00000040: 2066 6965 6c64 5f70 6174 683a 205b 5d0a   field_path: [].
-00000050: 2020 7265 7175 6573 7465 723a 0a20 2020    requester:.   
-00000060: 2075 726c 5f62 6173 653a 2022 6874 7470   url_base: "http
-00000070: 733a 2f2f 6170 692e 6970 3277 686f 6973  s://api.ip2whois
-00000080: 2e63 6f6d 220a 2020 2020 6874 7470 5f6d  .com".    http_m
-00000090: 6574 686f 643a 2022 4745 5422 0a20 2020  ethod: "GET".   
-000000a0: 2072 6571 7565 7374 5f70 6172 616d 6574   request_paramet
-000000b0: 6572 733a 0a20 2020 2020 206b 6579 3a20  ers:.      key: 
-000000c0: 227b 7b20 636f 6e66 6967 5b27 6170 695f  "{{ config['api_
-000000d0: 6b65 7927 5d20 7d7d 220a 2020 2020 2020  key'] }}".      
-000000e0: 646f 6d61 696e 3a20 227b 7b20 636f 6e66  domain: "{{ conf
-000000f0: 6967 5b27 646f 6d61 696e 275d 207d 7d22  ig['domain'] }}"
-00000100: 0a20 2072 6574 7269 6576 6572 3a0a 2020  .  retriever:.  
-00000110: 2020 7265 636f 7264 5f73 656c 6563 746f    record_selecto
-00000120: 723a 0a20 2020 2020 2024 7265 663a 2022  r:.      $ref: "
-00000130: 232f 6465 6669 6e69 7469 6f6e 732f 7365  #/definitions/se
-00000140: 6c65 6374 6f72 220a 2020 2020 7061 6769  lector".    pagi
-00000150: 6e61 746f 723a 0a20 2020 2020 2074 7970  nator:.      typ
-00000160: 653a 204e 6f50 6167 696e 6174 696f 6e0a  e: NoPagination.
-00000170: 2020 2020 7265 7175 6573 7465 723a 0a20      requester:. 
-00000180: 2020 2020 2024 7265 663a 2022 232f 6465       $ref: "#/de
-00000190: 6669 6e69 7469 6f6e 732f 7265 7175 6573  finitions/reques
-000001a0: 7465 7222 0a20 2062 6173 655f 7374 7265  ter".  base_stre
-000001b0: 616d 3a0a 2020 2020 7265 7472 6965 7665  am:.    retrieve
-000001c0: 723a 0a20 2020 2020 2024 7265 663a 2022  r:.      $ref: "
-000001d0: 232f 6465 6669 6e69 7469 6f6e 732f 7265  #/definitions/re
-000001e0: 7472 6965 7665 7222 0a20 2077 686f 6973  triever".  whois
-000001f0: 5f73 7472 6561 6d3a 0a20 2020 2024 7265  _stream:.    $re
-00000200: 663a 2022 232f 6465 6669 6e69 7469 6f6e  f: "#/definition
-00000210: 732f 6261 7365 5f73 7472 6561 6d22 0a20  s/base_stream". 
-00000220: 2020 2024 7061 7261 6d65 7465 7273 3a0a     $parameters:.
-00000230: 2020 2020 2020 6e61 6d65 3a20 2277 686f        name: "who
-00000240: 6973 220a 2020 2020 2020 7072 696d 6172  is".      primar
-00000250: 795f 6b65 793a 2022 646f 6d61 696e 5f69  y_key: "domain_i
-00000260: 6422 0a20 2020 2020 2070 6174 683a 2022  d".      path: "
-00000270: 2f76 3222 0a0a 2020 2020 7363 6865 6d61  /v2"..    schema
-00000280: 5f6c 6f61 6465 723a 0a20 2020 2020 2074  _loader:.      t
-00000290: 7970 653a 2049 6e6c 696e 6553 6368 656d  ype: InlineSchem
-000002a0: 614c 6f61 6465 720a 2020 2020 2020 7363  aLoader.      sc
-000002b0: 6865 6d61 3a0a 2020 2020 2020 2020 2473  hema:.        $s
-000002c0: 6368 656d 613a 2068 7474 703a 2f2f 6a73  chema: http://js
-000002d0: 6f6e 2d73 6368 656d 612e 6f72 672f 6472  on-schema.org/dr
-000002e0: 6166 742d 3037 2f73 6368 656d 6123 0a20  aft-07/schema#. 
-000002f0: 2020 2020 2020 2074 7970 653a 206f 626a         type: obj
-00000300: 6563 740a 2020 2020 2020 2020 7072 6f70  ect.        prop
-00000310: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
-00000320: 2020 646f 6d61 696e 3a0a 2020 2020 2020    domain:.      
-00000330: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-00000340: 6e3a 2044 6f6d 6169 6e20 6e61 6d65 0a20  n: Domain name. 
-00000350: 2020 2020 2020 2020 2020 2074 7970 653a             type:
-00000360: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
-00000370: 2020 646f 6d61 696e 5f69 643a 0a20 2020    domain_id:.   
-00000380: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00000390: 7469 6f6e 3a20 556e 6971 7565 2069 6465  tion: Unique ide
-000003a0: 6e74 6966 6965 7220 666f 7220 7468 6520  ntifier for the 
-000003b0: 646f 6d61 696e 0a20 2020 2020 2020 2020  domain.         
-000003c0: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
-000003d0: 2020 2020 2020 2020 2020 7374 6174 7573            status
-000003e0: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-000003f0: 7363 7269 7074 696f 6e3a 2053 7461 7475  scription: Statu
-00000400: 7320 6f66 2074 6865 2064 6f6d 6169 6e20  s of the domain 
-00000410: 7265 6769 7374 7261 7469 6f6e 0a20 2020  registration.   
-00000420: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
-00000430: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
-00000440: 6372 6561 7465 5f64 6174 653a 0a20 2020  create_date:.   
-00000450: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00000460: 7469 6f6e 3a20 4461 7465 2061 6e64 2074  tion: Date and t
-00000470: 696d 6520 7768 656e 2074 6865 2064 6f6d  ime when the dom
-00000480: 6169 6e20 7761 7320 6372 6561 7465 640a  ain was created.
-00000490: 2020 2020 2020 2020 2020 2020 7479 7065              type
-000004a0: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
-000004b0: 2020 2020 2066 6f72 6d61 743a 2064 6174       format: dat
-000004c0: 652d 7469 6d65 0a20 2020 2020 2020 2020  e-time.         
-000004d0: 2075 7064 6174 655f 6461 7465 3a0a 2020   update_date:.  
-000004e0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-000004f0: 7074 696f 6e3a 2044 6174 6520 616e 6420  ption: Date and 
-00000500: 7469 6d65 2077 6865 6e20 7468 6520 646f  time when the do
-00000510: 6d61 696e 2072 6563 6f72 6420 7761 7320  main record was 
-00000520: 6c61 7374 2075 7064 6174 6564 0a20 2020  last updated.   
-00000530: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
-00000540: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
-00000550: 2020 666f 726d 6174 3a20 6461 7465 2d74    format: date-t
-00000560: 696d 650a 2020 2020 2020 2020 2020 6578  ime.          ex
-00000570: 7069 7265 5f64 6174 653a 0a20 2020 2020  pire_date:.     
-00000580: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00000590: 6f6e 3a20 4461 7465 2061 6e64 2074 696d  on: Date and tim
-000005a0: 6520 7768 656e 2074 6865 2064 6f6d 6169  e when the domai
-000005b0: 6e20 7769 6c6c 2065 7870 6972 650a 2020  n will expire.  
-000005c0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-000005d0: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-000005e0: 2020 2066 6f72 6d61 743a 2064 6174 652d     format: date-
-000005f0: 7469 6d65 0a20 2020 2020 2020 2020 2064  time.          d
-00000600: 6f6d 6169 6e5f 6167 653a 0a20 2020 2020  omain_age:.     
-00000610: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00000620: 6f6e 3a20 4167 6520 6f66 2074 6865 2064  on: Age of the d
-00000630: 6f6d 6169 6e20 696e 2079 6561 7273 0a20  omain in years. 
-00000640: 2020 2020 2020 2020 2020 2074 7970 653a             type:
-00000650: 2069 6e74 6567 6572 0a20 2020 2020 2020   integer.       
-00000660: 2020 2077 686f 6973 5f73 6572 7665 723a     whois_server:
-00000670: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-00000680: 6372 6970 7469 6f6e 3a20 5768 6f69 7320  cription: Whois 
-00000690: 7365 7276 6572 2075 7365 6420 746f 2071  server used to q
-000006a0: 7565 7279 2074 6865 2064 6f6d 6169 6e20  uery the domain 
-000006b0: 7265 6769 7374 7261 7469 6f6e 2069 6e66  registration inf
-000006c0: 6f72 6d61 7469 6f6e 0a20 2020 2020 2020  ormation.       
-000006d0: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-000006e0: 670a 2020 2020 2020 2020 2020 7265 6769  g.          regi
-000006f0: 7374 7261 723a 0a20 2020 2020 2020 2020  strar:.         
-00000700: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-00000710: 4465 7461 696c 7320 6f66 2074 6865 2072  Details of the r
-00000720: 6567 6973 7472 6172 2066 6f72 2074 6865  egistrar for the
-00000730: 2064 6f6d 6169 6e0a 2020 2020 2020 2020   domain.        
-00000740: 2020 2020 7479 7065 3a20 6f62 6a65 6374      type: object
-00000750: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00000760: 7065 7274 6965 733a 0a20 2020 2020 2020  perties:.       
-00000770: 2020 2020 2020 2069 616e 615f 6964 3a0a         iana_id:.
-00000780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000790: 6465 7363 7269 7074 696f 6e3a 2049 414e  description: IAN
-000007a0: 4120 4944 206f 6620 7468 6520 7265 6769  A ID of the regi
-000007b0: 7374 7261 720a 2020 2020 2020 2020 2020  strar.          
-000007c0: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
-000007d0: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
-000007e0: 206e 616d 653a 0a20 2020 2020 2020 2020   name:.         
-000007f0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00000800: 6f6e 3a20 4e61 6d65 206f 6620 7468 6520  on: Name of the 
-00000810: 7265 6769 7374 7261 720a 2020 2020 2020  registrar.      
-00000820: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-00000830: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-00000840: 2020 2020 2075 726c 3a0a 2020 2020 2020       url:.      
-00000850: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00000860: 7074 696f 6e3a 2055 524c 206f 6620 7468  ption: URL of th
-00000870: 6520 7265 6769 7374 7261 720a 2020 2020  e registrar.    
-00000880: 2020 2020 2020 2020 2020 2020 7479 7065              type
-00000890: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
-000008a0: 2020 2020 2072 6571 7569 7265 643a 0a20       required:. 
-000008b0: 2020 2020 2020 2020 2020 2020 202d 2069               - i
-000008c0: 616e 615f 6964 0a20 2020 2020 2020 2020  ana_id.         
-000008d0: 2020 2020 202d 206e 616d 650a 2020 2020       - name.    
-000008e0: 2020 2020 2020 2020 2020 2d20 7572 6c0a            - url.
-000008f0: 2020 2020 2020 2020 2020 2020 6164 6469              addi
-00000900: 7469 6f6e 616c 5072 6f70 6572 7469 6573  tionalProperties
-00000910: 3a20 7472 7565 0a20 2020 2020 2020 2020  : true.         
-00000920: 2072 6567 6973 7472 616e 743a 0a20 2020   registrant:.   
-00000930: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00000940: 7469 6f6e 3a20 4465 7461 696c 7320 6f66  tion: Details of
-00000950: 2074 6865 2072 6567 6973 7472 616e 7420   the registrant 
-00000960: 636f 6e74 6163 740a 2020 2020 2020 2020  contact.        
-00000970: 2020 2020 7479 7065 3a20 6f62 6a65 6374      type: object
-00000980: 0a20 2020 2020 2020 2020 2020 2070 726f  .            pro
-00000990: 7065 7274 6965 733a 0a20 2020 2020 2020  perties:.       
-000009a0: 2020 2020 2020 206e 616d 653a 0a20 2020         name:.   
-000009b0: 2020 2020 2020 2020 2020 2020 2064 6573               des
-000009c0: 6372 6970 7469 6f6e 3a20 4e61 6d65 206f  cription: Name o
-000009d0: 6620 7468 6520 7265 6769 7374 7261 6e74  f the registrant
-000009e0: 2063 6f6e 7461 6374 0a20 2020 2020 2020   contact.       
-000009f0: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
-00000a00: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
-00000a10: 2020 2020 6f72 6761 6e69 7a61 7469 6f6e      organization
-00000a20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00000a30: 2020 6465 7363 7269 7074 696f 6e3a 204f    description: O
-00000a40: 7267 616e 697a 6174 696f 6e20 6f66 2074  rganization of t
-00000a50: 6865 2072 6567 6973 7472 616e 7420 636f  he registrant co
-00000a60: 6e74 6163 740a 2020 2020 2020 2020 2020  ntact.          
-00000a70: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
-00000a80: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
-00000a90: 2073 7472 6565 745f 6164 6472 6573 733a   street_address:
-00000aa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ab0: 2064 6573 6372 6970 7469 6f6e 3a20 5374   description: St
-00000ac0: 7265 6574 2061 6464 7265 7373 206f 6620  reet address of 
-00000ad0: 7468 6520 7265 6769 7374 7261 6e74 2063  the registrant c
-00000ae0: 6f6e 7461 6374 0a20 2020 2020 2020 2020  ontact.         
-00000af0: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-00000b00: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00000b10: 2020 6369 7479 3a0a 2020 2020 2020 2020    city:.        
-00000b20: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00000b30: 696f 6e3a 2043 6974 7920 6f66 2074 6865  ion: City of the
-00000b40: 2072 6567 6973 7472 616e 7420 636f 6e74   registrant cont
-00000b50: 6163 740a 2020 2020 2020 2020 2020 2020  act.            
-00000b60: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-00000b70: 0a20 2020 2020 2020 2020 2020 2020 2072  .              r
-00000b80: 6567 696f 6e3a 0a20 2020 2020 2020 2020  egion:.         
-00000b90: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00000ba0: 6f6e 3a20 5265 6769 6f6e 206f 6620 7468  on: Region of th
-00000bb0: 6520 7265 6769 7374 7261 6e74 2063 6f6e  e registrant con
-00000bc0: 7461 6374 0a20 2020 2020 2020 2020 2020  tact.           
-00000bd0: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-00000be0: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-00000bf0: 7a69 705f 636f 6465 3a0a 2020 2020 2020  zip_code:.      
-00000c00: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00000c10: 7074 696f 6e3a 205a 6970 2063 6f64 6520  ption: Zip code 
-00000c20: 6f66 2074 6865 2072 6567 6973 7472 616e  of the registran
-00000c30: 7420 636f 6e74 6163 740a 2020 2020 2020  t contact.      
-00000c40: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-00000c50: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-00000c60: 2020 2020 2063 6f75 6e74 7279 3a0a 2020       country:.  
-00000c70: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00000c80: 7363 7269 7074 696f 6e3a 2043 6f75 6e74  scription: Count
-00000c90: 7279 206f 6620 7468 6520 7265 6769 7374  ry of the regist
-00000ca0: 7261 6e74 2063 6f6e 7461 6374 0a20 2020  rant contact.   
-00000cb0: 2020 2020 2020 2020 2020 2020 2074 7970               typ
-00000cc0: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
-00000cd0: 2020 2020 2020 2020 7068 6f6e 653a 0a20          phone:. 
-00000ce0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00000cf0: 6573 6372 6970 7469 6f6e 3a20 5068 6f6e  escription: Phon
-00000d00: 6520 6e75 6d62 6572 206f 6620 7468 6520  e number of the 
-00000d10: 7265 6769 7374 7261 6e74 2063 6f6e 7461  registrant conta
-00000d20: 6374 0a20 2020 2020 2020 2020 2020 2020  ct.             
-00000d30: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
-00000d40: 2020 2020 2020 2020 2020 2020 2020 6661                fa
-00000d50: 783a 0a20 2020 2020 2020 2020 2020 2020  x:.             
-00000d60: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
-00000d70: 4661 7820 6e75 6d62 6572 206f 6620 7468  Fax number of th
-00000d80: 6520 7265 6769 7374 7261 6e74 2063 6f6e  e registrant con
-00000d90: 7461 6374 0a20 2020 2020 2020 2020 2020  tact.           
-00000da0: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-00000db0: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-00000dc0: 656d 6169 6c3a 0a20 2020 2020 2020 2020  email:.         
-00000dd0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00000de0: 6f6e 3a20 456d 6169 6c20 6f66 2074 6865  on: Email of the
-00000df0: 2072 6567 6973 7472 616e 7420 636f 6e74   registrant cont
-00000e00: 6163 740a 2020 2020 2020 2020 2020 2020  act.            
-00000e10: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-00000e20: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-00000e30: 7569 7265 643a 0a20 2020 2020 2020 2020  uired:.         
-00000e40: 2020 2020 202d 206e 616d 650a 2020 2020       - name.    
-00000e50: 2020 2020 2020 2020 2020 2d20 6f72 6761            - orga
-00000e60: 6e69 7a61 7469 6f6e 0a20 2020 2020 2020  nization.       
-00000e70: 2020 2020 2020 202d 2073 7472 6565 745f         - street_
-00000e80: 6164 6472 6573 730a 2020 2020 2020 2020  address.        
-00000e90: 2020 2020 2020 2d20 6369 7479 0a20 2020        - city.   
-00000ea0: 2020 2020 2020 2020 2020 202d 2072 6567             - reg
-00000eb0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00000ec0: 2020 2d20 7a69 705f 636f 6465 0a20 2020    - zip_code.   
-00000ed0: 2020 2020 2020 2020 2020 202d 2063 6f75             - cou
-00000ee0: 6e74 7279 0a20 2020 2020 2020 2020 2020  ntry.           
-00000ef0: 2020 202d 2070 686f 6e65 0a20 2020 2020     - phone.     
-00000f00: 2020 2020 2020 2020 202d 2066 6178 0a20           - fax. 
-00000f10: 2020 2020 2020 2020 2020 2020 202d 2065               - e
-00000f20: 6d61 696c 0a20 2020 2020 2020 2020 2020  mail.           
-00000f30: 2061 6464 6974 696f 6e61 6c50 726f 7065   additionalPrope
-00000f40: 7274 6965 733a 2074 7275 650a 2020 2020  rties: true.    
-00000f50: 2020 2020 2020 6164 6d69 6e3a 0a20 2020        admin:.   
-00000f60: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00000f70: 7469 6f6e 3a20 4465 7461 696c 7320 6f66  tion: Details of
-00000f80: 2074 6865 2061 646d 696e 6973 7472 6174   the administrat
-00000f90: 6976 6520 636f 6e74 6163 740a 2020 2020  ive contact.    
-00000fa0: 2020 2020 2020 2020 7479 7065 3a20 6f62          type: ob
-00000fb0: 6a65 6374 0a20 2020 2020 2020 2020 2020  ject.           
-00000fc0: 2070 726f 7065 7274 6965 733a 0a20 2020   properties:.   
-00000fd0: 2020 2020 2020 2020 2020 206e 616d 653a             name:
-00000fe0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00000ff0: 2064 6573 6372 6970 7469 6f6e 3a20 4e61   description: Na
-00001000: 6d65 206f 6620 7468 6520 6164 6d69 6e69  me of the admini
-00001010: 7374 7261 7469 7665 2063 6f6e 7461 6374  strative contact
-00001020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00001030: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
-00001040: 2020 2020 2020 2020 2020 2020 6f72 6761              orga
-00001050: 6e69 7a61 7469 6f6e 3a0a 2020 2020 2020  nization:.      
-00001060: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00001070: 7074 696f 6e3a 204f 7267 616e 697a 6174  ption: Organizat
-00001080: 696f 6e20 6f66 2074 6865 2061 646d 696e  ion of the admin
-00001090: 6973 7472 6174 6976 6520 636f 6e74 6163  istrative contac
-000010a0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-000010b0: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-000010c0: 2020 2020 2020 2020 2020 2020 2073 7472               str
-000010d0: 6565 745f 6164 6472 6573 733a 0a20 2020  eet_address:.   
-000010e0: 2020 2020 2020 2020 2020 2020 2064 6573               des
-000010f0: 6372 6970 7469 6f6e 3a20 5374 7265 6574  cription: Street
-00001100: 2061 6464 7265 7373 206f 6620 7468 6520   address of the 
-00001110: 6164 6d69 6e69 7374 7261 7469 7665 2063  administrative c
-00001120: 6f6e 7461 6374 0a20 2020 2020 2020 2020  ontact.         
-00001130: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-00001140: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00001150: 2020 6369 7479 3a0a 2020 2020 2020 2020    city:.        
-00001160: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00001170: 696f 6e3a 2043 6974 7920 6f66 2074 6865  ion: City of the
-00001180: 2061 646d 696e 6973 7472 6174 6976 6520   administrative 
-00001190: 636f 6e74 6163 740a 2020 2020 2020 2020  contact.        
-000011a0: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
-000011b0: 7269 6e67 0a20 2020 2020 2020 2020 2020  ring.           
-000011c0: 2020 2072 6567 696f 6e3a 0a20 2020 2020     region:.     
-000011d0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-000011e0: 6970 7469 6f6e 3a20 5265 6769 6f6e 206f  iption: Region o
-000011f0: 6620 7468 6520 6164 6d69 6e69 7374 7261  f the administra
-00001200: 7469 7665 2063 6f6e 7461 6374 0a20 2020  tive contact.   
-00001210: 2020 2020 2020 2020 2020 2020 2074 7970               typ
-00001220: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
-00001230: 2020 2020 2020 2020 7a69 705f 636f 6465          zip_code
-00001240: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001250: 2020 6465 7363 7269 7074 696f 6e3a 205a    description: Z
-00001260: 6970 2063 6f64 6520 6f66 2074 6865 2061  ip code of the a
-00001270: 646d 696e 6973 7472 6174 6976 6520 636f  dministrative co
-00001280: 6e74 6163 740a 2020 2020 2020 2020 2020  ntact.          
-00001290: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
-000012a0: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
-000012b0: 2063 6f75 6e74 7279 3a0a 2020 2020 2020   country:.      
-000012c0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-000012d0: 7074 696f 6e3a 2043 6f75 6e74 7279 206f  ption: Country o
-000012e0: 6620 7468 6520 6164 6d69 6e69 7374 7261  f the administra
-000012f0: 7469 7665 2063 6f6e 7461 6374 0a20 2020  tive contact.   
-00001300: 2020 2020 2020 2020 2020 2020 2074 7970               typ
-00001310: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
-00001320: 2020 2020 2020 2020 7068 6f6e 653a 0a20          phone:. 
-00001330: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00001340: 6573 6372 6970 7469 6f6e 3a20 5068 6f6e  escription: Phon
-00001350: 6520 6e75 6d62 6572 206f 6620 7468 6520  e number of the 
-00001360: 6164 6d69 6e69 7374 7261 7469 7665 2063  administrative c
-00001370: 6f6e 7461 6374 0a20 2020 2020 2020 2020  ontact.         
-00001380: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-00001390: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-000013a0: 2020 6661 783a 0a20 2020 2020 2020 2020    fax:.         
-000013b0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-000013c0: 6f6e 3a20 4661 7820 6e75 6d62 6572 206f  on: Fax number o
-000013d0: 6620 7468 6520 6164 6d69 6e69 7374 7261  f the administra
-000013e0: 7469 7665 2063 6f6e 7461 6374 0a20 2020  tive contact.   
-000013f0: 2020 2020 2020 2020 2020 2020 2074 7970               typ
-00001400: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
-00001410: 2020 2020 2020 2020 656d 6169 6c3a 0a20          email:. 
-00001420: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00001430: 6573 6372 6970 7469 6f6e 3a20 456d 6169  escription: Emai
-00001440: 6c20 6f66 2074 6865 2061 646d 696e 6973  l of the adminis
-00001450: 7472 6174 6976 6520 636f 6e74 6163 740a  trative contact.
-00001460: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001470: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
-00001480: 2020 2020 2020 2020 2072 6571 7569 7265           require
-00001490: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
-000014a0: 202d 206e 616d 650a 2020 2020 2020 2020   - name.        
-000014b0: 2020 2020 2020 2d20 6f72 6761 6e69 7a61        - organiza
-000014c0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-000014d0: 2020 202d 2073 7472 6565 745f 6164 6472     - street_addr
-000014e0: 6573 730a 2020 2020 2020 2020 2020 2020  ess.            
-000014f0: 2020 2d20 6369 7479 0a20 2020 2020 2020    - city.       
-00001500: 2020 2020 2020 202d 2072 6567 696f 6e0a         - region.
-00001510: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00001520: 7a69 705f 636f 6465 0a20 2020 2020 2020  zip_code.       
-00001530: 2020 2020 2020 202d 2063 6f75 6e74 7279         - country
-00001540: 0a20 2020 2020 2020 2020 2020 2020 202d  .              -
-00001550: 2070 686f 6e65 0a20 2020 2020 2020 2020   phone.         
-00001560: 2020 2020 202d 2066 6178 0a20 2020 2020       - fax.     
-00001570: 2020 2020 2020 2020 202d 2065 6d61 696c           - email
-00001580: 0a20 2020 2020 2020 2020 2020 2061 6464  .            add
-00001590: 6974 696f 6e61 6c50 726f 7065 7274 6965  itionalPropertie
-000015a0: 733a 2074 7275 650a 2020 2020 2020 2020  s: true.        
-000015b0: 2020 7465 6368 3a0a 2020 2020 2020 2020    tech:.        
-000015c0: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
-000015d0: 2044 6574 6169 6c73 206f 6620 7468 6520   Details of the 
-000015e0: 7465 6368 6e69 6361 6c20 636f 6e74 6163  technical contac
-000015f0: 740a 2020 2020 2020 2020 2020 2020 7479  t.            ty
-00001600: 7065 3a20 6f62 6a65 6374 0a20 2020 2020  pe: object.     
-00001610: 2020 2020 2020 2070 726f 7065 7274 6965         propertie
-00001620: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-00001630: 206e 616d 653a 0a20 2020 2020 2020 2020   name:.         
-00001640: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
-00001650: 6f6e 3a20 4e61 6d65 206f 6620 7468 6520  on: Name of the 
-00001660: 7465 6368 6e69 6361 6c20 636f 6e74 6163  technical contac
-00001670: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-00001680: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
-00001690: 2020 2020 2020 2020 2020 2020 206f 7267               org
-000016a0: 616e 697a 6174 696f 6e3a 0a20 2020 2020  anization:.     
-000016b0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-000016c0: 6970 7469 6f6e 3a20 4f72 6761 6e69 7a61  iption: Organiza
-000016d0: 7469 6f6e 206f 6620 7468 6520 7465 6368  tion of the tech
-000016e0: 6e69 6361 6c20 636f 6e74 6163 740a 2020  nical contact.  
-000016f0: 2020 2020 2020 2020 2020 2020 2020 7479                ty
-00001700: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
-00001710: 2020 2020 2020 2020 2073 7472 6565 745f           street_
-00001720: 6164 6472 6573 733a 0a20 2020 2020 2020  address:.       
-00001730: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00001740: 7469 6f6e 3a20 5374 7265 6574 2061 6464  tion: Street add
-00001750: 7265 7373 206f 6620 7468 6520 7465 6368  ress of the tech
-00001760: 6e69 6361 6c20 636f 6e74 6163 740a 2020  nical contact.  
-00001770: 2020 2020 2020 2020 2020 2020 2020 7479                ty
-00001780: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
-00001790: 2020 2020 2020 2020 2063 6974 793a 0a20           city:. 
-000017a0: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-000017b0: 6573 6372 6970 7469 6f6e 3a20 4369 7479  escription: City
-000017c0: 206f 6620 7468 6520 7465 6368 6e69 6361   of the technica
-000017d0: 6c20 636f 6e74 6163 740a 2020 2020 2020  l contact.      
-000017e0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-000017f0: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-00001800: 2020 2020 2072 6567 696f 6e3a 0a20 2020       region:.   
-00001810: 2020 2020 2020 2020 2020 2020 2064 6573               des
-00001820: 6372 6970 7469 6f6e 3a20 5265 6769 6f6e  cription: Region
-00001830: 206f 6620 7468 6520 7465 6368 6e69 6361   of the technica
-00001840: 6c20 636f 6e74 6163 740a 2020 2020 2020  l contact.      
-00001850: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-00001860: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-00001870: 2020 2020 207a 6970 5f63 6f64 653a 0a20       zip_code:. 
-00001880: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00001890: 6573 6372 6970 7469 6f6e 3a20 5a69 7020  escription: Zip 
-000018a0: 636f 6465 206f 6620 7468 6520 7465 6368  code of the tech
-000018b0: 6e69 6361 6c20 636f 6e74 6163 740a 2020  nical contact.  
-000018c0: 2020 2020 2020 2020 2020 2020 2020 7479                ty
-000018d0: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
-000018e0: 2020 2020 2020 2020 2063 6f75 6e74 7279           country
-000018f0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001900: 2020 6465 7363 7269 7074 696f 6e3a 2043    description: C
-00001910: 6f75 6e74 7279 206f 6620 7468 6520 7465  ountry of the te
-00001920: 6368 6e69 6361 6c20 636f 6e74 6163 740a  chnical contact.
-00001930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00001940: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
-00001950: 2020 2020 2020 2020 2020 2070 686f 6e65             phone
-00001960: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00001970: 2020 6465 7363 7269 7074 696f 6e3a 2050    description: P
-00001980: 686f 6e65 206e 756d 6265 7220 6f66 2074  hone number of t
-00001990: 6865 2074 6563 686e 6963 616c 2063 6f6e  he technical con
-000019a0: 7461 6374 0a20 2020 2020 2020 2020 2020  tact.           
-000019b0: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-000019c0: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-000019d0: 6661 783a 0a20 2020 2020 2020 2020 2020  fax:.           
-000019e0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
-000019f0: 3a20 4661 7820 6e75 6d62 6572 206f 6620  : Fax number of 
-00001a00: 7468 6520 7465 6368 6e69 6361 6c20 636f  the technical co
-00001a10: 6e74 6163 740a 2020 2020 2020 2020 2020  ntact.          
-00001a20: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
-00001a30: 6e67 0a20 2020 2020 2020 2020 2020 2020  ng.             
-00001a40: 2065 6d61 696c 3a0a 2020 2020 2020 2020   email:.        
-00001a50: 2020 2020 2020 2020 6465 7363 7269 7074          descript
-00001a60: 696f 6e3a 2045 6d61 696c 206f 6620 7468  ion: Email of th
-00001a70: 6520 7465 6368 6e69 6361 6c20 636f 6e74  e technical cont
-00001a80: 6163 740a 2020 2020 2020 2020 2020 2020  act.            
-00001a90: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
-00001aa0: 0a20 2020 2020 2020 2020 2020 2072 6571  .            req
-00001ab0: 7569 7265 643a 0a20 2020 2020 2020 2020  uired:.         
-00001ac0: 2020 2020 202d 206e 616d 650a 2020 2020       - name.    
-00001ad0: 2020 2020 2020 2020 2020 2d20 6f72 6761            - orga
-00001ae0: 6e69 7a61 7469 6f6e 0a20 2020 2020 2020  nization.       
-00001af0: 2020 2020 2020 202d 2073 7472 6565 745f         - street_
-00001b00: 6164 6472 6573 730a 2020 2020 2020 2020  address.        
-00001b10: 2020 2020 2020 2d20 6369 7479 0a20 2020        - city.   
-00001b20: 2020 2020 2020 2020 2020 202d 2072 6567             - reg
-00001b30: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-00001b40: 2020 2d20 7a69 705f 636f 6465 0a20 2020    - zip_code.   
-00001b50: 2020 2020 2020 2020 2020 202d 2063 6f75             - cou
-00001b60: 6e74 7279 0a20 2020 2020 2020 2020 2020  ntry.           
-00001b70: 2020 202d 2070 686f 6e65 0a20 2020 2020     - phone.     
-00001b80: 2020 2020 2020 2020 202d 2066 6178 0a20           - fax. 
-00001b90: 2020 2020 2020 2020 2020 2020 202d 2065               - e
-00001ba0: 6d61 696c 0a20 2020 2020 2020 2020 2020  mail.           
-00001bb0: 2061 6464 6974 696f 6e61 6c50 726f 7065   additionalPrope
-00001bc0: 7274 6965 733a 2074 7275 650a 2020 2020  rties: true.    
-00001bd0: 2020 2020 2020 6269 6c6c 696e 673a 0a20        billing:. 
-00001be0: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-00001bf0: 6970 7469 6f6e 3a20 4465 7461 696c 7320  iption: Details 
-00001c00: 6f66 2074 6865 2062 696c 6c69 6e67 2063  of the billing c
-00001c10: 6f6e 7461 6374 0a20 2020 2020 2020 2020  ontact.         
-00001c20: 2020 2074 7970 653a 206f 626a 6563 740a     type: object.
-00001c30: 2020 2020 2020 2020 2020 2020 7072 6f70              prop
-00001c40: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
-00001c50: 2020 2020 2020 6e61 6d65 3a0a 2020 2020        name:.    
-00001c60: 2020 2020 2020 2020 2020 2020 6465 7363              desc
-00001c70: 7269 7074 696f 6e3a 204e 616d 6520 6f66  ription: Name of
-00001c80: 2074 6865 2062 696c 6c69 6e67 2063 6f6e   the billing con
-00001c90: 7461 6374 0a20 2020 2020 2020 2020 2020  tact.           
-00001ca0: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-00001cb0: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-00001cc0: 6f72 6761 6e69 7a61 7469 6f6e 3a0a 2020  organization:.  
-00001cd0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00001ce0: 7363 7269 7074 696f 6e3a 204f 7267 616e  scription: Organ
-00001cf0: 697a 6174 696f 6e20 6f66 2074 6865 2062  ization of the b
-00001d00: 696c 6c69 6e67 2063 6f6e 7461 6374 0a20  illing contact. 
-00001d10: 2020 2020 2020 2020 2020 2020 2020 2074                 t
-00001d20: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
-00001d30: 2020 2020 2020 2020 2020 7374 7265 6574            street
-00001d40: 5f61 6464 7265 7373 3a0a 2020 2020 2020  _address:.      
-00001d50: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00001d60: 7074 696f 6e3a 2053 7472 6565 7420 6164  ption: Street ad
-00001d70: 6472 6573 7320 6f66 2074 6865 2062 696c  dress of the bil
-00001d80: 6c69 6e67 2063 6f6e 7461 6374 0a20 2020  ling contact.   
-00001d90: 2020 2020 2020 2020 2020 2020 2074 7970               typ
-00001da0: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
-00001db0: 2020 2020 2020 2020 6369 7479 3a0a 2020          city:.  
-00001dc0: 2020 2020 2020 2020 2020 2020 2020 6465                de
-00001dd0: 7363 7269 7074 696f 6e3a 2043 6974 7920  scription: City 
-00001de0: 6f66 2074 6865 2062 696c 6c69 6e67 2063  of the billing c
-00001df0: 6f6e 7461 6374 0a20 2020 2020 2020 2020  ontact.         
-00001e00: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-00001e10: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00001e20: 2020 7265 6769 6f6e 3a0a 2020 2020 2020    region:.      
+00000000: 7665 7273 696f 6e3a 2030 2e37 382e 350a  version: 0.78.5.
+00000010: 0a74 7970 653a 2044 6563 6c61 7261 7469  .type: Declarati
+00000020: 7665 536f 7572 6365 0a0a 6368 6563 6b3a  veSource..check:
+00000030: 0a20 2074 7970 653a 2043 6865 636b 5374  .  type: CheckSt
+00000040: 7265 616d 0a20 2073 7472 6561 6d5f 6e61  ream.  stream_na
+00000050: 6d65 733a 0a20 2020 202d 2077 686f 6973  mes:.    - whois
+00000060: 0a0a 6465 6669 6e69 7469 6f6e 733a 0a20  ..definitions:. 
+00000070: 2073 7472 6561 6d73 3a0a 2020 2020 7768   streams:.    wh
+00000080: 6f69 733a 0a20 2020 2020 2074 7970 653a  ois:.      type:
+00000090: 2044 6563 6c61 7261 7469 7665 5374 7265   DeclarativeStre
+000000a0: 616d 0a20 2020 2020 206e 616d 653a 2077  am.      name: w
+000000b0: 686f 6973 0a20 2020 2020 2070 7269 6d61  hois.      prima
+000000c0: 7279 5f6b 6579 3a0a 2020 2020 2020 2020  ry_key:.        
+000000d0: 2d20 646f 6d61 696e 5f69 640a 2020 2020  - domain_id.    
+000000e0: 2020 7265 7472 6965 7665 723a 0a20 2020    retriever:.   
+000000f0: 2020 2020 2074 7970 653a 2053 696d 706c       type: Simpl
+00000100: 6552 6574 7269 6576 6572 0a20 2020 2020  eRetriever.     
+00000110: 2020 2072 6571 7565 7374 6572 3a0a 2020     requester:.  
+00000120: 2020 2020 2020 2020 2472 6566 3a20 2223          $ref: "#
+00000130: 2f64 6566 696e 6974 696f 6e73 2f62 6173  /definitions/bas
+00000140: 655f 7265 7175 6573 7465 7222 0a20 2020  e_requester".   
+00000150: 2020 2020 2020 2070 6174 683a 202f 7632         path: /v2
+00000160: 0a20 2020 2020 2020 2020 2068 7474 705f  .          http_
+00000170: 6d65 7468 6f64 3a20 4745 540a 2020 2020  method: GET.    
+00000180: 2020 2020 2020 7265 7175 6573 745f 7061        request_pa
+00000190: 7261 6d65 7465 7273 3a0a 2020 2020 2020  rameters:.      
+000001a0: 2020 2020 2020 6b65 793a 2022 7b7b 2063        key: "{{ c
+000001b0: 6f6e 6669 675b 2761 7069 5f6b 6579 275d  onfig['api_key']
+000001c0: 207d 7d22 0a20 2020 2020 2020 2020 2020   }}".           
+000001d0: 2064 6f6d 6169 6e3a 2022 7b7b 2063 6f6e   domain: "{{ con
+000001e0: 6669 675b 2764 6f6d 6169 6e27 5d20 7d7d  fig['domain'] }}
+000001f0: 220a 2020 2020 2020 2020 7265 636f 7264  ".        record
+00000200: 5f73 656c 6563 746f 723a 0a20 2020 2020  _selector:.     
+00000210: 2020 2020 2074 7970 653a 2052 6563 6f72       type: Recor
+00000220: 6453 656c 6563 746f 720a 2020 2020 2020  dSelector.      
+00000230: 2020 2020 6578 7472 6163 746f 723a 0a20      extractor:. 
+00000240: 2020 2020 2020 2020 2020 2074 7970 653a             type:
+00000250: 2044 7061 7468 4578 7472 6163 746f 720a   DpathExtractor.
+00000260: 2020 2020 2020 2020 2020 2020 6669 656c              fiel
+00000270: 645f 7061 7468 3a20 5b5d 0a20 2020 2020  d_path: [].     
+00000280: 2073 6368 656d 615f 6c6f 6164 6572 3a0a   schema_loader:.
+00000290: 2020 2020 2020 2020 7479 7065 3a20 496e          type: In
+000002a0: 6c69 6e65 5363 6865 6d61 4c6f 6164 6572  lineSchemaLoader
+000002b0: 0a20 2020 2020 2020 2073 6368 656d 613a  .        schema:
+000002c0: 0a20 2020 2020 2020 2020 2024 7265 663a  .          $ref:
+000002d0: 2022 232f 7363 6865 6d61 732f 7768 6f69   "#/schemas/whoi
+000002e0: 7322 0a20 2062 6173 655f 7265 7175 6573  s".  base_reques
+000002f0: 7465 723a 0a20 2020 2074 7970 653a 2048  ter:.    type: H
+00000300: 7474 7052 6571 7565 7374 6572 0a20 2020  ttpRequester.   
+00000310: 2075 726c 5f62 6173 653a 2068 7474 7073   url_base: https
+00000320: 3a2f 2f61 7069 2e69 7032 7768 6f69 732e  ://api.ip2whois.
+00000330: 636f 6d0a 0a73 7472 6561 6d73 3a0a 2020  com..streams:.  
+00000340: 2d20 2472 6566 3a20 2223 2f64 6566 696e  - $ref: "#/defin
+00000350: 6974 696f 6e73 2f73 7472 6561 6d73 2f77  itions/streams/w
+00000360: 686f 6973 220a 0a73 7065 633a 0a20 2074  hois"..spec:.  t
+00000370: 7970 653a 2053 7065 630a 2020 636f 6e6e  ype: Spec.  conn
+00000380: 6563 7469 6f6e 5f73 7065 6369 6669 6361  ection_specifica
+00000390: 7469 6f6e 3a0a 2020 2020 7479 7065 3a20  tion:.    type: 
+000003a0: 6f62 6a65 6374 0a20 2020 2024 7363 6865  object.    $sche
+000003b0: 6d61 3a20 6874 7470 3a2f 2f6a 736f 6e2d  ma: http://json-
+000003c0: 7363 6865 6d61 2e6f 7267 2f64 7261 6674  schema.org/draft
+000003d0: 2d30 372f 7363 6865 6d61 230a 2020 2020  -07/schema#.    
+000003e0: 7265 7175 6972 6564 3a20 5b5d 0a20 2020  required: [].   
+000003f0: 2070 726f 7065 7274 6965 733a 0a20 2020   properties:.   
+00000400: 2020 2061 7069 5f6b 6579 3a0a 2020 2020     api_key:.    
+00000410: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+00000420: 0a20 2020 2020 2020 2074 6974 6c65 3a20  .        title: 
+00000430: 4150 4920 6b65 790a 2020 2020 2020 2020  API key.        
+00000440: 6465 7363 7269 7074 696f 6e3a 203e 2d0a  description: >-.
+00000450: 2020 2020 2020 2020 2020 596f 7572 2041            Your A
+00000460: 5049 204b 6579 2e20 5365 6520 3c61 0a20  PI Key. See <a. 
+00000470: 2020 2020 2020 2020 2068 7265 663d 2268           href="h
+00000480: 7474 7073 3a2f 2f77 7777 2e69 7032 7768  ttps://www.ip2wh
+00000490: 6f69 732e 636f 6d2f 6465 7665 6c6f 7065  ois.com/develope
+000004a0: 7273 2d61 7069 223e 6865 7265 3c2f 613e  rs-api">here</a>
+000004b0: 2e0a 2020 2020 2020 2020 6169 7262 7974  ..        airbyt
+000004c0: 655f 7365 6372 6574 3a20 7472 7565 0a20  e_secret: true. 
+000004d0: 2020 2020 2020 206f 7264 6572 3a20 300a         order: 0.
+000004e0: 2020 2020 2020 646f 6d61 696e 3a0a 2020        domain:.  
+000004f0: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+00000500: 6e67 0a20 2020 2020 2020 2074 6974 6c65  ng.        title
+00000510: 3a20 446f 6d61 696e 0a20 2020 2020 2020  : Domain.       
+00000520: 2064 6573 6372 6970 7469 6f6e 3a20 3e2d   description: >-
+00000530: 0a20 2020 2020 2020 2020 2044 6f6d 6169  .          Domai
+00000540: 6e20 6e61 6d65 2e20 5365 6520 3c61 0a20  n name. See <a. 
+00000550: 2020 2020 2020 2020 2068 7265 663d 2268           href="h
+00000560: 7474 7073 3a2f 2f77 7777 2e69 7032 7768  ttps://www.ip2wh
+00000570: 6f69 732e 636f 6d2f 6465 7665 6c6f 7065  ois.com/develope
+00000580: 7273 2d61 7069 223e 6865 7265 3c2f 613e  rs-api">here</a>
+00000590: 2e0a 2020 2020 2020 2020 6578 616d 706c  ..        exampl
+000005a0: 6573 3a0a 2020 2020 2020 2020 2020 2d20  es:.          - 
+000005b0: 7777 772e 676f 6f67 6c65 2e63 6f6d 0a20  www.google.com. 
+000005c0: 2020 2020 2020 2020 202d 2077 7777 2e66           - www.f
+000005d0: 6163 6562 6f6f 6b2e 636f 6d0a 2020 2020  acebook.com.    
+000005e0: 2020 2020 6f72 6465 723a 2031 0a20 2020      order: 1.   
+000005f0: 2061 6464 6974 696f 6e61 6c50 726f 7065   additionalPrope
+00000600: 7274 6965 733a 2074 7275 650a 0a6d 6574  rties: true..met
+00000610: 6164 6174 613a 0a20 2061 7574 6f49 6d70  adata:.  autoImp
+00000620: 6f72 7453 6368 656d 613a 0a20 2020 2077  ortSchema:.    w
+00000630: 686f 6973 3a20 6661 6c73 650a 0a73 6368  hois: false..sch
+00000640: 656d 6173 3a0a 2020 7768 6f69 733a 0a20  emas:.  whois:. 
+00000650: 2020 2074 7970 653a 206f 626a 6563 740a     type: object.
+00000660: 2020 2020 2473 6368 656d 613a 2068 7474      $schema: htt
+00000670: 703a 2f2f 6a73 6f6e 2d73 6368 656d 612e  p://json-schema.
+00000680: 6f72 672f 6472 6166 742d 3037 2f73 6368  org/draft-07/sch
+00000690: 656d 6123 0a20 2020 2061 6464 6974 696f  ema#.    additio
+000006a0: 6e61 6c50 726f 7065 7274 6965 733a 2074  nalProperties: t
+000006b0: 7275 650a 2020 2020 7072 6f70 6572 7469  rue.    properti
+000006c0: 6573 3a0a 2020 2020 2020 6164 6d69 6e3a  es:.      admin:
+000006d0: 0a20 2020 2020 2020 2074 7970 653a 206f  .        type: o
+000006e0: 626a 6563 740a 2020 2020 2020 2020 6164  bject.        ad
+000006f0: 6469 7469 6f6e 616c 5072 6f70 6572 7469  ditionalProperti
+00000700: 6573 3a20 7472 7565 0a20 2020 2020 2020  es: true.       
+00000710: 2064 6573 6372 6970 7469 6f6e 3a20 4465   description: De
+00000720: 7461 696c 7320 6f66 2074 6865 2061 646d  tails of the adm
+00000730: 696e 6973 7472 6174 6976 6520 636f 6e74  inistrative cont
+00000740: 6163 740a 2020 2020 2020 2020 7072 6f70  act.        prop
+00000750: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
+00000760: 2020 6369 7479 3a0a 2020 2020 2020 2020    city:.        
+00000770: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+00000780: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+00000790: 6372 6970 7469 6f6e 3a20 4369 7479 206f  cription: City o
+000007a0: 6620 7468 6520 6164 6d69 6e69 7374 7261  f the administra
+000007b0: 7469 7665 2063 6f6e 7461 6374 0a20 2020  tive contact.   
+000007c0: 2020 2020 2020 2063 6f75 6e74 7279 3a0a         country:.
+000007d0: 2020 2020 2020 2020 2020 2020 7479 7065              type
+000007e0: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+000007f0: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00000800: 3a20 436f 756e 7472 7920 6f66 2074 6865  : Country of the
+00000810: 2061 646d 696e 6973 7472 6174 6976 6520   administrative 
+00000820: 636f 6e74 6163 740a 2020 2020 2020 2020  contact.        
+00000830: 2020 656d 6169 6c3a 0a20 2020 2020 2020    email:.       
+00000840: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
+00000850: 670a 2020 2020 2020 2020 2020 2020 6465  g.            de
+00000860: 7363 7269 7074 696f 6e3a 2045 6d61 696c  scription: Email
+00000870: 206f 6620 7468 6520 6164 6d69 6e69 7374   of the administ
+00000880: 7261 7469 7665 2063 6f6e 7461 6374 0a20  rative contact. 
+00000890: 2020 2020 2020 2020 2066 6178 3a0a 2020           fax:.  
+000008a0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
+000008b0: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
+000008c0: 2020 2064 6573 6372 6970 7469 6f6e 3a20     description: 
+000008d0: 4661 7820 6e75 6d62 6572 206f 6620 7468  Fax number of th
+000008e0: 6520 6164 6d69 6e69 7374 7261 7469 7665  e administrative
+000008f0: 2063 6f6e 7461 6374 0a20 2020 2020 2020   contact.       
+00000900: 2020 206e 616d 653a 0a20 2020 2020 2020     name:.       
+00000910: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
+00000920: 670a 2020 2020 2020 2020 2020 2020 6465  g.            de
+00000930: 7363 7269 7074 696f 6e3a 204e 616d 6520  scription: Name 
+00000940: 6f66 2074 6865 2061 646d 696e 6973 7472  of the administr
+00000950: 6174 6976 6520 636f 6e74 6163 740a 2020  ative contact.  
+00000960: 2020 2020 2020 2020 6f72 6761 6e69 7a61          organiza
+00000970: 7469 6f6e 3a0a 2020 2020 2020 2020 2020  tion:.          
+00000980: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
+00000990: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+000009a0: 6970 7469 6f6e 3a20 4f72 6761 6e69 7a61  iption: Organiza
+000009b0: 7469 6f6e 206f 6620 7468 6520 6164 6d69  tion of the admi
+000009c0: 6e69 7374 7261 7469 7665 2063 6f6e 7461  nistrative conta
+000009d0: 6374 0a20 2020 2020 2020 2020 2070 686f  ct.          pho
+000009e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000009f0: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
+00000a00: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00000a10: 7469 6f6e 3a20 5068 6f6e 6520 6e75 6d62  tion: Phone numb
+00000a20: 6572 206f 6620 7468 6520 6164 6d69 6e69  er of the admini
+00000a30: 7374 7261 7469 7665 2063 6f6e 7461 6374  strative contact
+00000a40: 0a20 2020 2020 2020 2020 2072 6567 696f  .          regio
+00000a50: 6e3a 0a20 2020 2020 2020 2020 2020 2074  n:.            t
+00000a60: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
+00000a70: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00000a80: 696f 6e3a 2052 6567 696f 6e20 6f66 2074  ion: Region of t
+00000a90: 6865 2061 646d 696e 6973 7472 6174 6976  he administrativ
+00000aa0: 6520 636f 6e74 6163 740a 2020 2020 2020  e contact.      
+00000ab0: 2020 2020 7374 7265 6574 5f61 6464 7265      street_addre
+00000ac0: 7373 3a0a 2020 2020 2020 2020 2020 2020  ss:.            
+00000ad0: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
+00000ae0: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+00000af0: 7469 6f6e 3a20 5374 7265 6574 2061 6464  tion: Street add
+00000b00: 7265 7373 206f 6620 7468 6520 6164 6d69  ress of the admi
+00000b10: 6e69 7374 7261 7469 7665 2063 6f6e 7461  nistrative conta
+00000b20: 6374 0a20 2020 2020 2020 2020 207a 6970  ct.          zip
+00000b30: 5f63 6f64 653a 0a20 2020 2020 2020 2020  _code:.         
+00000b40: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
+00000b50: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00000b60: 7269 7074 696f 6e3a 205a 6970 2063 6f64  ription: Zip cod
+00000b70: 6520 6f66 2074 6865 2061 646d 696e 6973  e of the adminis
+00000b80: 7472 6174 6976 6520 636f 6e74 6163 740a  trative contact.
+00000b90: 2020 2020 2020 2020 7265 7175 6972 6564          required
+00000ba0: 3a0a 2020 2020 2020 2020 2020 2d20 6e61  :.          - na
+00000bb0: 6d65 0a20 2020 2020 2020 2020 202d 206f  me.          - o
+00000bc0: 7267 616e 697a 6174 696f 6e0a 2020 2020  rganization.    
+00000bd0: 2020 2020 2020 2d20 7374 7265 6574 5f61        - street_a
+00000be0: 6464 7265 7373 0a20 2020 2020 2020 2020  ddress.         
+00000bf0: 202d 2063 6974 790a 2020 2020 2020 2020   - city.        
+00000c00: 2020 2d20 7265 6769 6f6e 0a20 2020 2020    - region.     
+00000c10: 2020 2020 202d 207a 6970 5f63 6f64 650a       - zip_code.
+00000c20: 2020 2020 2020 2020 2020 2d20 636f 756e            - coun
+00000c30: 7472 790a 2020 2020 2020 2020 2020 2d20  try.          - 
+00000c40: 7068 6f6e 650a 2020 2020 2020 2020 2020  phone.          
+00000c50: 2d20 6661 780a 2020 2020 2020 2020 2020  - fax.          
+00000c60: 2d20 656d 6169 6c0a 2020 2020 2020 6269  - email.      bi
+00000c70: 6c6c 696e 673a 0a20 2020 2020 2020 2074  lling:.        t
+00000c80: 7970 653a 206f 626a 6563 740a 2020 2020  ype: object.    
+00000c90: 2020 2020 6164 6469 7469 6f6e 616c 5072      additionalPr
+00000ca0: 6f70 6572 7469 6573 3a20 7472 7565 0a20  operties: true. 
+00000cb0: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00000cc0: 6f6e 3a20 4465 7461 696c 7320 6f66 2074  on: Details of t
+00000cd0: 6865 2062 696c 6c69 6e67 2063 6f6e 7461  he billing conta
+00000ce0: 6374 0a20 2020 2020 2020 2070 726f 7065  ct.        prope
+00000cf0: 7274 6965 733a 0a20 2020 2020 2020 2020  rties:.         
+00000d00: 2063 6974 793a 0a20 2020 2020 2020 2020   city:.         
+00000d10: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
+00000d20: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00000d30: 7269 7074 696f 6e3a 2043 6974 7920 6f66  ription: City of
+00000d40: 2074 6865 2062 696c 6c69 6e67 2063 6f6e   the billing con
+00000d50: 7461 6374 0a20 2020 2020 2020 2020 2063  tact.          c
+00000d60: 6f75 6e74 7279 3a0a 2020 2020 2020 2020  ountry:.        
+00000d70: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+00000d80: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+00000d90: 6372 6970 7469 6f6e 3a20 436f 756e 7472  cription: Countr
+00000da0: 7920 6f66 2074 6865 2062 696c 6c69 6e67  y of the billing
+00000db0: 2063 6f6e 7461 6374 0a20 2020 2020 2020   contact.       
+00000dc0: 2020 2065 6d61 696c 3a0a 2020 2020 2020     email:.      
+00000dd0: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+00000de0: 6e67 0a20 2020 2020 2020 2020 2020 2064  ng.            d
+00000df0: 6573 6372 6970 7469 6f6e 3a20 456d 6169  escription: Emai
+00000e00: 6c20 6f66 2074 6865 2062 696c 6c69 6e67  l of the billing
+00000e10: 2063 6f6e 7461 6374 0a20 2020 2020 2020   contact.       
+00000e20: 2020 2066 6178 3a0a 2020 2020 2020 2020     fax:.        
+00000e30: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+00000e40: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+00000e50: 6372 6970 7469 6f6e 3a20 4661 7820 6e75  cription: Fax nu
+00000e60: 6d62 6572 206f 6620 7468 6520 6269 6c6c  mber of the bill
+00000e70: 696e 6720 636f 6e74 6163 740a 2020 2020  ing contact.    
+00000e80: 2020 2020 2020 6e61 6d65 3a0a 2020 2020        name:.    
+00000e90: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
+00000ea0: 7269 6e67 0a20 2020 2020 2020 2020 2020  ring.           
+00000eb0: 2064 6573 6372 6970 7469 6f6e 3a20 4e61   description: Na
+00000ec0: 6d65 206f 6620 7468 6520 6269 6c6c 696e  me of the billin
+00000ed0: 6720 636f 6e74 6163 740a 2020 2020 2020  g contact.      
+00000ee0: 2020 2020 6f72 6761 6e69 7a61 7469 6f6e      organization
+00000ef0: 3a0a 2020 2020 2020 2020 2020 2020 7479  :.            ty
+00000f00: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
+00000f10: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00000f20: 6f6e 3a20 4f72 6761 6e69 7a61 7469 6f6e  on: Organization
+00000f30: 206f 6620 7468 6520 6269 6c6c 696e 6720   of the billing 
+00000f40: 636f 6e74 6163 740a 2020 2020 2020 2020  contact.        
+00000f50: 2020 7068 6f6e 653a 0a20 2020 2020 2020    phone:.       
+00000f60: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
+00000f70: 670a 2020 2020 2020 2020 2020 2020 6465  g.            de
+00000f80: 7363 7269 7074 696f 6e3a 2050 686f 6e65  scription: Phone
+00000f90: 206e 756d 6265 7220 6f66 2074 6865 2062   number of the b
+00000fa0: 696c 6c69 6e67 2063 6f6e 7461 6374 0a20  illing contact. 
+00000fb0: 2020 2020 2020 2020 2072 6567 696f 6e3a           region:
+00000fc0: 0a20 2020 2020 2020 2020 2020 2074 7970  .            typ
+00000fd0: 653a 2073 7472 696e 670a 2020 2020 2020  e: string.      
+00000fe0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00000ff0: 6e3a 2052 6567 696f 6e20 6f66 2074 6865  n: Region of the
+00001000: 2062 696c 6c69 6e67 2063 6f6e 7461 6374   billing contact
+00001010: 0a20 2020 2020 2020 2020 2073 7472 6565  .          stree
+00001020: 745f 6164 6472 6573 733a 0a20 2020 2020  t_address:.     
+00001030: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+00001040: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00001050: 6465 7363 7269 7074 696f 6e3a 2053 7472  description: Str
+00001060: 6565 7420 6164 6472 6573 7320 6f66 2074  eet address of t
+00001070: 6865 2062 696c 6c69 6e67 2063 6f6e 7461  he billing conta
+00001080: 6374 0a20 2020 2020 2020 2020 207a 6970  ct.          zip
+00001090: 5f63 6f64 653a 0a20 2020 2020 2020 2020  _code:.         
+000010a0: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
+000010b0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+000010c0: 7269 7074 696f 6e3a 205a 6970 2063 6f64  ription: Zip cod
+000010d0: 6520 6f66 2074 6865 2062 696c 6c69 6e67  e of the billing
+000010e0: 2063 6f6e 7461 6374 0a20 2020 2020 2020   contact.       
+000010f0: 2072 6571 7569 7265 643a 0a20 2020 2020   required:.     
+00001100: 2020 2020 202d 206e 616d 650a 2020 2020       - name.    
+00001110: 2020 2020 2020 2d20 6f72 6761 6e69 7a61        - organiza
+00001120: 7469 6f6e 0a20 2020 2020 2020 2020 202d  tion.          -
+00001130: 2073 7472 6565 745f 6164 6472 6573 730a   street_address.
+00001140: 2020 2020 2020 2020 2020 2d20 6369 7479            - city
+00001150: 0a20 2020 2020 2020 2020 202d 2072 6567  .          - reg
+00001160: 696f 6e0a 2020 2020 2020 2020 2020 2d20  ion.          - 
+00001170: 7a69 705f 636f 6465 0a20 2020 2020 2020  zip_code.       
+00001180: 2020 202d 2063 6f75 6e74 7279 0a20 2020     - country.   
+00001190: 2020 2020 2020 202d 2070 686f 6e65 0a20         - phone. 
+000011a0: 2020 2020 2020 2020 202d 2066 6178 0a20           - fax. 
+000011b0: 2020 2020 2020 2020 202d 2065 6d61 696c           - email
+000011c0: 0a20 2020 2020 2063 7265 6174 655f 6461  .      create_da
+000011d0: 7465 3a0a 2020 2020 2020 2020 7479 7065  te:.        type
+000011e0: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+000011f0: 2064 6573 6372 6970 7469 6f6e 3a20 4461   description: Da
+00001200: 7465 2061 6e64 2074 696d 6520 7768 656e  te and time when
+00001210: 2074 6865 2064 6f6d 6169 6e20 7761 7320   the domain was 
+00001220: 6372 6561 7465 640a 2020 2020 2020 2020  created.        
+00001230: 666f 726d 6174 3a20 6461 7465 2d74 696d  format: date-tim
+00001240: 650a 2020 2020 2020 646f 6d61 696e 3a0a  e.      domain:.
+00001250: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
+00001260: 7269 6e67 0a20 2020 2020 2020 2064 6573  ring.        des
+00001270: 6372 6970 7469 6f6e 3a20 446f 6d61 696e  cription: Domain
+00001280: 206e 616d 650a 2020 2020 2020 646f 6d61   name.      doma
+00001290: 696e 5f61 6765 3a0a 2020 2020 2020 2020  in_age:.        
+000012a0: 7479 7065 3a20 696e 7465 6765 720a 2020  type: integer.  
+000012b0: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+000012c0: 6e3a 2041 6765 206f 6620 7468 6520 646f  n: Age of the do
+000012d0: 6d61 696e 2069 6e20 7965 6172 730a 2020  main in years.  
+000012e0: 2020 2020 646f 6d61 696e 5f69 643a 0a20      domain_id:. 
+000012f0: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+00001300: 696e 670a 2020 2020 2020 2020 6465 7363  ing.        desc
+00001310: 7269 7074 696f 6e3a 2055 6e69 7175 6520  ription: Unique 
+00001320: 6964 656e 7469 6669 6572 2066 6f72 2074  identifier for t
+00001330: 6865 2064 6f6d 6169 6e0a 2020 2020 2020  he domain.      
+00001340: 6578 7069 7265 5f64 6174 653a 0a20 2020  expire_date:.   
+00001350: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
+00001360: 670a 2020 2020 2020 2020 6465 7363 7269  g.        descri
+00001370: 7074 696f 6e3a 2044 6174 6520 616e 6420  ption: Date and 
+00001380: 7469 6d65 2077 6865 6e20 7468 6520 646f  time when the do
+00001390: 6d61 696e 2077 696c 6c20 6578 7069 7265  main will expire
+000013a0: 0a20 2020 2020 2020 2066 6f72 6d61 743a  .        format:
+000013b0: 2064 6174 652d 7469 6d65 0a20 2020 2020   date-time.     
+000013c0: 206e 616d 6573 6572 7665 7273 3a0a 2020   nameservers:.  
+000013d0: 2020 2020 2020 7479 7065 3a20 6172 7261        type: arra
+000013e0: 790a 2020 2020 2020 2020 6465 7363 7269  y.        descri
+000013f0: 7074 696f 6e3a 204c 6973 7420 6f66 206e  ption: List of n
+00001400: 616d 6573 6572 7665 7273 2061 7373 6f63  ameservers assoc
+00001410: 6961 7465 6420 7769 7468 2074 6865 2064  iated with the d
+00001420: 6f6d 6169 6e0a 2020 2020 2020 7265 6769  omain.      regi
+00001430: 7374 7261 6e74 3a0a 2020 2020 2020 2020  strant:.        
+00001440: 7479 7065 3a20 6f62 6a65 6374 0a20 2020  type: object.   
+00001450: 2020 2020 2061 6464 6974 696f 6e61 6c50       additionalP
+00001460: 726f 7065 7274 6965 733a 2074 7275 650a  roperties: true.
+00001470: 2020 2020 2020 2020 6465 7363 7269 7074          descript
+00001480: 696f 6e3a 2044 6574 6169 6c73 206f 6620  ion: Details of 
+00001490: 7468 6520 7265 6769 7374 7261 6e74 2063  the registrant c
+000014a0: 6f6e 7461 6374 0a20 2020 2020 2020 2070  ontact.        p
+000014b0: 726f 7065 7274 6965 733a 0a20 2020 2020  roperties:.     
+000014c0: 2020 2020 2063 6974 793a 0a20 2020 2020       city:.     
+000014d0: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+000014e0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+000014f0: 6465 7363 7269 7074 696f 6e3a 2043 6974  description: Cit
+00001500: 7920 6f66 2074 6865 2072 6567 6973 7472  y of the registr
+00001510: 616e 7420 636f 6e74 6163 740a 2020 2020  ant contact.    
+00001520: 2020 2020 2020 636f 756e 7472 793a 0a20        country:. 
+00001530: 2020 2020 2020 2020 2020 2074 7970 653a             type:
+00001540: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00001550: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00001560: 2043 6f75 6e74 7279 206f 6620 7468 6520   Country of the 
+00001570: 7265 6769 7374 7261 6e74 2063 6f6e 7461  registrant conta
+00001580: 6374 0a20 2020 2020 2020 2020 2065 6d61  ct.          ema
+00001590: 696c 3a0a 2020 2020 2020 2020 2020 2020  il:.            
+000015a0: 7479 7065 3a20 7374 7269 6e67 0a20 2020  type: string.   
+000015b0: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
+000015c0: 7469 6f6e 3a20 456d 6169 6c20 6f66 2074  tion: Email of t
+000015d0: 6865 2072 6567 6973 7472 616e 7420 636f  he registrant co
+000015e0: 6e74 6163 740a 2020 2020 2020 2020 2020  ntact.          
+000015f0: 6661 783a 0a20 2020 2020 2020 2020 2020  fax:.           
+00001600: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
+00001610: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+00001620: 7074 696f 6e3a 2046 6178 206e 756d 6265  ption: Fax numbe
+00001630: 7220 6f66 2074 6865 2072 6567 6973 7472  r of the registr
+00001640: 616e 7420 636f 6e74 6163 740a 2020 2020  ant contact.    
+00001650: 2020 2020 2020 6e61 6d65 3a0a 2020 2020        name:.    
+00001660: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
+00001670: 7269 6e67 0a20 2020 2020 2020 2020 2020  ring.           
+00001680: 2064 6573 6372 6970 7469 6f6e 3a20 4e61   description: Na
+00001690: 6d65 206f 6620 7468 6520 7265 6769 7374  me of the regist
+000016a0: 7261 6e74 2063 6f6e 7461 6374 0a20 2020  rant contact.   
+000016b0: 2020 2020 2020 206f 7267 616e 697a 6174         organizat
+000016c0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
+000016d0: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
+000016e0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
+000016f0: 7074 696f 6e3a 204f 7267 616e 697a 6174  ption: Organizat
+00001700: 696f 6e20 6f66 2074 6865 2072 6567 6973  ion of the regis
+00001710: 7472 616e 7420 636f 6e74 6163 740a 2020  trant contact.  
+00001720: 2020 2020 2020 2020 7068 6f6e 653a 0a20          phone:. 
+00001730: 2020 2020 2020 2020 2020 2074 7970 653a             type:
+00001740: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00001750: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00001760: 2050 686f 6e65 206e 756d 6265 7220 6f66   Phone number of
+00001770: 2074 6865 2072 6567 6973 7472 616e 7420   the registrant 
+00001780: 636f 6e74 6163 740a 2020 2020 2020 2020  contact.        
+00001790: 2020 7265 6769 6f6e 3a0a 2020 2020 2020    region:.      
+000017a0: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+000017b0: 6e67 0a20 2020 2020 2020 2020 2020 2064  ng.            d
+000017c0: 6573 6372 6970 7469 6f6e 3a20 5265 6769  escription: Regi
+000017d0: 6f6e 206f 6620 7468 6520 7265 6769 7374  on of the regist
+000017e0: 7261 6e74 2063 6f6e 7461 6374 0a20 2020  rant contact.   
+000017f0: 2020 2020 2020 2073 7472 6565 745f 6164         street_ad
+00001800: 6472 6573 733a 0a20 2020 2020 2020 2020  dress:.         
+00001810: 2020 2074 7970 653a 2073 7472 696e 670a     type: string.
+00001820: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+00001830: 7269 7074 696f 6e3a 2053 7472 6565 7420  ription: Street 
+00001840: 6164 6472 6573 7320 6f66 2074 6865 2072  address of the r
+00001850: 6567 6973 7472 616e 7420 636f 6e74 6163  egistrant contac
+00001860: 740a 2020 2020 2020 2020 2020 7a69 705f  t.          zip_
+00001870: 636f 6465 3a0a 2020 2020 2020 2020 2020  code:.          
+00001880: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
+00001890: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+000018a0: 6970 7469 6f6e 3a20 5a69 7020 636f 6465  iption: Zip code
+000018b0: 206f 6620 7468 6520 7265 6769 7374 7261   of the registra
+000018c0: 6e74 2063 6f6e 7461 6374 0a20 2020 2020  nt contact.     
+000018d0: 2020 2072 6571 7569 7265 643a 0a20 2020     required:.   
+000018e0: 2020 2020 2020 202d 206e 616d 650a 2020         - name.  
+000018f0: 2020 2020 2020 2020 2d20 6f72 6761 6e69          - organi
+00001900: 7a61 7469 6f6e 0a20 2020 2020 2020 2020  zation.         
+00001910: 202d 2073 7472 6565 745f 6164 6472 6573   - street_addres
+00001920: 730a 2020 2020 2020 2020 2020 2d20 6369  s.          - ci
+00001930: 7479 0a20 2020 2020 2020 2020 202d 2072  ty.          - r
+00001940: 6567 696f 6e0a 2020 2020 2020 2020 2020  egion.          
+00001950: 2d20 7a69 705f 636f 6465 0a20 2020 2020  - zip_code.     
+00001960: 2020 2020 202d 2063 6f75 6e74 7279 0a20       - country. 
+00001970: 2020 2020 2020 2020 202d 2070 686f 6e65           - phone
+00001980: 0a20 2020 2020 2020 2020 202d 2066 6178  .          - fax
+00001990: 0a20 2020 2020 2020 2020 202d 2065 6d61  .          - ema
+000019a0: 696c 0a20 2020 2020 2072 6567 6973 7472  il.      registr
+000019b0: 6172 3a0a 2020 2020 2020 2020 7479 7065  ar:.        type
+000019c0: 3a20 6f62 6a65 6374 0a20 2020 2020 2020  : object.       
+000019d0: 2061 6464 6974 696f 6e61 6c50 726f 7065   additionalPrope
+000019e0: 7274 6965 733a 2074 7275 650a 2020 2020  rties: true.    
+000019f0: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00001a00: 2044 6574 6169 6c73 206f 6620 7468 6520   Details of the 
+00001a10: 7265 6769 7374 7261 7220 666f 7220 7468  registrar for th
+00001a20: 6520 646f 6d61 696e 0a20 2020 2020 2020  e domain.       
+00001a30: 2070 726f 7065 7274 6965 733a 0a20 2020   properties:.   
+00001a40: 2020 2020 2020 2069 616e 615f 6964 3a0a         iana_id:.
+00001a50: 2020 2020 2020 2020 2020 2020 7479 7065              type
+00001a60: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+00001a70: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00001a80: 3a20 4941 4e41 2049 4420 6f66 2074 6865  : IANA ID of the
+00001a90: 2072 6567 6973 7472 6172 0a20 2020 2020   registrar.     
+00001aa0: 2020 2020 206e 616d 653a 0a20 2020 2020       name:.     
+00001ab0: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+00001ac0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00001ad0: 6465 7363 7269 7074 696f 6e3a 204e 616d  description: Nam
+00001ae0: 6520 6f66 2074 6865 2072 6567 6973 7472  e of the registr
+00001af0: 6172 0a20 2020 2020 2020 2020 2075 726c  ar.          url
+00001b00: 3a0a 2020 2020 2020 2020 2020 2020 7479  :.            ty
+00001b10: 7065 3a20 7374 7269 6e67 0a20 2020 2020  pe: string.     
+00001b20: 2020 2020 2020 2064 6573 6372 6970 7469         descripti
+00001b30: 6f6e 3a20 5552 4c20 6f66 2074 6865 2072  on: URL of the r
+00001b40: 6567 6973 7472 6172 0a20 2020 2020 2020  egistrar.       
+00001b50: 2072 6571 7569 7265 643a 0a20 2020 2020   required:.     
+00001b60: 2020 2020 202d 2069 616e 615f 6964 0a20       - iana_id. 
+00001b70: 2020 2020 2020 2020 202d 206e 616d 650a           - name.
+00001b80: 2020 2020 2020 2020 2020 2d20 7572 6c0a            - url.
+00001b90: 2020 2020 2020 7374 6174 7573 3a0a 2020        status:.  
+00001ba0: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+00001bb0: 6e67 0a20 2020 2020 2020 2064 6573 6372  ng.        descr
+00001bc0: 6970 7469 6f6e 3a20 5374 6174 7573 206f  iption: Status o
+00001bd0: 6620 7468 6520 646f 6d61 696e 2072 6567  f the domain reg
+00001be0: 6973 7472 6174 696f 6e0a 2020 2020 2020  istration.      
+00001bf0: 7465 6368 3a0a 2020 2020 2020 2020 7479  tech:.        ty
+00001c00: 7065 3a20 6f62 6a65 6374 0a20 2020 2020  pe: object.     
+00001c10: 2020 2061 6464 6974 696f 6e61 6c50 726f     additionalPro
+00001c20: 7065 7274 6965 733a 2074 7275 650a 2020  perties: true.  
+00001c30: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00001c40: 6e3a 2044 6574 6169 6c73 206f 6620 7468  n: Details of th
+00001c50: 6520 7465 6368 6e69 6361 6c20 636f 6e74  e technical cont
+00001c60: 6163 740a 2020 2020 2020 2020 7072 6f70  act.        prop
+00001c70: 6572 7469 6573 3a0a 2020 2020 2020 2020  erties:.        
+00001c80: 2020 6369 7479 3a0a 2020 2020 2020 2020    city:.        
+00001c90: 2020 2020 7479 7065 3a20 7374 7269 6e67      type: string
+00001ca0: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
+00001cb0: 6372 6970 7469 6f6e 3a20 4369 7479 206f  cription: City o
+00001cc0: 6620 7468 6520 7465 6368 6e69 6361 6c20  f the technical 
+00001cd0: 636f 6e74 6163 740a 2020 2020 2020 2020  contact.        
+00001ce0: 2020 636f 756e 7472 793a 0a20 2020 2020    country:.     
+00001cf0: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
+00001d00: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
+00001d10: 6465 7363 7269 7074 696f 6e3a 2043 6f75  description: Cou
+00001d20: 6e74 7279 206f 6620 7468 6520 7465 6368  ntry of the tech
+00001d30: 6e69 6361 6c20 636f 6e74 6163 740a 2020  nical contact.  
+00001d40: 2020 2020 2020 2020 656d 6169 6c3a 0a20          email:. 
+00001d50: 2020 2020 2020 2020 2020 2074 7970 653a             type:
+00001d60: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00001d70: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00001d80: 2045 6d61 696c 206f 6620 7468 6520 7465   Email of the te
+00001d90: 6368 6e69 6361 6c20 636f 6e74 6163 740a  chnical contact.
+00001da0: 2020 2020 2020 2020 2020 6661 783a 0a20            fax:. 
+00001db0: 2020 2020 2020 2020 2020 2074 7970 653a             type:
+00001dc0: 2073 7472 696e 670a 2020 2020 2020 2020   string.        
+00001dd0: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00001de0: 2046 6178 206e 756d 6265 7220 6f66 2074   Fax number of t
+00001df0: 6865 2074 6563 686e 6963 616c 2063 6f6e  he technical con
+00001e00: 7461 6374 0a20 2020 2020 2020 2020 206e  tact.          n
+00001e10: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
+00001e20: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
 00001e30: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00001e40: 7074 696f 6e3a 2052 6567 696f 6e20 6f66  ption: Region of
-00001e50: 2074 6865 2062 696c 6c69 6e67 2063 6f6e   the billing con
-00001e60: 7461 6374 0a20 2020 2020 2020 2020 2020  tact.           
-00001e70: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-00001e80: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-00001e90: 7a69 705f 636f 6465 3a0a 2020 2020 2020  zip_code:.      
-00001ea0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00001eb0: 7074 696f 6e3a 205a 6970 2063 6f64 6520  ption: Zip code 
-00001ec0: 6f66 2074 6865 2062 696c 6c69 6e67 2063  of the billing c
-00001ed0: 6f6e 7461 6374 0a20 2020 2020 2020 2020  ontact.         
-00001ee0: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-00001ef0: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00001f00: 2020 636f 756e 7472 793a 0a20 2020 2020    country:.     
-00001f10: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-00001f20: 6970 7469 6f6e 3a20 436f 756e 7472 7920  iption: Country 
-00001f30: 6f66 2074 6865 2062 696c 6c69 6e67 2063  of the billing c
-00001f40: 6f6e 7461 6374 0a20 2020 2020 2020 2020  ontact.         
-00001f50: 2020 2020 2020 2074 7970 653a 2073 7472         type: str
-00001f60: 696e 670a 2020 2020 2020 2020 2020 2020  ing.            
-00001f70: 2020 7068 6f6e 653a 0a20 2020 2020 2020    phone:.       
-00001f80: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00001f90: 7469 6f6e 3a20 5068 6f6e 6520 6e75 6d62  tion: Phone numb
-00001fa0: 6572 206f 6620 7468 6520 6269 6c6c 696e  er of the billin
-00001fb0: 6720 636f 6e74 6163 740a 2020 2020 2020  g contact.      
-00001fc0: 2020 2020 2020 2020 2020 7479 7065 3a20            type: 
-00001fd0: 7374 7269 6e67 0a20 2020 2020 2020 2020  string.         
-00001fe0: 2020 2020 2066 6178 3a0a 2020 2020 2020       fax:.      
-00001ff0: 2020 2020 2020 2020 2020 6465 7363 7269            descri
-00002000: 7074 696f 6e3a 2046 6178 206e 756d 6265  ption: Fax numbe
-00002010: 7220 6f66 2074 6865 2062 696c 6c69 6e67  r of the billing
-00002020: 2063 6f6e 7461 6374 0a20 2020 2020 2020   contact.       
-00002030: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
-00002040: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
-00002050: 2020 2020 656d 6169 6c3a 0a20 2020 2020      email:.     
-00002060: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-00002070: 6970 7469 6f6e 3a20 456d 6169 6c20 6f66  iption: Email of
-00002080: 2074 6865 2062 696c 6c69 6e67 2063 6f6e   the billing con
-00002090: 7461 6374 0a20 2020 2020 2020 2020 2020  tact.           
-000020a0: 2020 2020 2074 7970 653a 2073 7472 696e       type: strin
-000020b0: 670a 2020 2020 2020 2020 2020 2020 7265  g.            re
-000020c0: 7175 6972 6564 3a0a 2020 2020 2020 2020  quired:.        
-000020d0: 2020 2020 2020 2d20 6e61 6d65 0a20 2020        - name.   
-000020e0: 2020 2020 2020 2020 2020 202d 206f 7267             - org
-000020f0: 616e 697a 6174 696f 6e0a 2020 2020 2020  anization.      
-00002100: 2020 2020 2020 2020 2d20 7374 7265 6574          - street
-00002110: 5f61 6464 7265 7373 0a20 2020 2020 2020  _address.       
-00002120: 2020 2020 2020 202d 2063 6974 790a 2020         - city.  
-00002130: 2020 2020 2020 2020 2020 2020 2d20 7265              - re
-00002140: 6769 6f6e 0a20 2020 2020 2020 2020 2020  gion.           
-00002150: 2020 202d 207a 6970 5f63 6f64 650a 2020     - zip_code.  
-00002160: 2020 2020 2020 2020 2020 2020 2d20 636f              - co
-00002170: 756e 7472 790a 2020 2020 2020 2020 2020  untry.          
-00002180: 2020 2020 2d20 7068 6f6e 650a 2020 2020      - phone.    
-00002190: 2020 2020 2020 2020 2020 2d20 6661 780a            - fax.
-000021a0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-000021b0: 656d 6169 6c0a 2020 2020 2020 2020 2020  email.          
-000021c0: 2020 6164 6469 7469 6f6e 616c 5072 6f70    additionalProp
-000021d0: 6572 7469 6573 3a20 7472 7565 0a20 2020  erties: true.   
-000021e0: 2020 2020 2020 206e 616d 6573 6572 7665         nameserve
-000021f0: 7273 3a0a 2020 2020 2020 2020 2020 2020  rs:.            
-00002200: 6465 7363 7269 7074 696f 6e3a 204c 6973  description: Lis
-00002210: 7420 6f66 206e 616d 6573 6572 7665 7273  t of nameservers
-00002220: 2061 7373 6f63 6961 7465 6420 7769 7468   associated with
-00002230: 2074 6865 2064 6f6d 6169 6e0a 2020 2020   the domain.    
-00002240: 2020 2020 2020 2020 7479 7065 3a20 6172          type: ar
-00002250: 7261 790a 2020 2020 2020 2020 7265 7175  ray.        requ
-00002260: 6972 6564 3a0a 2020 2020 2020 2020 2020  ired:.          
-00002270: 2d20 646f 6d61 696e 0a20 2020 2020 2020  - domain.       
+00001e40: 7074 696f 6e3a 204e 616d 6520 6f66 2074  ption: Name of t
+00001e50: 6865 2074 6563 686e 6963 616c 2063 6f6e  he technical con
+00001e60: 7461 6374 0a20 2020 2020 2020 2020 206f  tact.          o
+00001e70: 7267 616e 697a 6174 696f 6e3a 0a20 2020  rganization:.   
+00001e80: 2020 2020 2020 2020 2074 7970 653a 2073           type: s
+00001e90: 7472 696e 670a 2020 2020 2020 2020 2020  tring.          
+00001ea0: 2020 6465 7363 7269 7074 696f 6e3a 204f    description: O
+00001eb0: 7267 616e 697a 6174 696f 6e20 6f66 2074  rganization of t
+00001ec0: 6865 2074 6563 686e 6963 616c 2063 6f6e  he technical con
+00001ed0: 7461 6374 0a20 2020 2020 2020 2020 2070  tact.          p
+00001ee0: 686f 6e65 3a0a 2020 2020 2020 2020 2020  hone:.          
+00001ef0: 2020 7479 7065 3a20 7374 7269 6e67 0a20    type: string. 
+00001f00: 2020 2020 2020 2020 2020 2064 6573 6372             descr
+00001f10: 6970 7469 6f6e 3a20 5068 6f6e 6520 6e75  iption: Phone nu
+00001f20: 6d62 6572 206f 6620 7468 6520 7465 6368  mber of the tech
+00001f30: 6e69 6361 6c20 636f 6e74 6163 740a 2020  nical contact.  
+00001f40: 2020 2020 2020 2020 7265 6769 6f6e 3a0a          region:.
+00001f50: 2020 2020 2020 2020 2020 2020 7479 7065              type
+00001f60: 3a20 7374 7269 6e67 0a20 2020 2020 2020  : string.       
+00001f70: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00001f80: 3a20 5265 6769 6f6e 206f 6620 7468 6520  : Region of the 
+00001f90: 7465 6368 6e69 6361 6c20 636f 6e74 6163  technical contac
+00001fa0: 740a 2020 2020 2020 2020 2020 7374 7265  t.          stre
+00001fb0: 6574 5f61 6464 7265 7373 3a0a 2020 2020  et_address:.    
+00001fc0: 2020 2020 2020 2020 7479 7065 3a20 7374          type: st
+00001fd0: 7269 6e67 0a20 2020 2020 2020 2020 2020  ring.           
+00001fe0: 2064 6573 6372 6970 7469 6f6e 3a20 5374   description: St
+00001ff0: 7265 6574 2061 6464 7265 7373 206f 6620  reet address of 
+00002000: 7468 6520 7465 6368 6e69 6361 6c20 636f  the technical co
+00002010: 6e74 6163 740a 2020 2020 2020 2020 2020  ntact.          
+00002020: 7a69 705f 636f 6465 3a0a 2020 2020 2020  zip_code:.      
+00002030: 2020 2020 2020 7479 7065 3a20 7374 7269        type: stri
+00002040: 6e67 0a20 2020 2020 2020 2020 2020 2064  ng.            d
+00002050: 6573 6372 6970 7469 6f6e 3a20 5a69 7020  escription: Zip 
+00002060: 636f 6465 206f 6620 7468 6520 7465 6368  code of the tech
+00002070: 6e69 6361 6c20 636f 6e74 6163 740a 2020  nical contact.  
+00002080: 2020 2020 2020 7265 7175 6972 6564 3a0a        required:.
+00002090: 2020 2020 2020 2020 2020 2d20 6e61 6d65            - name
+000020a0: 0a20 2020 2020 2020 2020 202d 206f 7267  .          - org
+000020b0: 616e 697a 6174 696f 6e0a 2020 2020 2020  anization.      
+000020c0: 2020 2020 2d20 7374 7265 6574 5f61 6464      - street_add
+000020d0: 7265 7373 0a20 2020 2020 2020 2020 202d  ress.          -
+000020e0: 2063 6974 790a 2020 2020 2020 2020 2020   city.          
+000020f0: 2d20 7265 6769 6f6e 0a20 2020 2020 2020  - region.       
+00002100: 2020 202d 207a 6970 5f63 6f64 650a 2020     - zip_code.  
+00002110: 2020 2020 2020 2020 2d20 636f 756e 7472          - countr
+00002120: 790a 2020 2020 2020 2020 2020 2d20 7068  y.          - ph
+00002130: 6f6e 650a 2020 2020 2020 2020 2020 2d20  one.          - 
+00002140: 6661 780a 2020 2020 2020 2020 2020 2d20  fax.          - 
+00002150: 656d 6169 6c0a 2020 2020 2020 7570 6461  email.      upda
+00002160: 7465 5f64 6174 653a 0a20 2020 2020 2020  te_date:.       
+00002170: 2074 7970 653a 2073 7472 696e 670a 2020   type: string.  
+00002180: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
+00002190: 6e3a 2044 6174 6520 616e 6420 7469 6d65  n: Date and time
+000021a0: 2077 6865 6e20 7468 6520 646f 6d61 696e   when the domain
+000021b0: 2072 6563 6f72 6420 7761 7320 6c61 7374   record was last
+000021c0: 2075 7064 6174 6564 0a20 2020 2020 2020   updated.       
+000021d0: 2066 6f72 6d61 743a 2064 6174 652d 7469   format: date-ti
+000021e0: 6d65 0a20 2020 2020 2077 686f 6973 5f73  me.      whois_s
+000021f0: 6572 7665 723a 0a20 2020 2020 2020 2074  erver:.        t
+00002200: 7970 653a 2073 7472 696e 670a 2020 2020  ype: string.    
+00002210: 2020 2020 6465 7363 7269 7074 696f 6e3a      description:
+00002220: 2057 686f 6973 2073 6572 7665 7220 7573   Whois server us
+00002230: 6564 2074 6f20 7175 6572 7920 7468 6520  ed to query the 
+00002240: 646f 6d61 696e 2072 6567 6973 7472 6174  domain registrat
+00002250: 696f 6e20 696e 666f 726d 6174 696f 6e0a  ion information.
+00002260: 2020 2020 7265 7175 6972 6564 3a0a 2020      required:.  
+00002270: 2020 2020 2d20 646f 6d61 696e 0a20 2020      - domain.   
 00002280: 2020 202d 2064 6f6d 6169 6e5f 6964 0a20     - domain_id. 
-00002290: 2020 2020 2020 2020 202d 2073 7461 7475           - statu
-000022a0: 730a 2020 2020 2020 2020 2020 2d20 6372  s.          - cr
-000022b0: 6561 7465 5f64 6174 650a 2020 2020 2020  eate_date.      
-000022c0: 2020 2020 2d20 7570 6461 7465 5f64 6174      - update_dat
-000022d0: 650a 2020 2020 2020 2020 2020 2d20 6578  e.          - ex
-000022e0: 7069 7265 5f64 6174 650a 2020 2020 2020  pire_date.      
-000022f0: 2020 2020 2d20 646f 6d61 696e 5f61 6765      - domain_age
-00002300: 0a20 2020 2020 2020 2020 202d 2077 686f  .          - who
-00002310: 6973 5f73 6572 7665 720a 2020 2020 2020  is_server.      
-00002320: 2020 2020 2d20 7265 6769 7374 7261 720a      - registrar.
-00002330: 2020 2020 2020 2020 2020 2d20 7265 6769            - regi
-00002340: 7374 7261 6e74 0a20 2020 2020 2020 2020  strant.         
-00002350: 202d 2061 646d 696e 0a20 2020 2020 2020   - admin.       
-00002360: 2020 202d 2074 6563 680a 2020 2020 2020     - tech.      
-00002370: 2020 2020 2d20 6269 6c6c 696e 670a 2020      - billing.  
-00002380: 2020 2020 2020 2020 2d20 6e61 6d65 7365          - namese
-00002390: 7276 6572 730a 2020 2020 2020 2020 6164  rvers.        ad
-000023a0: 6469 7469 6f6e 616c 5072 6f70 6572 7469  ditionalProperti
-000023b0: 6573 3a20 7472 7565 0a73 7472 6561 6d73  es: true.streams
-000023c0: 3a0a 2020 2d20 2223 2f64 6566 696e 6974  :.  - "#/definit
-000023d0: 696f 6e73 2f77 686f 6973 5f73 7472 6561  ions/whois_strea
-000023e0: 6d22 0a63 6865 636b 3a0a 2020 7374 7265  m".check:.  stre
-000023f0: 616d 5f6e 616d 6573 3a0a 2020 2020 2d20  am_names:.    - 
-00002400: 2277 686f 6973 220a                      "whois".
+00002290: 2020 2020 202d 2073 7461 7475 730a 2020       - status.  
+000022a0: 2020 2020 2d20 6372 6561 7465 5f64 6174      - create_dat
+000022b0: 650a 2020 2020 2020 2d20 7570 6461 7465  e.      - update
+000022c0: 5f64 6174 650a 2020 2020 2020 2d20 6578  _date.      - ex
+000022d0: 7069 7265 5f64 6174 650a 2020 2020 2020  pire_date.      
+000022e0: 2d20 646f 6d61 696e 5f61 6765 0a20 2020  - domain_age.   
+000022f0: 2020 202d 2077 686f 6973 5f73 6572 7665     - whois_serve
+00002300: 720a 2020 2020 2020 2d20 7265 6769 7374  r.      - regist
+00002310: 7261 720a 2020 2020 2020 2d20 7265 6769  rar.      - regi
+00002320: 7374 7261 6e74 0a20 2020 2020 202d 2061  strant.      - a
+00002330: 646d 696e 0a20 2020 2020 202d 2074 6563  dmin.      - tec
+00002340: 680a 2020 2020 2020 2d20 6269 6c6c 696e  h.      - billin
+00002350: 670a 2020 2020 2020 2d20 6e61 6d65 7365  g.      - namese
+00002360: 7276 6572 730a                           rvers.
```

### Comparing `airbyte_source_ip2whois-0.1.3/PKG-INFO` & `airbyte_source_ip2whois-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-ip2whois
-Version: 0.1.3
+Version: 0.1.4
 Summary: Source implementation for Ip2whois.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -15,96 +15,110 @@
 Requires-Dist: airbyte-cdk (==0.80.0)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/ip2whois
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Ip2Whois source connector
 
-
 This is the repository for the Ip2Whois source connector, written in Python.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/ip2whois).
 
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
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/ip2whois)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_ip2whois/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `sample_files/sample_config.json` for a sample config file.
 
-
 ### Locally running the connector
+
 ```
 poetry run source-ip2whois spec
 poetry run source-ip2whois check --config secrets/config.json
 poetry run source-ip2whois discover --config secrets/config.json
 poetry run source-ip2whois read --config secrets/config.json --catalog sample_files/configured_catalog.json
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
 airbyte-ci connectors --name=source-ip2whois build
 ```
 
 An image will be available on your host with the tag `airbyte/source-ip2whois:dev`.
 
-
 ### Running as a docker container
+
 Then run any of the connector commands as follows:
+
 ```
 docker run --rm airbyte/source-ip2whois:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-ip2whois:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-ip2whois:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-ip2whois:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
 ### Running our CI test suite
+
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
+
 ```bash
 airbyte-ci connectors --name=source-ip2whois test
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
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-ip2whois test`
-2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)): 
-    - bump the `dockerImageTag` value in in `metadata.yaml`
-    - bump the `version` value in `pyproject.toml`
+2. Bump the connector version (please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors)):
+   - bump the `dockerImageTag` value in in `metadata.yaml`
+   - bump the `version` value in `pyproject.toml`
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make sure the connector documentation and its changelog is up to date (`docs/integrations/sources/ip2whois.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 8. Once your PR is merged, the new version of the connector will be automatically published to Docker Hub and our connector registry.
+
```

