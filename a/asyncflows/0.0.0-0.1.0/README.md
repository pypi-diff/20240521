# Comparing `tmp/asyncflows-0.0.0.tar.gz` & `tmp/asyncflows-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncflows-0.0.0.tar", max compression
+gzip compressed data, was "asyncflows-0.1.0.tar", max compression
```

## Comparing `asyncflows-0.0.0.tar` & `asyncflows-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,100 @@
--rw-r--r--   0        0        0       13 2024-02-29 23:44:29.635354 asyncflows-0.0.0/README.md
--rw-r--r--   0        0        0        0 2024-02-29 23:43:43.549064 asyncflows-0.0.0/asyncflows/__init__.py
--rw-r--r--   0        0        0      270 2024-02-29 23:44:16.117606 asyncflows-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 asyncflows-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4019 2024-05-21 18:49:40.901669 asyncflows-0.1.0/LICENSE
+-rw-r--r--   0        0        0    28983 2024-05-21 13:33:57.563727 asyncflows-0.1.0/README.md
+-rw-r--r--   0        0        0      215 2024-05-15 09:58:03.335562 asyncflows-0.1.0/asyncflows/__init__.py
+-rw-r--r--   0        0        0      721 2024-05-12 10:10:05.034562 asyncflows-0.1.0/asyncflows/actions/__init__.py
+-rw-r--r--   0        0        0     6399 2024-05-20 20:30:23.072739 asyncflows-0.1.0/asyncflows/actions/base.py
+-rw-r--r--   0        0        0     1867 2024-05-20 16:40:21.250679 asyncflows-0.1.0/asyncflows/actions/execute_db_statement.py
+-rw-r--r--   0        0        0     1385 2024-05-21 18:49:40.902332 asyncflows-0.1.0/asyncflows/actions/extract_list.py
+-rw-r--r--   0        0        0     1523 2024-05-20 16:40:21.250950 asyncflows-0.1.0/asyncflows/actions/extract_pdf_text.py
+-rw-r--r--   0        0        0     1428 2024-05-20 16:40:21.251162 asyncflows-0.1.0/asyncflows/actions/extract_xml_tag.py
+-rw-r--r--   0        0        0     1168 2024-05-20 16:40:21.251328 asyncflows-0.1.0/asyncflows/actions/get_db_schema.py
+-rw-r--r--   0        0        0      582 2024-05-15 09:58:03.336490 asyncflows-0.1.0/asyncflows/actions/get_url.py
+-rw-r--r--   0        0        0      860 2024-05-20 16:40:21.251520 asyncflows-0.1.0/asyncflows/actions/ocr.py
+-rw-r--r--   0        0        0    12704 2024-05-21 18:49:40.902970 asyncflows-0.1.0/asyncflows/actions/prompt.py
+-rw-r--r--   0        0        0     1297 2024-05-15 09:58:03.337540 asyncflows-0.1.0/asyncflows/actions/score.py
+-rw-r--r--   0        0        0     4075 2024-05-15 09:58:03.337971 asyncflows-0.1.0/asyncflows/actions/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-12 09:54:44.485155 asyncflows-0.1.0/asyncflows/actions/utils/__init__.py
+-rw-r--r--   0        0        0     4960 2024-05-21 18:49:40.903405 asyncflows-0.1.0/asyncflows/actions/utils/prompt_context.py
+-rw-r--r--   0        0        0     3678 2024-05-21 18:49:40.903948 asyncflows-0.1.0/asyncflows/asyncflows.py
+-rw-r--r--   0        0        0     2232 2024-05-21 18:30:22.703561 asyncflows-0.1.0/asyncflows/examples/.ipynb_checkpoints/hello_world-checkpoint.ipynb
+-rw-r--r--   0        0        0        0 2024-05-12 10:10:05.035098 asyncflows-0.1.0/asyncflows/examples/__init__.py
+-rw-r--r--   0        0        0     1163 2024-05-20 16:51:26.438570 asyncflows-0.1.0/asyncflows/examples/chatbot.yaml.bak
+-rw-r--r--   0        0        0     7471 2024-05-16 14:38:00.823014 asyncflows-0.1.0/asyncflows/examples/contract.txt
+-rw-r--r--   0        0        0      804 2024-05-20 14:00:39.130519 asyncflows-0.1.0/asyncflows/examples/contract_review.py
+-rw-r--r--   0        0        0      474 2024-05-16 14:36:36.045578 asyncflows-0.1.0/asyncflows/examples/contract_review.yaml
+-rw-r--r--   0        0        0      716 2024-05-20 16:40:21.252454 asyncflows-0.1.0/asyncflows/examples/debono.py
+-rw-r--r--   0        0        0     3297 2024-05-21 13:33:57.564653 asyncflows-0.1.0/asyncflows/examples/debono.yaml
+-rw-r--r--   0        0        0      699 2024-05-20 16:40:21.252664 asyncflows-0.1.0/asyncflows/examples/get_page_title.py
+-rw-r--r--   0        0        0      357 2024-05-21 13:33:57.564814 asyncflows-0.1.0/asyncflows/examples/get_page_title.yaml
+-rw-r--r--   0        0        0   294692 2024-05-21 18:49:40.904420 asyncflows-0.1.0/asyncflows/examples/hello_world.ipynb
+-rw-r--r--   0        0        0      651 2024-05-21 10:49:12.457282 asyncflows-0.1.0/asyncflows/examples/hello_world.py
+-rw-r--r--   0        0        0      194 2024-05-21 13:33:57.564969 asyncflows-0.1.0/asyncflows/examples/hello_world.yaml
+-rw-r--r--   0        0        0      815 2024-05-21 13:02:52.598983 asyncflows-0.1.0/asyncflows/examples/langchain_duckduckgo.py
+-rw-r--r--   0        0        0     1215 2024-05-21 13:07:51.635794 asyncflows-0.1.0/asyncflows/examples/langchain_duckduckgo.yaml
+-rw-r--r--   0        0        0     1344 2024-05-20 16:40:21.253340 asyncflows-0.1.0/asyncflows/examples/rag.py
+-rw-r--r--   0        0        0     1004 2024-05-21 13:33:57.565127 asyncflows-0.1.0/asyncflows/examples/rag.yaml
+-rw-r--r--   0        0        0      280 2024-05-12 10:10:05.036224 asyncflows-0.1.0/asyncflows/examples/recipes/caprese.md
+-rw-r--r--   0        0        0      380 2024-05-12 10:10:05.036325 asyncflows-0.1.0/asyncflows/examples/recipes/chana_masala.md
+-rw-r--r--   0        0        0      329 2024-05-12 10:10:05.036421 asyncflows-0.1.0/asyncflows/examples/recipes/coconut_soup.md
+-rw-r--r--   0        0        0      413 2024-05-12 10:10:05.036539 asyncflows-0.1.0/asyncflows/examples/recipes/gazpacho.md
+-rw-r--r--   0        0        0      326 2024-05-12 10:10:05.036642 asyncflows-0.1.0/asyncflows/examples/recipes/guacamole.md
+-rw-r--r--   0        0        0      375 2024-05-12 10:10:05.036745 asyncflows-0.1.0/asyncflows/examples/recipes/hummus.md
+-rw-r--r--   0        0        0      326 2024-05-12 10:10:05.036867 asyncflows-0.1.0/asyncflows/examples/recipes/miso_soup.md
+-rw-r--r--   0        0        0      331 2024-05-12 10:10:05.036965 asyncflows-0.1.0/asyncflows/examples/recipes/omelette.md
+-rw-r--r--   0        0        0      327 2024-05-12 10:10:05.037094 asyncflows-0.1.0/asyncflows/examples/recipes/stir_fry.md
+-rw-r--r--   0        0        0      321 2024-05-12 10:10:05.037211 asyncflows-0.1.0/asyncflows/examples/recipes/yogurt_parfait.md
+-rw-r--r--   0        0        0     1105 2024-05-20 16:40:21.253570 asyncflows-0.1.0/asyncflows/examples/sql_rag.py
+-rw-r--r--   0        0        0     1475 2024-05-21 13:33:57.565292 asyncflows-0.1.0/asyncflows/examples/sql_rag.yaml
+-rw-r--r--   0        0        0     1890 2024-05-12 09:54:44.488014 asyncflows-0.1.0/asyncflows/log_config.py
+-rw-r--r--   0        0        0        0 2024-05-12 09:54:44.488049 asyncflows-0.1.0/asyncflows/models/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-12 09:54:44.488196 asyncflows-0.1.0/asyncflows/models/blob.py
+-rw-r--r--   0        0        0        0 2024-05-12 09:54:44.488229 asyncflows-0.1.0/asyncflows/models/config/__init__.py
+-rw-r--r--   0        0        0     2986 2024-05-20 19:35:12.153432 asyncflows-0.1.0/asyncflows/models/config/action.py
+-rw-r--r--   0        0        0     2681 2024-05-12 10:10:05.037646 asyncflows-0.1.0/asyncflows/models/config/common.py
+-rw-r--r--   0        0        0     1207 2024-05-20 19:35:12.153719 asyncflows-0.1.0/asyncflows/models/config/flow.py
+-rw-r--r--   0        0        0     2335 2024-05-21 13:33:57.565461 asyncflows-0.1.0/asyncflows/models/config/model.py
+-rw-r--r--   0        0        0     5142 2024-05-21 18:49:40.904847 asyncflows-0.1.0/asyncflows/models/config/transform.py
+-rw-r--r--   0        0        0     5022 2024-05-21 18:49:40.905219 asyncflows-0.1.0/asyncflows/models/config/value_declarations.py
+-rw-r--r--   0        0        0     3303 2024-05-21 18:49:40.905822 asyncflows-0.1.0/asyncflows/models/file.py
+-rw-r--r--   0        0        0      700 2024-05-13 16:17:35.880887 asyncflows-0.1.0/asyncflows/models/primitives.py
+-rw-r--r--   0        0        0        0 2024-05-12 09:54:44.489456 asyncflows-0.1.0/asyncflows/repos/__init__.py
+-rw-r--r--   0        0        0    20233 2024-05-19 22:22:13.202504 asyncflows-0.1.0/asyncflows/repos/blob_repo.py
+-rw-r--r--   0        0        0     4421 2024-05-12 09:54:44.489894 asyncflows-0.1.0/asyncflows/repos/cache_repo.py
+-rw-r--r--   0        0        0        0 2024-05-12 09:54:44.489980 asyncflows-0.1.0/asyncflows/scripts/__init__.py
+-rw-r--r--   0        0        0     4811 2024-05-21 18:49:40.906170 asyncflows-0.1.0/asyncflows/scripts/generate_config_schema.py
+-rw-r--r--   0        0        0        0 2024-05-12 09:54:44.490205 asyncflows-0.1.0/asyncflows/services/__init__.py
+-rw-r--r--   0        0        0    38289 2024-05-21 18:49:40.906598 asyncflows-0.1.0/asyncflows/services/action_service.py
+-rw-r--r--   0        0        0        0 2024-05-12 09:54:44.490657 asyncflows-0.1.0/asyncflows/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-12 09:54:44.490724 asyncflows-0.1.0/asyncflows/tests/action_tests/__init__.py
+-rw-r--r--   0        0        0      724 2024-05-20 19:35:14.241422 asyncflows-0.1.0/asyncflows/tests/action_tests/test_execute_db_statement.py
+-rw-r--r--   0        0        0     1260 2024-05-20 16:40:21.255826 asyncflows-0.1.0/asyncflows/tests/action_tests/test_extract_xml_tag.py
+-rw-r--r--   0        0        0      683 2024-05-20 19:35:14.241798 asyncflows-0.1.0/asyncflows/tests/action_tests/test_get_db_schema.py
+-rw-r--r--   0        0        0     7180 2024-05-21 18:49:40.906997 asyncflows-0.1.0/asyncflows/tests/action_tests/test_prompt.py
+-rw-r--r--   0        0        0     1902 2024-05-20 20:08:44.977289 asyncflows-0.1.0/asyncflows/tests/action_tests/test_transformers.py
+-rw-r--r--   0        0        0    11547 2024-05-20 19:35:14.242390 asyncflows-0.1.0/asyncflows/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-12 09:54:44.491406 asyncflows-0.1.0/asyncflows/tests/repos/__init__.py
+-rw-r--r--   0        0        0     8319 2024-05-12 09:54:44.491697 asyncflows-0.1.0/asyncflows/tests/repos/test_blob_repo.py
+-rw-r--r--   0        0        0     6567 2024-05-12 09:54:44.491921 asyncflows-0.1.0/asyncflows/tests/repos/test_cache_repo.py
+-rw-r--r--   0        0        0        0 2024-05-12 09:54:44.491954 asyncflows-0.1.0/asyncflows/tests/resources/__init__.py
+-rw-r--r--   0        0        0     5737 2024-05-15 09:58:03.339504 asyncflows-0.1.0/asyncflows/tests/resources/actions.py
+-rw-r--r--   0        0        0     4075 2024-05-20 16:40:21.256626 asyncflows-0.1.0/asyncflows/tests/resources/testing_actions.yaml
+-rw-r--r--   0        0        0    26138 2024-05-20 16:40:21.256882 asyncflows-0.1.0/asyncflows/tests/test_action_service.py
+-rw-r--r--   0        0        0     6172 2024-05-15 09:58:03.339805 asyncflows-0.1.0/asyncflows/tests/test_async_utils.py
+-rw-r--r--   0        0        0    11489 2024-05-13 16:17:35.887876 asyncflows-0.1.0/asyncflows/tests/test_config.py
+-rw-r--r--   0        0        0     2053 2024-05-20 19:35:14.242769 asyncflows-0.1.0/asyncflows/tests/test_run_examples.py
+-rw-r--r--   0        0        0        0 2024-05-12 09:54:44.493172 asyncflows-0.1.0/asyncflows/utils/__init__.py
+-rw-r--r--   0        0        0     9747 2024-05-21 18:49:40.907578 asyncflows-0.1.0/asyncflows/utils/async_utils.py
+-rw-r--r--   0        0        0      676 2024-05-12 09:54:44.493559 asyncflows-0.1.0/asyncflows/utils/cache_utils.py
+-rw-r--r--   0        0        0     8536 2024-05-21 18:49:40.908312 asyncflows-0.1.0/asyncflows/utils/config_utils.py
+-rw-r--r--   0        0        0      725 2024-05-20 16:40:21.258105 asyncflows-0.1.0/asyncflows/utils/db_utils.py
+-rw-r--r--   0        0        0      141 2024-05-15 12:42:30.812800 asyncflows-0.1.0/asyncflows/utils/docs_utils.py
+-rw-r--r--   0        0        0     1320 2024-05-12 09:54:44.493929 asyncflows-0.1.0/asyncflows/utils/jinja_utils.py
+-rw-r--r--   0        0        0     1482 2024-05-12 09:54:44.494040 asyncflows-0.1.0/asyncflows/utils/redis_utils.py
+-rw-r--r--   0        0        0     2686 2024-05-12 09:54:44.494175 asyncflows-0.1.0/asyncflows/utils/request_utils.py
+-rw-r--r--   0        0        0      382 2024-05-12 09:54:44.494297 asyncflows-0.1.0/asyncflows/utils/secret_utils.py
+-rw-r--r--   0        0        0      479 2024-05-12 09:54:44.494408 asyncflows-0.1.0/asyncflows/utils/sentinel_utils.py
+-rw-r--r--   0        0        0      451 2024-05-12 09:54:44.494528 asyncflows-0.1.0/asyncflows/utils/singleton_utils.py
+-rw-r--r--   0        0        0     3333 2024-05-20 16:40:21.258363 asyncflows-0.1.0/asyncflows/utils/transformers_utils.py
+-rw-r--r--   0        0        0     2507 2024-05-15 09:08:48.883647 asyncflows-0.1.0/asyncflows/utils/type_utils.py
+-rw-r--r--   0        0        0     2413 2024-05-21 18:49:40.910871 asyncflows-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    31207 1970-01-01 00:00:00.000000 asyncflows-0.1.0/PKG-INFO
```

