# Comparing `tmp/sdk_entrepot_gpf-0.1.26.tar.gz` & `tmp/sdk_entrepot_gpf-0.1.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdk_entrepot_gpf-0.1.26.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "sdk_entrepot_gpf-0.1.27.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `sdk_entrepot_gpf-0.1.26.tar` & `sdk_entrepot_gpf-0.1.27.tar`

### file list

```diff
@@ -1,267 +1,267 @@
--rw-r--r--   0        0        0      350 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/PULL_REQUEST_TEMPLATE/bug.md
--rw-r--r--   0        0        0      361 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/PULL_REQUEST_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      429 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/PULL_REQUEST_TEMPLATE/enhancement.md
--rw-r--r--   0        0        0      307 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/PULL_REQUEST_TEMPLATE/other.md
--rw-r--r--   0        0        0      370 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/PULL_REQUEST_TEMPLATE/quality.md
--rw-r--r--   0        0        0      383 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/PULL_REQUEST_TEMPLATE/tooling.md
--rw-r--r--   0        0        0      176 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/labeler.yml
--rw-r--r--   0        0        0      506 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/release.yml
--rw-r--r--   0        0        0     1412 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/workflows/ci-dev.yml
--rw-r--r--   0        0        0     1406 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/workflows/ci-prod.yml
--rw-r--r--   0        0        0      856 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.github/workflows/code-quality.yml
--rw-r--r--   0        0        0     1961 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.gitignore
--rw-r--r--   0        0        0    23461 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.pylintrc
--rw-r--r--   0        0        0      200 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.pypirc
--rw-r--r--   0        0        0     2299 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/.vscode/settings.json
--rw-r--r--   0        0        0     6826 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/LICENSE
--rw-r--r--   0        0        0      134 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/MANIFEST.in
--rw-r--r--   0        0        0      533 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/README.md
--rwxr-xr-x   0        0        0      691 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/check.sh
--rw-r--r--   0        0        0        5 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docker/.gitignore
--rw-r--r--   0        0        0     1968 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docker/Dockerfile
--rw-r--r--   0        0        0      808 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docker/README.md
--rw-r--r--   0        0        0      248 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docker/config/apache/website.conf
--rw-r--r--   0        0        0      291 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docker/docker-compose.yml
--rw-r--r--   0        0        0       46 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docs/.gitignore
--rw-r--r--   0        0        0      394 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docs/assets/css/custom.css
--rw-r--r--   0        0        0      748 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docs/assets/css/extra.css
--rw-r--r--   0        0        0    39005 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docs/assets/css/neoteroi.css
--rw-r--r--   0        0        0     1150 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docs/assets/images/favicon.ico
--rw-r--r--   0        0        0    12622 2024-04-18 15:00:20.681823 sdk_entrepot_gpf-0.1.26/docs/assets/images/index__utilisation_module.excalidraw
--rw-r--r--   0        0        0   193450 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/assets/images/index__utilisation_module.png
--rw-r--r--   0        0        0    15848 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/assets/images/logo.png
--rw-r--r--   0        0        0     4429 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/comme-executable.md
--rw-r--r--   0        0        0     4960 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/comme-module.md
--rw-r--r--   0        0        0     6776 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/configuration.md
--rw-r--r--   0        0        0    29083 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/configuration_details.md
--rw-r--r--   0        0        0     6052 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/development.md
--rw-r--r--   0        0        0     1327 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/index.md
--rw-r--r--   0        0        0      131 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/reference/auth.md
--rw-r--r--   0        0        0      336 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/reference/io.md
--rw-r--r--   0        0        0      338 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/reference/store.md
--rw-r--r--   0        0        0       68 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/reference/workflow.md
--rw-r--r--   0        0        0      314 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/reference/workflow/action.md
--rw-r--r--   0        0        0      368 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/reference/workflow/resolver.md
--rw-r--r--   0        0        0    11758 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/resolveurs.md
--rw-r--r--   0        0        0     5557 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/tutoriel_1_archive.md
--rw-r--r--   0        0        0     6731 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/tutoriel_2_flux_vecteur.md
--rw-r--r--   0        0        0     5137 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/tutoriel_3_flux_raster.md
--rw-r--r--   0        0        0     4161 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/upload_descriptor.md
--rw-r--r--   0        0        0    22205 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/docs/workflow.md
--rw-r--r--   0        0        0     2201 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/mkdocs.yml
--rw-r--r--   0        0        0      114 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/mypy.ini
--rw-r--r--   0        0        0     1371 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/pyproject.toml
--rw-r--r--   0        0        0      689 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/Errors.py
--rw-r--r--   0        0        0       93 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/__init__.py
--rw-r--r--   0        0        0    48883 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/__main__.py
--rw-r--r--   0        0        0    11504 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/default.ini
--rw-r--r--   0        0        0     1202 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/annexe_descriptor_file.json
--rw-r--r--   0        0        0      870 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/metadata_descriptor_file.json
--rw-r--r--   0        0        0     1226 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/static_descriptor_file.json
--rw-r--r--   0        0        0     1968 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/upload_descriptor_file.json
--rw-r--r--   0        0        0     6924 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/workflow.json
--rw-r--r--   0        0        0      255 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON.md5
--rwxr-xr-x   0        0        0        5 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2297 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf
--rwxr-xr-x   0        0        0      655 2024-04-18 15:00:20.685823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.prj
--rw-r--r--   0        0        0   430828 2024-04-18 15:00:20.689823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shp
--rw-r--r--   0        0        0      588 2024-04-18 15:00:20.689823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shx
--rw-r--r--   0        0        0     4003 2024-04-18 15:00:20.689823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON_style.sld
--rw-r--r--   0        0        0      529 2024-04-18 15:00:20.689823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/upload_descriptor.json
--rw-r--r--   0        0        0       52 2024-04-18 15:00:20.689823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON.md5
--rw-r--r--   0        0        0   991843 2024-04-18 15:00:20.693823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON/CANTON.zip
--rw-r--r--   0        0        0      525 2024-04-18 15:00:20.693823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/upload_descriptor.json
--rw-r--r--   0        0        0     4391 2024-04-18 15:00:20.693823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/installation.sld
--rw-r--r--   0        0        0      411 2024-04-18 15:00:20.693823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_1/installation-init.sql
--rw-r--r--   0        0        0   368640 2024-04-18 15:00:20.693823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_2/installation.gpkg
--rw-r--r--   0        0        0   676357 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csv
--rw-r--r--   0        0        0       84 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csvt
--rw-r--r--   0        0        0     1731 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/upload_descriptor.json
--rw-r--r--   0        0        0     5019 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_archive.jsonc
--rw-r--r--   0        0        0    15492 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_joincache.jsonc
--rw-r--r--   0        0        0     9884 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_maj_bdd.jsonc
--rw-r--r--   0        0        0    11561 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_moissonnage.jsonc
--rw-r--r--   0        0        0     9209 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_raster.jsonc
--rw-r--r--   0        0        0    15240 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_vecteur.jsonc
--rw-r--r--   0        0        0     8333 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/auth/Authentifier.py
--rw-r--r--   0        0        0      274 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/auth/Errors.py
--rw-r--r--   0        0        0     1493 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/auth/Token.py
--rw-r--r--   0        0        0       46 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/auth/__init__.py
--rw-r--r--   0        0        0     2589 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/FileHelper.py
--rw-r--r--   0        0        0     6939 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/JsonHelper.py
--rw-r--r--   0        0        0      916 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/PrintLogHelper.py
--rw-r--r--   0        0        0       59 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/__init__.py
--rw-r--r--   0        0        0    16028 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/ApiRequester.py
--rw-r--r--   0        0        0      607 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Color.py
--rw-r--r--   0        0        0     5695 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Config.py
--rw-r--r--   0        0        0     5318 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Dataset.py
--rw-r--r--   0        0        0     4143 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/DescriptorFileReader.py
--rw-r--r--   0        0        0     6878 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Errors.py
--rw-r--r--   0        0        0     2909 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/JsonConverter.py
--rw-r--r--   0        0        0     4416 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/OutputManager.py
--rw-r--r--   0        0        0     4075 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/UploadDescriptorFileReader.py
--rw-r--r--   0        0        0       47 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/__init__.py
--rw-r--r--   0        0        0      793 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/pattern/SingleInstance.py
--rw-r--r--   0        0        0      637 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/pattern/Singleton.py
--rw-r--r--   0        0        0       33 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/pattern/__init__.py
--rw-r--r--   0        0        0        1 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/py.typed
--rw-r--r--   0        0        0     1209 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/AbstractCommonFile.py
--rw-r--r--   0        0        0     2486 2024-04-18 15:00:20.697823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Annexe.py
--rw-r--r--   0        0        0      222 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Check.py
--rw-r--r--   0        0        0      584 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/CheckExecution.py
--rw-r--r--   0        0        0     4269 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Configuration.py
--rw-r--r--   0        0        0     3400 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Datastore.py
--rw-r--r--   0        0        0     3363 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Endpoint.py
--rw-r--r--   0        0        0      183 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Errors.py
--rw-r--r--   0        0        0     2586 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Metadata.py
--rw-r--r--   0        0        0     2140 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Offering.py
--rw-r--r--   0        0        0      332 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Permission.py
--rw-r--r--   0        0        0      231 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Processing.py
--rw-r--r--   0        0        0     2026 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/ProcessingExecution.py
--rw-r--r--   0        0        0     1005 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Static.py
--rw-r--r--   0        0        0    14998 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/StoreEntity.py
--rw-r--r--   0        0        0     1933 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/StoredData.py
--rw-r--r--   0        0        0      235 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Tms.py
--rw-r--r--   0        0        0     7270 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Upload.py
--rw-r--r--   0        0        0     1010 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/User.py
--rw-r--r--   0        0        0     1432 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/__init__.py
--rw-r--r--   0        0        0     2521 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/CommentInterface.py
--rw-r--r--   0        0        0     2025 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/CreatedByUploadFileInterface.py
--rw-r--r--   0        0        0     1051 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/CsfInterface.py
--rw-r--r--   0        0        0     1102 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/DownloadInterface.py
--rw-r--r--   0        0        0      805 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/EventInterface.py
--rw-r--r--   0        0        0     1262 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/FullEditInterface.py
--rw-r--r--   0        0        0      869 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/LogsInterface.py
--rw-r--r--   0        0        0     1116 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/PartialEditInterface.py
--rw-r--r--   0        0        0      998 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/ReUploadFileInterface.py
--rw-r--r--   0        0        0     2107 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/SharingInterface.py
--rw-r--r--   0        0        0     2329 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/TagInterface.py
--rw-r--r--   0        0        0       88 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/__init__.py
--rw-r--r--   0        0        0      512 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/Errors.py
--rw-r--r--   0        0        0    20884 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/Workflow.py
--rw-r--r--   0        0        0       40 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/__init__.py
--rw-r--r--   0        0        0     5726 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/ActionAbstract.py
--rw-r--r--   0        0        0     7077 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/ConfigurationAction.py
--rw-r--r--   0        0        0     1776 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/CopyConfigurationAction.py
--rw-r--r--   0        0        0     5149 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/DeleteAction.py
--rw-r--r--   0        0        0     3172 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/EditAction.py
--rw-r--r--   0        0        0     2551 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/EditUsedDataConfigurationAction.py
--rw-r--r--   0        0        0     6827 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/OfferingAction.py
--rw-r--r--   0        0        0     2153 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/PermissionAction.py
--rw-r--r--   0        0        0    19885 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/ProcessingExecutionAction.py
--rw-r--r--   0        0        0     7452 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/SynchronizeOfferingAction.py
--rw-r--r--   0        0        0    22943 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/UploadAction.py
--rw-r--r--   0        0        0       72 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/__init__.py
--rw-r--r--   0        0        0     2267 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/AbstractResolver.py
--rw-r--r--   0        0        0     3389 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/DateResolver.py
--rw-r--r--   0        0        0     1933 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/DictResolver.py
--rw-r--r--   0        0        0      708 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/DumbResolver.py
--rw-r--r--   0        0        0     4533 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/Errors.py
--rw-r--r--   0        0        0     6076 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/FileResolver.py
--rw-r--r--   0        0        0     3838 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/GlobalResolver.py
--rw-r--r--   0        0        0     5760 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/StoreEntityResolver.py
--rw-r--r--   0        0        0     1908 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/UserResolver.py
--rw-r--r--   0        0        0      110 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/__init__.py
--rw-r--r--   0        0        0      960 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/ErrorsTestCase.py
--rw-r--r--   0        0        0     1739 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/GpfTestCase.py
--rw-r--r--   0        0        0     3419 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/MainTestCase.py
--rw-r--r--   0        0        0        0 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/__init__.py
--rw-r--r--   0        0        0      369 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_conf/test_authentifier.ini
--rw-r--r--   0        0        0      308 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_conf/test_overload.ini
--rw-r--r--   0        0        0      594 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_conf/test_requester.ini
--rw-r--r--   0        0        0       40 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_conf/test_upload.ini
--rw-r--r--   0        0        0       69 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_conf/test_value_type.ini
--rw-r--r--   0        0        0      460 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/1_test_dataset_bad_pathes/upload_descriptor.json
--rw-r--r--   0        0        0      305 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON.md5
--rw-r--r--   0        0        0        5 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2318 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf
--rw-r--r--   0        0        0      145 2024-04-18 15:00:20.701823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.prj
--rw-r--r--   0        0        0  1279276 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp
--rw-r--r--   0        0        0      572 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx
--rw-r--r--   0        0        0        0 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/sous_dossier/coucou.txt
--rw-r--r--   0        0        0      567 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json
--rw-r--r--   0        0        0       11 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/.gitignore
--rw-r--r--   0        0        0        5 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.cpg
--rw-r--r--   0        0        0     2318 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf
--rw-r--r--   0        0        0      145 2024-04-18 15:00:20.709823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.prj
--rw-r--r--   0        0        0  1279276 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp
--rw-r--r--   0        0        0      572 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx
--rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/sous_dossier/coucou.txt
--rw-r--r--   0        0        0      567 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json
--rw-r--r--   0        0        0     2659 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_data/workflows/bad-workflow.jsonc
--rw-r--r--   0        0        0       53 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/helper/FileHelper/md5.txt
--rw-r--r--   0        0        0       78 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/helper/JsonHelper/json_not_parsable.json
--rw-r--r--   0        0        0       52 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/helper/JsonHelper/json_not_valid.json
--rw-r--r--   0        0        0      108 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/helper/JsonHelper/json_parsable.json
--rw-r--r--   0        0        0      563 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/helper/JsonHelper/schema.json
--rw-r--r--   0        0        0      485 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/helper/JsonHelper/schema_invalid.json
--rw-r--r--   0        0        0       23 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/workflow/resolver/FileResolver/dict.json
--rw-r--r--   0        0        0       21 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/workflow/resolver/FileResolver/list.json
--rw-r--r--   0        0        0        2 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/workflow/resolver/FileResolver/not-valid.json
--rw-r--r--   0        0        0       31 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/_test/workflow/resolver/FileResolver/text.txt
--rw-r--r--   0        0        0     7428 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/auth/AuthentifierTestCase.py
--rw-r--r--   0        0        0     1187 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/auth/TokenTestCase.py
--rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/auth/__init__.py
--rw-r--r--   0        0        0     1060 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/helper/FileHelperTestCase.py
--rw-r--r--   0        0        0     9967 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/helper/JsonHelperTestCase.py
--rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/helper/__init__.py
--rw-r--r--   0        0        0    23350 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/ApiRequesterTestCase.py
--rw-r--r--   0        0        0     3599 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/ConfigTestCase.py
--rw-r--r--   0        0        0     2225 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/DatasetTestCase.py
--rw-r--r--   0        0        0     3197 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/ErrorsTestCase.py
--rw-r--r--   0        0        0     1202 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/JsonConverterTestCase.py
--rw-r--r--   0        0        0     1774 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/UploadDescriptorFileReaderTestCase.py
--rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/io/__init__.py
--rw-r--r--   0        0        0     1122 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/AbstractCommonFileTestCase.py
--rw-r--r--   0        0        0     2587 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/AnnexeTestCase.py
--rw-r--r--   0        0        0     2025 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/CheckExecutionTestCase.py
--rw-r--r--   0        0        0     7221 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/ConfigurationTestCase.py
--rw-r--r--   0        0        0     4849 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/DatastoreTestCase.py
--rw-r--r--   0        0        0     5595 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/EndpointTestCase.py
--rw-r--r--   0        0        0     1152 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/ErrorsTestCase.py
--rw-r--r--   0        0        0     2297 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/MetadataTestCase.py
--rw-r--r--   0        0        0     2687 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/OfferingTestCase.py
--rw-r--r--   0        0        0     4691 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/ProcessingExecutionTestCase.py
--rw-r--r--   0        0        0    26065 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/StoreEntityTestCase.py
--rw-r--r--   0        0        0     3137 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/StoredDataTestCase.py
--rw-r--r--   0        0        0    11003 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/UploadTestCase.py
--rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/__init__.py
--rw-r--r--   0        0        0     5134 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/CommentInterfaceTestCase.py
--rw-r--r--   0        0        0     2790 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/CreatedByUploadFileInterfaceTestCase.py
--rw-r--r--   0        0        0     2536 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/CsfInterfaceTestCase.py
--rw-r--r--   0        0        0     1767 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/DownloadInterfaceTestCase.py
--rw-r--r--   0        0        0     1663 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/EventInterfaceTestCase.py
--rw-r--r--   0        0        0     2326 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/FullEditInterfaceTestCase.py
--rw-r--r--   0        0        0     2243 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/PartialEditInterfaceTestCase.py
--rw-r--r--   0        0        0     1569 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/ReUploadFileInterfaceTestCase.py
--rw-r--r--   0        0        0     4039 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/SharingInterfaceTestCase.py
--rw-r--r--   0        0        0     3899 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/TagInterfaceTestCase.py
--rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/store/interface/__init__.py
--rw-r--r--   0        0        0    28836 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/workflow/WorkflowTestCase.py
--rw-r--r--   0        0        0        0 2024-04-18 15:00:20.717823 sdk_entrepot_gpf-0.1.26/tests/workflow/__init__.py
--rw-r--r--   0        0        0     3595 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/ActionAbstractTestCase.py
--rw-r--r--   0        0        0    10471 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/ConfigurationActionTestCase.py
--rw-r--r--   0        0        0     2502 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/CopyConfigurationActionTestCase.py
--rw-r--r--   0        0        0    12123 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/DeleteActionTestCase.py
--rw-r--r--   0        0        0     5262 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/EditActionTestCase.py
--rw-r--r--   0        0        0     2392 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/EditUsedDataConfigurationActionTestCase.py
--rw-r--r--   0        0        0    16051 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/OfferingActionTestCase.py
--rw-r--r--   0        0        0     1547 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/PermissionActionTestCase.py
--rw-r--r--   0        0        0    24541 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/ProcessingExecutionActionTestCase.py
--rw-r--r--   0        0        0    10675 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/SynchronizeOfferingActionTestCase.py
--rw-r--r--   0        0        0    45012 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/UploadActionTestCase.py
--rw-r--r--   0        0        0        0 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/action/__init__.py
--rw-r--r--   0        0        0     2133 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/AbstractResolverTestCase.py
--rw-r--r--   0        0        0     2401 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/DateResolverTestCase.py
--rw-r--r--   0        0        0     1124 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/DictResolverTestCase.py
--rw-r--r--   0        0        0     5479 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/FileResolverTestCase.py
--rw-r--r--   0        0        0     7361 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/GlobalResolverTestCase.py
--rw-r--r--   0        0        0    15246 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/StoreEntityResolverTestCase.py
--rw-r--r--   0        0        0     2237 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/UserResolverTestCase.py
--rw-r--r--   0        0        0        0 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/__init__.py
--rw-r--r--   0        0        0   116760 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/uml/classes.png
--rw-r--r--   0        0        0     9175 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/uml/classes.uxf
--rw-r--r--   0        0        0    43510 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/uml/interfaces.png
--rw-r--r--   0        0        0     7059 2024-04-18 15:00:20.721823 sdk_entrepot_gpf-0.1.26/uml/interfaces.uxf
--rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 sdk_entrepot_gpf-0.1.26/PKG-INFO
+-rw-r--r--   0        0        0      350 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.github/PULL_REQUEST_TEMPLATE/bug.md
+-rw-r--r--   0        0        0      361 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.github/PULL_REQUEST_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      429 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.github/PULL_REQUEST_TEMPLATE/enhancement.md
+-rw-r--r--   0        0        0      307 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.github/PULL_REQUEST_TEMPLATE/other.md
+-rw-r--r--   0        0        0      370 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.github/PULL_REQUEST_TEMPLATE/quality.md
+-rw-r--r--   0        0        0      383 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.github/PULL_REQUEST_TEMPLATE/tooling.md
+-rw-r--r--   0        0        0      176 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.github/labeler.yml
+-rw-r--r--   0        0        0      506 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.github/release.yml
+-rw-r--r--   0        0        0     1412 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.github/workflows/ci-dev.yml
+-rw-r--r--   0        0        0     1406 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.github/workflows/ci-prod.yml
+-rw-r--r--   0        0        0      856 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.github/workflows/code-quality.yml
+-rw-r--r--   0        0        0     1961 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.gitignore
+-rw-r--r--   0        0        0    23461 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.pylintrc
+-rw-r--r--   0        0        0      200 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.pypirc
+-rw-r--r--   0        0        0     2415 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/.vscode/settings.json
+-rw-r--r--   0        0        0     7547 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/LICENSE
+-rw-r--r--   0        0        0      134 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/MANIFEST.in
+-rw-r--r--   0        0        0      533 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/README.md
+-rwxr-xr-x   0        0        0      691 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/check.sh
+-rw-r--r--   0        0        0        5 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/docker/.gitignore
+-rw-r--r--   0        0        0     1968 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/docker/Dockerfile
+-rw-r--r--   0        0        0      808 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/docker/README.md
+-rw-r--r--   0        0        0      248 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/docker/config/apache/website.conf
+-rw-r--r--   0        0        0      291 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/docker/docker-compose.yml
+-rw-r--r--   0        0        0       46 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/docs/.gitignore
+-rw-r--r--   0        0        0      394 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/docs/assets/css/custom.css
+-rw-r--r--   0        0        0      748 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/docs/assets/css/extra.css
+-rw-r--r--   0        0        0    39005 2024-05-21 09:10:59.013688 sdk_entrepot_gpf-0.1.27/docs/assets/css/neoteroi.css
+-rw-r--r--   0        0        0     1150 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/assets/images/favicon.ico
+-rw-r--r--   0        0        0    12622 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/assets/images/index__utilisation_module.excalidraw
+-rw-r--r--   0        0        0   193450 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/assets/images/index__utilisation_module.png
+-rw-r--r--   0        0        0    15848 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/assets/images/logo.png
+-rw-r--r--   0        0        0     4429 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/comme-executable.md
+-rw-r--r--   0        0        0     4960 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/comme-module.md
+-rw-r--r--   0        0        0     6776 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/configuration.md
+-rw-r--r--   0        0        0    29083 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/configuration_details.md
+-rw-r--r--   0        0        0     6052 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/development.md
+-rw-r--r--   0        0        0     1327 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/index.md
+-rw-r--r--   0        0        0      131 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/reference/auth.md
+-rw-r--r--   0        0        0      336 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/reference/io.md
+-rw-r--r--   0        0        0      338 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/reference/store.md
+-rw-r--r--   0        0        0       68 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/reference/workflow.md
+-rw-r--r--   0        0        0      314 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/reference/workflow/action.md
+-rw-r--r--   0        0        0      368 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/reference/workflow/resolver.md
+-rw-r--r--   0        0        0    11758 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/resolveurs.md
+-rw-r--r--   0        0        0     5851 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/tutoriel_1_archive.md
+-rw-r--r--   0        0        0     6731 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/tutoriel_2_flux_vecteur.md
+-rw-r--r--   0        0        0     5137 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/tutoriel_3_flux_raster.md
+-rw-r--r--   0        0        0     4161 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/upload_descriptor.md
+-rw-r--r--   0        0        0    24828 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/docs/workflow.md
+-rw-r--r--   0        0        0     2201 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/mkdocs.yml
+-rw-r--r--   0        0        0      114 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/mypy.ini
+-rw-r--r--   0        0        0     1371 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/pyproject.toml
+-rw-r--r--   0        0        0      689 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/Errors.py
+-rw-r--r--   0        0        0       93 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/__init__.py
+-rw-r--r--   0        0        0    49225 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/__main__.py
+-rw-r--r--   0        0        0    11504 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_conf/default.ini
+-rw-r--r--   0        0        0     1202 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_conf/json_schemas/annexe_descriptor_file.json
+-rw-r--r--   0        0        0      870 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_conf/json_schemas/metadata_descriptor_file.json
+-rw-r--r--   0        0        0     1226 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_conf/json_schemas/static_descriptor_file.json
+-rw-r--r--   0        0        0     2092 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_conf/json_schemas/upload_descriptor_file.json
+-rw-r--r--   0        0        0     7085 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_conf/json_schemas/workflow.json
+-rw-r--r--   0        0        0      255 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON.md5
+-rwxr-xr-x   0        0        0        5 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2297 2024-05-21 09:10:59.017688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf
+-rwxr-xr-x   0        0        0      655 2024-05-21 09:10:59.021688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.prj
+-rw-r--r--   0        0        0   430828 2024-05-21 09:10:59.021688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      588 2024-05-21 09:10:59.021688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shx
+-rw-r--r--   0        0        0     4003 2024-05-21 09:10:59.021688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON_style.sld
+-rw-r--r--   0        0        0      529 2024-05-21 09:10:59.021688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/upload_descriptor.json
+-rw-r--r--   0        0        0       52 2024-05-21 09:10:59.021688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON.md5
+-rw-r--r--   0        0        0   991843 2024-05-21 09:10:59.025688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON/CANTON.zip
+-rw-r--r--   0        0        0      525 2024-05-21 09:10:59.025688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/upload_descriptor.json
+-rw-r--r--   0        0        0     4391 2024-05-21 09:10:59.025688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/installation.sld
+-rw-r--r--   0        0        0      411 2024-05-21 09:10:59.025688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_1/installation-init.sql
+-rw-r--r--   0        0        0   368640 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_2/installation.gpkg
+-rw-r--r--   0        0        0   676357 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csv
+-rw-r--r--   0        0        0       84 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csvt
+-rw-r--r--   0        0        0     1731 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/upload_descriptor.json
+-rw-r--r--   0        0        0     6973 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/workflows/generic_archive.jsonc
+-rw-r--r--   0        0        0    15492 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/workflows/generic_joincache.jsonc
+-rw-r--r--   0        0        0     9884 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/workflows/generic_maj_bdd.jsonc
+-rw-r--r--   0        0        0    11561 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/workflows/generic_moissonnage.jsonc
+-rw-r--r--   0        0        0     9209 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/workflows/generic_raster.jsonc
+-rw-r--r--   0        0        0    15240 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/workflows/generic_vecteur.jsonc
+-rw-r--r--   0        0        0     8333 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/auth/Authentifier.py
+-rw-r--r--   0        0        0      274 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/auth/Errors.py
+-rw-r--r--   0        0        0     1493 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/auth/Token.py
+-rw-r--r--   0        0        0       46 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/auth/__init__.py
+-rw-r--r--   0        0        0     2589 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/helper/FileHelper.py
+-rw-r--r--   0        0        0     6939 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/helper/JsonHelper.py
+-rw-r--r--   0        0        0      916 2024-05-21 09:10:59.029688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/helper/PrintLogHelper.py
+-rw-r--r--   0        0        0       59 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/helper/__init__.py
+-rw-r--r--   0        0        0    16028 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/ApiRequester.py
+-rw-r--r--   0        0        0      607 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/Color.py
+-rw-r--r--   0        0        0     5695 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/Config.py
+-rw-r--r--   0        0        0     5318 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/Dataset.py
+-rw-r--r--   0        0        0     4143 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/DescriptorFileReader.py
+-rw-r--r--   0        0        0     6878 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/Errors.py
+-rw-r--r--   0        0        0     2909 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/JsonConverter.py
+-rw-r--r--   0        0        0     4416 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/OutputManager.py
+-rw-r--r--   0        0        0     4075 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/UploadDescriptorFileReader.py
+-rw-r--r--   0        0        0       47 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/__init__.py
+-rw-r--r--   0        0        0      793 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/pattern/SingleInstance.py
+-rw-r--r--   0        0        0      637 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/pattern/Singleton.py
+-rw-r--r--   0        0        0       33 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/pattern/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/py.typed
+-rw-r--r--   0        0        0     1209 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/AbstractCommonFile.py
+-rw-r--r--   0        0        0     2486 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Annexe.py
+-rw-r--r--   0        0        0      222 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Check.py
+-rw-r--r--   0        0        0      584 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/CheckExecution.py
+-rw-r--r--   0        0        0     4269 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Configuration.py
+-rw-r--r--   0        0        0     3400 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Datastore.py
+-rw-r--r--   0        0        0     3363 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Endpoint.py
+-rw-r--r--   0        0        0      183 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Errors.py
+-rw-r--r--   0        0        0     2586 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Metadata.py
+-rw-r--r--   0        0        0     2140 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Offering.py
+-rw-r--r--   0        0        0      332 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Permission.py
+-rw-r--r--   0        0        0      231 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Processing.py
+-rw-r--r--   0        0        0     2026 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/ProcessingExecution.py
+-rw-r--r--   0        0        0     1005 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Static.py
+-rw-r--r--   0        0        0    14998 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/StoreEntity.py
+-rw-r--r--   0        0        0     1933 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/StoredData.py
+-rw-r--r--   0        0        0      235 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Tms.py
+-rw-r--r--   0        0        0     7270 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Upload.py
+-rw-r--r--   0        0        0     1010 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/User.py
+-rw-r--r--   0        0        0     1432 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/__init__.py
+-rw-r--r--   0        0        0     2521 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/CommentInterface.py
+-rw-r--r--   0        0        0     2025 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/CreatedByUploadFileInterface.py
+-rw-r--r--   0        0        0     1051 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/CsfInterface.py
+-rw-r--r--   0        0        0     1102 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/DownloadInterface.py
+-rw-r--r--   0        0        0      805 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/EventInterface.py
+-rw-r--r--   0        0        0     1262 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/FullEditInterface.py
+-rw-r--r--   0        0        0     1584 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/LogsInterface.py
+-rw-r--r--   0        0        0     1116 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/PartialEditInterface.py
+-rw-r--r--   0        0        0      998 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/ReUploadFileInterface.py
+-rw-r--r--   0        0        0     2107 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/SharingInterface.py
+-rw-r--r--   0        0        0     2329 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/TagInterface.py
+-rw-r--r--   0        0        0       88 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/__init__.py
+-rw-r--r--   0        0        0      512 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/Errors.py
+-rw-r--r--   0        0        0    20884 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/Workflow.py
+-rw-r--r--   0        0        0       40 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/__init__.py
+-rw-r--r--   0        0        0     5757 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/ActionAbstract.py
+-rw-r--r--   0        0        0     7077 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/ConfigurationAction.py
+-rw-r--r--   0        0        0     1776 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/CopyConfigurationAction.py
+-rw-r--r--   0        0        0     5200 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/DeleteAction.py
+-rw-r--r--   0        0        0     3331 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/EditAction.py
+-rw-r--r--   0        0        0     2762 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/EditUsedDataConfigurationAction.py
+-rw-r--r--   0        0        0     6827 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/OfferingAction.py
+-rw-r--r--   0        0        0     2153 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/PermissionAction.py
+-rw-r--r--   0        0        0    20312 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/ProcessingExecutionAction.py
+-rw-r--r--   0        0        0     7514 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/SynchronizeOfferingAction.py
+-rw-r--r--   0        0        0    22972 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/UploadAction.py
+-rw-r--r--   0        0        0       72 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/__init__.py
+-rw-r--r--   0        0        0     2267 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/AbstractResolver.py
+-rw-r--r--   0        0        0     3389 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/DateResolver.py
+-rw-r--r--   0        0        0     1933 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/DictResolver.py
+-rw-r--r--   0        0        0      708 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/DumbResolver.py
+-rw-r--r--   0        0        0     4533 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/Errors.py
+-rw-r--r--   0        0        0     6076 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/FileResolver.py
+-rw-r--r--   0        0        0     3838 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/GlobalResolver.py
+-rw-r--r--   0        0        0     5760 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/StoreEntityResolver.py
+-rw-r--r--   0        0        0     1908 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/UserResolver.py
+-rw-r--r--   0        0        0      110 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/__init__.py
+-rw-r--r--   0        0        0      960 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/tests/ErrorsTestCase.py
+-rw-r--r--   0        0        0     1739 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/tests/GpfTestCase.py
+-rw-r--r--   0        0        0     3419 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/tests/MainTestCase.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/tests/__init__.py
+-rw-r--r--   0        0        0      369 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/tests/_conf/test_authentifier.ini
+-rw-r--r--   0        0        0      308 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/tests/_conf/test_overload.ini
+-rw-r--r--   0        0        0      594 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/tests/_conf/test_requester.ini
+-rw-r--r--   0        0        0       40 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/tests/_conf/test_upload.ini
+-rw-r--r--   0        0        0       69 2024-05-21 09:10:59.033688 sdk_entrepot_gpf-0.1.27/tests/_conf/test_value_type.ini
+-rw-r--r--   0        0        0      460 2024-05-21 09:10:59.037688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/1_test_dataset_bad_pathes/upload_descriptor.json
+-rw-r--r--   0        0        0      305 2024-05-21 09:10:59.037688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/2_test_dataset_bad_md5/CANTON.md5
+-rw-r--r--   0        0        0        5 2024-05-21 09:10:59.037688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2318 2024-05-21 09:10:59.037688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf
+-rw-r--r--   0        0        0      145 2024-05-21 09:10:59.037688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.prj
+-rw-r--r--   0        0        0  1279276 2024-05-21 09:10:59.041688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      572 2024-05-21 09:10:59.041688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx
+-rw-r--r--   0        0        0        0 2024-05-21 09:10:59.041688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/sous_dossier/coucou.txt
+-rw-r--r--   0        0        0      567 2024-05-21 09:10:59.041688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json
+-rw-r--r--   0        0        0       11 2024-05-21 09:10:59.041688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/3_test_dataset_sub_dir/.gitignore
+-rw-r--r--   0        0        0        5 2024-05-21 09:10:59.041688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.cpg
+-rw-r--r--   0        0        0     2318 2024-05-21 09:10:59.041688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf
+-rw-r--r--   0        0        0      145 2024-05-21 09:10:59.041688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.prj
+-rw-r--r--   0        0        0  1279276 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp
+-rw-r--r--   0        0        0      572 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx
+-rw-r--r--   0        0        0        0 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/sous_dossier/coucou.txt
+-rw-r--r--   0        0        0      567 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json
+-rw-r--r--   0        0        0     2659 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_data/workflows/bad-workflow.jsonc
+-rw-r--r--   0        0        0       53 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_test/helper/FileHelper/md5.txt
+-rw-r--r--   0        0        0       78 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_test/helper/JsonHelper/json_not_parsable.json
+-rw-r--r--   0        0        0       52 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_test/helper/JsonHelper/json_not_valid.json
+-rw-r--r--   0        0        0      108 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_test/helper/JsonHelper/json_parsable.json
+-rw-r--r--   0        0        0      563 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_test/helper/JsonHelper/schema.json
+-rw-r--r--   0        0        0      485 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_test/helper/JsonHelper/schema_invalid.json
+-rw-r--r--   0        0        0       23 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_test/workflow/resolver/FileResolver/dict.json
+-rw-r--r--   0        0        0       21 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_test/workflow/resolver/FileResolver/list.json
+-rw-r--r--   0        0        0        2 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_test/workflow/resolver/FileResolver/not-valid.json
+-rw-r--r--   0        0        0       31 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/_test/workflow/resolver/FileResolver/text.txt
+-rw-r--r--   0        0        0     7428 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/auth/AuthentifierTestCase.py
+-rw-r--r--   0        0        0     1187 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/auth/TokenTestCase.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/auth/__init__.py
+-rw-r--r--   0        0        0     1060 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/helper/FileHelperTestCase.py
+-rw-r--r--   0        0        0     9967 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/helper/JsonHelperTestCase.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/helper/__init__.py
+-rw-r--r--   0        0        0    23350 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/io/ApiRequesterTestCase.py
+-rw-r--r--   0        0        0     3599 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/io/ConfigTestCase.py
+-rw-r--r--   0        0        0     2225 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/io/DatasetTestCase.py
+-rw-r--r--   0        0        0     3197 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/io/ErrorsTestCase.py
+-rw-r--r--   0        0        0     1202 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/io/JsonConverterTestCase.py
+-rw-r--r--   0        0        0     1774 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/io/UploadDescriptorFileReaderTestCase.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/io/__init__.py
+-rw-r--r--   0        0        0     1122 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/store/AbstractCommonFileTestCase.py
+-rw-r--r--   0        0        0     2587 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/store/AnnexeTestCase.py
+-rw-r--r--   0        0        0     7221 2024-05-21 09:10:59.049688 sdk_entrepot_gpf-0.1.27/tests/store/ConfigurationTestCase.py
+-rw-r--r--   0        0        0     4849 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/DatastoreTestCase.py
+-rw-r--r--   0        0        0     5595 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/EndpointTestCase.py
+-rw-r--r--   0        0        0     1152 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/ErrorsTestCase.py
+-rw-r--r--   0        0        0     2297 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/MetadataTestCase.py
+-rw-r--r--   0        0        0     2687 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/OfferingTestCase.py
+-rw-r--r--   0        0        0     2972 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/ProcessingExecutionTestCase.py
+-rw-r--r--   0        0        0    26065 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/StoreEntityTestCase.py
+-rw-r--r--   0        0        0     3137 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/StoredDataTestCase.py
+-rw-r--r--   0        0        0    11003 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/UploadTestCase.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/__init__.py
+-rw-r--r--   0        0        0     5134 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/interface/CommentInterfaceTestCase.py
+-rw-r--r--   0        0        0     2790 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/interface/CreatedByUploadFileInterfaceTestCase.py
+-rw-r--r--   0        0        0     2536 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/interface/CsfInterfaceTestCase.py
+-rw-r--r--   0        0        0     1767 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/interface/DownloadInterfaceTestCase.py
+-rw-r--r--   0        0        0     1663 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/interface/EventInterfaceTestCase.py
+-rw-r--r--   0        0        0     2326 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/interface/FullEditInterfaceTestCase.py
+-rw-r--r--   0        0        0     4073 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/interface/LogsInterfaceTestCase.py
+-rw-r--r--   0        0        0     2243 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/interface/PartialEditInterfaceTestCase.py
+-rw-r--r--   0        0        0     1569 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/interface/ReUploadFileInterfaceTestCase.py
+-rw-r--r--   0        0        0     4039 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/interface/SharingInterfaceTestCase.py
+-rw-r--r--   0        0        0     3899 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/interface/TagInterfaceTestCase.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/store/interface/__init__.py
+-rw-r--r--   0        0        0    28973 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/WorkflowTestCase.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/__init__.py
+-rw-r--r--   0        0        0     3595 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/action/ActionAbstractTestCase.py
+-rw-r--r--   0        0        0    10471 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/action/ConfigurationActionTestCase.py
+-rw-r--r--   0        0        0     2502 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/action/CopyConfigurationActionTestCase.py
+-rw-r--r--   0        0        0    12123 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/action/DeleteActionTestCase.py
+-rw-r--r--   0        0        0     5262 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/action/EditActionTestCase.py
+-rw-r--r--   0        0        0     4450 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/action/EditUsedDataConfigurationActionTestCase.py
+-rw-r--r--   0        0        0    16051 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/action/OfferingActionTestCase.py
+-rw-r--r--   0        0        0     1547 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/action/PermissionActionTestCase.py
+-rw-r--r--   0        0        0    33433 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/action/ProcessingExecutionActionTestCase.py
+-rw-r--r--   0        0        0    10675 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/action/SynchronizeOfferingActionTestCase.py
+-rw-r--r--   0        0        0    45035 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/action/UploadActionTestCase.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/action/__init__.py
+-rw-r--r--   0        0        0     2133 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/AbstractResolverTestCase.py
+-rw-r--r--   0        0        0     2401 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/DateResolverTestCase.py
+-rw-r--r--   0        0        0     1124 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/DictResolverTestCase.py
+-rw-r--r--   0        0        0     5479 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/FileResolverTestCase.py
+-rw-r--r--   0        0        0     7361 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/GlobalResolverTestCase.py
+-rw-r--r--   0        0        0    15246 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/StoreEntityResolverTestCase.py
+-rw-r--r--   0        0        0     2237 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/UserResolverTestCase.py
+-rw-r--r--   0        0        0        0 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/__init__.py
+-rw-r--r--   0        0        0   116760 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/uml/classes.png
+-rw-r--r--   0        0        0     9175 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/uml/classes.uxf
+-rw-r--r--   0        0        0    43510 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/uml/interfaces.png
+-rw-r--r--   0        0        0     7059 2024-05-21 09:10:59.053688 sdk_entrepot_gpf-0.1.27/uml/interfaces.uxf
+-rw-r--r--   0        0        0     1773 1970-01-01 00:00:00.000000 sdk_entrepot_gpf-0.1.27/PKG-INFO
```

