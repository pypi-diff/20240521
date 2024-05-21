# Comparing `tmp/raga_llm_hub-1.0.0.11b2.tar.gz` & `tmp/raga-llm-hub-1.0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga_llm_hub-1.0.0.11b2.tar", last modified: Tue May 21 07:17:19 2024, max compression
+gzip compressed data, was "raga-llm-hub-1.0.0.9.tar", last modified: Thu Mar  7 10:50:34 2024, max compression
```

## Comparing `raga_llm_hub-1.0.0.11b2.tar` & `raga-llm-hub-1.0.0.9.tar`

### file list

```diff
@@ -1,355 +1,356 @@
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.923992 raga_llm_hub-1.0.0.11b2/
--rw-r--r--   0 kiran-raga   (501) staff       (20)    19126 2024-03-06 21:44:48.000000 raga_llm_hub-1.0.0.11b2/LICENSE
--rw-r--r--   0 kiran-raga   (501) staff       (20)      662 2024-03-06 20:18:08.000000 raga_llm_hub-1.0.0.11b2/MANIFEST.in
--rw-r--r--   0 kiran-raga   (501) staff       (20)    30908 2024-05-21 07:17:19.923666 raga_llm_hub-1.0.0.11b2/PKG-INFO
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5924 2024-03-07 20:42:11.000000 raga_llm_hub-1.0.0.11b2/README.md
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3108 2024-05-21 07:16:59.000000 raga_llm_hub-1.0.0.11b2/pyproject.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)       38 2024-05-21 07:17:19.924046 raga_llm_hub-1.0.0.11b2/setup.cfg
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.865261 raga_llm_hub-1.0.0.11b2/src/
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.867741 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1330 2024-05-21 07:17:05.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1599 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/api_client_manager.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4085 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/db_manager.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.872845 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1526 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)    14467 2024-03-07 08:27:54.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.873833 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      654 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4688 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/analyzer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)       52 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/exception.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2292 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/faker.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     7852 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/ner_mapping.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.874182 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      510 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      239 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/phone_recognizer.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.874811 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      380 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      294 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/crypto_recognizer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      626 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/custom_pattern_recognizer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      365 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/email_recognizer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1288 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/ip_recognizer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     9730 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/regex_patterns.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     7271 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/transformers_helpers.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)    14186 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/transformers_recognizer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3734 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/ban_competitors.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4232 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/ban_substrings.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4380 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/ban_topics.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6076 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/code.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5101 2024-03-07 09:40:54.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/deanonymize.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2668 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/factual_consistency.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1401 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/gibberish.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1718 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/invisible_text.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1178 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/ir_metrics_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3085 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/json_verify.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6764 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/language.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3192 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/language_same.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2573 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/malicious_url.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      327 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/match_type.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3387 2024-03-07 08:27:54.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/no_refusal.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1397 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/nsfw.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1293 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/politeness.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2047 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/profanity.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1595 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/reading_time.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4022 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/regex.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.874943 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.886863 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/
--rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      478 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/adafruit.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      622 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/adobe.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      350 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/age_secret_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      487 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/airtable_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      354 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/algolia_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      653 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/alibaba.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      762 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/asana.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      550 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/atlassian_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      572 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/authress_access_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      522 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/beamer_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      813 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/bitbucket.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      787 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/bittrex.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      362 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/clojars_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      535 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/codecov_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      543 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/coinbase_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      828 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/confluent.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      526 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/contentful_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      371 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/databricks_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      503 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/datadog_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      559 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/defined_networking_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      631 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/digitalocean.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1009 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/discord.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      361 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/doppler_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      534 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/droneci_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1046 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/dropbox.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      371 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/duffel_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      385 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/dynatrace_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      437 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/easypost.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      516 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/etsy_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      540 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/facebook_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      507 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/fastly_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      802 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/finicity.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      534 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/finnhub_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      528 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/flickr_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      563 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/flutterwave.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      367 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/frameio_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      552 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/freshbooks_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      366 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/gcp_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      638 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/github_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      539 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/gitlab.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      530 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/gitter_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      570 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/gocardless_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      748 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/grafana.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      462 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/hashicorp_tf_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      526 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/heroku_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      567 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/hubspot_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      579 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/huggingface.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      500 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/intercom_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      827 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/jfrog.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1145 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/jwt.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      539 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/kraken_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      829 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/kucoin.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      531 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/launchdarkly_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      609 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/linear.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      804 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/linkedin.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      778 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/lob.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1099 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/mailgun.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      531 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/mapbox_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      552 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/mattermost_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      891 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/messagebird.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      608 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/microsoft_teams_webhook.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      541 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/netlify_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1115 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/new_relic.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      556 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/nytimes_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      491 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/okta_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      395 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/openai_api_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      755 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/planetscale.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      396 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/postman_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      346 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/prefect_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      342 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/pulumi_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      337 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/pypi_upload_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      509 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/rapidapi_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      357 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/readme_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      366 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/rubygems_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      325 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/scalingo_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      832 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/sendbird.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      370 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/sendgrid_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      411 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/sendinblue_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      497 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/sentry_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      393 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/shippo_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      766 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/shopify.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      804 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/sidekiq.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1217 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/slack.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      523 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/snyk_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      570 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/squarespace_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      652 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/sumologic.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      419 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/telegram_bot_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      508 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/travisci_access_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      485 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/twitch_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1512 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/twitter.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      505 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/typeform_api_token.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      470 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/vault.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1028 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/yandex.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      494 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/zendesk_secret_key.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     9445 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/sensitive_patterns.json
--rw-r--r--   0 kiran-raga   (501) staff       (20)    16846 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/secrets.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6377 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/sensitive.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2704 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/sentiment.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2112 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/token_limit.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2441 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/url_reachability.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6341 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/utils.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1742 2024-03-07 08:27:54.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/valid_csv.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1338 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/valid_python.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      603 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/valid_sql.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1065 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/vault.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.887063 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      312 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/base_metrics.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1558 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/ir_metrics_test.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.891549 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      676 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      761 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/accuracy.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      699 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/ap.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1071 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/bpm.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      574 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/bpref.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      652 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/compat.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1984 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/f1_at_k.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2462 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/f1_score.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      574 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/infAP.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      831 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/insq.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      831 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/inst.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      853 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/iprec.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      588 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/judged.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      997 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/ndcg.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      838 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/nerr10.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      838 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/nerr11.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      948 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/nerr8.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      948 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/nerr9.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      514 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/numq.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      660 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/numrel.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      576 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/numret.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      752 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/p.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1585 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/precision.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1625 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/precision_at_k.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      752 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/r.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      716 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/rbp.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1573 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/recall.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1616 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/recall_at_k.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1081 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/retrieval_metrics.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      688 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/rprec.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1083 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/sdcg.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      688 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/setap.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      750 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/setf.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      829 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/setp.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      572 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/setr.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      764 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/success.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.891794 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/observer/
--rw-r--r--   0 kiran-raga   (501) staff       (20)      116 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/observer/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2403 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/observer/raga_observer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4350 2024-03-07 11:57:56.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/raga_llm_eval.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2862 2024-03-06 20:19:53.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/raga_llm_observer.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4773 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/result_manager.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)    10744 2024-03-06 20:20:13.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/test_manager.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.901081 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2929 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/__init__.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2007 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/bias_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2087 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/chunk_impact_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3398 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/coherence_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2663 2024-03-07 08:27:54.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/complexity_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4200 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/conciseness_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6496 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/consistency_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4090 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/context_retrieval_metrics_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5505 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/contextual_precision_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5313 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/contextual_recall_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5211 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/contextual_relevancy_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4540 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/correctness_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1593 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/cosine_similarity_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      913 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/cost_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1856 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/cover_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     8480 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/dan_detectors.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)    55588 2024-03-06 20:20:05.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/dan_probes.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4494 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/dan_vulnerability_scanner.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6258 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/faithfulness_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5343 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/generic_evaluation_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1505 2024-03-08 11:14:33.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/grade_score_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5070 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/hallucination_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4122 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/harmless_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5056 2024-03-07 08:27:54.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/ir_metrics_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)      953 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/latency_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1338 2024-03-07 11:06:22.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/length_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     8008 2024-03-06 20:20:29.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/lmrc_detectors.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     8537 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/lmrc_probes.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4833 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/lmrc_vulnerability_scanner.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2748 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/maliciousness_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1731 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/matcher.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2796 2024-03-07 08:27:54.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/overall_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1873 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/pos_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6641 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/prompt_injection_modeleval.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1068 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/prompt_injection_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)    34353 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/prompt_template.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3398 2024-03-08 11:08:55.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/readability_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1993 2024-03-06 20:20:52.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/refusal_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6157 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/relevancy_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4046 2024-03-08 12:00:17.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/response_toxicity_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1367 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/sentiment_analysis_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5739 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/summarisation_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5657 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/template.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.901322 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/
--rw-r--r--   0 kiran-raga   (501) staff       (20)       66 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/__init__.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.912612 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1387 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/anonymize_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      790 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/ban_competitors_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1033 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/ban_substrings_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1291 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/ban_topics_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1371 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/bias_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      998 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/chunk_impact_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2058 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/code.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2703 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/coherence_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      881 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/complexity_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2841 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/conciseness_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1236 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/consistency_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6412 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/context_retrieval_metrics_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2829 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/contextual_precision_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1525 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/contextual_recall_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2629 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/contextual_relevancy_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      940 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/correctness_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1951 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/cosine_similarity_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)       74 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/cost_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1162 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/cover_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2264 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/factual_consistency_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2195 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/faithfulness_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2801 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/generic_evaluation_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1297 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/grade_score_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1695 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/hallucination_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1467 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/harmful_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1467 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/harmless_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      772 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/invisible_text_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      866 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/ir_metrics_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      527 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/json_verify_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      665 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/language_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1342 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/language_same_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)       92 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/latency_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      300 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/length_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/lmrc_vulnerability_scanner.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      333 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/malicious_url_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2005 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/maliciousness_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2934 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/no_refusal_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1914 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/overall_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1343 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/pos_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)       24 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/prompt_injection_modeleval_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1322 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/prompt_injection_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)       24 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/promptinject_modelcompare_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1319 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/readability_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2733 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/reading_time_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1113 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/refusal_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      130 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/regex_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2296 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/relevancy_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1086 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/response_toxicity_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)       98 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/secrets_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1740 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/sensitive_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      843 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/sentiment_analysis_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      224 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/sentiment_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     4780 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/summarisation_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1036 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/tokenlimit_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      299 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/toxicity_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)      193 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/url_reachability_guardrail.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1019 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/winner_test.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1493 2024-03-06 20:20:42.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/test_data.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)    28078 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_details.toml
--rw-r--r--   0 kiran-raga   (501) staff       (20)    53009 2024-03-07 11:06:22.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_executor.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     5266 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_utils.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3855 2024-03-08 11:59:28.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/toxicity_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2378 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/winner_test.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3685 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/track_manager.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.912886 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1920 2024-05-02 09:23:07.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/app.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2489 2024-04-07 07:48:55.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/helpers.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.913136 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/pages/
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2468 2024-04-25 05:36:29.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/pages/index.py
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1331 2024-04-25 05:37:07.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/pages/trace.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.914547 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/static/
--rwxr-xr-x   0 kiran-raga   (501) staff       (20)    96080 2024-03-07 20:42:42.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/static/favicon.png
--rwxr-xr-x   0 kiran-raga   (501) staff       (20)    92761 2024-03-07 20:42:42.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/static/logoG.png
--rwxr-xr-x   0 kiran-raga   (501) staff       (20)     8535 2024-03-07 20:42:42.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/static/main.js
--rwxr-xr-x   0 kiran-raga   (501) staff       (20)    13425 2024-03-07 20:42:42.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/static/style.css
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.915355 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2192 2024-03-07 09:21:26.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/base.html
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.917475 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/components/
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1191 2024-03-07 20:42:42.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/components/card.html
--rw-r--r--   0 kiran-raga   (501) staff       (20)      637 2024-03-07 20:42:42.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/components/checkbox.html
--rw-r--r--   0 kiran-raga   (501) staff       (20)      232 2024-03-07 20:42:42.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/components/data-level-view-col.html
--rw-r--r--   0 kiran-raga   (501) staff       (20)      713 2024-03-07 20:42:42.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/components/data-level-view-row.html
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1530 2024-03-07 20:42:42.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/components/pagination.html
--rw-r--r--   0 kiran-raga   (501) staff       (20)      699 2024-03-07 20:42:42.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/components/tooltip.html
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2687 2024-03-07 09:21:26.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/index.html
--rw-r--r--   0 kiran-raga   (501) staff       (20)     6085 2024-03-07 09:21:26.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/trace.html
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.917710 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/utils/
--rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/utils/__init__.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.920230 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/utils/data_files/
--rw-r--r--   0 kiran-raga   (501) staff       (20)  1331653 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/utils/data_files/inthewild_jailbreak_llms.txt
--rw-r--r--   0 kiran-raga   (501) staff       (20)     3777 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/utils/data_files/ldnoobw-en.txt
--rw-r--r--   0 kiran-raga   (501) staff       (20)     2839 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/utils/data_files/ofcom-potentially-offensive.txt
--rw-r--r--   0 kiran-raga   (501) staff       (20)   104117 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/utils/data_files/profanity_en.csv
--rw-r--r--   0 kiran-raga   (501) staff       (20)     1609 2024-03-06 19:02:16.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/utils/utils.py
-drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-05-21 07:17:19.922476 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub.egg-info/
--rw-r--r--   0 kiran-raga   (501) staff       (20)    30908 2024-05-21 07:17:19.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub.egg-info/PKG-INFO
--rw-r--r--   0 kiran-raga   (501) staff       (20)    18787 2024-05-21 07:17:19.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub.egg-info/SOURCES.txt
--rw-r--r--   0 kiran-raga   (501) staff       (20)        1 2024-05-21 07:17:19.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub.egg-info/dependency_links.txt
--rw-r--r--   0 kiran-raga   (501) staff       (20)      780 2024-05-21 07:17:19.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub.egg-info/requires.txt
--rw-r--r--   0 kiran-raga   (501) staff       (20)       13 2024-05-21 07:17:19.000000 raga_llm_hub-1.0.0.11b2/src/raga_llm_hub.egg-info/top_level.txt
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.618921 raga-llm-hub-1.0.0.9/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    19126 2024-03-06 21:44:48.000000 raga-llm-hub-1.0.0.9/LICENSE
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      662 2024-03-06 20:18:08.000000 raga-llm-hub-1.0.0.9/MANIFEST.in
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    30209 2024-03-07 10:50:34.618673 raga-llm-hub-1.0.0.9/PKG-INFO
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5258 2024-03-06 21:44:48.000000 raga-llm-hub-1.0.0.9/README.md
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3079 2024-03-07 10:49:07.000000 raga-llm-hub-1.0.0.9/pyproject.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       38 2024-03-07 10:50:34.618960 raga-llm-hub-1.0.0.9/setup.cfg
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.529247 raga-llm-hub-1.0.0.9/src/
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.533997 raga-llm-hub-1.0.0.9/src/raga_llm_hub/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1323 2024-03-07 10:50:03.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1599 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/api_client_manager.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4085 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/db_manager.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.544487 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1526 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    14467 2024-03-07 08:27:54.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.547494 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      654 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4688 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/analyzer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       52 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/exception.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2292 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/faker.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     7852 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/ner_mapping.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.547996 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      510 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      239 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/phone_recognizer.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.550592 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      380 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      294 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/crypto_recognizer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      626 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/custom_pattern_recognizer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      365 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/email_recognizer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1288 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/ip_recognizer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     9730 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/regex_patterns.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     7271 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/transformers_helpers.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    14186 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/transformers_recognizer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3734 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/ban_competitors.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4232 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/ban_substrings.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4380 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/ban_topics.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6076 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/code.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5101 2024-03-07 09:40:54.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/deanonymize.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2668 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/factual_consistency.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1401 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/gibberish.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1718 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/invisible_text.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1178 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/ir_metrics_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3085 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/json_verify.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6764 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/language.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3192 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/language_same.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2573 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/malicious_url.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      327 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/match_type.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3387 2024-03-07 08:27:54.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/no_refusal.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1397 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/nsfw.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1293 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/politeness.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2047 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/profanity.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1595 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/reading_time.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4022 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/regex.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.550767 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.570580 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      478 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/adafruit.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      622 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/adobe.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      350 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/age_secret_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      487 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/airtable_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      354 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/algolia_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      653 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/alibaba.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      762 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/asana.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      550 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/atlassian_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      572 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/authress_access_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      522 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/beamer_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      813 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/bitbucket.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      787 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/bittrex.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      362 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/clojars_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      535 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/codecov_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      543 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/coinbase_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      828 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/confluent.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      526 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/contentful_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      371 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/databricks_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      503 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/datadog_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      559 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/defined_networking_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      631 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/digitalocean.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1009 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/discord.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      361 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/doppler_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      534 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/droneci_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1046 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/dropbox.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      371 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/duffel_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      385 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/dynatrace_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      437 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/easypost.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      516 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/etsy_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      540 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/facebook_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      507 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/fastly_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      802 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/finicity.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      534 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/finnhub_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      528 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/flickr_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      563 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/flutterwave.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      367 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/frameio_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      552 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/freshbooks_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      366 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/gcp_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      638 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/github_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      539 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/gitlab.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      530 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/gitter_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      570 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/gocardless_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      748 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/grafana.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      462 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/hashicorp_tf_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      526 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/heroku_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      567 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/hubspot_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      579 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/huggingface.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      500 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/intercom_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      827 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/jfrog.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1145 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/jwt.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      539 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/kraken_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      829 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/kucoin.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      531 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/launchdarkly_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      609 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/linear.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      804 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/linkedin.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      778 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/lob.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1099 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/mailgun.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      531 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/mapbox_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      552 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/mattermost_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      891 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/messagebird.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      608 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/microsoft_teams_webhook.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      541 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/netlify_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1115 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/new_relic.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      556 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/nytimes_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      491 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/okta_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      395 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/openai_api_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      755 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/planetscale.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      396 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/postman_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      346 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/prefect_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      342 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/pulumi_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      337 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/pypi_upload_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      509 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/rapidapi_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      357 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/readme_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      366 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/rubygems_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      325 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/scalingo_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      832 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/sendbird.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      370 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/sendgrid_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      411 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/sendinblue_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      497 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/sentry_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      393 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/shippo_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      766 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/shopify.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      804 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/sidekiq.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1217 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/slack.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      523 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/snyk_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      570 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/squarespace_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      652 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/sumologic.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      419 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/telegram_bot_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      508 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/travisci_access_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      485 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/twitch_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1512 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/twitter.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      505 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/typeform_api_token.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      470 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/vault.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1028 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/yandex.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      494 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/zendesk_secret_key.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     9445 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/sensitive_patterns.json
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    16846 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/secrets.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6377 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/sensitive.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2704 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/sentiment.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2112 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/token_limit.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2441 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/url_reachability.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6341 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/utils.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1742 2024-03-07 08:27:54.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/valid_csv.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1338 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/valid_python.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      603 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/valid_sql.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1065 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/vault.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.570883 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      312 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/base_metrics.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1558 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/ir_metrics_test.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.578803 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      676 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      761 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/accuracy.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      699 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/ap.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1071 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/bpm.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      574 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/bpref.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      652 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/compat.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1984 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/f1_at_k.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2462 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/f1_score.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      574 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/infAP.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      831 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/insq.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      831 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/inst.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      853 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/iprec.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      588 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/judged.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      997 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/ndcg.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      838 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/nerr10.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      838 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/nerr11.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      948 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/nerr8.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      948 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/nerr9.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      514 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/numq.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      660 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/numrel.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      576 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/numret.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      752 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/p.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1585 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/precision.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1625 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/precision_at_k.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      752 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/r.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      716 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/rbp.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1573 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/recall.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1616 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/recall_at_k.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1081 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/retrieval_metrics.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      688 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/rprec.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1083 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/sdcg.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      688 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/setap.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      750 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/setf.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      829 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/setp.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      572 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/setr.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      764 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/success.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.579109 raga-llm-hub-1.0.0.9/src/raga_llm_hub/observer/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      116 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/observer/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2403 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/observer/raga_observer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4330 2024-03-07 09:40:54.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/raga_llm_eval.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2862 2024-03-06 20:19:53.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/raga_llm_observer.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4773 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/result_manager.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    10744 2024-03-06 20:20:13.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/test_manager.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.592183 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2929 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2007 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/bias_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2087 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/chunk_impact_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3398 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/coherence_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2663 2024-03-07 08:27:54.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/complexity_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4200 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/conciseness_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6496 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/consistency_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4090 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/context_retrieval_metrics_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5505 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/contextual_precision_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5313 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/contextual_recall_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5211 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/contextual_relevancy_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4540 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/correctness_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1593 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/cosine_similarity_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      913 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/cost_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1856 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/cover_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     8480 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/dan_detectors.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    55588 2024-03-06 20:20:05.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/dan_probes.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4494 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/dan_vulnerability_scanner.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6258 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/faithfulness_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5343 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/generic_evaluation_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1371 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/grade_score_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5070 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/hallucination_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4122 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/harmless_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5056 2024-03-07 08:27:54.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/ir_metrics_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      953 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/latency_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1338 2024-03-07 10:35:00.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/length_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     8008 2024-03-06 20:20:29.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/lmrc_detectors.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     8537 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/lmrc_probes.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4833 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/lmrc_vulnerability_scanner.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2748 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/maliciousness_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1731 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/matcher.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2796 2024-03-07 08:27:54.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/overall_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1873 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/pos_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6641 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/prompt_injection_modeleval.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1068 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/prompt_injection_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    34353 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/prompt_template.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3342 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/readability_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1993 2024-03-06 20:20:52.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/refusal_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6157 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/relevancy_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3056 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/response_toxicity_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1367 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/sentiment_analysis_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5739 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/summarisation_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5657 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/template.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.593229 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       66 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/__init__.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.605036 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1387 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/anonymize_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      790 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/ban_competitors_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1033 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/ban_substrings_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1291 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/ban_topics_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1371 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/bias_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      998 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/chunk_impact_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2058 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/code.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2703 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/coherence_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      881 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/complexity_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2841 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/conciseness_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1236 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/consistency_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6412 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/context_retrieval_metrics_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2829 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/contextual_precision_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1525 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/contextual_recall_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2629 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/contextual_relevancy_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      940 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/correctness_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1951 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/cosine_similarity_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       74 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/cost_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1162 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/cover_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2264 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/factual_consistency_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2195 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/faithfulness_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2801 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/generic_evaluation_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1297 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/grade_score_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1695 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/hallucination_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1467 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/harmful_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1467 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/harmless_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      772 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/invisible_text_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      866 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/ir_metrics_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      527 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/json_verify_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      665 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/language_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1342 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/language_same_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       92 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/latency_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      300 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/length_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/lmrc_vulnerability_scanner.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      333 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/malicious_url_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2005 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/maliciousness_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2934 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/no_refusal_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1914 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/overall_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1343 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/pos_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       24 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/prompt_injection_modeleval_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1322 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/prompt_injection_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       24 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/promptinject_modelcompare_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1319 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/readability_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2733 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/reading_time_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1113 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/refusal_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      130 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/regex_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2296 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/relevancy_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1086 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/response_toxicity_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       98 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/secrets_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1740 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/sensitive_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      843 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/sentiment_analysis_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      224 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/sentiment_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     4780 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/summarisation_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1036 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/tokenlimit_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      299 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/toxicity_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      193 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/url_reachability_guardrail.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1019 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/winner_test.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1493 2024-03-06 20:20:42.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/test_data.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    28078 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_details.toml
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    53009 2024-03-07 10:35:56.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_executor.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     5266 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_utils.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2857 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/toxicity_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2378 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/winner_test.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3685 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/track_manager.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.605425 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1400 2024-03-07 10:49:00.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/app.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2400 2024-03-07 08:27:54.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/helpers.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.605941 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/pages/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-07 09:40:54.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/pages/__init__.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2046 2024-03-07 09:40:54.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/pages/index.py
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1302 2024-03-07 09:40:54.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/pages/trace.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.608602 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/static/
+-rwxr-xr-x   0 kiran-raga   (501) staff       (20)    96080 2024-03-07 08:22:43.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/static/favicon.png
+-rwxr-xr-x   0 kiran-raga   (501) staff       (20)    92761 2024-03-07 08:22:43.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/static/logoG.png
+-rwxr-xr-x   0 kiran-raga   (501) staff       (20)     8535 2024-03-07 08:22:43.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/static/main.js
+-rwxr-xr-x   0 kiran-raga   (501) staff       (20)    13425 2024-03-07 08:22:43.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/static/style.css
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.609413 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1816 2024-03-07 08:22:43.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/base.html
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.610573 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/components/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1191 2024-03-07 08:22:43.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/components/card.html
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      637 2024-03-07 08:22:43.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/components/checkbox.html
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      232 2024-03-07 08:22:43.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/components/data-level-view-col.html
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      713 2024-03-07 08:22:43.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/components/data-level-view-row.html
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1530 2024-03-07 08:22:43.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/components/pagination.html
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      699 2024-03-07 08:22:43.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/components/tooltip.html
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2379 2024-03-07 08:22:43.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/index.html
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     6021 2024-03-07 08:22:43.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/trace.html
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.610823 raga-llm-hub-1.0.0.9/src/raga_llm_hub/utils/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)        0 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/utils/__init__.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.614293 raga-llm-hub-1.0.0.9/src/raga_llm_hub/utils/data_files/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)  1331653 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/utils/data_files/inthewild_jailbreak_llms.txt
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     3777 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/utils/data_files/ldnoobw-en.txt
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     2839 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/utils/data_files/ofcom-potentially-offensive.txt
+-rw-r--r--   0 kiran-raga   (501) staff       (20)   104117 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/utils/data_files/profanity_en.csv
+-rw-r--r--   0 kiran-raga   (501) staff       (20)     1609 2024-03-06 19:02:16.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub/utils/utils.py
+drwxr-xr-x   0 kiran-raga   (501) staff       (20)        0 2024-03-07 10:50:34.617604 raga-llm-hub-1.0.0.9/src/raga_llm_hub.egg-info/
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    30209 2024-03-07 10:50:34.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub.egg-info/PKG-INFO
+-rw-r--r--   0 kiran-raga   (501) staff       (20)    18825 2024-03-07 10:50:34.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub.egg-info/SOURCES.txt
+-rw-r--r--   0 kiran-raga   (501) staff       (20)        1 2024-03-07 10:50:34.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub.egg-info/dependency_links.txt
+-rw-r--r--   0 kiran-raga   (501) staff       (20)      765 2024-03-07 10:50:34.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub.egg-info/requires.txt
+-rw-r--r--   0 kiran-raga   (501) staff       (20)       13 2024-03-07 10:50:34.000000 raga-llm-hub-1.0.0.9/src/raga_llm_hub.egg-info/top_level.txt
```

### Comparing `raga_llm_hub-1.0.0.11b2/LICENSE` & `raga-llm-hub-1.0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/MANIFEST.in` & `raga-llm-hub-1.0.0.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/PKG-INFO` & `raga-llm-hub-1.0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-llm-hub
-Version: 1.0.0.11b2
+Version: 1.0.0.9
 Summary: Package for LLM Evaluation
 Author-email: Raga AI <rehan.asif@raga.ai>
 License: Attribution-NonCommercial-NoDerivatives 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
