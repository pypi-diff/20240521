# Comparing `tmp/dvcx-0.82.0.tar.gz` & `tmp/dvcx-0.82.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.82.0.tar", last modified: Mon May 20 11:45:42 2024, max compression
+gzip compressed data, was "dvcx-0.82.1.tar", last modified: Tue May 21 08:48:12 2024, max compression
```

## Comparing `dvcx-0.82.0.tar` & `dvcx-0.82.1.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.146879 dvcx-0.82.0/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-20 11:45:33.000000 dvcx-0.82.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 11:45:33.000000 dvcx-0.82.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.098879 dvcx-0.82.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.102879 dvcx-0.82.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.102879 dvcx-0.82.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-20 11:45:33.000000 dvcx-0.82.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-20 11:45:33.000000 dvcx-0.82.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.102879 dvcx-0.82.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 11:45:33.000000 dvcx-0.82.0/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-20 11:45:33.000000 dvcx-0.82.0/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-20 11:45:33.000000 dvcx-0.82.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-20 11:45:33.000000 dvcx-0.82.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-20 11:45:33.000000 dvcx-0.82.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.102879 dvcx-0.82.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-20 11:45:33.000000 dvcx-0.82.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-20 11:45:33.000000 dvcx-0.82.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-20 11:45:33.000000 dvcx-0.82.0/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-20 11:45:42.146879 dvcx-0.82.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-20 11:45:33.000000 dvcx-0.82.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.102879 dvcx-0.82.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-20 11:45:33.000000 dvcx-0.82.0/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.106879 dvcx-0.82.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/llm-claude-aggregate-query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/llm-claude-simple-query.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/llm-claude.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.106879 dvcx-0.82.0/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.110879 dvcx-0.82.0/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.110879 dvcx-0.82.0/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-20 11:45:33.000000 dvcx-0.82.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-20 11:45:33.000000 dvcx-0.82.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:45:42.146879 dvcx-0.82.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.094879 dvcx-0.82.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.114879 dvcx-0.82.0/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-20 11:45:41.000000 dvcx-0.82.0/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.114879 dvcx-0.82.0/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72515 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.118879 dvcx-0.82.0/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.118879 dvcx-0.82.0/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45790 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26305 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    33673 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.122879 dvcx-0.82.0/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/feature_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/tar_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.126879 dvcx-0.82.0/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    61468 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.126879 dvcx-0.82.0/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.126879 dvcx-0.82.0/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.126879 dvcx-0.82.0/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.126879 dvcx-0.82.0/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.130879 dvcx-0.82.0/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10452 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.142879 dvcx-0.82.0/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-20 11:45:42.000000 dvcx-0.82.0/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-20 11:45:42.000000 dvcx-0.82.0/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:45:42.000000 dvcx-0.82.0/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 11:45:42.000000 dvcx-0.82.0/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-20 11:45:42.000000 dvcx-0.82.0/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 11:45:42.000000 dvcx-0.82.0/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.130879 dvcx-0.82.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.130879 dvcx-0.82.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16483 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.134879 dvcx-0.82.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35078 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   113497 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    28872 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.134879 dvcx-0.82.0/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/scripts/name_len_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/scripts/name_len_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/test_cli_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/test_query_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.138879 dvcx-0.82.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.138879 dvcx-0.82.0/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.142879 dvcx-0.82.0/tests/unit/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.142879 dvcx-0.82.0/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_dataset_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.919056 dvcx-0.82.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-21 08:48:06.000000 dvcx-0.82.1/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-21 08:48:06.000000 dvcx-0.82.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.871056 dvcx-0.82.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.871056 dvcx-0.82.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-21 08:48:06.000000 dvcx-0.82.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-21 08:48:06.000000 dvcx-0.82.1/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-21 08:48:06.000000 dvcx-0.82.1/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-21 08:48:06.000000 dvcx-0.82.1/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-21 08:48:06.000000 dvcx-0.82.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.875056 dvcx-0.82.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-21 08:48:06.000000 dvcx-0.82.1/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-21 08:48:06.000000 dvcx-0.82.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-21 08:48:06.000000 dvcx-0.82.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-21 08:48:06.000000 dvcx-0.82.1/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-21 08:48:06.000000 dvcx-0.82.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-21 08:48:06.000000 dvcx-0.82.1/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.875056 dvcx-0.82.1/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 08:48:06.000000 dvcx-0.82.1/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-21 08:48:06.000000 dvcx-0.82.1/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-21 08:48:06.000000 dvcx-0.82.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-21 08:48:06.000000 dvcx-0.82.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-21 08:48:06.000000 dvcx-0.82.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.875056 dvcx-0.82.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-21 08:48:06.000000 dvcx-0.82.1/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-21 08:48:06.000000 dvcx-0.82.1/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-21 08:48:06.000000 dvcx-0.82.1/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-21 08:48:12.919056 dvcx-0.82.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-21 08:48:06.000000 dvcx-0.82.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.875056 dvcx-0.82.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-21 08:48:06.000000 dvcx-0.82.1/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.879056 dvcx-0.82.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/llm-claude-aggregate-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/llm-claude-simple-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/llm-claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.879056 dvcx-0.82.1/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.879056 dvcx-0.82.1/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.879056 dvcx-0.82.1/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 08:48:06.000000 dvcx-0.82.1/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-21 08:48:06.000000 dvcx-0.82.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-05-21 08:48:06.000000 dvcx-0.82.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:48:12.919056 dvcx-0.82.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.867056 dvcx-0.82.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.883056 dvcx-0.82.1/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-21 08:48:12.000000 dvcx-0.82.1/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.887056 dvcx-0.82.1/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72545 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.887056 dvcx-0.82.1/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.891056 dvcx-0.82.1/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45790 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26305 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33738 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.895056 dvcx-0.82.1/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/feature_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/tar_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.895056 dvcx-0.82.1/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61474 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/query/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.895056 dvcx-0.82.1/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.899056 dvcx-0.82.1/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.899056 dvcx-0.82.1/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.899056 dvcx-0.82.1/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.899056 dvcx-0.82.1/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10323 2024-05-21 08:48:06.000000 dvcx-0.82.1/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.911056 dvcx-0.82.1/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-05-21 08:48:12.000000 dvcx-0.82.1/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-21 08:48:12.000000 dvcx-0.82.1/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:48:12.000000 dvcx-0.82.1/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 08:48:12.000000 dvcx-0.82.1/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-21 08:48:12.000000 dvcx-0.82.1/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-21 08:48:12.000000 dvcx-0.82.1/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.899056 dvcx-0.82.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.903056 dvcx-0.82.1/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16483 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.903056 dvcx-0.82.1/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35078 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113497 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28872 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/func/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.903056 dvcx-0.82.1/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/scripts/name_len_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/scripts/name_len_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/test_cli_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/test_query_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.907056 dvcx-0.82.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.911056 dvcx-0.82.1/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/lib/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/lib/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/lib/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.911056 dvcx-0.82.1/tests/unit/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:12.911056 dvcx-0.82.1/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5851 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_dataset_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-21 08:48:06.000000 dvcx-0.82.1/tests/utils.py
```

### Comparing `dvcx-0.82.0/.cruft.json` & `dvcx-0.82.1/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.82.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.82.1/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/.github/workflows/benchmarks.yml` & `dvcx-0.82.1/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/.github/workflows/release.yml` & `dvcx-0.82.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/.github/workflows/tests.yml` & `dvcx-0.82.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/.gitignore` & `dvcx-0.82.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/.pre-commit-config.yaml` & `dvcx-0.82.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/CODE_OF_CONDUCT.rst` & `dvcx-0.82.1/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/CONTRIBUTING.rst` & `dvcx-0.82.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/LICENSE` & `dvcx-0.82.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/LICENSES/Apache-2.0.txt` & `dvcx-0.82.1/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/LICENSES/BSD-3-Clause.txt` & `dvcx-0.82.1/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/LICENSES/Python-2.0.txt` & `dvcx-0.82.1/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/PKG-INFO` & `dvcx-0.82.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.82.0
+Version: 0.82.1
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -27,16 +27,15 @@
 Requires-Dist: adlfs>=2024.2.0
 Requires-Dist: dvc-data<4,>=3.10
 Requires-Dist: dvc-objects<6,>=4
 Requires-Dist: shtab<2,>=1.3.4
 Requires-Dist: sqlalchemy>=2
 Requires-Dist: multiprocess==0.70.16
 Requires-Dist: dill==0.3.8
