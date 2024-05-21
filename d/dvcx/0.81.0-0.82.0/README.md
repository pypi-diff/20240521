# Comparing `tmp/dvcx-0.81.0.tar.gz` & `tmp/dvcx-0.82.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvcx-0.81.0.tar", last modified: Mon May 20 05:05:01 2024, max compression
+gzip compressed data, was "dvcx-0.82.0.tar", last modified: Mon May 20 11:45:42 2024, max compression
```

## Comparing `dvcx-0.81.0.tar` & `dvcx-0.82.0.tar`

### file list

```diff
@@ -1,252 +1,252 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.046252 dvcx-0.81.0/
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-20 05:04:50.000000 dvcx-0.81.0/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 05:04:50.000000 dvcx-0.81.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:00.994253 dvcx-0.81.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:00.994253 dvcx-0.81.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-20 05:04:50.000000 dvcx-0.81.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 05:04:50.000000 dvcx-0.81.0/.github/ISSUE_TEMPLATE/empty_issue.md
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-20 05:04:50.000000 dvcx-0.81.0/.github/ISSUE_TEMPLATE/epic-or-story.md
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 05:04:50.000000 dvcx-0.81.0/.github/codecov.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 05:04:50.000000 dvcx-0.81.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:00.994253 dvcx-0.81.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-20 05:04:50.000000 dvcx-0.81.0/.github/workflows/benchmarks.yml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-20 05:04:50.000000 dvcx-0.81.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-20 05:04:50.000000 dvcx-0.81.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 05:04:50.000000 dvcx-0.81.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-20 05:04:50.000000 dvcx-0.81.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-20 05:04:50.000000 dvcx-0.81.0/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:00.994253 dvcx-0.81.0/.reuse/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 05:04:50.000000 dvcx-0.81.0/.reuse/dep5
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-20 05:04:50.000000 dvcx-0.81.0/.safety-policy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-20 05:04:50.000000 dvcx-0.81.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-20 05:04:50.000000 dvcx-0.81.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-20 05:04:50.000000 dvcx-0.81.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:00.998252 dvcx-0.81.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-20 05:04:50.000000 dvcx-0.81.0/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-20 05:04:50.000000 dvcx-0.81.0/LICENSES/BSD-3-Clause.txt
--rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-20 05:04:50.000000 dvcx-0.81.0/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-20 05:05:01.046252 dvcx-0.81.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-20 05:04:50.000000 dvcx-0.81.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:00.998252 dvcx-0.81.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-20 05:04:50.000000 dvcx-0.81.0/docs/udfs.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:00.998252 dvcx-0.81.0/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/blip2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/clip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/common_sql_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/dir_expansion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/iptc_exif_xmp_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/llava2_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/llm-claude-aggregate-query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/llm-claude-simple-query.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/llm-claude.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.002252 dvcx-0.81.0/examples/neurips/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/neurips/README
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/neurips/distance_to_query.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/neurips/llm_chat.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/neurips/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/neurips/single_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/neurips/text_loaders.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/openai_image_desc_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/openimage-detect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/pose_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/torch-loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.002252 dvcx-0.81.0/examples/udfs/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/udfs/batching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/udfs/image_transformation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/udfs/parallel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/udfs/simple.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/udfs/stateful.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/udfs/stateful_similarity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/unstructured-text.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/wds.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/wds_filtered.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/wds_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.002252 dvcx-0.81.0/examples/zalando/
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/zalando/zalando_clip.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/zalando/zalando_dir_as_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/zalando/zalando_splits_and_classes_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-20 05:04:50.000000 dvcx-0.81.0/examples/zalando/zalando_splits_and_classes_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-20 05:04:50.000000 dvcx-0.81.0/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-20 05:04:50.000000 dvcx-0.81.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 05:05:01.046252 dvcx-0.81.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:00.990253 dvcx-0.81.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.006253 dvcx-0.81.0/src/dvcx/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-20 05:05:00.000000 dvcx-0.81.0/src/dvcx/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.010253 dvcx-0.81.0/src/dvcx/catalog/
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72515 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/catalog/catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/catalog/datasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/catalog/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/cli_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.010253 dvcx-0.81.0/src/dvcx/client/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/client/azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/client/fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/client/fsspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/client/gcs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/client/local.py
--rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/client/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.014253 dvcx-0.81.0/src/dvcx/data_storage/
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/data_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/data_storage/db_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/data_storage/id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)    45892 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/data_storage/metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/data_storage/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/data_storage/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)    26305 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/data_storage/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    33673 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/data_storage/warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)    17256 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.018252 dvcx-0.81.0/src/dvcx/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/claude.py
--rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/feature.py
--rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/feature_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/gpt4_vision.py
--rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/hf_image_to_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/hf_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/image_transform.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/iptc_exif_xmp.py
--rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/tar_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/unstructured.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/webdataset_laion.py
--rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/lib/webdataset_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/nodes_fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/nodes_thread_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.022252 dvcx-0.81.0/src/dvcx/query/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/query/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/query/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)    61468 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/query/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/query/dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/query/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/query/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/query/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/query/udf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.022252 dvcx-0.81.0/src/dvcx/remote/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/remote/studio.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.022252 dvcx-0.81.0/src/dvcx/sql/
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.022252 dvcx-0.81.0/src/dvcx/sql/default/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/default/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.026253 dvcx-0.81.0/src/dvcx/sql/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/functions/array.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/functions/conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/functions/path.py
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/functions/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/functions/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/selectable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.026253 dvcx-0.81.0/src/dvcx/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/sqlite/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/sqlite/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/sqlite/vector.py
--rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/sql/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    10452 2024-05-20 05:04:50.000000 dvcx-0.81.0/src/dvcx/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.038252 dvcx-0.81.0/src/dvcx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-20 05:05:00.000000 dvcx-0.81.0/src/dvcx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-20 05:05:00.000000 dvcx-0.81.0/src/dvcx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 05:05:00.000000 dvcx-0.81.0/src/dvcx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 05:05:00.000000 dvcx-0.81.0/src/dvcx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-20 05:05:00.000000 dvcx-0.81.0/src/dvcx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 05:05:00.000000 dvcx-0.81.0/src/dvcx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.026253 dvcx-0.81.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.026253 dvcx-0.81.0/tests/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/benchmarks/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/benchmarks/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/benchmarks/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    16483 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.030253 dvcx-0.81.0/tests/func/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/func/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    35078 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/func/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/func/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)   113497 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/func/test_dataset_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    28872 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/func/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/func/test_ls.py
--rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/func/test_pull.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/func/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/func/test_query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.030253 dvcx-0.81.0/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/scripts/name_len_normal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/scripts/name_len_slow.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/test_cli_e2e.py
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/test_query_e2e.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.034253 dvcx-0.81.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.038252 dvcx-0.81.0/tests/unit/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/lib/test_cached_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/lib/test_feature.py
--rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/lib/test_feature_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/lib/test_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/lib/test_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/lib/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/lib/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/lib/test_webdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/lib/test_webdataset_meta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.038252 dvcx-0.81.0/tests/unit/sql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 05:05:01.038252 dvcx-0.81.0/tests/unit/sql/sqlite/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/sql/sqlite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/sql/sqlite/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/sql/test_array.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/sql/test_conditional.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/sql/test_path.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/sql/test_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/sql/test_selectable.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/sql/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_asyn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_catalog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_catalog_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_cli_parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_client_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_data_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_database_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_dataset_row.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_fileslice.py
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_id_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_listing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_metastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_query_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_session.py
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_udf.py
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/unit/test_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-20 05:04:50.000000 dvcx-0.81.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.146879 dvcx-0.82.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-20 11:45:33.000000 dvcx-0.82.0/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-20 11:45:33.000000 dvcx-0.82.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.098879 dvcx-0.82.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.102879 dvcx-0.82.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/ISSUE_TEMPLATE/empty_issue.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/ISSUE_TEMPLATE/epic-or-story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.102879 dvcx-0.82.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/workflows/benchmarks.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3660 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 11:45:33.000000 dvcx-0.82.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-20 11:45:33.000000 dvcx-0.82.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-20 11:45:33.000000 dvcx-0.82.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.102879 dvcx-0.82.0/.reuse/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 11:45:33.000000 dvcx-0.82.0/.reuse/dep5
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-20 11:45:33.000000 dvcx-0.82.0/.safety-policy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5392 2024-05-20 11:45:33.000000 dvcx-0.82.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-20 11:45:33.000000 dvcx-0.82.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-20 11:45:33.000000 dvcx-0.82.0/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.102879 dvcx-0.82.0/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-05-20 11:45:33.000000 dvcx-0.82.0/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-20 11:45:33.000000 dvcx-0.82.0/LICENSES/BSD-3-Clause.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     9411 2024-05-20 11:45:33.000000 dvcx-0.82.0/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-20 11:45:42.146879 dvcx-0.82.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-20 11:45:33.000000 dvcx-0.82.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.102879 dvcx-0.82.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2778 2024-05-20 11:45:33.000000 dvcx-0.82.0/docs/udfs.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.106879 dvcx-0.82.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/blip2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/common_sql_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/dir_expansion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2648 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/iptc_exif_xmp_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/llava2_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/llm-claude-aggregate-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/llm-claude-simple-query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/llm-claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.106879 dvcx-0.82.0/examples/neurips/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/neurips/README
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/neurips/distance_to_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/neurips/llm_chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/neurips/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/neurips/single_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/neurips/text_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/openai_image_desc_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/openimage-detect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/pose_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/torch-loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.110879 dvcx-0.82.0/examples/udfs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/udfs/batching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/udfs/image_transformation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/udfs/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/udfs/simple.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/udfs/stateful.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/udfs/stateful_similarity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/unstructured-text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/wds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/wds_filtered.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/wds_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.110879 dvcx-0.82.0/examples/zalando/
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/zalando/zalando_clip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/zalando/zalando_dir_as_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/zalando/zalando_splits_and_classes_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-20 11:45:33.000000 dvcx-0.82.0/examples/zalando/zalando_splits_and_classes_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-20 11:45:33.000000 dvcx-0.82.0/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5273 2024-05-20 11:45:33.000000 dvcx-0.82.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 11:45:42.146879 dvcx-0.82.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.094879 dvcx-0.82.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.114879 dvcx-0.82.0/src/dvcx/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-20 11:45:41.000000 dvcx-0.82.0/src/dvcx/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.114879 dvcx-0.82.0/src/dvcx/catalog/
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72515 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/catalog/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/catalog/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7156 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/catalog/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31848 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2418 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/cli_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.118879 dvcx-0.82.0/src/dvcx/client/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1876 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/fsspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/gcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3563 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/client/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.118879 dvcx-0.82.0/src/dvcx/data_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3235 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/db_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45790 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26305 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33673 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/data_storage/warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17004 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.122879 dvcx-0.82.0/src/dvcx/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3564 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/claude.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16438 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10195 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4617 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/feature_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10249 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5991 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/gpt4_vision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3295 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/hf_image_to_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/hf_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3047 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/image_transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/iptc_exif_xmp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4385 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/tar_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7782 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/unstructured.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/webdataset_laion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/lib/webdataset_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6675 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/nodes_fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/nodes_thread_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4276 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.126879 dvcx-0.82.0/src/dvcx/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2562 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61468 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7014 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/query/udf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.126879 dvcx-0.82.0/src/dvcx/remote/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7471 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/remote/studio.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.126879 dvcx-0.82.0/src/dvcx/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.126879 dvcx-0.82.0/src/dvcx/sql/default/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/default/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.126879 dvcx-0.82.0/src/dvcx/sql/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/functions/array.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/functions/conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/functions/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/functions/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/functions/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/selectable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.130879 dvcx-0.82.0/src/dvcx/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/sqlite/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/sqlite/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/sqlite/vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/sql/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10452 2024-05-20 11:45:33.000000 dvcx-0.82.0/src/dvcx/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.142879 dvcx-0.82.0/src/dvcx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-05-20 11:45:42.000000 dvcx-0.82.0/src/dvcx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-20 11:45:42.000000 dvcx-0.82.0/src/dvcx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 11:45:42.000000 dvcx-0.82.0/src/dvcx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 11:45:42.000000 dvcx-0.82.0/src/dvcx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-20 11:45:42.000000 dvcx-0.82.0/src/dvcx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-20 11:45:42.000000 dvcx-0.82.0/src/dvcx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.130879 dvcx-0.82.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.130879 dvcx-0.82.0/tests/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/benchmarks/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/benchmarks/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/benchmarks/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16483 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5410 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.134879 dvcx-0.82.0/tests/func/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35078 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113497 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_dataset_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28872 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11153 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_ls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10517 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_pull.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9017 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/func/test_query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.134879 dvcx-0.82.0/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/scripts/name_len_normal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/scripts/name_len_slow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/test_cli_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/test_query_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.138879 dvcx-0.82.0/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.138879 dvcx-0.82.0/tests/unit/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_cached_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15029 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_feature.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10158 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_feature_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4111 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_webdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/lib/test_webdataset_meta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.142879 dvcx-0.82.0/tests/unit/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:42.142879 dvcx-0.82.0/tests/unit/sql/sqlite/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/sqlite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/sqlite/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/test_array.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/test_conditional.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/test_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/test_selectable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/sql/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4696 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_asyn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6963 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_catalog_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3228 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_cli_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2012 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_client_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_data_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2603 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_database_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_dataset_row.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1415 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_fileslice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_id_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_listing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_metastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_query_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3913 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/unit/test_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8201 2024-05-20 11:45:33.000000 dvcx-0.82.0/tests/utils.py
```

### Comparing `dvcx-0.81.0/.cruft.json` & `dvcx-0.82.0/.cruft.json`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/.github/ISSUE_TEMPLATE/bug_report.md` & `dvcx-0.82.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/.github/ISSUE_TEMPLATE/epic-or-story.md` & `dvcx-0.82.0/.github/ISSUE_TEMPLATE/epic-or-story.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/.github/workflows/benchmarks.yml` & `dvcx-0.82.0/.github/workflows/benchmarks.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/.github/workflows/release.yml` & `dvcx-0.82.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/.github/workflows/tests.yml` & `dvcx-0.82.0/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/.gitignore` & `dvcx-0.82.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/.pre-commit-config.yaml` & `dvcx-0.82.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/CODE_OF_CONDUCT.rst` & `dvcx-0.82.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/CONTRIBUTING.rst` & `dvcx-0.82.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/LICENSE` & `dvcx-0.82.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/LICENSES/Apache-2.0.txt` & `dvcx-0.82.0/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/LICENSES/BSD-3-Clause.txt` & `dvcx-0.82.0/LICENSES/BSD-3-Clause.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/LICENSES/Python-2.0.txt` & `dvcx-0.82.0/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/PKG-INFO` & `dvcx-0.82.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.81.0
+Version: 0.82.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.81.0/README.rst` & `dvcx-0.82.0/README.rst`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/docs/udfs.md` & `dvcx-0.82.0/docs/udfs.md`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/blip2_image_desc_lib.py` & `dvcx-0.82.0/examples/blip2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/clip.py` & `dvcx-0.82.0/examples/clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/common_sql_functions.py` & `dvcx-0.82.0/examples/common_sql_functions.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/dir_expansion.py` & `dvcx-0.82.0/examples/dir_expansion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/hf_pipeline.py` & `dvcx-0.82.0/examples/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/llava2_image_desc_lib.py` & `dvcx-0.82.0/examples/llava2_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/llm-claude-aggregate-query.py` & `dvcx-0.82.0/examples/llm-claude-aggregate-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/llm-claude-simple-query.py` & `dvcx-0.82.0/examples/llm-claude-simple-query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/llm-claude.py` & `dvcx-0.82.0/examples/llm-claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/loader.py` & `dvcx-0.82.0/examples/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/neurips/README` & `dvcx-0.82.0/examples/neurips/README`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/neurips/distance_to_query.py` & `dvcx-0.82.0/examples/neurips/distance_to_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/neurips/llm_chat.py` & `dvcx-0.82.0/examples/neurips/llm_chat.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/neurips/single_query.py` & `dvcx-0.82.0/examples/neurips/single_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/neurips/text_loaders.py` & `dvcx-0.82.0/examples/neurips/text_loaders.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/openai_image_desc_lib.py` & `dvcx-0.82.0/examples/openai_image_desc_lib.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/openimage-detect.py` & `dvcx-0.82.0/examples/openimage-detect.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/pose_detection.py` & `dvcx-0.82.0/examples/pose_detection.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/torch-loader.py` & `dvcx-0.82.0/examples/torch-loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/udfs/batching.py` & `dvcx-0.82.0/examples/udfs/batching.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/udfs/image_transformation.py` & `dvcx-0.82.0/examples/udfs/image_transformation.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/udfs/parallel.py` & `dvcx-0.82.0/examples/udfs/parallel.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/udfs/simple.py` & `dvcx-0.82.0/examples/udfs/simple.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/udfs/stateful.py` & `dvcx-0.82.0/examples/udfs/stateful.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/udfs/stateful_similarity.py` & `dvcx-0.82.0/examples/udfs/stateful_similarity.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/unstructured-text.py` & `dvcx-0.82.0/examples/unstructured-text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/wds.py` & `dvcx-0.82.0/examples/wds.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/wds_filtered.py` & `dvcx-0.82.0/examples/wds_filtered.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/wds_meta.py` & `dvcx-0.82.0/examples/wds_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/zalando/zalando_clip.py` & `dvcx-0.82.0/examples/zalando/zalando_clip.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/examples/zalando/zalando_dir_as_class.py` & `dvcx-0.82.0/examples/zalando/zalando_dir_as_class.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/noxfile.py` & `dvcx-0.82.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/pyproject.toml` & `dvcx-0.82.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/asyn.py` & `dvcx-0.82.0/src/dvcx/asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/cache.py` & `dvcx-0.82.0/src/dvcx/cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/catalog/catalog.py` & `dvcx-0.82.0/src/dvcx/catalog/catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/catalog/datasource.py` & `dvcx-0.82.0/src/dvcx/catalog/datasource.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/catalog/loader.py` & `dvcx-0.82.0/src/dvcx/catalog/loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/cli.py` & `dvcx-0.82.0/src/dvcx/cli.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/cli_utils.py` & `dvcx-0.82.0/src/dvcx/cli_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/client/azure.py` & `dvcx-0.82.0/src/dvcx/client/azure.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/client/fileslice.py` & `dvcx-0.82.0/src/dvcx/client/fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/client/fsspec.py` & `dvcx-0.82.0/src/dvcx/client/fsspec.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/client/gcs.py` & `dvcx-0.82.0/src/dvcx/client/gcs.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/client/local.py` & `dvcx-0.82.0/src/dvcx/client/local.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/client/s3.py` & `dvcx-0.82.0/src/dvcx/client/s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/config.py` & `dvcx-0.82.0/src/dvcx/config.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/data_storage/db_engine.py` & `dvcx-0.82.0/src/dvcx/data_storage/db_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/data_storage/id_generator.py` & `dvcx-0.82.0/src/dvcx/data_storage/id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/data_storage/metastore.py` & `dvcx-0.82.0/src/dvcx/data_storage/metastore.py`

 * *Files 0% similar despite different names*

```diff
@@ -415,15 +415,14 @@
             Column("shadow", Boolean, nullable=False),
             Column("status", Integer, nullable=False),
             Column("created_at", DateTime(timezone=True)),
             Column("finished_at", DateTime(timezone=True)),
             Column("error_message", Text, nullable=False, default=""),
             Column("error_stack", Text, nullable=False, default=""),
             Column("script_output", Text, nullable=False, default=""),