@@ -443,17 +443,16 @@
 Requires-Dist: langchain==0.1.9
 Requires-Dist: openai==1.11.1
 Requires-Dist: transformers==4.38.1
 Requires-Dist: Faker==23.2.1
 Requires-Dist: structlog==24.1.0
 Requires-Dist: json-repair==0.9.0
 Requires-Dist: fuzzysearch==0.7.3
-Requires-Dist: waitress~=3.0.0
+Requires-Dist: waitress==3.0.0
 Requires-Dist: sqlvalidator==0.0.20
-Requires-Dist: pyngrok==7.1.6
 Provides-Extra: ui
 Requires-Dist: Flask==3.0.2; extra == "ui"
 Provides-Extra: onnxruntime
 Provides-Extra: onnxruntime-gpu
 Provides-Extra: docs-dev
 Requires-Dist: mkdocs==1.5.3; extra == "docs-dev"
 Requires-Dist: mkdocs-autorefs==0.5.0; extra == "docs-dev"
@@ -491,57 +490,72 @@
 
 [![PyPI - Version](https://img.shields.io/pypi/v/raga-llm-hub?label=PyPI%20Package)](https://badge.fury.io/py/raga-llm-hub) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1PQGqDGdcSUxhSvpSQYX8ZdHf5r90WSYf?usp=sharing)
 </a> [![Python Compatibility](https://img.shields.io/pypi/pyversions/raga-llm-hub)](https://pypi.org/project/raga-llm-hub/) []()
 
 </div>
 
 
-Welcome to Raga LLM Hub, a comprehensive evaluation toolkit for Language and Learning Models (LLMs). With over 100 meticulously designed metrics, it is the most comprehensive platform that allows developers and organizations to evaluate and compare LLMs effectively and establish essential guardrails for LLMs and Retrieval Augmented Generation(RAG)  applications. These tests assess various aspects including Relevance & Understanding, Content Quality, Hallucination, Safety & Bias, Context Relevance, Guardrails, and Vulnerability scanning, along with a suite of Metric-Based Tests for quantitative analysis.
+Welcome to Raga LLM Eval, a comprehensive evaluation toolkit for Language and Learning Models (LLMs). With over 100 meticulously designed metrics, it is the most comprehensive platform that allows developers and organizations to evaluate and compare LLMs effectively and establish essential guardrails for LLMs and Retrieval Augmented Generation(RAG)  applications. These tests assess various aspects including Relevance & Understanding, Content Quality, Hallucination, Safety & Bias, Context Relevance, Guardrails, and Vulnerability scanning, along with a suite of Metric-Based Tests for quantitative analysis.
 
 The RagaAI LLM Hub is uniquely designed to help teams identify issues and fix them throughout the LLM lifecycle, by identifying issues across the entire RAG pipeline. This is pivotal for understanding the root cause of failures within an LLM application and addressing them at their source, revolutionizing the approach to ensuring reliability and trustworthiness.
 
 ## Installation
 
 ### Via pip
 
 ```bash
 # Create and activate a new Python environment
 python -m venv venv
 source venv/bin/activate
-
 # Install Raga LLM Hub
 pip install raga-llm-hub
 ```
 
 
 ### Via conda
 ```py
 # Create and activate a new Conda environment
 conda create --name myenv python=3.11
 conda activate myenv
-
 # Install Raga LLM Hub
 python -m pip install raga-llm-hub
 
 ```
 
 ## Quick Tour
 ### Initialization
 
 ```py
-from raga_llm_hub import RagaLLMEval
+from raga_llm_hub import RagaLLMEval, get_data
 
 # Initialize the evaluator with your API key
 evaluator = RagaLLMEval(api_key="your_api_key")
 ```
 
-### Run Tests
+
+
+4. Re-using Previous Results
+Leverage previous results for comparative analysis or to track your LLM's performance over time.
 
 ```py
+PREV_EVAL_ID = "PREVIOUS_RUN_ID"
+
+evaluator.load_eval(
+    eval_name=PREV_EVAL_ID
+)
+
+evaluator.print_results()
+evaluator.save_results("filename.json")
+```
 
+### Discover and Run Tests
+
+```py
+# List all available tests
+evaluator.list_available_tests()
 
 # Add and run a custom test
 evaluator.add_test(
     test_name="relevancy_test",
     data={
         "prompt": "How are you?",
         "context": "Responding as a student to a teacher.",
@@ -575,24 +589,14 @@
 previous_eval_id = "your_previous_eval_id_here"
 evaluator.load_eval(previous_eval_id)
 
 # After loading, you can print, save, or further analyze these results
 evaluator.print_results()
 ```
 
-## Examples
-- **Evaluation Tests**: Evaluation Tests assesse a Large Language Model's (LLM's) performance in generating responses that are accurate, relevant, and linguistically coherent to a wide array of prompts. This evaluation is pivotal in determining the model's ability to understand and respond appropriately to diverse user inputs, ranging from simple queries to complex, context-rich requests. 
-
-    [![Evaluation Tests](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1cY5eN5w7bK1CH8L8MYEAfrfzaVZ7LNS5?usp=sharing)
-
-- **Guardrail Tests**: Guardrails ensure that the models operate within predefined ethical, legal, and safety boundaries. These mechanisms are implemented to prevent the generation of biased, offensive, or harmful content, making sure that the outputs align with societal norms and values. 
-
-     [![Guardrails](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1TAX2PeicBBWHtdiZZelpXN5YcOB7WnEk?usp=sharing)
-
-
 ## Enterprise
 Enterprise Version
 Introducing raga-llm-platform,(enterprise version of raga-llm-hub)  for Large Language Model (LLM) evaluation and guardrails, designed to empower organizations to harness the full potential of LLMs securely and efficiently. Here’s what sets raga-llm-platform apart:
 1. **Production Scale Analysis**
 2. **State-of-the-Art Evaluation Methods and Metrics**
 3. **Issue Diagnosis and Remediation**
 4. **On-Prem/Private Cloud Deployment with Real-Time Streaming Support**
```

### Comparing `raga_llm_hub-1.0.0.11b2/README.md` & `raga-llm-hub-1.0.0.9/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -19,57 +19,72 @@
 
 [![PyPI - Version](https://img.shields.io/pypi/v/raga-llm-hub?label=PyPI%20Package)](https://badge.fury.io/py/raga-llm-hub) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1PQGqDGdcSUxhSvpSQYX8ZdHf5r90WSYf?usp=sharing)
 </a> [![Python Compatibility](https://img.shields.io/pypi/pyversions/raga-llm-hub)](https://pypi.org/project/raga-llm-hub/) []()
 
 </div>
 
 
-Welcome to Raga LLM Hub, a comprehensive evaluation toolkit for Language and Learning Models (LLMs). With over 100 meticulously designed metrics, it is the most comprehensive platform that allows developers and organizations to evaluate and compare LLMs effectively and establish essential guardrails for LLMs and Retrieval Augmented Generation(RAG)  applications. These tests assess various aspects including Relevance & Understanding, Content Quality, Hallucination, Safety & Bias, Context Relevance, Guardrails, and Vulnerability scanning, along with a suite of Metric-Based Tests for quantitative analysis.
+Welcome to Raga LLM Eval, a comprehensive evaluation toolkit for Language and Learning Models (LLMs). With over 100 meticulously designed metrics, it is the most comprehensive platform that allows developers and organizations to evaluate and compare LLMs effectively and establish essential guardrails for LLMs and Retrieval Augmented Generation(RAG)  applications. These tests assess various aspects including Relevance & Understanding, Content Quality, Hallucination, Safety & Bias, Context Relevance, Guardrails, and Vulnerability scanning, along with a suite of Metric-Based Tests for quantitative analysis.
 
 The RagaAI LLM Hub is uniquely designed to help teams identify issues and fix them throughout the LLM lifecycle, by identifying issues across the entire RAG pipeline. This is pivotal for understanding the root cause of failures within an LLM application and addressing them at their source, revolutionizing the approach to ensuring reliability and trustworthiness.
 
 ## Installation
 
 ### Via pip
 
 ```bash
 # Create and activate a new Python environment
 python -m venv venv
 source venv/bin/activate
-
 # Install Raga LLM Hub
 pip install raga-llm-hub
 ```
 
 
 ### Via conda
 ```py
 # Create and activate a new Conda environment
 conda create --name myenv python=3.11
 conda activate myenv
-
 # Install Raga LLM Hub
 python -m pip install raga-llm-hub
 
 ```
 
 ## Quick Tour
 ### Initialization
 
 ```py
-from raga_llm_hub import RagaLLMEval
+from raga_llm_hub import RagaLLMEval, get_data
 
 # Initialize the evaluator with your API key
 evaluator = RagaLLMEval(api_key="your_api_key")
 ```
 
-### Run Tests
+
+
+4. Re-using Previous Results
+Leverage previous results for comparative analysis or to track your LLM's performance over time.
 
 ```py
+PREV_EVAL_ID = "PREVIOUS_RUN_ID"
+
+evaluator.load_eval(
+    eval_name=PREV_EVAL_ID
+)
+
+evaluator.print_results()
+evaluator.save_results("filename.json")
+```
 
+### Discover and Run Tests
+
+```py
+# List all available tests
+evaluator.list_available_tests()
 
 # Add and run a custom test
 evaluator.add_test(
     test_name="relevancy_test",
     data={
         "prompt": "How are you?",
         "context": "Responding as a student to a teacher.",
@@ -103,24 +118,14 @@
 previous_eval_id = "your_previous_eval_id_here"
 evaluator.load_eval(previous_eval_id)
 
 # After loading, you can print, save, or further analyze these results
 evaluator.print_results()
 ```
 
-## Examples
-- **Evaluation Tests**: Evaluation Tests assesse a Large Language Model's (LLM's) performance in generating responses that are accurate, relevant, and linguistically coherent to a wide array of prompts. This evaluation is pivotal in determining the model's ability to understand and respond appropriately to diverse user inputs, ranging from simple queries to complex, context-rich requests. 
-
-    [![Evaluation Tests](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1cY5eN5w7bK1CH8L8MYEAfrfzaVZ7LNS5?usp=sharing)
-
-- **Guardrail Tests**: Guardrails ensure that the models operate within predefined ethical, legal, and safety boundaries. These mechanisms are implemented to prevent the generation of biased, offensive, or harmful content, making sure that the outputs align with societal norms and values. 
-
-     [![Guardrails](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1TAX2PeicBBWHtdiZZelpXN5YcOB7WnEk?usp=sharing)
-
-
 ## Enterprise
 Enterprise Version
 Introducing raga-llm-platform,(enterprise version of raga-llm-hub)  for Large Language Model (LLM) evaluation and guardrails, designed to empower organizations to harness the full potential of LLMs securely and efficiently. Here’s what sets raga-llm-platform apart:
 1. **Production Scale Analysis**
 2. **State-of-the-Art Evaluation Methods and Metrics**
 3. **Issue Diagnosis and Remediation**
 4. **On-Prem/Private Cloud Deployment with Real-Time Streaming Support**
```

#### html2text {}

```diff
@@ -3,15 +3,15 @@
               ******** _RR_aa_gg_aa_ _AA_II || _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn || _GG_ee_tt_tt_ii_nn_gg_ _SS_tt_aa_rr_tt_ee_dd ********
           [![PyPI - Version](https://img.shields.io/pypi/v/raga-llm-
  hub?label=PyPI%20Package)](https://badge.fury.io/py/raga-llm-hub) [![Open In
   Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://
 colab.research.google.com/drive/1PQGqDGdcSUxhSvpSQYX8ZdHf5r90WSYf?usp=sharing)
 [![Python Compatibility](https://img.shields.io/pypi/pyversions/raga-llm-hub)]
 (https://pypi.org/project/raga-llm-hub/) []()
-Welcome to Raga LLM Hub, a comprehensive evaluation toolkit for Language and
+Welcome to Raga LLM Eval, a comprehensive evaluation toolkit for Language and
 Learning Models (LLMs). With over 100 meticulously designed metrics, it is the
 most comprehensive platform that allows developers and organizations to
 evaluate and compare LLMs effectively and establish essential guardrails for
 LLMs and Retrieval Augmented Generation(RAG) applications. These tests assess
 various aspects including Relevance & Understanding, Content Quality,
 Hallucination, Safety & Bias, Context Relevance, Guardrails, and Vulnerability
 scanning, along with a suite of Metric-Based Tests for quantitative analysis.
@@ -21,55 +21,45 @@
 an LLM application and addressing them at their source, revolutionizing the
 approach to ensuring reliability and trustworthiness. ## Installation ### Via
 pip ```bash # Create and activate a new Python environment python -m venv venv
 source venv/bin/activate # Install Raga LLM Hub pip install raga-llm-hub ```
 ### Via conda ```py # Create and activate a new Conda environment conda create
 --name myenv python=3.11 conda activate myenv # Install Raga LLM Hub python -
 m pip install raga-llm-hub ``` ## Quick Tour ### Initialization ```py from
-raga_llm_hub import RagaLLMEval # Initialize the evaluator with your API key
-evaluator = RagaLLMEval(api_key="your_api_key") ``` ### Run Tests ```py # Add
-and run a custom test evaluator.add_test( test_name="relevancy_test", data=
-{ "prompt": "How are you?", "context": "Responding as a student to a teacher.",
-"response": "I am well, thank you.", }, arguments={"model": "gpt-4",
-"threshold": 0.5}, ).run() # Review the results evaluator.print_results() ```
-## Managing Results - **Instant Overview**: Quickly view your test results
-directly. - **Save for Detailed Analysis**: Export your results for
-comprehensive examination or sharing with your team. - **In-depth Access**:
-Utilize the app for advanced result processing and visualization. -
-**Historical Comparisons**: Leverage past evaluations for ongoing performance
-tracking. ```py # Printing Results: View your test results immediately for a
-quick analysis evaluator.print_results() # Saving Results: Export your results
-to a JSON file for in-depth analysis evaluator.save_results
-("my_test_results.json") # Accessing Results: Utilize the fetched detailed
-results and metrics for further processing or visualization detailed_results =
-evaluator.get_results() # Re-using Previous Results: If you have an evaluation
-ID from a previous run, you can load and compare those results previous_eval_id
-= "your_previous_eval_id_here" evaluator.load_eval(previous_eval_id) # After
-loading, you can print, save, or further analyze these results
-evaluator.print_results() ``` ## Examples - **Evaluation Tests**: Evaluation
-Tests assesse a Large Language Model's (LLM's) performance in generating
-responses that are accurate, relevant, and linguistically coherent to a wide
-array of prompts. This evaluation is pivotal in determining the model's ability
-to understand and respond appropriately to diverse user inputs, ranging from
-simple queries to complex, context-rich requests. [![Evaluation Tests](https://
-colab.research.google.com/assets/colab-badge.svg)](https://
-colab.research.google.com/drive/1cY5eN5w7bK1CH8L8MYEAfrfzaVZ7LNS5?usp=sharing)
-- **Guardrail Tests**: Guardrails ensure that the models operate within
-predefined ethical, legal, and safety boundaries. These mechanisms are
-implemented to prevent the generation of biased, offensive, or harmful content,
-making sure that the outputs align with societal norms and values. [!
-[Guardrails](https://colab.research.google.com/assets/colab-badge.svg)](https:/
-/colab.research.google.com/drive/1TAX2PeicBBWHtdiZZelpXN5YcOB7WnEk?usp=sharing)
-## Enterprise Enterprise Version Introducing raga-llm-platform,(enterprise
-version of raga-llm-hub) for Large Language Model (LLM) evaluation and
-guardrails, designed to empower organizations to harness the full potential of
-LLMs securely and efficiently. Hereâs what sets raga-llm-platform apart: 1.
-**Production Scale Analysis** 2. **State-of-the-Art Evaluation Methods and
-Metrics** 3. **Issue Diagnosis and Remediation** 4. **On-Prem/Private Cloud
-Deployment with Real-Time Streaming Support** 5. **Real-Time Evaluation and
-Guardrails** To learn more and see how raga-llm-platform can benefit your
-organization, [book a call with our team today](https://calendly.com/vijay-
-srinivas/ragaai-product-offering?month=2024-03). Discover the value of
-enterprise-grade LLM management tailored to your needs. ## Learn More For those
-who wish to dive deeper, we encourage exploring [our extensive documentation]
-(https://docs.raga.ai) For more details and the latest news from RagaAI, visit
-[our official website](https://raga.ai).
+raga_llm_hub import RagaLLMEval, get_data # Initialize the evaluator with your
+API key evaluator = RagaLLMEval(api_key="your_api_key") ``` 4. Re-using
+Previous Results Leverage previous results for comparative analysis or to track
+your LLM's performance over time. ```py PREV_EVAL_ID = "PREVIOUS_RUN_ID"
+evaluator.load_eval( eval_name=PREV_EVAL_ID ) evaluator.print_results()
+evaluator.save_results("filename.json") ``` ### Discover and Run Tests ```py #
+List all available tests evaluator.list_available_tests() # Add and run a
+custom test evaluator.add_test( test_name="relevancy_test", data={ "prompt":
+"How are you?", "context": "Responding as a student to a teacher.", "response":
+"I am well, thank you.", }, arguments={"model": "gpt-4", "threshold": 0.5},
+).run() # Review the results evaluator.print_results() ``` ## Managing Results
+- **Instant Overview**: Quickly view your test results directly. - **Save for
+Detailed Analysis**: Export your results for comprehensive examination or
+sharing with your team. - **In-depth Access**: Utilize the app for advanced
+result processing and visualization. - **Historical Comparisons**: Leverage
+past evaluations for ongoing performance tracking. ```py # Printing Results:
+View your test results immediately for a quick analysis evaluator.print_results
+() # Saving Results: Export your results to a JSON file for in-depth analysis
+evaluator.save_results("my_test_results.json") # Accessing Results: Utilize the
+fetched detailed results and metrics for further processing or visualization
+detailed_results = evaluator.get_results() # Re-using Previous Results: If you
+have an evaluation ID from a previous run, you can load and compare those
+results previous_eval_id = "your_previous_eval_id_here" evaluator.load_eval
+(previous_eval_id) # After loading, you can print, save, or further analyze
+these results evaluator.print_results() ``` ## Enterprise Enterprise Version
+Introducing raga-llm-platform,(enterprise version of raga-llm-hub) for Large
+Language Model (LLM) evaluation and guardrails, designed to empower
+organizations to harness the full potential of LLMs securely and efficiently.
+Hereâs what sets raga-llm-platform apart: 1. **Production Scale Analysis** 2.
+**State-of-the-Art Evaluation Methods and Metrics** 3. **Issue Diagnosis and
+Remediation** 4. **On-Prem/Private Cloud Deployment with Real-Time Streaming
+Support** 5. **Real-Time Evaluation and Guardrails** To learn more and see how
+raga-llm-platform can benefit your organization, [book a call with our team
+today](https://calendly.com/vijay-srinivas/ragaai-product-offering?month=2024-
+03). Discover the value of enterprise-grade LLM management tailored to your
+needs. ## Learn More For those who wish to dive deeper, we encourage exploring
+[our extensive documentation](https://docs.raga.ai) For more details and the
+latest news from RagaAI, visit [our official website](https://raga.ai).
```

### Comparing `raga_llm_hub-1.0.0.11b2/pyproject.toml` & `raga-llm-hub-1.0.0.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "raga-llm-hub"
-version = "1.0.0.11.beta2"
+version = "1.0.0.9"
 authors = [{ name = "Raga AI", email = "rehan.asif@raga.ai" }]
 description = "Package for LLM Evaluation"
 readme = "README.md"
 keywords = ["ragaai", "raga", "llm", "testing", "llm-eval", "llm-hub"]
 license = { file = "LICENSE" }
 
 classifiers = [
@@ -42,17 +42,16 @@
     "langchain==0.1.9",
     "openai==1.11.1",
     "transformers==4.38.1",
     "Faker==23.2.1",
     "structlog==24.1.0",
     "json-repair==0.9.0",
     "fuzzysearch==0.7.3",
-    "waitress~=3.0.0",
-    "sqlvalidator==0.0.20",
-    "pyngrok==7.1.6"
+    "waitress==3.0.0",
+    "sqlvalidator==0.0.20"
 ]
 
 [project.optional-dependencies]
 ui = ["Flask==3.0.2"]
 onnxruntime = []
 onnxruntime-gpu = []
 docs-dev = [
```

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/__init__.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "RagaLLMObserver",
     "TestExecutor",
     "get_data",
     "raga_observer",
     "launch_app",
 ]
 
-__version__ = "1.0.0.11.beta2"
+__version__ = "1.0.0.9"
 
 
 def check_latest_version(package_name):
     """
     Check the latest version of the package on PyPI and inform the user if an update is available.
     """
     try:
```

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/api_client_manager.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/api_client_manager.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/db_manager.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/db_manager.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/__init__.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/__init__.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/__init__.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/analyzer.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/analyzer.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/faker.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/faker.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/ner_mapping.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/ner_mapping.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/custom_pattern_recognizer.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/custom_pattern_recognizer.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/ip_recognizer.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/predefined_recognizers/zh/ip_recognizer.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/regex_patterns.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/regex_patterns.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/transformers_helpers.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/transformers_helpers.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/anonymize_helpers/transformers_recognizer.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/anonymize_helpers/transformers_recognizer.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/ban_competitors.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/ban_competitors.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/ban_substrings.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/ban_substrings.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/ban_topics.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/ban_topics.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/code.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/code.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/deanonymize.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/deanonymize.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/factual_consistency.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/factual_consistency.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/gibberish.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/gibberish.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/invisible_text.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/invisible_text.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/ir_metrics_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/ir_metrics_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/json_verify.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/json_verify.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/language.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/language.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/language_same.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/language_same.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/malicious_url.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/malicious_url.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/no_refusal.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/no_refusal.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/nsfw.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/nsfw.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/politeness.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/politeness.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/profanity.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/profanity.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/reading_time.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/reading_time.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/regex.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/regex.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/adobe.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/adobe.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/alibaba.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/alibaba.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/asana.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/asana.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/atlassian_api_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/atlassian_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/authress_access_key.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/authress_access_key.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/beamer_api_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/beamer_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/bitbucket.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/bitbucket.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/bittrex.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/bittrex.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/codecov_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/codecov_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/coinbase_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/coinbase_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/confluent.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/confluent.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/contentful_api_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/contentful_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/defined_networking_api_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/defined_networking_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/digitalocean.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/digitalocean.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/discord.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/discord.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/droneci_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/droneci_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/dropbox.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/dropbox.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/etsy_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/etsy_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/facebook_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/facebook_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/finicity.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/finicity.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/finnhub_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/finnhub_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/flickr_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/flickr_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/flutterwave.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/flutterwave.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/freshbooks_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/freshbooks_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/github_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/github_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/gitlab.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/gitlab.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/gitter_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/gitter_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/gocardless_api_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/gocardless_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/grafana.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/grafana.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/heroku_api_key.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/heroku_api_key.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/hubspot_api_key.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/hubspot_api_key.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/huggingface.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/huggingface.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/jfrog.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/jfrog.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/jwt.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/jwt.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/kraken_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/kraken_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/kucoin.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/kucoin.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/launchdarkly_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/launchdarkly_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/linear.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/linear.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/linkedin.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/linkedin.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/lob.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/lob.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/mailgun.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/mailgun.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/mapbox_api_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/mapbox_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/mattermost_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/mattermost_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/messagebird.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/messagebird.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/microsoft_teams_webhook.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/microsoft_teams_webhook.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/netlify_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/netlify_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/new_relic.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/new_relic.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/nytimes_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/nytimes_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/planetscale.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/planetscale.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/sendbird.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/sendbird.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/shopify.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/shopify.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/sidekiq.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/sidekiq.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/slack.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/slack.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/snyk_api_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/snyk_api_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/squarespace_access_token.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/squarespace_access_token.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/sumologic.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/sumologic.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/twitter.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/twitter.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/secrets_plugins/yandex.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/secrets_plugins/yandex.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/resources/sensitive_patterns.json` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/resources/sensitive_patterns.json`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/secrets.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/secrets.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/sensitive.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/sensitive.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/sentiment.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/sentiment.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/token_limit.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/token_limit.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/url_reachability.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/url_reachability.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/utils.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/utils.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/valid_csv.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/valid_csv.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/valid_python.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/valid_python.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/valid_sql.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/valid_sql.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/guardrails/vault.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/guardrails/vault.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/ir_metrics_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/ir_metrics_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/__init__.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/accuracy.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/accuracy.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/ap.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/ap.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/bpm.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/bpm.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/bpref.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/bpref.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/compat.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/compat.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/f1_at_k.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/f1_at_k.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/f1_score.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/f1_score.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/infAP.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/infAP.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/insq.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/insq.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/inst.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/inst.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/iprec.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/iprec.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/judged.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/judged.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/ndcg.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/ndcg.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/nerr10.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/nerr10.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/nerr11.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/nerr11.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/nerr8.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/nerr8.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/nerr9.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/nerr9.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/numq.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/numq.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/numrel.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/numrel.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/numret.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/numret.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/p.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/p.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/precision.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/precision.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/precision_at_k.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/precision_at_k.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/r.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/r.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/rbp.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/rbp.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/recall.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/recall.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/recall_at_k.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/recall_at_k.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/retrieval_metrics.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/retrieval_metrics.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/rprec.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/rprec.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/sdcg.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/sdcg.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/setap.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/setap.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/setf.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/setf.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/setp.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/setp.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/setr.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/setr.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/metrics/retrieval/success.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/metrics/retrieval/success.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/observer/raga_observer.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/observer/raga_observer.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/raga_llm_eval.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/raga_llm_eval.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,18 +109,17 @@
         """
         Run the tests, save run details, and return the current object.
         """
         try:
             self._final_results = self._run(
                 self._tests_to_execute, eval_id=self.eval_name
             )
-        except Exception as e:
+        except Exception as _:
             print("🚫 Error while running the tests. Resetting...")
             self._clear_added_tests()
-            raise e
 
         # Save run details
         self.save_run_details(
             eval_name=self.eval_name, final_results=self._final_results
         )
 
         # Flush the tests to be executed
```

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/raga_llm_observer.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/raga_llm_observer.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/result_manager.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/result_manager.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/test_manager.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/test_manager.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/__init__.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/bias_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/bias_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/chunk_impact_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/chunk_impact_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/coherence_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/coherence_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/complexity_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/complexity_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/conciseness_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/conciseness_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/consistency_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/consistency_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/context_retrieval_metrics_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/context_retrieval_metrics_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/contextual_precision_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/contextual_precision_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/contextual_recall_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/contextual_recall_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/contextual_relevancy_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/contextual_relevancy_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/correctness_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/correctness_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/cosine_similarity_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/cosine_similarity_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/cost_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/cost_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/cover_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/cover_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/dan_detectors.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/dan_detectors.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/dan_probes.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/dan_probes.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/dan_vulnerability_scanner.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/dan_vulnerability_scanner.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/faithfulness_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/faithfulness_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/generic_evaluation_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/generic_evaluation_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/hallucination_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/hallucination_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/harmless_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/harmless_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/ir_metrics_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/ir_metrics_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/latency_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/latency_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/length_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/length_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/lmrc_detectors.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/lmrc_detectors.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/lmrc_probes.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/lmrc_probes.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/lmrc_vulnerability_scanner.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/lmrc_vulnerability_scanner.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/maliciousness_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/maliciousness_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/matcher.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/matcher.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/overall_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/overall_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/pos_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/pos_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/prompt_injection_modeleval.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/prompt_injection_modeleval.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/prompt_injection_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/prompt_injection_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/prompt_template.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/prompt_template.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/readability_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/readability_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,32 +70,30 @@
         )
     else:
         response_readability_average = None
         is_readable = True if (prompt_readability_average <= threshold) else False
 
     reason = ""
 
-    # Adding score
-    score = prompt_readability_average + response_readability_average
-
     # Adding Prompt heading
     reason += "Prompt:\n"
-    reason += f"Score: {prompt_readability_average}\n"
     reason += "\n".join(f"{key}: {value}" for key, value in prompt_submetrics.items())
     reason += "\n"
 
     # Adding Response heading
     reason += "\nResponse:\n"
-    reason += f"Score: {response_readability_average}\n"
     reason += "\n".join(f"{key}: {value}" for key, value in response_submetrics.items())
 
     result = {
         "prompt": prompt,
         "response": response,
-        "score": score,
+        "score": {
+            "prompt_readability_score": prompt_readability_average,
+            "response_readability_score": response_readability_average,
+        },
         "is_passed": is_readable,
         "prompt_submetrics": prompt_submetrics,
         "response_submetrics": response_submetrics,
         "reason": reason,
         "threshold": threshold,
     }
```

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/refusal_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/refusal_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/relevancy_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/relevancy_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/sentiment_analysis_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/sentiment_analysis_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/summarisation_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/summarisation_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/template.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/template.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/anonymize_guardrail.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/anonymize_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/ban_competitors_guardrail.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/ban_competitors_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/ban_substrings_guardrail.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/ban_substrings_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/ban_topics_guardrail.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/ban_topics_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/bias_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/bias_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/chunk_impact_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/chunk_impact_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/code.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/code.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/coherence_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/coherence_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/complexity_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/complexity_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/conciseness_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/conciseness_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/consistency_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/consistency_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/context_retrieval_metrics_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/context_retrieval_metrics_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/contextual_precision_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/contextual_precision_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/contextual_recall_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/contextual_recall_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/contextual_relevancy_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/contextual_relevancy_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/correctness_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/correctness_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/cosine_similarity_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/cosine_similarity_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/cover_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/cover_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/factual_consistency_guardrail.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/factual_consistency_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/faithfulness_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/faithfulness_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/generic_evaluation_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/generic_evaluation_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/grade_score_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/grade_score_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/hallucination_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/hallucination_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/harmful_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/harmful_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/harmless_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/harmless_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/invisible_text_guardrail.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/invisible_text_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/ir_metrics_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/ir_metrics_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/json_verify_guardrail.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/json_verify_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/language_guardrail.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/language_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/language_same_guardrail.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/language_same_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/maliciousness_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/maliciousness_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/no_refusal_guardrail.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/no_refusal_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/overall_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/overall_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/pos_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/pos_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/prompt_injection_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/prompt_injection_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/readability_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/readability_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/reading_time_guardrail.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/reading_time_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/refusal_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/refusal_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/relevancy_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/relevancy_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/response_toxicity_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/response_toxicity_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/sensitive_guardrail.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/sensitive_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/sentiment_analysis_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/sentiment_analysis_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/summarisation_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/summarisation_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/tokenlimit_guardrail.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/tokenlimit_guardrail.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/data_files/winner_test.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/data_files/winner_test.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_data/test_data.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_data/test_data.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_details.toml` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_details.toml`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_executor.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/test_utils.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/toxicity_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/toxicity_test.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import json
-import time
 
 from .prompt_template import ResponseToxicityTemplate
 
 
 class ToxicityTest:
     def __init__(
         self,
@@ -62,44 +61,20 @@
             prompt=self.prompt
         )
         response_toxicity = self.model(toxicity_test)
         toxicity_verdict = json.loads(self.trim_to_json(response_toxicity))
 
         return toxicity_verdict
 
-    def evaluate_with_retry(self, max_retries=3, initial_delay=1.0, backoff_factor=2.0):
-        """
-        Evaluate toxicity with retries.
-
-        :param max_retries: The maximum number of retries (default is 3).
-        :param initial_delay: The initial delay in seconds (default is 1.0).
-        :param backoff_factor: The backoff factor for exponential backoff (default is 2.0).
-        :return: The toxicity verdict.
-        """
-        attempts = 0
-        while attempts < max_retries:
-            try:
-                toxicity_verdict = self.evaluate_toxicity()
-                return toxicity_verdict  # Return on success
-            except Exception as e:
-                attempts += 1
-                if "JSONDecodeError" in str(e) and attempts < max_retries:
-                    time.sleep(
-                        initial_delay * (backoff_factor ** (attempts - 1))
-                    )  # Exponential backoff
-                else:
-                    raise e
-
     def run(self):
         """
         Run the toxicity evaluation process and generate the result including input question, response, toxicity verdict, score, threshold, and evaluation details.
         """
-        toxicity_verdict = self.evaluate_with_retry()
-
-        score = float(toxicity_verdict.get("score", 0.0))
+        toxicity_verdict = self.evaluate_toxicity()
+        score = toxicity_verdict.get("score", 0.0)
         reason = toxicity_verdict.get("reason", "No reason provided.")
 
         result = {
             "prompt": self.prompt,
             "toxicity_verdict": toxicity_verdict,
             "score": score,
             "threshold": self.threshold,
```

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/tests/winner_test.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/tests/winner_test.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/track_manager.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/track_manager.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/helpers.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/helpers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,17 @@
-import sys
-import time
+from signal import SIGTERM  # or SIGKILL
 
-from pyngrok import ngrok
-from pyngrok.ngrok import PyngrokConfig
+from psutil import process_iter
+
+
+def killport(port: int):
+    for proc in process_iter():
+        for conns in proc.connections(kind='inet'):
+            if conns.laddr.port == port:
+                proc.send_signal(SIGTERM)  # or SIGKILL
 
 
 def pick_matching_keys_from_dict(target_dict: dict, keys: list[str] = None):
     if keys is None or len(keys) < 1:
         return target_dict
     result = {}
     for k in list(filter(None, keys)):
@@ -15,64 +20,49 @@
                 result[dk] = target_dict[dk]
     return result
 
 
 def group_by_data_point_id(results: list):
     groups = {}
     for result in results:
-        data_point_id = result.get("dataset_id")
+        data_point_id = result.get('dataset_id')
         if data_point_id not in groups:
             groups[data_point_id] = []
         groups[data_point_id].append(result)
     result = []
     for data_point_id, tests in groups.items():
         row = {}
-        row["data_point_id"] = data_point_id
+        row['data_point_id'] = data_point_id
         for test in tests:
-            row["prompt"] = test.get("prompt", row.get("prompt"))
-            row["response"] = test.get("response", row.get("response"))
-            row["context"] = test.get("context", row.get("context"))
-            row["expected_response"] = test.get(
-                "expected_response", row.get("expected_response")
-            )
-            if "dynamic" not in row:
-                row["dynamic"] = []
+            row['prompt'] = test.get('prompt', row.get('prompt'))
+            row['response'] = test.get('response', row.get('response'))
+            row['context'] = test.get('context', row.get('context'))
+            row['expected_response'] = test.get(
+                'expected_response', row.get('expected_response'))
+            if 'dynamic' not in row:
+                row['dynamic'] = []
 
-            score = test.get("score")
+            score = test.get('score')
             if score is not None:
-                if isinstance(test.get("score"), dict):
-                    score = ", ".join(
-                        map(lambda x: "%.3f" % (x), test.get("score").values())
-                    )
+                if isinstance(test.get('score'), dict):
+                    score = ', '.join(map(lambda x: '%.3f'%(x), test.get('score').values()))
                 else:
-                    score = float("%.3f" % (test.get("score")))
-            row["dynamic"].append(
-                {
-                    "test_name": test.get("test_name"),
-                    "test_run_id": test.get("test_run_id"),
-                    "is_passed": test.get("is_passed"),
-                    "threshold": test.get("threshold"),
-                    "score": score,
-                    "evaluated_with": test.get("evaluated_with"),
-                }
-            )
+                    score = float('%.3f'%(test.get('score')))
+            row['dynamic'].append({
+                'test_name': test.get('test_name'),
+                'test_run_id': test.get('test_run_id'),
+                'is_passed': test.get('is_passed'),
+                'threshold': test.get('threshold'),
+                'score': score,
+                'evaluated_with': test.get('evaluated_with'),
+            })
         result.append(row)
     return result
 
 
 def get_test_for_test_run_id(jsonData, testRunId):
     for d in jsonData:
-        if d.get("test_run_id") == testRunId:
+        if d.get('test_run_id') == testRunId:
             return d
 
-
 def get_test_name_for_test_run_id(jsonData, testRunId):
-    return get_test_for_test_run_id(jsonData, testRunId).get("test_name")
-
-
-def kill_ngrok(pyngrok_config: PyngrokConfig):
-    # kill tunnel
-    time.sleep(2)
-    ngrok.kill(pyngrok_config)
-
-
-IN_COLAB = "google.colab" in sys.modules
+    return get_test_for_test_run_id(jsonData, testRunId).get('test_name')
```

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/pages/index.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/pages/index.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,37 @@
 import json
 import math
-from threading import Thread
 
 from flask import Blueprint, abort, render_template, request
 from jinja2 import TemplateNotFound
-from pyngrok import ngrok
-from pyngrok.ngrok import PyngrokConfig
 
 from ..helpers import (
     get_test_for_test_run_id,
     get_test_name_for_test_run_id,
     group_by_data_point_id,
-    kill_ngrok,
-    IN_COLAB,
+    pick_matching_keys_from_dict,
 )
 
 
-def index_page_creator(
-    fileName: str, session_id: str, pyngrok_config: PyngrokConfig
-) -> Blueprint:
+def index_page_creator(context: dict):
     index_page = Blueprint("index_page", __name__, template_folder="templates")
 
     @index_page.route("/")
     def page():
-        if IN_COLAB:
-            if request.args.get("id") != session_id:
-                abort(404)
-
-        f = open(fileName)
-        results = json.load(f)
+        results = context.get("results")
 
         # region pagination related code
         page = request.args.get("page", 0, int)
         size = request.args.get("size", len(results), int)
         offset = page * size
         total_pages = 0 if len(results) == 0 else math.ceil(len(results) / size)
         target_results = results[offset : offset + size]
         # endregion
 
         groups = group_by_test_run_id(target_results)
-        if IN_COLAB:
-            # kill tunnel
-            thread = Thread(target=kill_ngrok, args=[pyngrok_config])
-            thread.start()
-
         try:
             return render_template(
                 "index.html",
                 target_results=json.dumps(group_by_data_point_id(target_results)),
                 total_elements=len(target_results),
                 total_pages=total_pages,
                 current_page=page,
```

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/pages/trace.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/pages/trace.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-import json
 from flask import Blueprint, abort, render_template, request
 from jinja2 import TemplateNotFound
 from datetime import datetime
 
 from ..helpers import group_by_data_point_id
 
 
-def trace_page_creator(fileName: str):
+def trace_page_creator(context: dict):
     trace_page = Blueprint("trace_page", __name__, template_folder="templates")
 
     @trace_page.route("/trace/<data_point_id>")
     def page(data_point_id):
-        f = open(fileName)
-        results = json.load(f)
+        results = context.get("results")
         result = list(
             filter(
                 lambda x: x.get("data_point_id") == data_point_id,
                 group_by_data_point_id(results),
             )
         )[0]
         if result is None:
```

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/static/favicon.png` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/static/favicon.png`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/static/logoG.png` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/static/logoG.png`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/static/main.js` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/static/main.js`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/static/style.css` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/static/style.css`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/base.html` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/base.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,10 @@
 <!DOCTYPE html>
 <html lang="en">
   <head>
-    <!-- Google tag (gtag.js) -->
-    <script
-      async
-      src="https://www.googletagmanager.com/gtag/js?id=G-RGPZE5DH8S"
-    ></script>
-    <script>
-      window.dataLayer = window.dataLayer || [];
-      function gtag() {
-        dataLayer.push(arguments);
-      }
-      gtag("js", new Date());
-      gtag("config", "G-RGPZE5DH8S");
-    </script>
     <meta charset="UTF-8" />
     <meta
       http-equiv="Cache-Control"
       content="no-cache, no-store, must-revalidate"
     />
     <meta http-equiv="Pragma" content="no-cache" />
     <meta http-equiv="Expires" content="0" />
@@ -43,19 +30,15 @@
     />
     <link rel="stylesheet" href="/style.css" />
     <title>Raga Ai</title>
   </head>
 
   <body>
     {% block content %} {% endblock %}
-    <script
-      src="https://code.jquery.com/jquery-3.7.1.min.js"
-      integrity="sha256-/JqT3SQfawRcv/BIHPThkBvs0OEvtFFmqPF/lYI/Cxo="
-      crossorigin="anonymous"
-    ></script>
+    <script src="https://code.jquery.com/jquery-3.7.1.min.js" integrity="sha256-/JqT3SQfawRcv/BIHPThkBvs0OEvtFFmqPF/lYI/Cxo=" crossorigin="anonymous"></script>
     <script
       src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.2/dist/js/bootstrap.bundle.min.js"
       integrity="sha384-C6RzsynM9kWDrMNeT87bh95OGNyZPhcTNXj1NW7RuBCsyN/o0jlpcV8Qyq46cDfL"
       crossorigin="anonymous"
     ></script>
     <script src="https://code.jquery.com/jquery-3.6.0.min.js"></script>
     <script src="/main.js"></script>
```

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/components/card.html` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/components/card.html`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/components/checkbox.html` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/components/checkbox.html`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/components/data-level-view-row.html` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/components/data-level-view-row.html`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/components/pagination.html` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/components/pagination.html`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/components/tooltip.html` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/components/tooltip.html`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/index.html` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/index.html`

 * *Files 20% similar despite different names*

```diff
@@ -56,34 +56,22 @@
           <div class="raga-card-header-first">
             <h4 class="mb-0">Data Level View</h4>
           </div>
         </div>
         <div id="table-scroll" class="table-scroll">
           <div class="table-wrap">
             <table class="p-table">
-              <thead></thead>
-              <tbody></tbody>
+              <thead>
+              </thead>
+              <tbody>
+              </tbody>
             </table>
           </div>
         </div>
       </div>
     </div>
   </div>
 </div>
 <script>
   window.jsonData=JSON.parse({{target_results|tojson}})
 </script>
-<script>
-  window.gtag("event", "page_launch");
-
-  const uniqueTestNames = new Set(
-    window.jsonData.flatMap((e) => e.dynamic.map((t) => t.test_name))
-  );
-  const testNames = Array.from(uniqueTestNames);
-
-  testNames.forEach((testName) => {
-    window.gtag("event", "test_loaded", {
-      test_name: testName,
-    });
-  });
-</script>
 {% endblock %}
```

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/ui/templates/trace.html` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/ui/templates/trace.html`

 * *Files 2% similar despite different names*

```diff
@@ -169,12 +169,8 @@
             </div>
           </div> -->
         </div>
       </div>
     </div>
   </div>
 </div>
-<script>
-  window.gtag('event', 'trace_view_loaded')
-</script>
-
 {% endblock %}
```

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/utils/data_files/inthewild_jailbreak_llms.txt` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/utils/data_files/inthewild_jailbreak_llms.txt`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/utils/data_files/ldnoobw-en.txt` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/utils/data_files/ldnoobw-en.txt`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/utils/data_files/ofcom-potentially-offensive.txt` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/utils/data_files/ofcom-potentially-offensive.txt`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/utils/data_files/profanity_en.csv` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/utils/data_files/profanity_en.csv`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub/utils/utils.py` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub/utils/utils.py`

 * *Files identical despite different names*

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub.egg-info/PKG-INFO` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-llm-hub
-Version: 1.0.0.11b2
+Version: 1.0.0.9
 Summary: Package for LLM Evaluation
 Author-email: Raga AI <rehan.asif@raga.ai>
 License: Attribution-NonCommercial-NoDerivatives 4.0 International
         
         =======================================================================
         
         Creative Commons Corporation ("Creative Commons") is not a law firm and
@@ -443,17 +443,16 @@
 Requires-Dist: langchain==0.1.9
 Requires-Dist: openai==1.11.1
 Requires-Dist: transformers==4.38.1
 Requires-Dist: Faker==23.2.1
 Requires-Dist: structlog==24.1.0
 Requires-Dist: json-repair==0.9.0
 Requires-Dist: fuzzysearch==0.7.3
-Requires-Dist: waitress~=3.0.0
+Requires-Dist: waitress==3.0.0
 Requires-Dist: sqlvalidator==0.0.20
-Requires-Dist: pyngrok==7.1.6
 Provides-Extra: ui
 Requires-Dist: Flask==3.0.2; extra == "ui"
 Provides-Extra: onnxruntime
 Provides-Extra: onnxruntime-gpu
 Provides-Extra: docs-dev
 Requires-Dist: mkdocs==1.5.3; extra == "docs-dev"
 Requires-Dist: mkdocs-autorefs==0.5.0; extra == "docs-dev"
@@ -491,57 +490,72 @@
 
 [![PyPI - Version](https://img.shields.io/pypi/v/raga-llm-hub?label=PyPI%20Package)](https://badge.fury.io/py/raga-llm-hub) [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1PQGqDGdcSUxhSvpSQYX8ZdHf5r90WSYf?usp=sharing)
 </a> [![Python Compatibility](https://img.shields.io/pypi/pyversions/raga-llm-hub)](https://pypi.org/project/raga-llm-hub/) []()
 
 </div>
 
 
-Welcome to Raga LLM Hub, a comprehensive evaluation toolkit for Language and Learning Models (LLMs). With over 100 meticulously designed metrics, it is the most comprehensive platform that allows developers and organizations to evaluate and compare LLMs effectively and establish essential guardrails for LLMs and Retrieval Augmented Generation(RAG)  applications. These tests assess various aspects including Relevance & Understanding, Content Quality, Hallucination, Safety & Bias, Context Relevance, Guardrails, and Vulnerability scanning, along with a suite of Metric-Based Tests for quantitative analysis.
+Welcome to Raga LLM Eval, a comprehensive evaluation toolkit for Language and Learning Models (LLMs). With over 100 meticulously designed metrics, it is the most comprehensive platform that allows developers and organizations to evaluate and compare LLMs effectively and establish essential guardrails for LLMs and Retrieval Augmented Generation(RAG)  applications. These tests assess various aspects including Relevance & Understanding, Content Quality, Hallucination, Safety & Bias, Context Relevance, Guardrails, and Vulnerability scanning, along with a suite of Metric-Based Tests for quantitative analysis.
 
 The RagaAI LLM Hub is uniquely designed to help teams identify issues and fix them throughout the LLM lifecycle, by identifying issues across the entire RAG pipeline. This is pivotal for understanding the root cause of failures within an LLM application and addressing them at their source, revolutionizing the approach to ensuring reliability and trustworthiness.
 
 ## Installation
 
 ### Via pip
 
 ```bash
 # Create and activate a new Python environment
 python -m venv venv
 source venv/bin/activate
-
 # Install Raga LLM Hub
 pip install raga-llm-hub
 ```
 
 
 ### Via conda
 ```py
 # Create and activate a new Conda environment
 conda create --name myenv python=3.11
 conda activate myenv
-
 # Install Raga LLM Hub
 python -m pip install raga-llm-hub
 
 ```
 
 ## Quick Tour
 ### Initialization
 
 ```py
-from raga_llm_hub import RagaLLMEval
+from raga_llm_hub import RagaLLMEval, get_data
 
 # Initialize the evaluator with your API key
 evaluator = RagaLLMEval(api_key="your_api_key")
 ```
 
-### Run Tests
+
+
+4. Re-using Previous Results
+Leverage previous results for comparative analysis or to track your LLM's performance over time.
 
 ```py
+PREV_EVAL_ID = "PREVIOUS_RUN_ID"
+
+evaluator.load_eval(
+    eval_name=PREV_EVAL_ID
+)
+
+evaluator.print_results()
+evaluator.save_results("filename.json")
+```
 
+### Discover and Run Tests
+
+```py
+# List all available tests
+evaluator.list_available_tests()
 
 # Add and run a custom test
 evaluator.add_test(
     test_name="relevancy_test",
     data={
         "prompt": "How are you?",
         "context": "Responding as a student to a teacher.",
@@ -575,24 +589,14 @@
 previous_eval_id = "your_previous_eval_id_here"
 evaluator.load_eval(previous_eval_id)
 
 # After loading, you can print, save, or further analyze these results
 evaluator.print_results()
 ```
 
-## Examples
-- **Evaluation Tests**: Evaluation Tests assesse a Large Language Model's (LLM's) performance in generating responses that are accurate, relevant, and linguistically coherent to a wide array of prompts. This evaluation is pivotal in determining the model's ability to understand and respond appropriately to diverse user inputs, ranging from simple queries to complex, context-rich requests. 
-
-    [![Evaluation Tests](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1cY5eN5w7bK1CH8L8MYEAfrfzaVZ7LNS5?usp=sharing)
-
-- **Guardrail Tests**: Guardrails ensure that the models operate within predefined ethical, legal, and safety boundaries. These mechanisms are implemented to prevent the generation of biased, offensive, or harmful content, making sure that the outputs align with societal norms and values. 
-
-     [![Guardrails](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1TAX2PeicBBWHtdiZZelpXN5YcOB7WnEk?usp=sharing)
-
-
 ## Enterprise
 Enterprise Version
 Introducing raga-llm-platform,(enterprise version of raga-llm-hub)  for Large Language Model (LLM) evaluation and guardrails, designed to empower organizations to harness the full potential of LLMs securely and efficiently. Here’s what sets raga-llm-platform apart:
 1. **Production Scale Analysis**
 2. **State-of-the-Art Evaluation Methods and Metrics**
 3. **Issue Diagnosis and Remediation**
 4. **On-Prem/Private Cloud Deployment with Real-Time Streaming Support**
```

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub.egg-info/SOURCES.txt` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -303,14 +303,15 @@
 src/raga_llm_hub/tests/test_data/data_files/summarisation_test.toml
 src/raga_llm_hub/tests/test_data/data_files/tokenlimit_guardrail.toml
 src/raga_llm_hub/tests/test_data/data_files/toxicity_test.toml
 src/raga_llm_hub/tests/test_data/data_files/url_reachability_guardrail.toml
 src/raga_llm_hub/tests/test_data/data_files/winner_test.toml
 src/raga_llm_hub/ui/app.py
 src/raga_llm_hub/ui/helpers.py
+src/raga_llm_hub/ui/pages/__init__.py
 src/raga_llm_hub/ui/pages/index.py
 src/raga_llm_hub/ui/pages/trace.py
 src/raga_llm_hub/ui/static/favicon.png
 src/raga_llm_hub/ui/static/logoG.png
 src/raga_llm_hub/ui/static/main.js
 src/raga_llm_hub/ui/static/style.css
 src/raga_llm_hub/ui/templates/base.html
```

### Comparing `raga_llm_hub-1.0.0.11b2/src/raga_llm_hub.egg-info/requires.txt` & `raga-llm-hub-1.0.0.9/src/raga_llm_hub.egg-info/requires.txt`

 * *Files 16% similar despite different names*

```diff
@@ -19,17 +19,16 @@
 langchain==0.1.9
 openai==1.11.1
 transformers==4.38.1
 Faker==23.2.1
 structlog==24.1.0
 json-repair==0.9.0
 fuzzysearch==0.7.3
-waitress~=3.0.0
+waitress==3.0.0
 sqlvalidator==0.0.20
-pyngrok==7.1.6
 
 [dev]
 black
 flake8
 isort
 mypy
 pytest
```