-Requires-Dist: ujson==5.9.0
-Requires-Dist: types-ujson==5.9.0.0
+Requires-Dist: ujson>=5.9.0
 Requires-Dist: pydantic<3,>=2
 Provides-Extra: cv
 Requires-Dist: Pillow<11,>=10.0.0; extra == "cv"
 Requires-Dist: torch>=2.1.0; extra == "cv"
 Requires-Dist: torchvision; extra == "cv"
 Requires-Dist: numpy; extra == "cv"
 Requires-Dist: transformers>=4.36.0; extra == "cv"
@@ -65,20 +64,22 @@
 Requires-Dist: virtualenv; extra == "tests"
 Requires-Dist: dulwich; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: numpy; extra == "tests"
 Requires-Dist: open_clip_torch; extra == "tests"
 Requires-Dist: aiotools>=1.7.0; extra == "tests"
 Requires-Dist: requests-mock; extra == "tests"
+Requires-Dist: requests<2.32.0; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: dvcx[tests]; extra == "dev"
 Requires-Dist: mypy==1.10.0; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
+Requires-Dist: types-ujson; extra == "dev"
 
 |PyPI| |Status| |Python Version| |License|
 
 |Tests| |Codecov| |pre-commit| |Black|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/dvcx.svg
    :target: https://pypi.org/project/dvcx/