-            Column("job_id", Text, nullable=True),
             Column("sources", Text, nullable=False, default=""),
             Column("query_script", Text, nullable=False, default=""),
             Column("custom_column_types", JSON, nullable=True),
         ]
 
     @cached_property
     def _dataset_fields(self) -> list[str]:
@@ -451,15 +450,14 @@
             Column("finished_at", DateTime(timezone=True)),
             Column("error_message", Text, nullable=False, default=""),
             Column("error_stack", Text, nullable=False, default=""),
             Column("script_output", Text, nullable=False, default=""),
             Column("num_objects", BigInteger, nullable=True),
             Column("size", BigInteger, nullable=True),
             Column("preview", JSON, nullable=True),
-            Column("job_id", Text, nullable=True),
             Column("sources", Text, nullable=False, default=""),
             Column("query_script", Text, nullable=False, default=""),
             Column("custom_column_types", JSON, nullable=True),
             UniqueConstraint("dataset_id", "version"),
         ]
 
     @cached_property
```

### Comparing `dvcx-0.81.0/src/dvcx/data_storage/schema.py` & `dvcx-0.82.0/src/dvcx/data_storage/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/data_storage/serializer.py` & `dvcx-0.82.0/src/dvcx/data_storage/serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/data_storage/sqlite.py` & `dvcx-0.82.0/src/dvcx/data_storage/sqlite.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/data_storage/warehouse.py` & `dvcx-0.82.0/src/dvcx/data_storage/warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/dataset.py` & `dvcx-0.82.0/src/dvcx/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -166,34 +166,32 @@
     error_message: str
     error_stack: str
     script_output: str
     custom_column_types: dict[str, Union[SQLType, type[SQLType]]]
     num_objects: Optional[int]
     size: Optional[int]
     preview: Optional[list[dict]]