### Comparing `sdk_entrepot_gpf-0.1.26/.github/workflows/ci-dev.yml` & `sdk_entrepot_gpf-0.1.27/.github/workflows/ci-dev.yml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/.github/workflows/ci-prod.yml` & `sdk_entrepot_gpf-0.1.27/.github/workflows/ci-prod.yml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/.github/workflows/code-quality.yml` & `sdk_entrepot_gpf-0.1.27/.github/workflows/code-quality.yml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/.gitignore` & `sdk_entrepot_gpf-0.1.27/.gitignore`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/.pylintrc` & `sdk_entrepot_gpf-0.1.27/.pylintrc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/.vscode/settings.json` & `sdk_entrepot_gpf-0.1.27/.vscode/settings.json`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 {
     "cSpell.words": [
         "autorefs",
         "bbox",
         "dateutil",
+        "dépublication",
+        "dépubliée",
+        "dépubliées",
+        "dépublier",
         "EPSG",
         "fontawesome",
         "Géoplateforme",
         "GEOSERVER",
         "geotuileur",
         "ignf",
         "inlinehilite",
         "insee",
         "isoparse",
         "jsonschema",
         "linenums",
+        "metadatas",
         "mkapi",
         "mkdocs",
         "mkdocstrings",
         "mypy",
         "parsables",
         "pathes",
         "pathlib",
```

### Comparing `sdk_entrepot_gpf-0.1.26/CHANGELOG.md` & `sdk_entrepot_gpf-0.1.27/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,27 @@
 # CHANGE LOG
 
+## v0.1.27
+
+### [Added]
+
+* ProcessingExecutionAction: ajout d'un mode reprise (`RESUME`). #143
+* EditUsedDataConfigurationAction: possibilité de mise à jour de la BBox de la configuration selon les données. #140
+
+### [Changed]
+
+* Mise à jour de la documentation de publication d'une archive pour ajouter l'étape de patch sur la donnée stockée
+* affichage des actions: harmonisation des affichages pour les actions #138
+* utilisation en ligne de commande : enrichissement de l'aide.
+
+### [Fixed]
+
+* upload_descriptor_file.json: ajout de type_infos suite à l'ajout du paramètre dans la requête GPF. #117
+* LogsInterface: récupération des logs en prenant compte de la pagination (+ refonte test api_logs). #135
+
 ## v0.1.26
 
 ### [Added]
 
 * UploadAction: possibilité vérification totale des fichiers livrés avant de fermer la livraison #124
 
 ### [Changed]
```

### Comparing `sdk_entrepot_gpf-0.1.26/LICENSE` & `sdk_entrepot_gpf-0.1.27/LICENSE`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/README.md` & `sdk_entrepot_gpf-0.1.27/README.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/check.sh` & `sdk_entrepot_gpf-0.1.27/check.sh`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docker/Dockerfile` & `sdk_entrepot_gpf-0.1.27/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docker/README.md` & `sdk_entrepot_gpf-0.1.27/docker/README.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/assets/css/extra.css` & `sdk_entrepot_gpf-0.1.27/docs/assets/css/extra.css`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/assets/css/neoteroi.css` & `sdk_entrepot_gpf-0.1.27/docs/assets/css/neoteroi.css`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/assets/images/favicon.ico` & `sdk_entrepot_gpf-0.1.27/docs/assets/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/assets/images/index__utilisation_module.excalidraw` & `sdk_entrepot_gpf-0.1.27/docs/assets/images/index__utilisation_module.excalidraw`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/assets/images/index__utilisation_module.png` & `sdk_entrepot_gpf-0.1.27/docs/assets/images/index__utilisation_module.png`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/assets/images/logo.png` & `sdk_entrepot_gpf-0.1.27/docs/assets/images/logo.png`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/comme-executable.md` & `sdk_entrepot_gpf-0.1.27/docs/comme-executable.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/comme-module.md` & `sdk_entrepot_gpf-0.1.27/docs/comme-module.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/configuration.md` & `sdk_entrepot_gpf-0.1.27/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/configuration_details.md` & `sdk_entrepot_gpf-0.1.27/docs/configuration_details.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/development.md` & `sdk_entrepot_gpf-0.1.27/docs/development.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/index.md` & `sdk_entrepot_gpf-0.1.27/docs/index.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/resolveurs.md` & `sdk_entrepot_gpf-0.1.27/docs/resolveurs.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/tutoriel_1_archive.md` & `sdk_entrepot_gpf-0.1.27/docs/tutoriel_1_archive.md`

 * *Files 5% similar despite different names*

```diff
@@ -72,37 +72,40 @@
 
 Ouvrez le fichier. Vous trouverez plus de détails dans la [documentation sur les workflows](workflow.md), mais vous pouvez dès à présent voir que le workflow est composé de 3 étapes. Il faudra lancer une commande pour chacune d'elles.
 
 ```mermaid
 %% doc mermaid ici https://mermaid-js.github.io/mermaid/#/flowchart?id=flowcharts-basic-syntax
 flowchart TD
     A("upload") -->|intégration-archive-livrée| B("dataset")
-    B -->|configuration-archive-livrée| C(configuration)
-    C -->|publication-archive-livrée| D(publication)
+    B -->|patch-donnée-stockée|C("patch")
+    C-->|configuration-archive-livrée| D(configuration)
+    D -->|publication-archive-livrée| E(publication)
 ```
 
 ## Traitement et publication
 
 Le workflow « generic_archive » permet de passer de la livraison à une lien permettant de télécharger la donnée. Il comporte 3 étapes :
 
 * `intégration-archive-livrée` : transformation des données livrées temporaires en une Donnée Stockée pérenne ;
+* `patch-donnée-stockée` : ajout de la description des Données Stockée;
 * `configuration-archive-livrée` : configuration d'un service de téléchargement permettant de télécharger les données ;
 * `publication-archive-livrée` : publication du service de téléchargement.
 
 Lancez les 3 commandes suivantes pour exécuter les 3 étapes :
 
 ```sh
 python -m sdk_entrepot_gpf workflow -f generic_archive.jsonc -s intégration-archive-livrée
+python -m sdk_entrepot_gpf workflow -f generic_archive.jsonc -s patch-donnée-stockée
 python -m sdk_entrepot_gpf workflow -f generic_archive.jsonc -s configuration-archive-livrée
 python -m sdk_entrepot_gpf workflow -f generic_archive.jsonc -s publication-archive-livrée
 ```
 
 La première commande ne doit pas être instantanée : un traitement est effectué et les logs doivent vous être remontés.
 
-Les deux étapes suivantes sont instantanées. A la fin, vous devez voir s'afficher un lien.
+Les trois étapes suivantes sont instantanées. A la fin, vous devez voir s'afficher un lien.
 
 Exemple :
 
 ```txt
 INFO - Offre créée : Offering(id=62c708e72246434ac40ee3ad)
    - download|https://geoservices-geotuileur.ccs-ign-plage.ccs.cegedim.cloud/download/plage/archive
 ```
@@ -126,12 +129,13 @@
 ```sh
 # récupération des données d'exemple
 python -m sdk_entrepot_gpf dataset -n 2_dataset_archive
 # livraison des données sur la Géoplateforme
 python -m sdk_entrepot_gpf upload -f 2_dataset_archive/upload_descriptor.json
 # récupération du workflow de traitement et publication d'une archive
 python -m sdk_entrepot_gpf workflow -n generic_archive.jsonc
-# exécution des 3 étapes pour le traitement et la publication de l'archive
+# exécution des 4 étapes pour le traitement et la publication de l'archive
 python -m sdk_entrepot_gpf workflow -f generic_archive.jsonc -s intégration-archive-livrée
+python -m sdk_entrepot_gpf workflow -f generic_archive.jsonc -s patch-donnée-stockée
 python -m sdk_entrepot_gpf workflow -f generic_archive.jsonc -s configuration-archive-livrée
 python -m sdk_entrepot_gpf workflow -f generic_archive.jsonc -s publication-archive-livrée
 ```
```

### Comparing `sdk_entrepot_gpf-0.1.26/docs/tutoriel_2_flux_vecteur.md` & `sdk_entrepot_gpf-0.1.27/docs/tutoriel_2_flux_vecteur.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/tutoriel_3_flux_raster.md` & `sdk_entrepot_gpf-0.1.27/docs/tutoriel_3_flux_raster.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/upload_descriptor.md` & `sdk_entrepot_gpf-0.1.27/docs/upload_descriptor.md`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/docs/workflow.md` & `sdk_entrepot_gpf-0.1.27/docs/workflow.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 Les actions sont les suivantes :
 
 * lancer un traitement (càd créer une processing exécution) ;
 * configurer un géoservice (càd créer une configuration) ;
 * publier un géoservice (càd créer une offering) ;
 * supprimer une entité de type upload, stored_data, configuration ou offering ;
 * modifier une entité de type upload, stored_data, configuration ou offering ;
+* mise à jour des used_data et bbox d'une configuration
 * copier une configuration (création d'une nouvelle configuration en reprenant les paramètres non précisés de la précédente) ;
 * synchroniser une offre (mettre à jour avec la donnée stockée et une offering).
 
 ## Définition
 
 Le fichier doit contenir un dictionnaire `workflow`. Qui contient deux clefs :
 
@@ -49,14 +50,15 @@
 Les actions possibles sont les suivante :
 
 * [exécuter un traitement](Exécuter un traitement)
 * [configurer d'un flux](Configurer d'un flux)
 * [publier un flux](Publier un flux)
 * [supprimer une entité](Supprimer une entité)
 * [modifier une entité](Modifier une entité)
+* [mise à jour des used_data et bbox d'une configuration](Mise à jour des used_data et bbox d'une configuration)
 * [copier une configuration](Copier une configuration)
 * [synchroniser une publication](Synchroniser une publication)
 
 ### Exécuter un traitement
 
 * `type`: `processing-execution`
 * `body_parameters`: dictionnaire paramétrant l’exécution :
@@ -293,14 +295,16 @@
     // Suppression en cascade autorisée ou pas ? par défaut à false
     "cascade": true,
     // Ok si non trouvée ? par défaut à true
     "not_found_ok": true,
 }
 ```
 
+***ATTENTION** ici la valeur **`{uuid}` doit être une uuid en dur et non une uuid récupérée par le résolveur `store_entity`**(StoreEntityResolver) pour que l'option `"not_found_ok": true,`(valeur par défaut) fonctionne. **S'il y a besoin d'utiliser le résolveur `store_entity` il faut utiliser la solution suivante**. Avec l'utilisation du résolveur `store_entity` si l'entité n'existe pas une erreur sera levée pendant la résolution de l'action et les résolveurs gardant en mémoire les valeurs déjà trouvées la réutilisation du résolveur avec les même filtre pointera vers l'entité supprimée.*
+
 * suppression par filtre sur la liste :
 
 ```jsonc
 {
     "type": "delete-entity",
     // Type de l'entité à supprimer (upload, stored_data, configuration, offering)
     "entity_type": "configuration",
@@ -342,16 +346,38 @@
 
 * upload *(partiel)* : PATCH [/datastores/{datastore}/uploads/{upload}](https://data.geopf.fr/api/swagger-ui/index.html#/Livraisons%20et%20v%C3%A9rifications/update_2)
   * Seul le nom de la livraison, sa description et sa visibilité sont modifiables, et uniquement par le propriétaire. Les autres informations, comme le type de la livraison, sont figées.
 * stored_data *(partiel)* : PATCH [/datastores/{datastore}/stored_data/{stored_data}](https://data.geopf.fr/api/swagger-ui/index.html#/Donn%C3%A9es%20stock%C3%A9es/update_3)
   * Seul le nom de la donnée et sa visibilité sont modifiables, et uniquement par le propriétaire. Les autres informations, comme le type de la donnée, sont figées pour une donnée.
 * configuration *(totale)* : PUT [/datastores/{datastore}/configurations/{configuration}](https://data.geopf.fr/api/swagger-ui/index.html#/Configurations%20et%20publications/update_1)
   * Si la configuration est liée à des offres en cours de publication, la modification n'est pas possible. Si la configuration est liée à des offres publiées, les modifications sont répercutées sur les serveurs de diffusion. Le nom technique et le type ne sont pas modifiable.
+  * Cas particulier de la modification des used_data (`[type_infos][used_data]`), la liste doit être de la même longueur que celle de la configuration et chaque dictionnaire sera fusionné avec l'ancien cf [#83](https://github.com/Geoplateforme/sdk-entrepot/issues/83) [#66](https://github.com/Geoplateforme/sdk-entrepot/issues/66). Pour supprimer/ajouter une used_data cf action suivante [Mise à jour des used_data d'une configuration](#mise-à-jour-des-used_data-dune-configuration)
 * offering *(partiel)*: PATCH [/datastores/{datastore}/offerings/{offering}](https://data.geopf.fr/api/swagger-ui/index.html#/Configurations%20et%20publications/update_4)
-  * Il est possible de modifier la visibilité d'une offre afin qu'elle apparaisse dans les catalogues ou qu'on puisse donner des permissions, ou au contraire qu'elle en disparaisse. On peut également désactiver une offre pour en couper la consommation rapidement, sans déconfigurer les permissions
+  * Il est possible de modifier la visibilité d'une offre afin qu'elle apparaisse dans les catalogues ou qu'on puisse donner des permissions, ou au contraire qu'elle en disparaisse. On peut également désactiver une offre pour en couper la consommation rapidement, sans déconfigurer les permissions.
+
+### Mise à jour des used_data et bbox d'une Configuration
+
+L'action d'édition d'une configuration ne permet pas de supprimer ni ajouter une used_data. Cette action permet donc de supprimer/ajouter une used_data ainsi que de pouvoir mettre à jour la BBox avec les données utilisées.
+
+```jsonc
+{
+  // mise à jour de la bbox de la configuration
+  "type": "used_data-configuration",
+  "entity_id":  "{uuid_config}",
+  // Optionnel : liste des used_data à supprimer, toutes les used_data existantes qui sont l'intersection des clefs spécifiées seront supprimées
+  // dans l'exemple, on supprime toutes les used_data liées à la stored_data "id_store_data" et toutes celles qui sont liées à la zone "ZONE"
+  "delete_used_data": [{"stored_data": "id_store_data"}, {"zone": "ZONE"}],
+  // Optionnel : liste des used_data à ajouter, selon le format demandé par l'API Entrepôt
+  "append_used_data": [{...}],
+  // Optionnel : si on veut mettre à jour la BBox avec les données utilisées (bbox calculée après la modification des used_data). Par défaut à false.
+  "reset_bbox": true
+}
+```
+
+**Note** : La modification de la configuration n'est pas prise en compte automatiquement par les publications il faut les [synchroniser](#synchroniser-une-publication) pour que la modification soit visible dans le flux lié à la configuration.
 
 ### Copier une configuration
 
 Création d'une configuration à partir d'une configuration déjà existante
 
 ```jsonc
 {
```

### Comparing `sdk_entrepot_gpf-0.1.26/mkdocs.yml` & `sdk_entrepot_gpf-0.1.27/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/pyproject.toml` & `sdk_entrepot_gpf-0.1.27/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/Errors.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/Errors.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/__main__.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from sdk_entrepot_gpf.io.Errors import ConflictError, NotFoundError
 from sdk_entrepot_gpf.io.ApiRequester import ApiRequester
 from sdk_entrepot_gpf.store.Annexe import Annexe
 from sdk_entrepot_gpf.store.Metadata import Metadata
 from sdk_entrepot_gpf.store.Static import Static
 from sdk_entrepot_gpf.workflow.Workflow import Workflow
 from sdk_entrepot_gpf.workflow.action.DeleteAction import DeleteAction
+from sdk_entrepot_gpf.workflow.action.ProcessingExecutionAction import ProcessingExecutionAction
 from sdk_entrepot_gpf.workflow.resolver.DateResolver import DateResolver
 from sdk_entrepot_gpf.workflow.resolver.GlobalResolver import GlobalResolver
 from sdk_entrepot_gpf.workflow.resolver.StoreEntityResolver import StoreEntityResolver
 from sdk_entrepot_gpf.workflow.action.UploadAction import UploadAction
 from sdk_entrepot_gpf.io.Config import Config
 from sdk_entrepot_gpf.io.UploadDescriptorFileReader import UploadDescriptorFileReader
 from sdk_entrepot_gpf.store.Upload import Upload
@@ -96,122 +97,122 @@
         o_parser.add_argument("--ini", dest="config", default="config.ini", help="Chemin vers le fichier de config à utiliser (config.ini par défaut)")
         o_parser.add_argument("--version", action="version", version=f"%(prog)s v{sdk_entrepot_gpf.__version__}")
         o_parser.add_argument("--debug", dest="debug", required=False, default=False, action="store_true", help="Passe l'appli en mode debug (plus de messages affichés)")
         o_parser.add_argument("--datastore", "-d", dest="datastore", required=False, default=None, help="Identifiant du datastore à utiliser")
         o_sub_parsers = o_parser.add_subparsers(dest="task", metavar="TASK", required=True, help="Tâche à effectuer")
 
         # Parser pour auth
-        o_sub_parser = o_sub_parsers.add_parser("auth", help="Authentification")
+        o_sub_parser = o_sub_parsers.add_parser("auth", help="Gestion de l'authentification")
         o_sub_parser.add_argument("--show", type=str, choices=["token", "header"], default=None, help="Donnée à renvoyer")
 
         # Parser pour me
         o_sub_parser = o_sub_parsers.add_parser("me", help="Mes informations")
 
         # Parser pour config
-        o_sub_parser = o_sub_parsers.add_parser("config", help="Configuration")
+        o_sub_parser = o_sub_parsers.add_parser("config", help="Affichage de la configuration")
         o_sub_parser.add_argument("--file", "-f", type=str, default=None, help="Chemin du fichier où sauvegarder la configuration (si null, la configuration est affichée)")
         o_sub_parser.add_argument("--section", "-s", type=str, default=None, help="Se limiter à une section")
         o_sub_parser.add_argument("--option", "-o", type=str, default=None, help="Se limiter à une option (la section doit être renseignée)")
 
         # Parser pour upload
         s_epilog_upload = """Trois types de lancement :
         * création / mise à jour de livraison : `--file FILE [--behavior BEHAVIOR] [--check-before-close]`
         * détail d'une livraison, optionnel ouverture ou fermeture : `--id ID [--open | --close]`
         * liste des livraisons, optionnel filtre sur l'info et tags : `[--infos INFOS] [--tags TAGS]`
         """
-        o_sub_parser = o_sub_parsers.add_parser("upload", help="Livraisons", epilog=s_epilog_upload, formatter_class=argparse.RawTextHelpFormatter)
+        o_sub_parser = o_sub_parsers.add_parser("upload", help="Livraisons (téléversement, listing, ...)", epilog=s_epilog_upload, formatter_class=argparse.RawTextHelpFormatter)
         o_sub_parser.add_argument("--file", "-f", type=str, default=None, help="Chemin vers le fichier descriptor dont on veut effectuer la livraison)")
         o_sub_parser.add_argument("--check-before-close", action="store_true", default=False, help="Si on vérifie l'ensemble de la livraison avant de fermer la livraison (uniquement avec --file|-f)")
         o_sub_parser.add_argument("--behavior", "-b", choices=UploadAction.BEHAVIORS, default=None, help="Action à effectuer si la livraison existe déjà (uniquement avec -f)")
         o_sub_parser.add_argument("--id", type=str, default=None, help="Affiche la livraison demandée")
         o_exclusive = o_sub_parser.add_mutually_exclusive_group()
         o_exclusive.add_argument("--open", action="store_true", default=False, help="Rouvrir une livraison fermée (uniquement avec --id)")
         o_exclusive.add_argument("--close", action="store_true", default=False, help="Fermer une livraison ouverte (uniquement avec --id)")
         o_sub_parser.add_argument("--infos", "-i", type=str, default=None, help="Filtrer les livraisons selon les infos")
         o_sub_parser.add_argument("--tags", "-t", type=str, default=None, help="Filtrer les livraisons selon les tags")
 
         # Parser pour dataset
-        o_sub_parser = o_sub_parsers.add_parser("dataset", help="Jeux de données")
+        o_sub_parser = o_sub_parsers.add_parser("dataset", help="Jeux de données d'exemple (listing, récupération)")
         o_sub_parser.add_argument("--name", "-n", type=str, default=None, help="Nom du dataset à extraire")
         o_sub_parser.add_argument("--folder", "-f", type=str, default=None, help="Dossier où enregistrer le dataset")
 
         # Parser pour workflow
-        s_epilog_workflow = """Quatre types de lancement :
+        s_epilog_workflow = """quatre types de lancement :
         * liste des exemples de workflow disponibles : `` (aucun arguments)
         * Récupération d'un workflow exemple : `--name NAME`
         * Vérification de la structure du fichier workflow et affichage des étapes : `--file FILE`
         * Lancement l'une étape d'un workflow: `--file FILE --step STEP [--behavior BEHAVIOR]`
         """
-        o_sub_parser = o_sub_parsers.add_parser("workflow", help="Workflow", epilog=s_epilog_workflow, formatter_class=argparse.RawTextHelpFormatter)
+        o_sub_parser = o_sub_parsers.add_parser("workflow", help="Workflow (lancement, vérification)", epilog=s_epilog_workflow, formatter_class=argparse.RawTextHelpFormatter)
         o_sub_parser.add_argument("--file", "-f", type=str, default=None, help="Chemin du fichier à utiliser OU chemin où extraire le dataset")
         o_sub_parser.add_argument("--name", "-n", type=str, default=None, help="Nom du workflow à extraire")
         o_sub_parser.add_argument("--step", "-s", type=str, default=None, help="Étape du workflow à lancer")
-        o_sub_parser.add_argument("--behavior", "-b", type=str, default=None, help="Action à effectuer si l'exécution de traitement existe déjà")
+        o_sub_parser.add_argument("--behavior", "-b", choices=ProcessingExecutionAction.BEHAVIORS, default=None, help="Action à effectuer si l'exécution de traitement existe déjà")
         o_sub_parser.add_argument("--tag", "-t", type=str, nargs=2, action="append", metavar=("Clef", "Valeur"), default=[], help="Tag à ajouter aux actions (plusieurs tags possible)")
         o_sub_parser.add_argument(
             "--comment",
             "-c",
             type=str,
             default=[],
             action="append",
             metavar='"Le commentaire"',
             help="Commentaire à ajouter aux actions (plusieurs commentaires possible, mettre le commentaire entre guillemets)",
         )
 
         # Parser pour delete
-        o_sub_parser = o_sub_parsers.add_parser("delete", help="Delete")
+        o_sub_parser = o_sub_parsers.add_parser("delete", help="Suppression d'entité")
         o_sub_parser.add_argument("--type", choices=DeleteAction.DELETABLE_TYPES, required=True, help="Type de l'entité à supprimer")
         o_sub_parser.add_argument("--id", type=str, required=True, help="Identifiant de l'entité à supprimer")
         o_sub_parser.add_argument("--cascade", action="store_true", help="Action à effectuer si l'exécution de traitement existe déjà")
         o_sub_parser.add_argument("--force", action="store_true", help="Mode forcé, les suppressions sont faites sans aucune interaction")
 
         # Parser pour annexes
-        s_epilog_annexe = """quatre types de lancement :
+        s_epilog_annexe = """Quatre types de lancement :
         * livraison d'annexes : `-f FICHIER`
         * liste des annexes, avec filtre en option : `[--info filtre1=valeur1,filtre2=valeur2]`
-        * détail d'une annexe, avec option publication/dépublication : `--id ID [--publish|--unpublish]`
-        * publication /dépublication par label : `--publish-by-label label1,lable2` et `--unpublish-by-label label1,lable2`
+        * détail d'une annexe, avec option publication / dépublication : `--id ID [--publish|--unpublish]`
+        * publication / dépublication par label : `--publish-by-label label1,label2` et `--unpublish-by-label label1,label2`
         """
-        o_sub_parser = o_sub_parsers.add_parser("annexe", help="Annexes", epilog=s_epilog_annexe, formatter_class=argparse.RawTextHelpFormatter)
+        o_sub_parser = o_sub_parsers.add_parser("annexe", help="Gestion des annexes", epilog=s_epilog_annexe, formatter_class=argparse.RawTextHelpFormatter)
         o_sub_parser.add_argument("--file", "-f", type=str, default=None, help="Chemin vers le fichier descriptor dont on veut effectuer la livraison)")
         o_sub_parser.add_argument("--infos", "-i", type=str, default=None, help="Filtrer les livraisons selon les infos")
         o_sub_parser.add_argument("--id", type=str, default=None, help="Affiche l'annexe demandée")
-        o_sub_parser.add_argument("--publish", action="store_true", help="publication de l'annexe (uniquement avec --id)")
-        o_sub_parser.add_argument("--unpublish", action="store_true", help="dépublication de l'annexe (uniquement avec --id)")
-        o_sub_parser.add_argument("--publish-by-label", type=str, default=None, help="publication des annexes portant les labels donnés (ex: label1,label2)")
-        o_sub_parser.add_argument("--unpublish-by-label", type=str, default=None, help="dépublication des annexes portant les labels donnés (ex: label1,label2)")
+        o_sub_parser.add_argument("--publish", action="store_true", help="Publication de l'annexe (uniquement avec --id)")
+        o_sub_parser.add_argument("--unpublish", action="store_true", help="Dépublication de l'annexe (uniquement avec --id)")
+        o_sub_parser.add_argument("--publish-by-label", type=str, default=None, help="Publication des annexes portant les labels donnés (ex: label1,label2)")
+        o_sub_parser.add_argument("--unpublish-by-label", type=str, default=None, help="Dépublication des annexes portant les labels donnés (ex: label1,label2)")
 
         # Parser pour static
-        s_epilog_static = """trois types de lancement :
+        s_epilog_static = """Trois types de lancement :
         * livraison de fichiers statics : `-f FICHIER`
         * liste des fichiers statics, avec filtre en option : `[--info filtre1=valeur1,filtre2=valeur2]`
         * détail d'un ficher static : `--id ID`
         """
-        o_sub_parser = o_sub_parsers.add_parser("static", help="Fichiers statiques", epilog=s_epilog_static, formatter_class=argparse.RawTextHelpFormatter)
+        o_sub_parser = o_sub_parsers.add_parser("static", help="Gestion des fichiers statiques", epilog=s_epilog_static, formatter_class=argparse.RawTextHelpFormatter)
         o_sub_parser.add_argument("--file", "-f", type=str, default=None, help="Chemin vers le fichier descriptor dont on veut effectuer la livraison)")
         o_sub_parser.add_argument("--infos", "-i", type=str, default=None, help="Filtrer les livraisons selon les infos")
         o_sub_parser.add_argument("--id", type=str, default=None, help="Affiche du fichier demandée")
 
         # Parser pour metadata
-        s_epilog_metadata = """quatre types de lancement :
-        * livraison d'une metadonnées : `-f FICHIER`
-        * liste des metadonnées, avec filtre en option : `[--info filtre1=valeur1,filtre2=valeur2]` ``
-        * détail d'une metadonnée : `--id ID`
-        * publication /dépublication : `--publish NOM_FICHIER [NOM_FICHIER] --id-endpoint ID_ENDPOINT` et `--unpublish NOM_FICHIER [NOM_FICHIER] --id-endpoint ID_ENDPOINT`
-        """
-        o_sub_parser = o_sub_parsers.add_parser("metadata", help="Métadonnées", epilog=s_epilog_metadata, formatter_class=argparse.RawTextHelpFormatter)
-        o_sub_parser.add_argument("--file", "-f", type=str, default=None, help="Chemin vers le fichier descriptor dont on veut effectuer la livraison)")
-        o_sub_parser.add_argument("--infos", "-i", type=str, default=None, help="Filtrer les livraisons selon les infos")
-        o_sub_parser.add_argument("--id", type=str, default=None, help="Affiche du fichier métadonnée demandée")
-        o_sub_parser.add_argument("--id-endpoint", type=str, default=None, metavar="ID_ENDPOINT", help="endpoint sur le quel est fait la publication ou la dépublication")
+        s_epilog_metadata = """Quatre types de lancement :
+        * livraison d'une métadonnée : `-f FICHIER`
+        * liste des métadonnées, avec filtre en option : `[--info filtre1=valeur1,filtre2=valeur2]`
+        * détail d'une métadonnée : `--id ID`
+        * publication / dépublication : `--publish NOM_FICHIER [NOM_FICHIER] --id-endpoint ID_ENDPOINT` et `--unpublish NOM_FICHIER [NOM_FICHIER] --id-endpoint ID_ENDPOINT`
+        """
+        o_sub_parser = o_sub_parsers.add_parser("metadata", help="Gestion des métadonnées", epilog=s_epilog_metadata, formatter_class=argparse.RawTextHelpFormatter)
+        o_sub_parser.add_argument("--file", "-f", type=str, default=None, help="Chemin vers le fichier de métadonnées que l'on veut téléverser)")
+        o_sub_parser.add_argument("--infos", "-i", type=str, default=None, help="Filtrer les métadonnées selon les infos")
+        o_sub_parser.add_argument("--id", type=str, default=None, help="Affiche la métadonnée demandée")
+        o_sub_parser.add_argument("--id-endpoint", type=str, default=None, metavar="ID_ENDPOINT", help="Point d'accès sur lequel est faite la publication ou la dépublication")
         o_sub_parser.add_argument(
-            "--publish", type=str, action="extend", nargs="+", default=None, metavar=("NOM_FICHIER"), help="publie les métadonnées listées sur le endpoint donné par --id-endpoint"
+            "--publish", type=str, action="extend", nargs="+", default=None, metavar=("NOM_FICHIER"), help="Publie les métadonnées listées sur le point d'accès donné par --id-endpoint"
         )
         o_sub_parser.add_argument(
-            "--unpublish", type=str, action="extend", nargs="+", default=None, metavar=("NOM_FICHIER"), help="dépublie les métadonnées listées sur le endpoint donné par --id-endpoint"
+            "--unpublish", type=str, action="extend", nargs="+", default=None, metavar=("NOM_FICHIER"), help="Dé-publie les métadonnées listées sur le point d'accès donné par --id-endpoint"
         )
 
         return o_parser.parse_args(args)
 
     def __datastore(self) -> Optional[str]:
         """Fonction pour récupérer l'id du datastore indiqué si l'utilisateur a indiqué son nom.
 
@@ -517,29 +518,29 @@
         """fonction callback pour la gestion du ctrl-C
         Renvoie un booléen d'arrêt de traitement. Si True, on doit arrêter le traitement.
         """
         # issues/9 :
         # sortie => sortie du monitoring, ne pas arrêter le traitement
         # stopper l’exécution de traitement => stopper le traitement (et donc le monitoring) [par défaut] (raise une erreur d'interruption volontaire)
         # ignorer / "erreur de manipulation" => reprendre le suivi
-        s_reponse = "rien"
-        while s_reponse not in ["a", "s", "c", ""]:
+        s_response = "rien"
+        while s_response not in ["a", "s", "c", ""]:
             Config().om.info(
                 "Vous avez taper ctrl-C. Que souhaitez-vous faire ?\n\
                                 \t* 'a' : pour sortir et <Arrêter> le traitement [par défaut]\n\
                                 \t* 's' : pour sortir <Sans arrêter> le traitement\n\
                                 \t* 'c' : pour annuler et <Continuer> le traitement"
             )
-            s_reponse = input().lower()
+            s_response = input().lower()
 
-        if s_reponse == "s":
+        if s_response == "s":
             Config().om.info("\t 's' : sortir <Sans arrêter> le traitement")
             sys.exit(0)
 
-        if s_reponse == "c":
+        if s_response == "c":
             Config().om.info("\t 'c' : annuler et <Continuer> le traitement")
             return False
 
         # on arrête le traitement
         Config().om.info("\t 'a' : sortir et <Arrêter> le traitement [par défaut]")
         return True
 
@@ -548,29 +549,29 @@
         """fonction callback pour la gestion du ctrl-C
         Renvoie un booléen d'arrêt de traitement. Si True, on doit arrêter le traitement.
         """
         # issues/9 :
         # sortie => sortie du monitoring, ne pas arrêter le traitement
         # stopper l’exécution de traitement => stopper le traitement (et donc le monitoring) [par défaut] (raise une erreur d'interruption volontaire)
         # ignorer / "erreur de manipulation" => reprendre le suivi
-        s_reponse = "rien"
-        while s_reponse not in ["a", "s", "c", ""]:
+        s_response = "rien"
+        while s_response not in ["a", "s", "c", ""]:
             Config().om.info(
                 "Vous avez taper ctrl-C. Que souhaitez-vous faire ?\n\
                                 \t* 'a' : pour sortir et <Arrêter> les vérifications [par défaut]\n\
                                 \t* 's' : pour sortir <Sans arrêter> les vérifications\n\
                                 \t* 'c' : pour annuler et <Continuer> les vérifications"
             )
-            s_reponse = input().lower()
+            s_response = input().lower()
 
-        if s_reponse == "s":
+        if s_response == "s":
             Config().om.info("\t 's' : sortir <Sans arrêter> les vérifications")
             sys.exit(0)
 
-        if s_reponse == "c":
+        if s_response == "c":
             Config().om.info("\t 'c' : annuler et <Continuer> les vérifications")
             return False
 
         # on arrête le traitement
         Config().om.info("\t 'a' : sortir et <Arrêter> les vérifications [par défaut]")
         return True
 
@@ -706,15 +707,15 @@
         elif self.o_args.publish_by_label is not None:
             l_labels = self.o_args.publish_by_label.split(",")
             i_nb = Annexe.publish_by_label(l_labels, datastore=self.datastore)
             Config().om.info(f"{i_nb} annexe(s) viennent d'être publié.")
         elif self.o_args.unpublish_by_label is not None:
             l_labels = self.o_args.unpublish_by_label.split(",")
             i_nb = Annexe.unpublish_by_label(l_labels, datastore=self.datastore)
-            Config().om.info(f"{i_nb} annexe(s) viennent d'être dépublié.")
+            Config().om.info(f"{i_nb} annexe(s) viennent d'être dépubliée(s).")
         else:
             # on liste toutes les annexes selon les filtres
             d_infos_filter = StoreEntity.filter_dict_from_str(self.o_args.infos)
             l_annexes = Annexe.api_list(infos_filter=d_infos_filter, datastore=self.datastore)
             for o_annexe in l_annexes:
                 Config().om.info(f"{o_annexe}")
 
@@ -813,21 +814,21 @@
             d_res = self.upload_metadata_from_descriptor_file(self.o_args.file, self.o_args.datastore)
             self._display_bilan_upload_file(d_res)
         elif self.o_args.id is not None:
             o_metadata = Metadata.api_get(self.o_args.id, datastore=self.datastore)
             # affichage
             Config().om.info(o_metadata.to_json(indent=3))
         elif (self.o_args.publish or self.o_args.unpublish) and self.o_args.id_endpoint is None:
-            raise GpfSdkError("Pour pubiler/depublier les métadonnées il faut définir --id-endpoint")
+            raise GpfSdkError("Pour publier / dépublier les métadonnées il faut définir --id-endpoint")
         elif self.o_args.publish is not None:
             Metadata.publish(self.o_args.publish, self.o_args.id_endpoint, self.o_args.datastore)
-            Config().om.info(f"Les métadonnées ont été publié sur le endpoint {self.o_args.id_endpoint}")
+            Config().om.info(f"Les métadonnées ont été publiées sur le endpoint {self.o_args.id_endpoint}")
         elif self.o_args.unpublish is not None:
             Metadata.unpublish(self.o_args.unpublish, self.o_args.id_endpoint, self.o_args.datastore)
-            Config().om.info(f"Les métadonnées ont été dépublié sur le endpoint {self.o_args.id_endpoint}")
+            Config().om.info(f"Les métadonnées ont été dépubliées sur le endpoint {self.o_args.id_endpoint}")
         else:
             # on liste toutes les fichiers métadonnées selon les filtres
             d_infos_filter = StoreEntity.filter_dict_from_str(self.o_args.infos)
             l_metadatas = Metadata.api_list(infos_filter=d_infos_filter, datastore=self.datastore)
             for o_metadata in l_metadatas:
                 Config().om.info(f"{o_metadata}")
```

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/default.ini` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_conf/default.ini`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/annexe_descriptor_file.json` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_conf/json_schemas/annexe_descriptor_file.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/metadata_descriptor_file.json` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_conf/json_schemas/metadata_descriptor_file.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/static_descriptor_file.json` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_conf/json_schemas/static_descriptor_file.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/upload_descriptor_file.json` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_conf/json_schemas/upload_descriptor_file.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999951774691359%*

 * *Differences: {"'properties'": "{'datasets': {'items': {'properties': {'upload_infos': {'properties': "*

 * *                 "{'type_infos': OrderedDict([('type', 'object')])}}}}}}"}*

```diff
@@ -28,14 +28,17 @@
                                 "type": "string"
                             },
                             "srs": {
                                 "type": "string"
                             },
                             "type": {
                                 "type": "string"
+                            },
+                            "type_infos": {
+                                "type": "object"
                             }
                         },
                         "required": [
                             "description",
                             "name",
                             "srs",
                             "type"
```

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_conf/json_schemas/workflow.json` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_conf/json_schemas/workflow.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999979964825%*

 * *Differences: {"'properties'": "{'workflow': {'properties': {'steps': {'additionalProperties': {'properties': "*

 * *                 "{'actions': {'items': {'properties': {'reset_bbox': OrderedDict([('type', "*

 * *                 "'boolean')])}}}}}}}}}"}*

```diff
@@ -75,14 +75,17 @@
                                                 "error"
                                             ],
                                             "type": "string"
                                         },
                                         "not_found_ok": {
                                             "type": "boolean"
                                         },
+                                        "reset_bbox": {
+                                            "type": "boolean"
+                                        },
                                         "tags": {
                                             "type": "object"
                                         },
                                         "type": {
                                             "enum": [
                                                 "delete-entity",
                                                 "processing-execution",
```

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.prj` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.prj`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shp` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shx` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON_style.sld` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/CANTON_style.sld`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/1_dataset_vector/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON/CANTON.zip` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/CANTON/CANTON.zip`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/2_dataset_archive/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/installation.sld` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/installation.sld`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_2/installation.gpkg` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_2/installation.gpkg`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csv` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/lot_3/installation.csv`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/datasets/5_dataset_maj_bd_gpf/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_joincache.jsonc` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/workflows/generic_joincache.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_maj_bdd.jsonc` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/workflows/generic_maj_bdd.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_moissonnage.jsonc` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/workflows/generic_moissonnage.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_raster.jsonc` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/workflows/generic_raster.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/_data/workflows/generic_vecteur.jsonc` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/_data/workflows/generic_vecteur.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/auth/Authentifier.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/auth/Authentifier.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/auth/Token.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/auth/Token.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/FileHelper.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/helper/FileHelper.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/JsonHelper.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/helper/JsonHelper.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/helper/PrintLogHelper.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/helper/PrintLogHelper.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/ApiRequester.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/ApiRequester.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Color.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/Color.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Config.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/Config.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Dataset.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/Dataset.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/DescriptorFileReader.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/DescriptorFileReader.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/Errors.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/Errors.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/JsonConverter.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/JsonConverter.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/OutputManager.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/OutputManager.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/io/UploadDescriptorFileReader.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/io/UploadDescriptorFileReader.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/pattern/SingleInstance.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/pattern/SingleInstance.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/pattern/Singleton.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/pattern/Singleton.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/AbstractCommonFile.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/AbstractCommonFile.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Annexe.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Annexe.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/CheckExecution.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/CheckExecution.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Configuration.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Configuration.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Datastore.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Datastore.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Endpoint.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Endpoint.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Metadata.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Metadata.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Offering.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Offering.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/ProcessingExecution.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/ProcessingExecution.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Static.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Static.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/StoreEntity.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/StoreEntity.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/StoredData.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/StoredData.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/Upload.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/Upload.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/User.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/User.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/__init__.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/__init__.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/CommentInterface.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/CommentInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/CreatedByUploadFileInterface.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/CreatedByUploadFileInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/CsfInterface.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/CsfInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/DownloadInterface.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/DownloadInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/EventInterface.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/EventInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/FullEditInterface.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/FullEditInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/PartialEditInterface.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/PartialEditInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/ReUploadFileInterface.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/ReUploadFileInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/SharingInterface.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/SharingInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/store/interface/TagInterface.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/store/interface/TagInterface.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/Errors.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/Errors.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/Workflow.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/Workflow.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/ActionAbstract.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/ActionAbstract.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         __parent_action (Optional["Action"]): action parente
     """
 
     # comportements possibles (que peut écrire l'utilisateur)
     BEHAVIOR_STOP = "STOP"
     BEHAVIOR_DELETE = "DELETE"
     BEHAVIOR_CONTINUE = "CONTINUE"
+    BEHAVIOR_RESUME = "RESUME"
 
     def __init__(self, workflow_context: str, definition_dict: Dict[str, Any], parent_action: Optional["ActionAbstract"] = None) -> None:
         super().__init__()
         self.__workflow_context: str = workflow_context
         self.__definition_dict: Dict[str, Any] = definition_dict
         self.__parent_action: Optional["ActionAbstract"] = parent_action
```

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/ConfigurationAction.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/ConfigurationAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/CopyConfigurationAction.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/CopyConfigurationAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/DeleteAction.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/DeleteAction.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,7 +102,8 @@
             l_entities = l_entities_cascade
 
         # choix de la fonction d'affichage.
         o_before_delete = self.question_before_delete if self.definition_dict.get("confirm", True) else self.print_before_delete
 
         # suppression
         StoreEntity.delete_liste_entities(l_entities, o_before_delete)
+        Config().om.info("Suppression : terminé")
```

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/EditAction.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/EditAction.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,26 +21,29 @@
         __definition_dict (Dict[str, Any]): définition de l'action
         __parent_action (Optional["Action"]): action parente
     """
 
     UPDATABLE_TYPES = [Upload.entity_name(), StoredData.entity_name(), Configuration.entity_name(), Offering.entity_name()]
 
     def run(self, datastore: Optional[str] = None) -> None:
-        Config().om.info("Suppression...")
+        Config().om.info("Edition ...")
         if "entity_type" not in self.definition_dict:
             raise StepActionError('La clef "entity_type" est obligatoire pour cette action')
         if self.definition_dict["entity_type"] not in EditAction.UPDATABLE_TYPES:
             raise StepActionError(f"Type {self.definition_dict['entity_type']} non reconnu. Types valides : {', '.join(EditAction.UPDATABLE_TYPES)}")
         if not self.definition_dict.get("entity_id"):
             raise StepActionError('La clef "entity_id" est obligatoire pour cette action.')
         o_entity: StoreEntity = store.TYPE__ENTITY[self.definition_dict["entity_type"]].api_get(self.definition_dict["entity_id"], datastore=datastore)
 
+        Config().om.info(f"Edition de {o_entity}.")
+
         # Lancement de la mise à jour si demandé
         if self.definition_dict.get("body_parameters"):
             o_entity.edit(self.definition_dict["body_parameters"])
+            Config().om.info(f"Mise à jour de {o_entity} .")
 
         # ajout des tags si possible
         if self.definition_dict.get("tags") and isinstance(o_entity, TagInterface):
             Config().om.info(f"ajout des {len(self.definition_dict['tags'])} tags...")
             o_entity.api_add_tags(self.definition_dict["tags"])
             Config().om.info(f"les {len(self.definition_dict['tags'])} tags ont été ajoutés avec succès.")
         # ajout des commentaires si possible
@@ -48,7 +51,8 @@
             l_actual_comments = [d_comment["text"] for d_comment in o_entity.api_list_comments() if d_comment]
             Config().om.info(f"Ajout des {len(self.definition_dict['comments'])} commentaires...")
             for s_comment in self.definition_dict["comments"]:
                 # si le commentaire n'existe pas déjà on l'ajoute
                 if s_comment not in l_actual_comments:
                     o_entity.api_add_comment({"text": s_comment})
             Config().om.info(f"Les {len(self.definition_dict['comments'])} commentaires ont été ajoutés avec succès.")
+        Config().om.info("Edition : terminé")
```

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/EditUsedDataConfigurationAction.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/EditUsedDataConfigurationAction.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,19 +29,23 @@
         # ajout des used_data
         if self.definition_dict.get("append_used_data"):
             l_new_use_data.extend(self.definition_dict["append_used_data"])
 
         # enregistrement de la modification
         d_parameter["type_infos"]["used_data"] = l_new_use_data
 
+        # suppression de la bbox pour qu'elle soit mise à jour avec les données
+        if self.definition_dict.get("reset_bbox", False) and "bbox" in d_parameter["type_infos"]:
+            del d_parameter["type_infos"]["bbox"]
+
         # lancement de la modification
         Config().om.info(f"Modification de la configuration {o_base_config} ...")
 
         o_base_config.api_full_edit(d_parameter)
-        Config().om.info("Modification de la configuration : terminé", green_colored=True)
+        Config().om.info("Modification de la configuration : terminé")
 
     def _delete_used_data(self, d_data_delete: Dict[str, str], l_used_data: List[Dict[str, Any]]) -> List[Dict[str, Any]]:
         l_new_use_data = []
         for d_data in l_used_data:
             b_keep = True
             # Si on a une totale correspondance on supprime
             for s_key, s_val in d_data_delete.items():
```

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/OfferingAction.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/OfferingAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/PermissionAction.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/PermissionAction.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/ProcessingExecutionAction.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/ProcessingExecutionAction.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,22 @@
         __definition_dict (Dict[str, Any]): définition de l'action
         __parent_action (Optional["Action"]): action parente
         __processing_execution (Optional[ProcessingExecution]): représentation Python de l'exécution de traitement créée
         __Upload (Optional[Upload]): représentation Python de la livraison en sortie (null si donnée stockée en sortie)
         __StoredData (Optional[StoredData]): représentation Python de la donnée stockée en sortie (null si livraison en sortie)
     """
 
+    # Comportements possibles pour une ProcessingExecutionAction
+    BEHAVIORS = [
+        ActionAbstract.BEHAVIOR_STOP,
+        ActionAbstract.BEHAVIOR_DELETE,
+        ActionAbstract.BEHAVIOR_CONTINUE,
+        ActionAbstract.BEHAVIOR_RESUME,
+    ]
+
     # status possibles d'une ProcessingExecution (status délivrés par l'api)
     # STATUS_CREATED
     # STATUS_ABORTED STATUS_SUCCESS STATUS_FAILURE
 
     # status possibles d'une Stored data (status délivrés par l'api)
     # STATUS_CREATED
     # STATUS_UNSTABLE
@@ -69,25 +77,27 @@
             # On vérifie si une Donnée Stockée équivalente à celle du dictionnaire de définition (champ name) existe déjà sur la gpf
             o_stored_data = self.find_stored_data(datastore)
             # Si on a trouvé une Donnée Stockée sur la gpf :
             if o_stored_data is not None:
                 # Comportement d'arrêt du programme
                 if self.__behavior == self.BEHAVIOR_STOP:
                     raise GpfSdkError(f"Impossible de créer l’exécution de traitement, une donnée stockée en sortie équivalente {o_stored_data} existe déjà.")
+
+                # on met à jour o_stored_data pour avoir son status
+                o_stored_data.api_update()
                 # Comportement de suppression des entités détectées
-                if self.__behavior == self.BEHAVIOR_DELETE:
+                if self.__behavior == self.BEHAVIOR_DELETE or (o_stored_data["status"] == StoredData.STATUS_UNSTABLE and self.__behavior == self.BEHAVIOR_RESUME):
                     Config().om.warning(f"Une donnée stockée équivalente à {o_stored_data} va être supprimée puis recréée.")
                     # Suppression de la donnée stockée
                     o_stored_data.api_delete()
                     # on force à None pour que la création soit faite
                     self.__processing_execution = None
                 # Comportement "on continue l'exécution"
-                elif self.__behavior == self.BEHAVIOR_CONTINUE:
-                    o_stored_data.api_update()
-                    # on regarde si le résultat du traitement précédent est en échec
+                elif self.__behavior in [self.BEHAVIOR_CONTINUE, self.BEHAVIOR_RESUME]:
+                    # on regarde si le résultat du traitement précédent est en échec (cas pour self.BEHAVIOR_RESUME, déjà traité)
                     if o_stored_data["status"] == StoredData.STATUS_UNSTABLE:
                         raise GpfSdkError(f"Le traitement précédent a échoué sur la donnée stockée en sortie {o_stored_data}. Impossible de lancer le traitement demandé.")
 
                     # on est donc dans un des cas suivants :
                     # le processing_execution a été créé mais pas exécuté (StoredData.STATUS_CREATED)
                     # ou le processing execution est en cours d'exécution (StoredData.STATUS_GENERATING ou StoredData.STATUS_MODIFYING)
                     # ou le processing execution est terminé (StoredData.STATUS_GENERATED)
@@ -97,17 +107,15 @@
                         raise GpfSdkError(f"Impossible de trouver l'exécution de traitement liée à la donnée stockée {o_stored_data}")
                     # arbitrairement, on prend le premier de la liste
                     self.__processing_execution = l_proc_exec[0]
                     Config().om.info(f"La donnée stocké en sortie {o_stored_data} déjà existante, on reprend le traitement associé : {self.__processing_execution}.")
                     return
                 # Comportement non reconnu
                 else:
-                    raise GpfSdkError(
-                        f"Le comportement {self.__behavior} n'est pas reconnu ({self.BEHAVIOR_STOP}|{self.BEHAVIOR_DELETE}|{self.BEHAVIOR_CONTINUE}), l'exécution de traitement n'est pas possible."
-                    )
+                    raise GpfSdkError(f"Le comportement {self.__behavior} n'est pas reconnu ({'|'.join(self.BEHAVIORS)}), l'exécution de traitement n'est pas possible.")
 
         # A ce niveau là, si on a encore self.__processing_execution qui est None, c'est qu'on peut créer l'Exécution de Traitement sans problème
         if self.__processing_execution is None:
             # création de la ProcessingExecution
             self.__processing_execution = ProcessingExecution.api_create(self.definition_dict["body_parameters"], {"datastore": datastore})
             d_info = self.__processing_execution.get_store_properties()["output"]
 
@@ -174,15 +182,15 @@
         if self.processing_execution is None:
             raise StepActionError("Aucune exécution de traitement trouvée. Impossible de lancer le traitement")
 
         if self.processing_execution["status"] == ProcessingExecution.STATUS_CREATED:
             Config().om.info(f"Exécution de traitement {self.processing_execution['processing']['name']} : lancement...")
             self.processing_execution.api_launch()
             Config().om.info(f"Exécution de traitement {self.processing_execution['processing']['name']} : lancée avec succès.")
-        elif self.__behavior == self.BEHAVIOR_CONTINUE:
+        elif self.__behavior in [self.BEHAVIOR_CONTINUE, self.BEHAVIOR_RESUME]:
             Config().om.info(f"Exécution de traitement {self.processing_execution['processing']['name']} : déjà lancée.")
         else:
             # processing_execution est déjà lancé ET le __behavior n'est pas en "continue", on ne devrait pas être ici :
             raise StepActionError("L'exécution de traitement est déjà lancée.")
 
     def find_stored_data(self, datastore: Optional[str] = None) -> Optional[StoredData]:
         """Fonction permettant de récupérer une Stored Data ressemblant à celle qui devrait être créée par
```

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/SynchronizeOfferingAction.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/SynchronizeOfferingAction.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
             datastore (Optional[str], optional): surcharge du datastore, sinon utilisation de celui par défaut. Defaults to None.
 
         Raises:
             StepActionError: Aucune offre trouvée pour la synchronisation
             StepActionError: Plusieurs offres trouvées pour la synchronisation (uniquement si "if_multi" == "error")
             StepActionError: La synchronisation d'au moins une offre est terminée en erreur
         """
-        Config().om.info("Synchronisation d'une offre...")
+        Config().om.info("Synchronisation d'offres ...")
         # récupération des offres
         l_offering = self._find_offerings(datastore)
         # gestion des cas particuliers
         if len(l_offering) == 0:
             raise StepActionError("Aucune offre trouvée pour la synchronisation")
         if len(l_offering) > 1:
             if self.definition_dict.get("if_multi") == "error":
@@ -131,7 +131,8 @@
                     l_errors.append(f"Synchronisation de {o_offering} : terminé en erreur.")
                     break
                 # on fixe à 1 seconde, normalement quasiment instantané
                 Config().om.debug(f"Status : '{s_status}', on attend ...")
                 time.sleep(1)
         if l_errors:
             raise StepActionError("La synchronisation d'au moins une offre est terminée en erreur \n * " + "\n * ".join(l_errors))
+        Config().om.info("Synchronisation d'offres : terminé")
```

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/action/UploadAction.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/action/UploadAction.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,15 @@
                 # cas livraison fermé : message particulier
                 if not o_upload.is_open():
                     Config().om.warning(f"Livraison identique {o_upload} trouvée et fermée, cette livraison ne sera pas mise à jour.")
                 else:
                     Config().om.info(f"Livraison identique {o_upload} trouvée, le programme va la reprendre et la compléter.")
                 self.__upload = o_upload
             else:
-                raise GpfSdkError(f"Le comportement {self.__behavior} n'est pas reconnu, l'exécution de traitement est annulée.")
+                raise GpfSdkError(f"Le comportement {self.__behavior} n'est pas reconnu ({'|'.join(self.BEHAVIORS)}), l'exécution de traitement est annulée.")
         else:
             # Si la livraison est nulle, on en crée une nouvelle (on utilise les champs de "upload_infos" du dataset)
             self.__upload = Upload.api_create(self.__dataset.upload_infos, route_params={"datastore": datastore})
             Config().om.info(f"Livraison {self.__upload['name']} créée avec succès.")
 
     def __add_tags(self) -> None:
         """Ajoute les tags."""
@@ -178,15 +178,15 @@
             nom (str): non du ficher md5
         """
         if self.__upload is None:
             raise GpfSdkError(f"Aucune livraison de définie - impossible de livrer {nom}")
         self.__upload.api_push_md5_file(path)
 
     def __push_files(self, l_files: List[Tuple[Path, str]], f_api_push: Callable[[Path, str], None], f_api_delete: Callable[[str], None], check_conflict: bool = True) -> int:
-        """pousse un ficher de données ou un ficher md5 sur le store. Gére la reprise de Livraison et les conflicts lors de la livraison.
+        """pousse un ficher de données ou un ficher md5 sur le store. Gère la reprise de Livraison et les conflicts lors de la livraison.
 
         Args:
             l_files (List[Tuple[Path, str]]): liste de tuple Path du ficher à livre, nom du ficher sous la gpf
             f_api_push (Callable[[Path, str], None]): fonction pour livrer les données
             f_api_delete (Callable[[str], None]): fonction pour supprimé les données si livrer partiellement.
             check_conflict (bool): Si une vérification de la bonne livraison des fichier en conflict ou en timeout est lancée..
```

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/AbstractResolver.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/AbstractResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/DateResolver.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/DateResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/DictResolver.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/DictResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/DumbResolver.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/DumbResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/Errors.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/Errors.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/FileResolver.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/FileResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/GlobalResolver.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/GlobalResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/StoreEntityResolver.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/StoreEntityResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/sdk_entrepot_gpf/workflow/resolver/UserResolver.py` & `sdk_entrepot_gpf-0.1.27/sdk_entrepot_gpf/workflow/resolver/UserResolver.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/ErrorsTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/GpfTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/GpfTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/MainTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/MainTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/_conf/test_requester.ini` & `sdk_entrepot_gpf-0.1.27/tests/_conf/test_requester.ini`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf` & `sdk_entrepot_gpf-0.1.27/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp` & `sdk_entrepot_gpf-0.1.27/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx` & `sdk_entrepot_gpf-0.1.27/tests/_data/datasets/2_test_dataset_bad_md5/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.27/tests/_data/datasets/2_test_dataset_bad_md5/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf` & `sdk_entrepot_gpf-0.1.27/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.dbf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp` & `sdk_entrepot_gpf-0.1.27/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shp`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx` & `sdk_entrepot_gpf-0.1.27/tests/_data/datasets/3_test_dataset_sub_dir/CANTON/CANTON.shx`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json` & `sdk_entrepot_gpf-0.1.27/tests/_data/datasets/3_test_dataset_sub_dir/upload_descriptor.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/_data/workflows/bad-workflow.jsonc` & `sdk_entrepot_gpf-0.1.27/tests/_data/workflows/bad-workflow.jsonc`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/_test/helper/JsonHelper/schema.json` & `sdk_entrepot_gpf-0.1.27/tests/_test/helper/JsonHelper/schema.json`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/auth/AuthentifierTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/auth/AuthentifierTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/auth/TokenTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/auth/TokenTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/helper/FileHelperTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/helper/FileHelperTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/helper/JsonHelperTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/helper/JsonHelperTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/io/ApiRequesterTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/io/ApiRequesterTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/io/ConfigTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/io/ConfigTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/io/DatasetTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/io/DatasetTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/io/ErrorsTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/io/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/io/JsonConverterTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/io/JsonConverterTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/io/UploadDescriptorFileReaderTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/io/UploadDescriptorFileReaderTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/AbstractCommonFileTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/AbstractCommonFileTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/AnnexeTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/AnnexeTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/CheckExecutionTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/MetadataTestCase.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,52 @@
-from typing import Any, Dict, List
 from unittest.mock import patch
 
 from sdk_entrepot_gpf.io.ApiRequester import ApiRequester
-from sdk_entrepot_gpf.store.CheckExecution import CheckExecution
+from sdk_entrepot_gpf.store.Metadata import Metadata
 from tests.GpfTestCase import GpfTestCase
 
 
-class CheckExecutionTestCase(GpfTestCase):
-    """Tests CheckExecution class.
+class MetadataTestCase(GpfTestCase):
+    """Tests Metadata class.
 
-    cmd : python3 -m unittest -b tests.store.CheckExecutionTestCase
+    cmd : python3 -m unittest -b tests.store.MetadataTestCase
     """
 
-    def test_api_logs(self) -> None:
-        "Vérifie le bon fonctionnement de api_logs."
-        s_data = "2022/05/18 14:29:25       INFO §USER§ Envoi du signal de début de l'exécution à l'API.\n2022/05/18 14:29:25       INFO §USER§ Signal transmis avec succès."
-        l_rep: List[Dict[str, Any]] = [
-            {"datastore": "datastore_id", "data": s_data.split("\n"), "rep": s_data},
-            {"datastore": "datastore_id", "data": "", "rep": ""},
-            {"datastore": "datastore_id", "data": [], "rep": ""},
-            {"datastore": "datastore_id", "data": ["log1", "log2", ' log "complexe"'], "rep": 'log1\nlog2\n log "complexe"'},
-        ]
+    def test_publish(self) -> None:
+        "Vérifie le bon fonctionnement de publish."
+        l_file = ["a", "b", "c"]
+        s_endpoint_id = "hdsfkhdlfh"
 
-        for d_rep in l_rep:
-            o_response = GpfTestCase.get_response(json=d_rep["data"])
+        for s_datastore in [None, "publish"]:
             # On mock la fonction route_request, on veut vérifier qu'elle est appelée avec les bons params
+            o_response = GpfTestCase.get_response()
             with patch.object(ApiRequester, "route_request", return_value=o_response) as o_mock_request:
-                # on appelle la fonction à tester : api_logs
-                o_check_execution = CheckExecution({"_id": "id_entité"}, datastore=d_rep["datastore"])
-                s_data_recupere = o_check_execution.api_logs()
+                # on appelle la fonction à tester : publish
+                Metadata.publish(l_file, s_endpoint_id, s_datastore)
+
+                # on vérifie que route_request est appelé correctement
+                o_mock_request.assert_called_once_with(
+                    "metadata_publish",
+                    route_params={"datastore": s_datastore},
+                    data={"file_identifiers": l_file, "endpoint": s_endpoint_id},
+                    method=ApiRequester.POST,
+                )
+
+    def test_unpublish(self) -> None:
+        "Vérifie le bon fonctionnement de unpublish."
+        l_file = ["a", "b", "c"]
+        s_endpoint_id = "hdsfkhdlfh"
+
+        for s_datastore in [None, "unpublish"]:
+            # On mock la fonction route_request, on veut vérifier qu'elle est appelée avec les bons params
+            o_response = GpfTestCase.get_response()
+            with patch.object(ApiRequester, "route_request", return_value=o_response) as o_mock_request:
+                # on appelle la fonction à tester : unpublish
+                Metadata.unpublish(l_file, s_endpoint_id, s_datastore)
+
                 # on vérifie que route_request est appelé correctement
                 o_mock_request.assert_called_once_with(
-                    "check_execution_logs",
-                    route_params={"datastore": d_rep["datastore"], "check_execution": "id_entité"},
+                    "metadata_unpublish",
+                    route_params={"datastore": s_datastore},
+                    data={"file_identifiers": l_file, "endpoint": s_endpoint_id},
+                    method=ApiRequester.POST,
                 )
-                # on vérifie la similitude des données retournées
-                self.assertEqual(d_rep["rep"], s_data_recupere)
```

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/ConfigurationTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/ConfigurationTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/DatastoreTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/DatastoreTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/EndpointTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/EndpointTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/ErrorsTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/ErrorsTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/OfferingTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/OfferingTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/StoreEntityTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/StoreEntityTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/StoredDataTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/StoredDataTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/UploadTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/UploadTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/interface/CommentInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/interface/CommentInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/interface/CreatedByUploadFileInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/interface/CreatedByUploadFileInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/interface/CsfInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/interface/CsfInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/interface/DownloadInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/interface/DownloadInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/interface/EventInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/interface/EventInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/interface/FullEditInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/interface/FullEditInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/interface/PartialEditInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/interface/PartialEditInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/interface/ReUploadFileInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/interface/ReUploadFileInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/interface/SharingInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/interface/SharingInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/store/interface/TagInterfaceTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/store/interface/TagInterfaceTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/WorkflowTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/WorkflowTestCase.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,15 +421,15 @@
 
     def test_open_workflow(self) -> None:
         """Test de la fonction open_workflow."""
         p_workflows = Config().data_dir_path / "workflows"
         # On teste le workflow generic_archive.jsonc
         o_workflow_1 = Workflow.open_workflow(p_workflows / "generic_archive.jsonc")
         self.assertEqual(o_workflow_1.name, "generic_archive.jsonc")
-        self.assertEqual(len(o_workflow_1.steps), 3)
+        self.assertEqual(len(o_workflow_1.steps), 4)
         # On teste le workflow generic_vecteur.jsonc
         o_workflow_2 = Workflow.open_workflow(p_workflows / "generic_vecteur.jsonc", "wfs generic")
         self.assertEqual(o_workflow_2.name, "wfs generic")
         self.assertEqual(len(o_workflow_2.steps), 8)
         # On teste un fichier inexistant
         with self.assertRaises(GpfSdkError) as o_arc:
             Workflow.open_workflow(Path("pas_là.json"))
@@ -458,16 +458,17 @@
         self.assertEqual(l_errors[3], "L'action n°1 de l'étape « configuration-wfs » n'est pas instantiable (Aucune correspondance pour ce type d'action : type-not-found).")
         self.assertEqual(l_errors[4], "L'action n°2 de l'étape « configuration-wfs » n'a pas la clef obligatoire ('type').")
         ## cas erreur non valide
         with patch.object(Workflow, "generate", side_effect=Exception("error")) as o_mock_jsonschema:
             l_errors = o_workflow_1.validate()
             self.assertTrue(l_errors)
             self.assertEqual(l_errors[0], "L'action n°1 de l'étape « intégration-archive-livrée » lève une erreur inattendue (error).")
-            self.assertEqual(l_errors[1], "L'action n°1 de l'étape « configuration-archive-livrée » lève une erreur inattendue (error).")
-            self.assertEqual(l_errors[2], "L'action n°1 de l'étape « publication-archive-livrée » lève une erreur inattendue (error).")
+            self.assertEqual(l_errors[1], "L'action n°1 de l'étape « patch-donnée-stockée » lève une erreur inattendue (error).")
+            self.assertEqual(l_errors[2], "L'action n°1 de l'étape « configuration-archive-livrée » lève une erreur inattendue (error).")
+            self.assertEqual(l_errors[3], "L'action n°1 de l'étape « publication-archive-livrée » lève une erreur inattendue (error).")
 
         # problème avec le schema du fichier workflow
         p_schema = Config.conf_dir_path / "json_schemas" / "workflow.json"
         with patch.object(jsonschema, "validate", side_effect=jsonschema.exceptions.SchemaError("error")) as o_mock_jsonschema:
             with self.assertRaises(GpfSdkError) as o_arc:
                 o_workflow_2.validate()
             self.assertEqual(o_arc.exception.message, f"Le schéma décrivant la structure d'un workflow {p_schema} est invalide. Contactez le support.")
```

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/action/ActionAbstractTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/action/ActionAbstractTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/action/ConfigurationActionTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/action/ConfigurationActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/action/CopyConfigurationActionTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/action/CopyConfigurationActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/action/DeleteActionTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/action/DeleteActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/action/EditActionTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/action/EditActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/action/OfferingActionTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/action/OfferingActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/action/PermissionActionTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/action/PermissionActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/action/ProcessingExecutionActionTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/action/ProcessingExecutionActionTestCase.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 # fmt: off
 class ProcessingExecutionActionTestCase(GpfTestCase):
     """Tests ProcessingExecutionAction class.
 
     cmd : python3 -m unittest -b tests.workflow.action.ProcessingExecutionActionTestCase
     """
 
+    i = 0
+
     def test_find_stored_data(self) -> None:
         """Test find_stored_data."""
         o_pe1 = ProcessingExecution({"_id": "pe_1"})
         o_pe2 = ProcessingExecution({"_id": "pe_2"})
         # création du dict décrivant l'action
         d_action:Dict[str, Any] = {
             "type": "processing-execution",
@@ -49,14 +51,23 @@
                 with patch.object(StoredData, "api_list", return_value=[o_pe1, o_pe2]) as o_mock_api_list :
                     # Appel de la fonction find_stored_data
                     o_stored_data = o_ua.find_stored_data(s_datastore)
                     # Vérifications
                     o_mock_get_filters.assert_called_once_with("processing_execution", d_action["body_parameters"]["output"]["stored_data"], d_action["tags"])
                     o_mock_api_list.assert_called_once_with(infos_filter={"info":"val"}, tags_filter={"tag":"val"}, datastore=s_datastore)
                     self.assertEqual(o_stored_data, o_pe1)
+        # pas de stored data trouvé
+        with patch.object(ActionAbstract, "get_filters", return_value=({"info":"val"}, {"tag":"val"})) as o_mock_get_filters:
+            with patch.object(StoredData, "api_list", return_value=[]) as o_mock_api_list :
+                # Appel de la fonction find_stored_data
+                o_stored_data = o_ua.find_stored_data(s_datastore)
+                # Vérifications
+                o_mock_get_filters.assert_called_once_with("processing_execution", d_action["body_parameters"]["output"]["stored_data"], d_action["tags"])
+                o_mock_api_list.assert_called_once_with(infos_filter={"info":"val"}, tags_filter={"tag":"val"}, datastore=s_datastore)
+                self.assertEqual(o_stored_data, None)
 
     def run_args(self,
         tags: Optional[Dict[str,Any]],
         comments: Optional[List[str]],
         s_key: str,
         s_type_output: str,
         datastore: Optional[str],
@@ -66,184 +77,296 @@
         """lancement + test de ProcessingExecutionAction.run selon param
 
         Args:
             tags (Optional[Dict[str, Any]]): dictionnaire des tags ou None
             comments (Optional[List]): liste des commentaires ou None
             s_type_output (str): type de l'output (stored_data ou upload)
         """
-        d_action: Dict[str, Any] = {"type": "processing-execution", "body_parameters":{"output":{s_key:"test"}}}
-        if tags is not None:
-            d_action["tags"] = tags
-        if comments is not None:
-            d_action["comments"] = comments
-
-        # initialisation de ProcessingExecutionAction
-        o_pea = ProcessingExecutionAction("contexte", d_action, behavior=behavior)
+        self.i += 1
+        with self.subTest(i=self.i):
+            d_action: Dict[str, Any] = {"type": "processing-execution", "body_parameters":{"output":{s_key:"test"}}}
+            if tags is not None:
+                d_action["tags"] = tags
+            if comments is not None:
+                d_action["comments"] = comments
+
+            # initialisation de ProcessingExecutionAction
+            o_pea = ProcessingExecutionAction("contexte", d_action, behavior=behavior)
+
+            # mock de processing execution
+            d_store_properties = {"output": {s_type_output: {"_id": "id"}}}
+            o_mock_processing_execution = MagicMock()
+            o_mock_processing_execution.get_store_properties.return_value = d_store_properties
+            o_mock_processing_execution.api_launch.return_value = None
+            # o_mock_processing_execution.__getitem__.return_value = ProcessingExecution.STATUS_CREATED
+            # ça veut dire que : o_mock_processing_execution["quelchechose"] = "CREATED"
+            def get_items_processing(key:str) -> Any:
+                if key == "status":
+                    return "CREATED"
+                return MagicMock()
+            o_mock_processing_execution.__getitem__.side_effect = get_items_processing
+
+            # mock de upload d'entrée
+            o_mock_upload = MagicMock()
+            o_mock_upload.api_add_tags.return_value = None
+            o_mock_upload.api_add_comment.return_value = None
+
+            # mock de stored_data d'entrée
+            o_mock_stored_data = MagicMock()
+            o_mock_stored_data.api_add_tags.return_value = None
+            o_mock_stored_data.api_add_comment.return_value = None
 
-        # mock de processing execution
-        d_store_properties = {"output": {s_type_output: {"_id": "id"}}}
-        o_mock_processing_execution = MagicMock()
-        o_mock_processing_execution.get_store_properties.return_value = d_store_properties
-        o_mock_processing_execution.api_launch.return_value = None
-        # o_mock_processing_execution.__getitem__.return_value = ProcessingExecution.STATUS_CREATED
-        # ça veut dire que : o_mock_processing_execution["quelchechose"] = "CREATED"
-        def get_items_processing(key:str) -> Any:
-            if key == "status":
-                return "CREATED"
-            return MagicMock()
-        o_mock_processing_execution.__getitem__.side_effect = get_items_processing
-
-        # mock de upload d'entrée
-        o_mock_upload = MagicMock()
-        o_mock_upload.api_add_tags.return_value = None
-        o_mock_upload.api_add_comment.return_value = None
-
-        # mock de stored_data d'entrée
-        o_mock_stored_data = MagicMock()
-        o_mock_stored_data.api_add_tags.return_value = None
-        o_mock_stored_data.api_add_comment.return_value = None
-
-        # résultat de ProcessingExecutionAction."find_stored_data" : stored_data de sortie
-        o_exist_output = None
-        if output_already_exist:
-            o_mock_exist_output = MagicMock()
-            o_mock_exist_output.api_delete.return_value = None
-            o_exist_output = o_mock_exist_output
-
-        # suppression de la mise en page forcée pour le with
-        with patch.object(Upload, "api_get", return_value=o_mock_upload) as o_mock_upload_api_get, \
-            patch.object(StoredData, "api_get", return_value=o_mock_stored_data) as o_mock_stored_data_api_get, \
-            patch.object(ProcessingExecution, "api_create", return_value=o_mock_processing_execution) as o_mock_pe_api_create, \
-            patch.object(ProcessingExecution, "api_list", return_value=[o_mock_processing_execution]) as o_mock_pe_api_list, \
-            patch.object(ProcessingExecutionAction, "find_stored_data", return_value=o_exist_output) as o_mock_pea_find_stored_data, \
-            patch.object(ProcessingExecutionAction, "output_new_entity", new_callable=PropertyMock, return_value=output_already_exist), \
-            patch.object(Config, "get_str", return_value="STOP") \
-        :
-            # dans le cas où une entité existe déjà dans la gpf :
+            # résultat de ProcessingExecutionAction."find_stored_data" : stored_data de sortie
+            o_exist_output = None
             if output_already_exist:
-                if not behavior or behavior == "STOP":
-                    # on attend une erreur
-                    with self.assertRaises(GpfSdkError) as o_err:
-                        o_pea.run(datastore)
-                    self.assertEqual(o_err.exception.message, f"Impossible de créer l’exécution de traitement, une donnée stockée en sortie équivalente {o_exist_output} existe déjà.")
-                    return
+                o_mock_exist_output = MagicMock()
+                o_mock_exist_output.api_delete.return_value = None
+                o_exist_output = o_mock_exist_output
+
+            # suppression de la mise en page forcée pour le with
+            with patch.object(Upload, "api_get", return_value=o_mock_upload) as o_mock_upload_api_get, \
+                patch.object(StoredData, "api_get", return_value=o_mock_stored_data) as o_mock_stored_data_api_get, \
+                patch.object(ProcessingExecution, "api_create", return_value=o_mock_processing_execution) as o_mock_pe_api_create, \
+                patch.object(ProcessingExecution, "api_list", return_value=[o_mock_processing_execution]) as o_mock_pe_api_list, \
+                patch.object(ProcessingExecutionAction, "find_stored_data", return_value=o_exist_output) as o_mock_pea_find_stored_data, \
+                patch.object(ProcessingExecutionAction, "output_new_entity", new_callable=PropertyMock, return_value=output_already_exist), \
+                patch.object(Config, "get_str", return_value="STOP") \
+            :
+                # dans le cas où une entité existe déjà dans la gpf :
+                if output_already_exist:
+                    if not behavior or behavior == "STOP":
+                        # on attend une erreur
+                        with self.assertRaises(GpfSdkError) as o_err:
+                            o_pea.run(datastore)
+                        self.assertEqual(o_err.exception.message, f"Impossible de créer l’exécution de traitement, une donnée stockée en sortie équivalente {o_exist_output} existe déjà.")
+                        return
 
-                if behavior == "DELETE":
-                    # suppression de l'existant puis normal
-                    ### @Ludivine, ça veut dire quoi ??
-                    o_pea.run(datastore)
-                    # un appel à find_stored_data
-                    o_mock_pea_find_stored_data.assert_called_once_with(datastore)
-                    o_mock_exist_output.api_delete.assert_called_once_with()
-                elif behavior == "CONTINUE":
-                    # premier test sur STATUS_UNSTABLE
-                    o_mock_exist_output.__getitem__.return_value = StoredData.STATUS_UNSTABLE
-                    with self.assertRaises(GpfSdkError) as o_err:
+                    if behavior == "DELETE":
+                        # suppression de l'existant puis normal
                         o_pea.run(datastore)
-                    self.assertEqual(o_err.exception.message, f"Le traitement précédent a échoué sur la donnée stockée en sortie {o_mock_exist_output}. Impossible de lancer le traitement demandé.")
-
-                    # deuxième test sur la stored data créée
-                    o_mock_exist_output.__getitem__.return_value = StoredData.STATUS_CREATED
-                    o_pea.run(datastore)
-                    o_mock_pe_api_list.assert_called_once_with({"output_stored_data":o_mock_exist_output.id}, datastore=datastore)
-                    self.assertEqual(o_pea.processing_execution, o_mock_processing_execution)
+                        # un appel à find_stored_data
+                        o_mock_pea_find_stored_data.assert_called_once_with(datastore)
+                        o_mock_exist_output.api_delete.assert_called_once_with()
+                    elif behavior == "CONTINUE":
+                        # premier test sur STATUS_UNSTABLE
+                        o_mock_exist_output.__getitem__.return_value = StoredData.STATUS_UNSTABLE
+                        with self.assertRaises(GpfSdkError) as o_err:
+                            o_pea.run(datastore)
+                        self.assertEqual(
+                            o_err.exception.message,
+                            f"Le traitement précédent a échoué sur la donnée stockée en sortie {o_mock_exist_output}. Impossible de lancer le traitement demandé."
+                        )
 
-                    # troisième test sur l'absence de la processing execution
-                    o_mock_pe_api_list.return_value = []
-                    with self.assertRaises(GpfSdkError) as o_err:
+                        # deuxième test sur la stored data créée
+                        o_mock_exist_output.__getitem__.return_value = StoredData.STATUS_CREATED
                         o_pea.run(datastore)
-                    self.assertEqual(o_err.exception.message, f"Impossible de trouver l'exécution de traitement liée à la donnée stockée {o_mock_exist_output}")
+                        o_mock_pe_api_list.assert_called_once_with({"output_stored_data":o_mock_exist_output.id}, datastore=datastore)
+                        self.assertEqual(o_pea.processing_execution, o_mock_processing_execution)
 
-                    return
-                else:
-                    # behavior non reconnu. On attend une erreur
-                    with self.assertRaises(GpfSdkError) as o_err:
+                        # troisième test sur l'absence de la processing execution
+                        o_mock_pe_api_list.return_value = []
+                        with self.assertRaises(GpfSdkError) as o_err:
+                            o_pea.run(datastore)
+                        self.assertEqual(o_err.exception.message, f"Impossible de trouver l'exécution de traitement liée à la donnée stockée {o_mock_exist_output}")
+
+                        return
+                    elif behavior == "RESUME":
+                        # premier test sur la stored data créée
+                        o_mock_exist_output.__getitem__.return_value = StoredData.STATUS_CREATED
                         o_pea.run(datastore)
-                    self.assertEqual(o_err.exception.message, f"Le comportement {behavior} n'est pas reconnu (STOP|DELETE|CONTINUE), l'exécution de traitement n'est pas possible.")
-                    return
+                        o_mock_pe_api_list.assert_called_once_with({"output_stored_data":o_mock_exist_output.id}, datastore=datastore)
+                        self.assertEqual(o_pea.processing_execution, o_mock_processing_execution)
 
-            else:
-                # on appelle la méthode à tester
-                o_pea.run(datastore)
-                o_mock_pea_find_stored_data.assert_not_called()
-
-            # test de l'appel à ProcessingExecution.api_create
-            o_mock_pe_api_create.assert_called_once_with(d_action['body_parameters'], {"datastore":datastore})
-            # un appel à ProcessingExecution().get_store_properties
-            o_mock_processing_execution.get_store_properties.assert_called_once_with()
-
-            # verif appel à Upload/StoredData
-            if "stored_data" in d_store_properties["output"]:
-                # test  .api_get
-                o_mock_stored_data_api_get.assert_called_once_with("id", datastore=datastore)
-                o_mock_upload_api_get.assert_not_called()
-
-                # test api_add_tags
-                if "tags" in d_action and d_action["tags"]:
-                    o_mock_stored_data.api_add_tags.assert_called_once_with(d_action["tags"])
-                else:
-                    o_mock_stored_data.api_add_tags.assert_not_called()
-                o_mock_upload.api_add_tags.assert_not_called()
+                        o_mock_exist_output.reset_mock()
+                        o_mock_pea_find_stored_data.reset_mock()
 
-                # test commentaires
-                if "comments" in d_action and d_action["comments"]:
-                    self.assertEqual(len(d_action["comments"]), o_mock_stored_data.api_add_comment.call_count)
-                    for s_comm in d_action["comments"]:
-                        o_mock_stored_data.api_add_comment.assert_any_call({"text": s_comm})
-                else:
-                    o_mock_stored_data.api_add_comment.assert_not_called()
-                o_mock_upload.api_add_comment.assert_not_called()
+                        # deuxième test sur l'absence de la processing execution
+                        o_mock_pe_api_list.return_value = []
+                        with self.assertRaises(GpfSdkError) as o_err:
+                            o_pea.run(datastore)
+                        self.assertEqual(o_err.exception.message, f"Impossible de trouver l'exécution de traitement liée à la donnée stockée {o_mock_exist_output}")
+
+                        o_mock_exist_output.reset_mock()
+                        o_mock_pea_find_stored_data.reset_mock()
+                        o_mock_processing_execution.api_launch.reset_mock()
 
+                        # troisième test sur STATUS_UNSTABLE => suppression puis normal
+                        o_mock_exist_output.__getitem__.return_value = StoredData.STATUS_UNSTABLE
+                        o_pea.run(datastore)
+                        # un appel à find_stored_data
+                        o_mock_pea_find_stored_data.assert_called_once_with(datastore)
+                        o_mock_exist_output.api_delete.assert_called_once_with()
+                    else:
+                        # behavior non reconnu. On attend une erreur
+                        with self.assertRaises(GpfSdkError) as o_err:
+                            o_pea.run(datastore)
+                        self.assertEqual(o_err.exception.message, f"Le comportement {behavior} n'est pas reconnu (STOP|DELETE|CONTINUE|RESUME), l'exécution de traitement n'est pas possible.")
+                        return
 
-            elif "upload" in  d_store_properties["output"]:
-                # test api_get
-                o_mock_upload_api_get.assert_called_once_with("id", datastore=datastore)
-                o_mock_stored_data_api_get.assert_not_called()
-
-                # test api_add_tags
-                if "tags" in d_action and d_action["tags"]:
-                    o_mock_upload.api_add_tags.assert_called_once_with(d_action["tags"])
                 else:
+                    # on appelle la méthode à tester
+                    o_pea.run(datastore)
+                    o_mock_pea_find_stored_data.assert_not_called()
+
+                # test de l'appel à ProcessingExecution.api_create
+                o_mock_pe_api_create.assert_called_once_with(d_action['body_parameters'], {"datastore":datastore})
+                # un appel à ProcessingExecution().get_store_properties
+                o_mock_processing_execution.get_store_properties.assert_called_once_with()
+
+                # verif appel à Upload/StoredData
+                if "stored_data" in d_store_properties["output"]:
+                    # test  .api_get
+                    o_mock_stored_data_api_get.assert_called_once_with("id", datastore=datastore)
+                    o_mock_upload_api_get.assert_not_called()
+
+                    # test api_add_tags
+                    if "tags" in d_action and d_action["tags"]:
+                        o_mock_stored_data.api_add_tags.assert_called_once_with(d_action["tags"])
+                    else:
+                        o_mock_stored_data.api_add_tags.assert_not_called()
                     o_mock_upload.api_add_tags.assert_not_called()
-                o_mock_stored_data.api_add_tags.assert_not_called()
 
-                # test commentaires
-                if "comments" in d_action and d_action["comments"]:
-                    self.assertEqual(len(d_action["comments"]), o_mock_upload.api_add_comment.call_count)
-                    for s_comm in d_action["comments"]:
-                        o_mock_upload.api_add_comment.assert_any_call({"text": s_comm})
-                else:
+                    # test commentaires
+                    if "comments" in d_action and d_action["comments"]:
+                        self.assertEqual(len(d_action["comments"]), o_mock_stored_data.api_add_comment.call_count)
+                        for s_comm in d_action["comments"]:
+                            o_mock_stored_data.api_add_comment.assert_any_call({"text": s_comm})
+                    else:
+                        o_mock_stored_data.api_add_comment.assert_not_called()
                     o_mock_upload.api_add_comment.assert_not_called()
-                o_mock_stored_data.api_add_comment.assert_not_called()
 
-            # un appel à api_launch
-            o_mock_processing_execution.api_launch.assert_called_once_with()
+
+                elif "upload" in  d_store_properties["output"]:
+                    # test api_get
+                    o_mock_upload_api_get.assert_called_once_with("id", datastore=datastore)
+                    o_mock_stored_data_api_get.assert_not_called()
+
+                    # test api_add_tags
+                    if "tags" in d_action and d_action["tags"]:
+                        o_mock_upload.api_add_tags.assert_called_once_with(d_action["tags"])
+                    else:
+                        o_mock_upload.api_add_tags.assert_not_called()
+                    o_mock_stored_data.api_add_tags.assert_not_called()
+
+                    # test commentaires
+                    if "comments" in d_action and d_action["comments"]:
+                        self.assertEqual(len(d_action["comments"]), o_mock_upload.api_add_comment.call_count)
+                        for s_comm in d_action["comments"]:
+                            o_mock_upload.api_add_comment.assert_any_call({"text": s_comm})
+                    else:
+                        o_mock_upload.api_add_comment.assert_not_called()
+                    o_mock_stored_data.api_add_comment.assert_not_called()
+
+                # un appel à api_launch
+                o_mock_processing_execution.api_launch.assert_called_once_with()
 
     def test_run(self) -> None:
         """test de run"""
+        s_key = "name"
         # test upload
         for s_datastore in [None, "datastore"]:
             for s_type_output in [ "upload", "stored_data"]:
-                s_key = "name"
                 ## sans tag + sans commentaire
                 self.run_args(None, None, s_key, s_type_output, s_datastore)
                 ## tag vide + commentaire vide
                 self.run_args({}, [], s_key, s_type_output, s_datastore)
                 ## 1 tag + 1 commentaire
                 self.run_args({"tag1": "val1"}, ["comm1"], s_key, s_type_output, s_datastore)
                 ## 2 tag + 4 commentaire
                 self.run_args({"tag1": "val1", "tag2": "val2"}, ["comm1", "comm2", "comm3", "comm4"], s_key, s_type_output, s_datastore)
 
         # tests particuliers pour cas ou la sortie existe déjà
         self.run_args({"tag1": "val1", "tag2": "val2"}, ["comm1", "comm2", "comm3", "comm4"], s_key, s_type_output, s_datastore, True, "STOP")
         self.run_args({"tag1": "val1", "tag2": "val2"}, ["comm1", "comm2", "comm3", "comm4"], s_key, s_type_output, s_datastore, True, "DELETE")
         self.run_args({"tag1": "val1", "tag2": "val2"}, ["comm1", "comm2", "comm3", "comm4"], s_key, s_type_output, s_datastore, True, "CONTINUE")
+        self.run_args({"tag1": "val1", "tag2": "val2"}, ["comm1", "comm2", "comm3", "comm4"], s_key, s_type_output, s_datastore, True, "RESUME")
         self.run_args({"tag1": "val1", "tag2": "val2"}, ["comm1", "comm2", "comm3", "comm4"], s_key, s_type_output, s_datastore, True, "Toto")
         self.run_args({"tag1": "val1", "tag2": "val2"}, ["comm1", "comm2", "comm3", "comm4"], s_key, s_type_output, s_datastore, True, None)
 
+        # cas en erreurs non spécifique
+        d_action: Dict[str, Any] = {"type": "processing-execution", "body_parameters":{"output":{s_key:"test"}}, "tags": {"key":"val"}, "comments": ["comm"]}
+        o_mock_processing_execution = MagicMock()
+        o_mock_processing_execution.get_store_properties.return_value = {"output":None}
+
+        ## processing_execution.get_store_properties vide après création
+        o_pea = ProcessingExecutionAction("contexte", d_action, behavior="STOP")
+        with patch.object(ProcessingExecution, "api_create", return_value=o_mock_processing_execution), \
+            patch.object(ProcessingExecutionAction, "output_new_entity", new_callable=PropertyMock, return_value=False), \
+            patch.object(Config, "get_str", return_value="STOP") \
+        :
+            with self.assertRaises(GpfSdkError) as o_err_gpf:
+                o_pea.run()
+            s_message = "Erreur à la création de l'exécution de traitement : impossible de récupérer l'entité en sortie."
+            self.assertEqual(o_err_gpf.exception.message, s_message)
+
+        ## impossible de récupérer le donnée en sortie depuis processing_execution
+        d_output={"autre": "", "key": ""}
+        o_mock_processing_execution.get_store_properties.return_value = {"output":d_output}
+        o_pea = ProcessingExecutionAction("contexte", d_action, behavior="STOP")
+        with patch.object(ProcessingExecution, "api_create", return_value=o_mock_processing_execution), \
+            patch.object(ProcessingExecutionAction, "output_new_entity", new_callable=PropertyMock, return_value=False), \
+            patch.object(Config, "get_str", return_value="STOP") \
+        :
+            with self.assertRaises(StepActionError) as o_err_step:
+                o_pea.run()
+            s_message = f"Aucune correspondance pour {d_output.keys()}"
+            self.assertEqual(o_err_step.exception.message, s_message)
+
+        ## impossible d'ajouté un tag, pas de donnée en sortie
+        o_pea = ProcessingExecutionAction("contexte", d_action, behavior="STOP")
+        with patch.object(ProcessingExecutionAction, "upload", new_callable=PropertyMock, return_value=None), \
+            patch.object(ProcessingExecutionAction, "stored_data", new_callable=PropertyMock, return_value=None), \
+            patch.object(Config, "get_str", return_value="STOP"), \
+            patch.object(ProcessingExecutionAction, "_ProcessingExecutionAction__create_processing_execution", return_value=None) \
+        :
+            with self.assertRaises(StepActionError) as o_err_step:
+                o_pea.run()
+            s_message = "ni upload ni stored-data trouvé. Impossible d'ajouter les tags"
+            self.assertEqual(o_err_step.exception.message, s_message)
+
+        ## impossible d'ajouté un commentaire, pas de donnée en sortie
+        o_pea = ProcessingExecutionAction("contexte", d_action, behavior="STOP")
+        with patch.object(ProcessingExecutionAction, "upload", new_callable=PropertyMock, return_value=None), \
+            patch.object(ProcessingExecutionAction, "stored_data", new_callable=PropertyMock, return_value=None), \
+            patch.object(Config, "get_str", return_value="STOP"), \
+            patch.object(ProcessingExecutionAction, "_ProcessingExecutionAction__create_processing_execution", return_value=None), \
+            patch.object(ProcessingExecutionAction, "_ProcessingExecutionAction__add_tags", return_value=None) \
+        :
+            with self.assertRaises(StepActionError) as o_err_step:
+                o_pea.run()
+            s_message = "ni upload ni stored-data trouvé. Impossible d'ajouter les commentaires"
+            self.assertEqual(o_err_step.exception.message, s_message)
+
+        ## __launch pas de processing_execution
+        o_pea = ProcessingExecutionAction("contexte", d_action, behavior="STOP")
+        with patch.object(ProcessingExecutionAction, "processing_execution", new_callable=PropertyMock, return_value=None), \
+            patch.object(Config, "get_str", return_value="STOP"), \
+            patch.object(ProcessingExecutionAction, "_ProcessingExecutionAction__create_processing_execution", return_value=None), \
+            patch.object(ProcessingExecutionAction, "_ProcessingExecutionAction__add_tags", return_value=None), \
+            patch.object(ProcessingExecutionAction, "_ProcessingExecutionAction__add_comments", return_value=None) \
+        :
+            with self.assertRaises(StepActionError) as o_err_step:
+                o_pea.run()
+            s_message = "Aucune exécution de traitement trouvée. Impossible de lancer le traitement"
+            self.assertEqual(o_err_step.exception.message, s_message)
+
+        ## __launch traitement pas déjà lancé et pas en mode continue ou reprise
+        o_pea = ProcessingExecutionAction("contexte", d_action, behavior="STOP")
+        with patch.object(ProcessingExecutionAction, "processing_execution", new_callable=PropertyMock, return_value={"status": "autre"}), \
+            patch.object(Config, "get_str", return_value="STOP"), \
+            patch.object(ProcessingExecutionAction, "_ProcessingExecutionAction__create_processing_execution", return_value=None), \
+            patch.object(ProcessingExecutionAction, "_ProcessingExecutionAction__add_tags", return_value=None), \
+            patch.object(ProcessingExecutionAction, "_ProcessingExecutionAction__add_comments", return_value=None) \
+        :
+            with self.assertRaises(StepActionError) as o_err_step:
+                o_pea.run()
+            s_message = "L'exécution de traitement est déjà lancée."
+            self.assertEqual(o_err_step.exception.message, s_message)
+
+
     def monitoring_until_end_args(self, s_status_end: str, b_waits: bool, b_callback: bool) -> None:
         """lancement + test de ProcessingExecutionAction.monitoring_until_end() selon param
 
         Args:
             s_status_end (str): status de fin
             b_waits (bool): si on a des status intermédiaire
             b_callback (bool): si on a une fonction callback
```

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/action/SynchronizeOfferingActionTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/action/SynchronizeOfferingActionTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/action/UploadActionTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/action/UploadActionTestCase.py`

 * *Files 0% similar despite different names*

```diff
@@ -360,15 +360,15 @@
         o_mock_upload = MagicMock()
         o_dataset=MagicMock()
         o_ua = UploadActionNoPrivate(o_dataset, behavior=s_behavior)
         with patch.object(UploadAction, "find_upload", return_value = o_mock_upload) as o_mock_find_upload, \
             patch.object(Upload, "api_create") as o_mock_api_create:
             with self.assertRaises(GpfSdkError) as e_err:
                 o_ua.create_upload(datastore=s_datastore)
-            self.assertEqual(f"Le comportement {s_behavior} n'est pas reconnu, l'exécution de traitement est annulée.", e_err.exception.message)
+            self.assertEqual(f"Le comportement {s_behavior} n'est pas reconnu (STOP|CONTINUE|DELETE), l'exécution de traitement est annulée.", e_err.exception.message)
             o_mock_find_upload.assert_called_once_with(s_datastore)
             o_mock_api_create.assert_not_called()
             o_mock_upload.is_open.assert_not_called()
 
     def test_add_tags(self) -> None:
         """test de __add_tags"""
         # pas d'upload ou pas de tags => rien de fait
```

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/AbstractResolverTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/AbstractResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/DateResolverTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/DateResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/DictResolverTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/DictResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/FileResolverTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/FileResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/GlobalResolverTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/GlobalResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/StoreEntityResolverTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/StoreEntityResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/tests/workflow/resolver/UserResolverTestCase.py` & `sdk_entrepot_gpf-0.1.27/tests/workflow/resolver/UserResolverTestCase.py`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/uml/classes.png` & `sdk_entrepot_gpf-0.1.27/uml/classes.png`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/uml/classes.uxf` & `sdk_entrepot_gpf-0.1.27/uml/classes.uxf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/uml/interfaces.png` & `sdk_entrepot_gpf-0.1.27/uml/interfaces.png`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/uml/interfaces.uxf` & `sdk_entrepot_gpf-0.1.27/uml/interfaces.uxf`

 * *Files identical despite different names*

### Comparing `sdk_entrepot_gpf-0.1.26/PKG-INFO` & `sdk_entrepot_gpf-0.1.27/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdk_entrepot_gpf
-Version: 0.1.26
+Version: 0.1.27
 Summary: SDK Python pour simplifier l'utilisation de l'API Entrepôt de la Géoplateforme.
 Author-email: Valentin Sasyan <valentin.sasyan@ign.fr>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