```

### Comparing `dvcx-0.82.0/README.rst` & `dvcx-0.82.1/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/docs/udfs.md` & `dvcx-0.82.1/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/blip2_image_desc_lib.py` & `dvcx-0.82.1/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/clip.py` & `dvcx-0.82.1/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/common_sql_functions.py` & `dvcx-0.82.1/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/dir_expansion.py` & `dvcx-0.82.1/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/hf_pipeline.py` & `dvcx-0.82.1/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/llava2_image_desc_lib.py` & `dvcx-0.82.1/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/llm-claude-aggregate-query.py` & `dvcx-0.82.1/examples/llm-claude-aggregate-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/llm-claude-simple-query.py` & `dvcx-0.82.1/examples/llm-claude-simple-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/llm-claude.py` & `dvcx-0.82.1/examples/llm-claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/loader.py` & `dvcx-0.82.1/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/neurips/README` & `dvcx-0.82.1/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/neurips/distance_to_query.py` & `dvcx-0.82.1/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/neurips/llm_chat.py` & `dvcx-0.82.1/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/neurips/single_query.py` & `dvcx-0.82.1/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/neurips/text_loaders.py` & `dvcx-0.82.1/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/openai_image_desc_lib.py` & `dvcx-0.82.1/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/openimage-detect.py` & `dvcx-0.82.1/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/pose_detection.py` & `dvcx-0.82.1/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/torch-loader.py` & `dvcx-0.82.1/examples/torch-loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/udfs/batching.py` & `dvcx-0.82.1/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/udfs/image_transformation.py` & `dvcx-0.82.1/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/udfs/parallel.py` & `dvcx-0.82.1/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/udfs/simple.py` & `dvcx-0.82.1/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/udfs/stateful.py` & `dvcx-0.82.1/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/udfs/stateful_similarity.py` & `dvcx-0.82.1/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/unstructured-text.py` & `dvcx-0.82.1/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/wds.py` & `dvcx-0.82.1/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/wds_filtered.py` & `dvcx-0.82.1/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/wds_meta.py` & `dvcx-0.82.1/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/zalando/zalando_clip.py` & `dvcx-0.82.1/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.82.1/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/noxfile.py` & `dvcx-0.82.1/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/pyproject.toml` & `dvcx-0.82.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,16 +31,15 @@
   "adlfs>=2024.2.0",
   "dvc-data>=3.10,<4",
   "dvc-objects>=4,<6",
   "shtab>=1.3.4,<2",
   "sqlalchemy>=2",
   "multiprocess==0.70.16",
   "dill==0.3.8",