-    job_id: Optional[str] = None
     sources: str = ""
     query_script: str = ""
 
     @classmethod
-    def parse(  # noqa: PLR0913
+    def parse(
         cls: type[V],
         id: int,
         dataset_id: int,
         version: int,
         status: int,
         created_at: datetime,
         finished_at: Optional[datetime],
         error_message: str,
         error_stack: str,
         script_output: str,
         num_objects: Optional[int],
         size: Optional[int],
         preview: Optional[str],
-        job_id: Optional[str],
         custom_column_types: dict[str, Union[SQLType, type[SQLType]]],
         sources: str = "",
         query_script: str = "",
     ):
         return cls(
             id,
             dataset_id,
@@ -204,15 +202,14 @@
             error_message,
             error_stack,
             script_output,
             custom_column_types,
             num_objects,
             size,
             json.loads(preview) if preview else None,
-            job_id,
             sources,
             query_script,
         )
 
     def __eq__(self, other):
         if not isinstance(other, DatasetVersion):
             return False
@@ -263,15 +260,14 @@
     versions: list[DatasetVersion]
     status: int = Status.CREATED
     created_at: Optional[datetime] = None
     finished_at: Optional[datetime] = None
     error_message: str = ""
     error_stack: str = ""
     script_output: str = ""
-    job_id: Optional[str] = None
     sources: str = ""
     query_script: str = ""
 
     @staticmethod
     def parse_custom_column_types(
         ct: dict[str, Any],
     ) -> dict[str, Union[SQLType, type[SQLType]]]:
@@ -290,15 +286,14 @@
         shadow: int,
         status: int,
         created_at: datetime,
         finished_at: Optional[datetime],
         error_message: str,
         error_stack: str,
         script_output: str,
-        job_id: Optional[str],
         sources: str,
         query_script: str,
         custom_column_types: str,
         version_id: int,
         version_dataset_id: int,
         version: int,
         version_status: int,
@@ -306,15 +301,14 @@
         version_finished_at: Optional[datetime],
         version_error_message: str,
         version_error_stack: str,
         version_script_output: str,
         version_num_objects: Optional[int],
         version_size: Optional[int],
         version_preview: Optional[str],
-        version_job_id: Optional[str],
         version_sources: Optional[str],
         version_query_script: Optional[str],
         version_custom_column_types: str,
     ) -> "DatasetRecord":
         labels_lst: list[str] = json.loads(labels) if labels else []
         custom_column_types_dct: dict[str, Any] = (
             json.loads(custom_column_types) if custom_column_types else {}
@@ -334,15 +328,14 @@
             version_finished_at,
             version_error_message,
             version_error_stack,
             version_script_output,
             version_num_objects,
             version_size,
             version_preview,
-            version_job_id,
             cls.parse_custom_column_types(version_custom_column_types_dct),  # type: ignore[arg-type]
             version_sources,  # type: ignore[arg-type]
             version_query_script,  # type: ignore[arg-type]
         )
 
         return cls(
             id,
@@ -354,15 +347,14 @@
             [dataset_version],
             status,
             created_at,
             finished_at,
             error_message,
             error_stack,
             script_output,
-            job_id,
             sources,
             query_script,
         )
 
     @property
     def custom_column_types_serialized(self) -> dict[str, Any]:
         if not self.custom_column_types:
```

### Comparing `dvcx-0.81.0/src/dvcx/error.py` & `dvcx-0.82.0/src/dvcx/error.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/cached_stream.py` & `dvcx-0.82.0/src/dvcx/lib/cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/claude.py` & `dvcx-0.82.0/src/dvcx/lib/claude.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/dataset.py` & `dvcx-0.82.0/src/dvcx/lib/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/feature.py` & `dvcx-0.82.0/src/dvcx/lib/feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/feature_types.py` & `dvcx-0.82.0/src/dvcx/lib/feature_types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/feature_udf.py` & `dvcx-0.82.0/src/dvcx/lib/feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/file.py` & `dvcx-0.82.0/src/dvcx/lib/file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/gpt4_vision.py` & `dvcx-0.82.0/src/dvcx/lib/gpt4_vision.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/hf_image_to_text.py` & `dvcx-0.82.0/src/dvcx/lib/hf_image_to_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/hf_pipeline.py` & `dvcx-0.82.0/src/dvcx/lib/hf_pipeline.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/image.py` & `dvcx-0.82.0/src/dvcx/lib/image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/image_transform.py` & `dvcx-0.82.0/src/dvcx/lib/image_transform.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/iptc_exif_xmp.py` & `dvcx-0.82.0/src/dvcx/lib/iptc_exif_xmp.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/pytorch.py` & `dvcx-0.82.0/src/dvcx/lib/pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/reader.py` & `dvcx-0.82.0/src/dvcx/lib/reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/tar_file.py` & `dvcx-0.82.0/src/dvcx/lib/tar_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/text.py` & `dvcx-0.82.0/src/dvcx/lib/text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/udf.py` & `dvcx-0.82.0/src/dvcx/lib/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/unstructured.py` & `dvcx-0.82.0/src/dvcx/lib/unstructured.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/utils.py` & `dvcx-0.82.0/src/dvcx/lib/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/webdataset.py` & `dvcx-0.82.0/src/dvcx/lib/webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/webdataset_laion.py` & `dvcx-0.82.0/src/dvcx/lib/webdataset_laion.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/lib/webdataset_meta.py` & `dvcx-0.82.0/src/dvcx/lib/webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/listing.py` & `dvcx-0.82.0/src/dvcx/listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/node.py` & `dvcx-0.82.0/src/dvcx/node.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/nodes_fetcher.py` & `dvcx-0.82.0/src/dvcx/nodes_fetcher.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/nodes_thread_pool.py` & `dvcx-0.82.0/src/dvcx/nodes_thread_pool.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/progress.py` & `dvcx-0.82.0/src/dvcx/progress.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/query/batch.py` & `dvcx-0.82.0/src/dvcx/query/batch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/query/builtins.py` & `dvcx-0.82.0/src/dvcx/query/builtins.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/query/dataset.py` & `dvcx-0.82.0/src/dvcx/query/dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/query/dispatch.py` & `dvcx-0.82.0/src/dvcx/query/dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/query/params.py` & `dvcx-0.82.0/src/dvcx/query/params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/query/schema.py` & `dvcx-0.82.0/src/dvcx/query/schema.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/query/session.py` & `dvcx-0.82.0/src/dvcx/query/session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/query/udf.py` & `dvcx-0.82.0/src/dvcx/query/udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/remote/studio.py` & `dvcx-0.82.0/src/dvcx/remote/studio.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/sql/default/base.py` & `dvcx-0.82.0/src/dvcx/sql/default/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/sql/functions/array.py` & `dvcx-0.82.0/src/dvcx/sql/functions/array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/sql/functions/path.py` & `dvcx-0.82.0/src/dvcx/sql/functions/path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/sql/selectable.py` & `dvcx-0.82.0/src/dvcx/sql/selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/sql/sqlite/base.py` & `dvcx-0.82.0/src/dvcx/sql/sqlite/base.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/sql/sqlite/types.py` & `dvcx-0.82.0/src/dvcx/sql/sqlite/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/sql/types.py` & `dvcx-0.82.0/src/dvcx/sql/types.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/sql/utils.py` & `dvcx-0.82.0/src/dvcx/sql/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/storage.py` & `dvcx-0.82.0/src/dvcx/storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx/utils.py` & `dvcx-0.82.0/src/dvcx/utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx.egg-info/PKG-INFO` & `dvcx-0.82.0/src/dvcx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvcx
-Version: 0.81.0
+Version: 0.82.0
 Summary: DVCx
 Author-email: Dmitry Petrov <support@dvc.org>
 License: Apache-2.0
 Project-URL: Issues, https://github.com/iterative/dvcx/issues
 Project-URL: Source, https://github.com/iterative/dvcx
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dvcx-0.81.0/src/dvcx.egg-info/SOURCES.txt` & `dvcx-0.82.0/src/dvcx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/src/dvcx.egg-info/requires.txt` & `dvcx-0.82.0/src/dvcx.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/benchmarks/conftest.py` & `dvcx-0.82.0/tests/benchmarks/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/conftest.py` & `dvcx-0.82.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/data.py` & `dvcx-0.82.0/tests/data.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/func/test_catalog.py` & `dvcx-0.82.0/tests/func/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/func/test_client.py` & `dvcx-0.82.0/tests/func/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/func/test_dataset_query.py` & `dvcx-0.82.0/tests/func/test_dataset_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/func/test_datasets.py` & `dvcx-0.82.0/tests/func/test_datasets.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/func/test_ls.py` & `dvcx-0.82.0/tests/func/test_ls.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/func/test_pull.py` & `dvcx-0.82.0/tests/func/test_pull.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/func/test_pytorch.py` & `dvcx-0.82.0/tests/func/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/func/test_query.py` & `dvcx-0.82.0/tests/func/test_query.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/scripts/name_len_normal.py` & `dvcx-0.82.0/tests/scripts/name_len_normal.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/scripts/name_len_slow.py` & `dvcx-0.82.0/tests/scripts/name_len_slow.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/test_cli_e2e.py` & `dvcx-0.82.0/tests/test_cli_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/test_query_e2e.py` & `dvcx-0.82.0/tests/test_query_e2e.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/lib/test_cached_stream.py` & `dvcx-0.82.0/tests/unit/lib/test_cached_stream.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/lib/test_feature.py` & `dvcx-0.82.0/tests/unit/lib/test_feature.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/lib/test_feature_udf.py` & `dvcx-0.82.0/tests/unit/lib/test_feature_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/lib/test_file.py` & `dvcx-0.82.0/tests/unit/lib/test_file.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/lib/test_image.py` & `dvcx-0.82.0/tests/unit/lib/test_image.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/lib/test_reader.py` & `dvcx-0.82.0/tests/unit/lib/test_reader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/lib/test_text.py` & `dvcx-0.82.0/tests/unit/lib/test_text.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/lib/test_webdataset.py` & `dvcx-0.82.0/tests/unit/lib/test_webdataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/lib/test_webdataset_meta.py` & `dvcx-0.82.0/tests/unit/lib/test_webdataset_meta.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/sql/test_array.py` & `dvcx-0.82.0/tests/unit/sql/test_array.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/sql/test_conditional.py` & `dvcx-0.82.0/tests/unit/sql/test_conditional.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/sql/test_path.py` & `dvcx-0.82.0/tests/unit/sql/test_path.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/sql/test_selectable.py` & `dvcx-0.82.0/tests/unit/sql/test_selectable.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/sql/test_string.py` & `dvcx-0.82.0/tests/unit/sql/test_string.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_asyn.py` & `dvcx-0.82.0/tests/unit/test_asyn.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_cache.py` & `dvcx-0.82.0/tests/unit/test_cache.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_catalog.py` & `dvcx-0.82.0/tests/unit/test_catalog.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_catalog_loader.py` & `dvcx-0.82.0/tests/unit/test_catalog_loader.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_cli_parsing.py` & `dvcx-0.82.0/tests/unit/test_cli_parsing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_client.py` & `dvcx-0.82.0/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_client_s3.py` & `dvcx-0.82.0/tests/unit/test_client_s3.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_data_storage.py` & `dvcx-0.82.0/tests/unit/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_database_engine.py` & `dvcx-0.82.0/tests/unit/test_database_engine.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_dataset.py` & `dvcx-0.82.0/tests/unit/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_dataset_row.py` & `dvcx-0.82.0/tests/unit/test_dataset_row.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_dispatch.py` & `dvcx-0.82.0/tests/unit/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_fileslice.py` & `dvcx-0.82.0/tests/unit/test_fileslice.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_id_generator.py` & `dvcx-0.82.0/tests/unit/test_id_generator.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_listing.py` & `dvcx-0.82.0/tests/unit/test_listing.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_metastore.py` & `dvcx-0.82.0/tests/unit/test_metastore.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_query_params.py` & `dvcx-0.82.0/tests/unit/test_query_params.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_serializer.py` & `dvcx-0.82.0/tests/unit/test_serializer.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_session.py` & `dvcx-0.82.0/tests/unit/test_session.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_storage.py` & `dvcx-0.82.0/tests/unit/test_storage.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_udf.py` & `dvcx-0.82.0/tests/unit/test_udf.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_utils.py` & `dvcx-0.82.0/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/unit/test_warehouse.py` & `dvcx-0.82.0/tests/unit/test_warehouse.py`

 * *Files identical despite different names*

### Comparing `dvcx-0.81.0/tests/utils.py` & `dvcx-0.82.0/tests/utils.py`

 * *Files identical despite different names*