-  "ujson==5.9.0",
-  "types-ujson==5.9.0.0",
+  "ujson>=5.9.0",
   "pydantic>=2,<3"
 ]
 
 [project.optional-dependencies]
 cv = [
   "Pillow>=10.0.0,<11",
   "torch>=2.1.0",
@@ -73,22 +72,24 @@
   "pytest-xdist>=3.3.1",
   "virtualenv",
   "dulwich",
   "hypothesis",
   "numpy",
   "open_clip_torch",
   "aiotools>=1.7.0",
-  "requests-mock"
+  "requests-mock",
+  "requests<2.32.0"
 ]
 dev = [
   "dvcx[tests]",
   "mypy==1.10.0",
   "types-python-dateutil",
   "types-PyYAML",
-  "types-requests"
+  "types-requests",
+  "types-ujson"
 ]
 
 [project.urls]
 Issues = "https://github.com/iterative/dvcx/issues"
 Source = "https://github.com/iterative/dvcx"
 
 [project.scripts]
```

### Comparing `dvcx-0.82.0/src/dvcx/asyn.py` & `dvcx-0.82.1/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/cache.py` & `dvcx-0.82.1/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/catalog/catalog.py` & `dvcx-0.82.1/src/dvcx/catalog/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
 from dvcx.node import DirType, Node, NodeWithPath
 from dvcx.nodes_thread_pool import NodesThreadPool
 from dvcx.remote.studio import StudioClient
 from dvcx.sql.types import DateTime, SQLType, String
 from dvcx.storage import Status, Storage, StorageStats, StorageURI
 from dvcx.utils import (
     DVCXDir,
-    chunk,
+    batched,
     dvcx_paths_join,
     import_object,
     parse_params_string,
 )
 
 from .datasource import DataSource
 
@@ -234,14 +234,15 @@
         import lz4.frame
         import pandas as pd
 
         metastore = self.metastore.clone()  # metastore is not thread safe
         warehouse = self.warehouse.clone()  # warehouse is not thread safe
         dataset = metastore.get_dataset(self.dataset_name)
 
+        urls = list(urls)
         while urls:
             for url in urls:
                 if self.should_check_for_status():
                     self.check_for_status()
 
                 r = requests.get(url, timeout=PULL_DATASET_CHUNK_TIMEOUT)
                 if r.status_code == 404:
@@ -1673,15 +1674,15 @@
                 remote_config,
                 dataset.name,
                 version,
                 custom_column_types,
             )
             try:
                 rows_fetcher.run(
-                    chunk(
+                    batched(
                         signed_urls,
                         math.ceil(len(signed_urls) / PULL_DATASET_MAX_THREADS),
                     ),
                     dataset_save_progress_bar,
                 )
             except:
                 self.remove_dataset(dataset.name, version)
```

### Comparing `dvcx-0.82.0/src/dvcx/catalog/datasource.py` & `dvcx-0.82.1/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/catalog/loader.py` & `dvcx-0.82.1/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/cli.py` & `dvcx-0.82.1/src/dvcx/cli.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/cli_utils.py` & `dvcx-0.82.1/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/client/azure.py` & `dvcx-0.82.1/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/client/fileslice.py` & `dvcx-0.82.1/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/client/fsspec.py` & `dvcx-0.82.1/src/dvcx/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/client/gcs.py` & `dvcx-0.82.1/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/client/local.py` & `dvcx-0.82.1/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/client/s3.py` & `dvcx-0.82.1/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/config.py` & `dvcx-0.82.1/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/data_storage/db_engine.py` & `dvcx-0.82.1/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/data_storage/id_generator.py` & `dvcx-0.82.1/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/data_storage/metastore.py` & `dvcx-0.82.1/src/dvcx/data_storage/metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/data_storage/schema.py` & `dvcx-0.82.1/src/dvcx/data_storage/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/data_storage/serializer.py` & `dvcx-0.82.1/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/data_storage/sqlite.py` & `dvcx-0.82.1/src/dvcx/data_storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/data_storage/warehouse.py` & `dvcx-0.82.1/src/dvcx/data_storage/warehouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,14 +91,15 @@
         If value is a list or some other iterable, it tries to convert sub elements
         as well
         """
         if numpy_imported and isinstance(val, (np.ndarray, np.generic)):
             val = val.tolist()
 
         col_python_type = self.python_type(col_type)
+        col_type_name = type(col_type).__name__
         value_type = type(val)
 
         exc = None
         try:
             if col_python_type == list and value_type in (list, tuple, set):
                 if len(val) == 0:
                     return []
@@ -106,15 +107,15 @@
                 if item_pyton_type != list:
                     if isinstance(val[0], item_pyton_type):
                         return val
                     if item_pyton_type == float and isinstance(val[0], int):
                         return [float(i) for i in val]
                 return [self.convert_type(i, col_type.item_type) for i in val]
             # special use case with JSON type as we save it as string
-            if col_python_type == dict:
+            if col_python_type == dict or col_type_name == "JSON":
                 if value_type == str:
                     return val
                 if value_type in (dict, list):
                     return json.dumps(val)
                 raise ValueError(
                     f"Cannot convert value {val!r} with type" f"{value_type} to JSON"
                 )
@@ -123,15 +124,15 @@
                 return val
             if col_python_type == float and isinstance(val, int):
                 return float(val)
         except Exception as e:  # noqa: BLE001
             exc = e
         raise ValueError(
             f"Value {val!r} with type {value_type} incompatible for "
-            f"column type {type(col_type).__name__}"
+            f"column type {col_type_name}"
         ) from exc
 
     @abstractmethod
     def clone(
         self,
         uri: StorageURI = StorageURI(""),
         partial_id: Optional[int] = None,
```

### Comparing `dvcx-0.82.0/src/dvcx/dataset.py` & `dvcx-0.82.1/src/dvcx/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/error.py` & `dvcx-0.82.1/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/cached_stream.py` & `dvcx-0.82.1/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/claude.py` & `dvcx-0.82.1/src/dvcx/lib/claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/dataset.py` & `dvcx-0.82.1/src/dvcx/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/feature.py` & `dvcx-0.82.1/src/dvcx/lib/feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/feature_types.py` & `dvcx-0.82.1/src/dvcx/lib/feature_types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/feature_udf.py` & `dvcx-0.82.1/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/file.py` & `dvcx-0.82.1/src/dvcx/lib/file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.82.1/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.82.1/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.82.1/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/image.py` & `dvcx-0.82.1/src/dvcx/lib/image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/image_transform.py` & `dvcx-0.82.1/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.82.1/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/pytorch.py` & `dvcx-0.82.1/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/reader.py` & `dvcx-0.82.1/src/dvcx/lib/reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/tar_file.py` & `dvcx-0.82.1/src/dvcx/lib/tar_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/text.py` & `dvcx-0.82.1/src/dvcx/lib/text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/udf.py` & `dvcx-0.82.1/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/unstructured.py` & `dvcx-0.82.1/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/utils.py` & `dvcx-0.82.1/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/webdataset.py` & `dvcx-0.82.1/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.82.1/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.82.1/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/listing.py` & `dvcx-0.82.1/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/node.py` & `dvcx-0.82.1/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/nodes_fetcher.py` & `dvcx-0.82.1/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/nodes_thread_pool.py` & `dvcx-0.82.1/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/progress.py` & `dvcx-0.82.1/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/query/batch.py` & `dvcx-0.82.1/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/query/builtins.py` & `dvcx-0.82.1/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/query/dataset.py` & `dvcx-0.82.1/src/dvcx/query/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 )
 from dvcx.dataset import DatasetRow
 from dvcx.dataset import Status as DatasetStatus
 from dvcx.error import DatasetNotFoundError, QueryScriptCancelError
 from dvcx.sql.functions import rand
 from dvcx.sql.types import SQLType
 from dvcx.storage import StorageURI
-from dvcx.utils import chunk, determine_processes
+from dvcx.utils import batched, determine_processes
 
 from .batch import DatasetRowsBatch
 from .schema import C, UDFParamSpec, normalize_param
 from .session import Session
 from .udf import UDFBase, UDFClassWrapper, UDFFactory, UDFType
 
 if TYPE_CHECKING:
@@ -376,20 +376,20 @@
     for udf_output in udf_results:
         if not udf_output:
             continue
         for row in udf_output:
             cb.relative_update()
             rows.append(adjust_outputs(warehouse, row, udf))
             if len(rows) >= batch_size:
-                for row_chunk in chunk(rows, batch_size):
+                for row_chunk in batched(rows, batch_size):
                     warehouse.insert_rows(udf_table, row_chunk)
                 rows.clear()
 
     if rows:
-        for row_chunk in chunk(rows, batch_size):
+        for row_chunk in batched(rows, batch_size):
             warehouse.insert_rows(udf_table, row_chunk)
 
 
 def get_processed_callback() -> Callback:
     return TqdmCallback({"desc": "Processed", "unit": " rows"})
```

### Comparing `dvcx-0.82.0/src/dvcx/query/dispatch.py` & `dvcx-0.82.1/src/dvcx/query/dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/query/params.py` & `dvcx-0.82.1/src/dvcx/query/params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/query/schema.py` & `dvcx-0.82.1/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/query/session.py` & `dvcx-0.82.1/src/dvcx/query/session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/query/udf.py` & `dvcx-0.82.1/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/remote/studio.py` & `dvcx-0.82.1/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/sql/default/base.py` & `dvcx-0.82.1/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/sql/functions/array.py` & `dvcx-0.82.1/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/sql/functions/path.py` & `dvcx-0.82.1/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/sql/selectable.py` & `dvcx-0.82.1/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/sql/sqlite/base.py` & `dvcx-0.82.1/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/sql/sqlite/types.py` & `dvcx-0.82.1/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/sql/types.py` & `dvcx-0.82.1/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/sql/utils.py` & `dvcx-0.82.1/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/storage.py` & `dvcx-0.82.1/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx/utils.py` & `dvcx-0.82.1/src/dvcx/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import json
 import os
 import os.path as osp
 import random
 import stat
 import sys
 import time
-from collections.abc import Iterable, Sequence
+from collections.abc import Iterable, Iterator, Sequence
 from datetime import date, datetime, timezone
 from itertools import islice
 from typing import TYPE_CHECKING, Any, Optional, TypeVar, Union
 from uuid import UUID
 
 from dateutil import tz
 from dateutil.parser import isoparse
@@ -230,31 +230,28 @@
         else:
             args.append(part)
     if any((args, kwargs)):
         return args, kwargs
     return None, None
 
 
-def batched(iterable, n):
+_T_co = TypeVar("_T_co", covariant=True)
+
+
+def batched(iterable: Iterable[_T_co], n: int) -> Iterator[tuple[_T_co, ...]]:
     "Batch data into tuples of length n. The last batch may be shorter."
     # Based on: https://docs.python.org/3/library/itertools.html#itertools-recipes
     # batched('ABCDEFG', 3) --> ABC DEF G
     if n < 1:
         raise ValueError("Batch size must be at least one")
     it = iter(iterable)
     while batch := tuple(islice(it, n)):
         yield batch
 
 
-def chunk(input_list: list[Any], chunk_size: int) -> Iterable[list[Any]]:
-    """Breaks list into iterable of chunks of defined size"""
-    for i in range(0, len(input_list), chunk_size):
-        yield input_list[i : i + chunk_size]
-
-
 def flatten(items):
     for item in items:
         if isinstance(item, list):
             yield from item
         else:
             yield item
```

### Comparing `dvcx-0.82.0/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.82.1/src/dvcx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.82.0
+Version: 0.82.1
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -27,16 +27,15 @@
 Requires-Dist: adlfs>=2024.2.0
 Requires-Dist: dvc-data<4,>=3.10
 Requires-Dist: dvc-objects<6,>=4
 Requires-Dist: shtab<2,>=1.3.4
 Requires-Dist: sqlalchemy>=2
 Requires-Dist: multiprocess==0.70.16
 Requires-Dist: dill==0.3.8
-Requires-Dist: ujson==5.9.0
-Requires-Dist: types-ujson==5.9.0.0
+Requires-Dist: ujson>=5.9.0
 Requires-Dist: pydantic<3,>=2
 Provides-Extra: cv
 Requires-Dist: Pillow<11,>=10.0.0; extra == "cv"
 Requires-Dist: torch>=2.1.0; extra == "cv"
 Requires-Dist: torchvision; extra == "cv"
 Requires-Dist: numpy; extra == "cv"
 Requires-Dist: transformers>=4.36.0; extra == "cv"
@@ -65,20 +64,22 @@
 Requires-Dist: virtualenv; extra == "tests"
 Requires-Dist: dulwich; extra == "tests"
 Requires-Dist: hypothesis; extra == "tests"
 Requires-Dist: numpy; extra == "tests"
 Requires-Dist: open_clip_torch; extra == "tests"
 Requires-Dist: aiotools>=1.7.0; extra == "tests"
 Requires-Dist: requests-mock; extra == "tests"
+Requires-Dist: requests<2.32.0; extra == "tests"
 Provides-Extra: dev
 Requires-Dist: dvcx[tests]; extra == "dev"
 Requires-Dist: mypy==1.10.0; extra == "dev"
 Requires-Dist: types-python-dateutil; extra == "dev"
 Requires-Dist: types-PyYAML; extra == "dev"
 Requires-Dist: types-requests; extra == "dev"
+Requires-Dist: types-ujson; extra == "dev"
 
 |PyPI| |Status| |Python Version| |License|
 
 |Tests| |Codecov| |pre-commit| |Black|
 
 .. |PyPI| image:: https://img.shields.io/pypi/v/dvcx.svg
    :target: https://pypi.org/project/dvcx/
```

### Comparing `dvcx-0.82.0/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.82.1/src/dvcx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/src/dvcx.egg-info/requires.txt` & `dvcx-0.82.1/src/dvcx.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -10,16 +10,15 @@
 adlfs>=2024.2.0
 dvc-data<4,>=3.10
 dvc-objects<6,>=4
 shtab<2,>=1.3.4
 sqlalchemy>=2
 multiprocess==0.70.16
 dill==0.3.8
-ujson==5.9.0
-types-ujson==5.9.0.0
+ujson>=5.9.0
 pydantic<3,>=2
 
 [cv]
 Pillow<11,>=10.0.0
 torch>=2.1.0
 torchvision
 numpy
@@ -27,14 +26,15 @@
 
 [dev]
 dvcx[tests]
 mypy==1.10.0
 types-python-dateutil
 types-PyYAML
 types-requests
+types-ujson
 
 [pandas]
 pandas>=1.4.0
 
 [remote]
 dvcx[pandas]
 lz4
@@ -56,11 +56,12 @@
 virtualenv
 dulwich
 hypothesis
 numpy
 open_clip_torch
 aiotools>=1.7.0
 requests-mock
+requests<2.32.0
 
 [vector]
 numpy
 scipy
```

### Comparing `dvcx-0.82.0/tests/benchmarks/conftest.py` & `dvcx-0.82.1/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/conftest.py` & `dvcx-0.82.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/data.py` & `dvcx-0.82.1/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/func/test_catalog.py` & `dvcx-0.82.1/tests/func/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/func/test_client.py` & `dvcx-0.82.1/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/func/test_dataset_query.py` & `dvcx-0.82.1/tests/func/test_dataset_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/func/test_datasets.py` & `dvcx-0.82.1/tests/func/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/func/test_ls.py` & `dvcx-0.82.1/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/func/test_pull.py` & `dvcx-0.82.1/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/func/test_pytorch.py` & `dvcx-0.82.1/tests/func/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/func/test_query.py` & `dvcx-0.82.1/tests/func/test_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/scripts/name_len_normal.py` & `dvcx-0.82.1/tests/scripts/name_len_normal.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/scripts/name_len_slow.py` & `dvcx-0.82.1/tests/scripts/name_len_slow.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/test_cli_e2e.py` & `dvcx-0.82.1/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/test_query_e2e.py` & `dvcx-0.82.1/tests/test_query_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/lib/test_cached_stream.py` & `dvcx-0.82.1/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/lib/test_feature.py` & `dvcx-0.82.1/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/lib/test_feature_udf.py` & `dvcx-0.82.1/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/lib/test_file.py` & `dvcx-0.82.1/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/lib/test_image.py` & `dvcx-0.82.1/tests/unit/lib/test_image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/lib/test_reader.py` & `dvcx-0.82.1/tests/unit/lib/test_reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/lib/test_text.py` & `dvcx-0.82.1/tests/unit/lib/test_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/lib/test_webdataset.py` & `dvcx-0.82.1/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.82.1/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/sql/test_array.py` & `dvcx-0.82.1/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/sql/test_conditional.py` & `dvcx-0.82.1/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/sql/test_path.py` & `dvcx-0.82.1/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/sql/test_selectable.py` & `dvcx-0.82.1/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/sql/test_string.py` & `dvcx-0.82.1/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_asyn.py` & `dvcx-0.82.1/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_cache.py` & `dvcx-0.82.1/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_catalog.py` & `dvcx-0.82.1/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_catalog_loader.py` & `dvcx-0.82.1/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_cli_parsing.py` & `dvcx-0.82.1/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_client.py` & `dvcx-0.82.1/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_client_s3.py` & `dvcx-0.82.1/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_data_storage.py` & `dvcx-0.82.1/tests/unit/test_data_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,21 @@
     assert warehouse.convert_type([1.5, 2.5], Array(Float)) == [1.5, 2.5]
     assert warehouse.convert_type(["a", "b"], Array(String)) == ["a", "b"]
     assert warehouse.convert_type([[1, 2], [3, 4]], Array(Array(Int))) == [
         [1, 2],
         [3, 4],
     ]
 
+    # JSON Tests
+    assert warehouse.convert_type('{"a": 1}', JSON()) == '{"a": 1}'
+    assert warehouse.convert_type({"a": 1}, JSON()) == '{"a": 1}'
+    assert warehouse.convert_type([{"a": 1}], JSON()) == '[{"a": 1}]'
+    with pytest.raises(ValueError):
+        warehouse.convert_type(0.5, JSON())
+
     # convert array to compatible type
     converted = warehouse.convert_type([1, 2], Array(Float))
     assert converted == [1.0, 2.0]
     assert all(isinstance(c, float) for c in converted)
 
     # convert nested array to compatible type
     converted = warehouse.convert_type([[1, 2], [3, 4]], Array(Array(Float)))
@@ -152,11 +159,7 @@
     # error, float to int
     with pytest.raises(ValueError):
         warehouse.convert_type(1.5, Int())
 
     # error, float to int in list
     with pytest.raises(ValueError):
         warehouse.convert_type([1.5, 1], Array(Int))
-
-    # error, string to json
-    with pytest.raises(ValueError):
-        warehouse.convert_type('{"a": 1}', JSON)
```

### Comparing `dvcx-0.82.0/tests/unit/test_database_engine.py` & `dvcx-0.82.1/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_dataset.py` & `dvcx-0.82.1/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_dataset_row.py` & `dvcx-0.82.1/tests/unit/test_dataset_row.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_dispatch.py` & `dvcx-0.82.1/tests/unit/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_fileslice.py` & `dvcx-0.82.1/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_id_generator.py` & `dvcx-0.82.1/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_listing.py` & `dvcx-0.82.1/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_metastore.py` & `dvcx-0.82.1/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_query_params.py` & `dvcx-0.82.1/tests/unit/test_query_params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_serializer.py` & `dvcx-0.82.1/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_session.py` & `dvcx-0.82.1/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_storage.py` & `dvcx-0.82.1/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_udf.py` & `dvcx-0.82.1/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_utils.py` & `dvcx-0.82.1/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/unit/test_warehouse.py` & `dvcx-0.82.1/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.82.0/tests/utils.py` & `dvcx-0.82.1/tests/utils.py`

 * *Files identical despite different names*

