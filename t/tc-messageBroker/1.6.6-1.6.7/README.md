# Comparing `tmp/tc-messageBroker-1.6.6.tar.gz` & `tmp/tc_messagebroker-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tc-messageBroker-1.6.6.tar", last modified: Thu Jan 18 12:32:43 2024, max compression
+gzip compressed data, was "tc_messagebroker-1.6.7.tar", last modified: Tue May 21 14:16:20 2024, max compression
```

## Comparing `tc-messageBroker-1.6.6.tar` & `tc_messagebroker-1.6.7.tar`

### file list

```diff
@@ -1,91 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.351442 tc-messageBroker-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-01-18 12:32:43.351442 tc-messageBroker-1.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 12:32:43.351442 tc-messageBroker-1.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.335442 tc-messageBroker-1.6.6/tc_messageBroker/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14544 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/message_broker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.335442 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.335442 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/db_operations/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/db_operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.339442 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/event/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/event/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/event/events_microservice.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.339442 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.339442 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.343442 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/allowed_mentions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/embed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/interaction_callback_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/chat_input_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/create_followup_message_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/edit_webhook_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/interaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/type.py
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/payload_microservices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.343442 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/queue/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/queue/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/queue/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.343442 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/choreography.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/choreography_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/saga.py
--rw-r--r--   0 runner    (1001) docker     (127)     9441 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/saga_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/transaction_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.343442 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.347442 tc-messageBroker-1.6.6/tc_messageBroker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-01-18 12:32:43.000000 tc-messageBroker-1.6.6/tc_messageBroker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-01-18 12:32:43.000000 tc-messageBroker-1.6.6/tc_messageBroker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 12:32:43.000000 tc-messageBroker-1.6.6/tc_messageBroker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-01-18 12:32:43.000000 tc-messageBroker-1.6.6/tc_messageBroker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-01-18 12:32:43.000000 tc-messageBroker-1.6.6/tc_messageBroker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.343442 tc-messageBroker-1.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.343442 tc-messageBroker-1.6.6/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/integration/test_message_broker_exchange_points.py
--rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/integration/test_message_broker_singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     7308 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/integration/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/integration/test_saga.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:43.347442 tc-messageBroker-1.6.6/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_choreagraphy_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_enum_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_interaction_callback_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_interaction_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_message_broker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_mongodb.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_payload.py
--rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_payload_discord_chat_input_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_payload_discord_followup_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_payload_discord_guild.py
--rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_payload_discord_member.py
--rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_payload_discord_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_predefined_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_queue_declare_params.py
--rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_saga_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_saga_base_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_saga_next.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_saga_start.py
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-01-18 12:32:36.000000 tc-messageBroker-1.6.6/tests/unit/test_transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.078529 tc_messagebroker-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-21 14:16:20.078529 tc_messagebroker-1.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 14:16:20.078529 tc_messagebroker-1.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.066529 tc_messagebroker-1.6.7/tc_messageBroker/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14544 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/message_broker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.066529 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.066529 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/db_operations/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/db_operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6930 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/db_operations/mongodb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.066529 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/event/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/event/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/event/events_microservice.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.066529 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.070529 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.070529 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/allowed_mentions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12335 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2354 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/interaction_callback_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2587 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3713 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/chat_input_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/create_followup_message_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3140 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/edit_webhook_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/interaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4340 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/payload_microservices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.070529 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/queue/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/queue/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/queue/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.074530 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/choreography.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/choreography_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/saga.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10317 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/transaction_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.074530 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.074530 tc_messagebroker-1.6.7/tc_messageBroker/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tc_messageBroker/utils/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.078529 tc_messagebroker-1.6.7/tc_messageBroker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-21 14:16:20.000000 tc_messagebroker-1.6.7/tc_messageBroker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-21 14:16:20.000000 tc_messagebroker-1.6.7/tc_messageBroker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:16:20.000000 tc_messagebroker-1.6.7/tc_messageBroker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-21 14:16:20.000000 tc_messagebroker-1.6.7/tc_messageBroker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 14:16:20.000000 tc_messagebroker-1.6.7/tc_messageBroker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.074530 tc_messagebroker-1.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.074530 tc_messagebroker-1.6.7/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/integration/test_message_broker_exchange_points.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2815 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/integration/test_message_broker_singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7420 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/integration/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/integration/test_saga.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:20.078529 tc_messagebroker-1.6.7/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_choreagraphy_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_enum_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5199 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_interaction_callback_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_interaction_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_message_broker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_mongodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_payload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7349 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_payload_discord_chat_input_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4094 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_payload_discord_followup_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3554 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_payload_discord_guild.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2976 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_payload_discord_member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3107 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_payload_discord_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_predefined_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_queue_declare_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5335 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_saga_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_saga_base_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_saga_next.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_saga_start.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-05-21 14:16:13.000000 tc_messagebroker-1.6.7/tests/unit/test_transactions.py
```

### Comparing `tc-messageBroker-1.6.6/PKG-INFO` & `tc_messagebroker-1.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.6.6
+Version: 1.6.7
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.24.1
 Requires-Dist: pymongo>=4.3.3
```

### Comparing `tc-messageBroker-1.6.6/README.md` & `tc_messagebroker-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/setup.py` & `tc_messagebroker-1.6.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("requirements.txt") as f:
     requirements = f.read().splitlines()
 
 
 setup(
     name="tc-messageBroker",
-    version="1.6.6",
+    version="1.6.7",
     author="Mohammad Amin Dadgar, RnDAO",
     maintainer="Mohammad Amin Dadgar",
     maintainer_email="dadgaramin96@gmail.com",
     packages=find_packages(),
     description="Shared library for message broker in Python",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/message_broker.py` & `tc_messagebroker-1.6.7/tc_messageBroker/message_broker.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/db_operations/mongodb.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/db_operations/mongodb.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/event/events_microservice.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/event/events_microservice.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/allowed_mentions.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/allowed_mentions.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/attachment.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/attachment.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/embed.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/embed.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/flags.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/flags.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/guild.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/guild.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/interaction_callback_data.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/interaction_callback_data.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/member.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/member.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/user.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/base_types/user.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/chat_input_interaction.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/chat_input_interaction.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/create_followup_message_data.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/create_followup_message_data.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/edit_webhook_data.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/edit_webhook_data.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/discord_bot/interaction_response.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/discord_bot/interaction_response.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/payload/payload_microservices.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/payload/payload_microservices.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/choreography.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/choreography.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/saga.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/saga.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/saga_base.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/saga_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import uuid
 from datetime import datetime
 from typing import Any, Callable, Optional
 
 import numpy as np
 from tc_messageBroker.rabbit_mq.db_operations import MongoDB
 from tc_messageBroker.rabbit_mq.status import Status
+from tc_messageBroker.utils.credentials import load_mongo_credentials
 
 from .choreography_base import IChoreography
 from .transaction_base import ITransaction
 from .utils.saga_base_utils import convert_tx_dict, get_transactions
 
 
 class Saga:
@@ -52,34 +53,51 @@
             content={"uuid": self.uuid},
         )
 
     def next(
         self,
         publish_method: Callable,
         call_function: Callable,
-        mongo_creds: dict[str, Any],
-        test_mode=False,
+        mongo_creds: dict[str, Any] | None = None,
+        **kwargs,
     ):
         """
         calling the next transaction within the saga
         and updating the saga state in db
 
         Parameters:
         ------------
         publish_method : RabbitMQ.publish | RabbitMQ.publish_on_exchange
             the publish methods that are from the RabbitMQ
         call_function : Callable
             a function to be called when the message recieved
-        mongo_creds : dict[str, Any]
-            the mongodb credentials to update the db
-            the keys must be `connection_str`, `db_name`, and `collection_name`
-        test_mode : bool
-            testing the function indicates that we wouldn't read or write on DB
-            default is False
+        **kwargs :
+            test_mode : bool
+                testing the function indicates that we wouldn't read or write on DB
+                default is False
+            mongo_creds : dict[str, Any] | None
+                the mongodb credentials to update the db
+                if not `None`, the keys must be `connection_str`, `db_name`, and `collection_name`
+            saga_db_name : str
+                the saga database that data is going to be saved within it
+                default would be `Saga`
+            saga_collection_name : str
+                the saga collection that data is going to be saved within it
+                default would be `sagas`
         """
+        test_mode = kwargs.get("test_mode", False)
+        mongo_creds = kwargs.get("mongo_creds", None)
+        saga_db_name = kwargs.get("saga_db_name", "Saga")
+        saga_collection_name = kwargs.get("saga_db_name", "sagas")
+
+        if mongo_creds is None:
+            mongo_creds = load_mongo_credentials()
+            mongo_creds["db_name"] = saga_db_name
+            mongo_creds["collection_name"] = saga_collection_name
+
         tx_sorted, tx_not_started_count = self._sort_transactions(
             self.choreography.transactions
         )
 
         self.status = Status.IN_PROGRESS
 
         # get the first order transaction
```

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/transaction_base.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/transaction_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/transactions.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/transactions.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py` & `tc_messagebroker-1.6.7/tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker.egg-info/PKG-INFO` & `tc_messagebroker-1.6.7/tc_messageBroker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tc-messageBroker
-Version: 1.6.6
+Version: 1.6.7
 Summary: Shared library for message broker in Python
 Author: Mohammad Amin Dadgar, RnDAO
 Maintainer: Mohammad Amin Dadgar
 Maintainer-email: dadgaramin96@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: numpy>=1.24.1
 Requires-Dist: pymongo>=4.3.3
```

### Comparing `tc-messageBroker-1.6.6/tc_messageBroker.egg-info/SOURCES.txt` & `tc_messagebroker-1.6.7/tc_messageBroker.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -40,22 +40,25 @@
 tc_messageBroker/rabbit_mq/saga/saga.py
 tc_messageBroker/rabbit_mq/saga/saga_base.py
 tc_messageBroker/rabbit_mq/saga/transaction_base.py
 tc_messageBroker/rabbit_mq/saga/transactions.py
 tc_messageBroker/rabbit_mq/saga/utils/__init__.py
 tc_messageBroker/rabbit_mq/saga/utils/choreography_schema.py
 tc_messageBroker/rabbit_mq/saga/utils/saga_base_utils.py
+tc_messageBroker/utils/__init__.py
+tc_messageBroker/utils/credentials.py
 tests/__init__.py
 tests/integration/__init__.py
 tests/integration/test_message_broker_exchange_points.py
 tests/integration/test_message_broker_singleton.py
 tests/integration/test_mongodb.py
 tests/integration/test_saga.py
 tests/unit/__init__.py
 tests/unit/test_choreagraphy_base.py
+tests/unit/test_credentials.py
 tests/unit/test_enum_status.py
 tests/unit/test_event.py
 tests/unit/test_interaction_callback_data.py
 tests/unit/test_interaction_response.py
 tests/unit/test_message_broker.py
 tests/unit/test_mongodb.py
 tests/unit/test_payload.py
```

### Comparing `tc-messageBroker-1.6.6/tests/integration/test_message_broker_exchange_points.py` & `tc_messagebroker-1.6.7/tests/integration/test_message_broker_exchange_points.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/integration/test_message_broker_singleton.py` & `tc_messagebroker-1.6.7/tests/integration/test_message_broker_singleton.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/integration/test_mongodb.py` & `tc_messagebroker-1.6.7/tests/integration/test_mongodb.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 from dotenv import load_dotenv
 from numpy.random import randint
 from tc_messageBroker.rabbit_mq.db_operations import MongoDB
 
 
 def test_insert_one():
     load_dotenv()
-    host = os.getenv("DB_HOST")
-    port = os.getenv("DB_PORT")
-    user = os.getenv("DB_USER")
-    password = os.getenv("DB_PASSWORD")
+    host = os.getenv("MONGODB_HOST")
+    port = os.getenv("MONGODB_PORT")
+    user = os.getenv("MONGODB_USER")
+    password = os.getenv("MONGODB_PASS")
 
     connection_url = f"mongodb://{user}:{password}@{host}:{port}"
 
     db_name = os.getenv("DB_SAGA_NAME")
     collection_name = os.getenv("DB_SAGA_COLLECTION_NAME")
     mongodb = MongoDB(
         connection_str=connection_url, db_name=db_name, collection_name=collection_name
@@ -26,18 +26,18 @@
     data = create_random_data()
 
     mongodb.write(data=[data])
 
 
 def test_insert_multiple():
     load_dotenv()
-    host = os.getenv("DB_HOST")
-    port = os.getenv("DB_PORT")
-    user = os.getenv("DB_USER")
-    password = os.getenv("DB_PASSWORD")
+    host = os.getenv("MONGODB_HOST")
+    port = os.getenv("MONGODB_PORT")
+    user = os.getenv("MONGODB_USER")
+    password = os.getenv("MONGODB_PASS")
 
     connection_url = f"mongodb://{user}:{password}@{host}:{port}"
     db_name = os.getenv("DB_SAGA_NAME")
     collection_name = os.getenv("DB_SAGA_COLLECTION_NAME")
     mongodb = MongoDB(
         connection_str=connection_url, db_name=db_name, collection_name=collection_name
     )
@@ -52,18 +52,18 @@
 
 
 def test_read_count_one():
     """
     read from db after writing using the previous function (above)
     """
     load_dotenv()
-    host = os.getenv("DB_HOST")
-    port = os.getenv("DB_PORT")
-    user = os.getenv("DB_USER")
-    password = os.getenv("DB_PASSWORD")
+    host = os.getenv("MONGODB_HOST")
+    port = os.getenv("MONGODB_PORT")
+    user = os.getenv("MONGODB_USER")
+    password = os.getenv("MONGODB_PASS")
 
     connection_url = f"mongodb://{user}:{password}@{host}:{port}"
     db_name = os.getenv("DB_SAGA_NAME")
     collection_name = os.getenv("DB_SAGA_COLLECTION_NAME")
     mongodb = MongoDB(
         connection_str=connection_url, db_name=db_name, collection_name=collection_name
     )
@@ -89,18 +89,18 @@
 
 
 def test_read_count_multiple():
     """
     read from db after writing using the previous function (above)
     """
     load_dotenv()
-    host = os.getenv("DB_HOST")
-    port = os.getenv("DB_PORT")
-    user = os.getenv("DB_USER")
-    password = os.getenv("DB_PASSWORD")
+    host = os.getenv("MONGODB_HOST")
+    port = os.getenv("MONGODB_PORT")
+    user = os.getenv("MONGODB_USER")
+    password = os.getenv("MONGODB_PASS")
 
     connection_url = f"mongodb://{user}:{password}@{host}:{port}"
     db_name = os.getenv("DB_SAGA_NAME")
     collection_name = os.getenv("DB_SAGA_COLLECTION_NAME")
     mongodb = MongoDB(
         connection_str=connection_url, db_name=db_name, collection_name=collection_name
     )
@@ -131,18 +131,18 @@
 
 
 def test_replace():
     """
     test replacing a document we just inserted
     """
     load_dotenv()
-    host = os.getenv("DB_HOST")
-    port = os.getenv("DB_PORT")
-    user = os.getenv("DB_USER")
-    password = os.getenv("DB_PASSWORD")
+    host = os.getenv("MONGODB_HOST")
+    port = os.getenv("MONGODB_PORT")
+    user = os.getenv("MONGODB_USER")
+    password = os.getenv("MONGODB_PASS")
 
     connection_url = f"mongodb://{user}:{password}@{host}:{port}"
     db_name = os.getenv("DB_SAGA_NAME")
     collection_name = os.getenv("DB_SAGA_COLLECTION_NAME")
     mongodb = MongoDB(
         connection_str=connection_url, db_name=db_name, collection_name=collection_name
     )
@@ -174,18 +174,18 @@
 
 
 def test_delete():
     """
     delete all except one of the ligitimate data which we choose
     """
     load_dotenv()
-    host = os.getenv("DB_HOST")
-    port = os.getenv("DB_PORT")
-    user = os.getenv("DB_USER")
-    password = os.getenv("DB_PASSWORD")
+    host = os.getenv("MONGODB_HOST")
+    port = os.getenv("MONGODB_PORT")
+    user = os.getenv("MONGODB_USER")
+    password = os.getenv("MONGODB_PASS")
 
     connection_url = f"mongodb://{user}:{password}@{host}:{port}"
     db_name = os.getenv("DB_SAGA_NAME")
     collection_name = os.getenv("DB_SAGA_COLLECTION_NAME")
     mongodb = MongoDB(
         connection_str=connection_url, db_name=db_name, collection_name=collection_name
     )
@@ -197,18 +197,18 @@
 
 
 def test_wrong_input():
     """
     give wrong input to insert
     """
     load_dotenv()
-    host = os.getenv("DB_HOST")
-    port = os.getenv("DB_PORT")
-    user = os.getenv("DB_USER")
-    password = os.getenv("DB_PASSWORD")
+    host = os.getenv("MONGODB_HOST")
+    port = os.getenv("MONGODB_PORT")
+    user = os.getenv("MONGODB_USER")
+    password = os.getenv("MONGODB_PASS")
 
     connection_url = f"mongodb://{user}:{password}@{host}:{port}"
     db_name = os.getenv("DB_SAGA_NAME")
     collection_name = os.getenv("DB_SAGA_COLLECTION_NAME")
     mongodb = MongoDB(
         connection_str=connection_url, db_name=db_name, collection_name=collection_name
     )
```

### Comparing `tc-messageBroker-1.6.6/tests/integration/test_saga.py` & `tc_messagebroker-1.6.7/tests/integration/test_saga.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,18 +14,18 @@
     DISCORD_UPDATE_CHANNELS_TRANSACTIONS,
 )
 from tc_messageBroker.rabbit_mq.status import Status
 
 
 def test_inputs():
     load_dotenv()
-    host = os.getenv("DB_HOST")
-    port = os.getenv("DB_PORT")
-    user = os.getenv("DB_USER")
-    password = os.getenv("DB_PASSWORD")
+    host = os.getenv("MONGODB_HOST")
+    port = os.getenv("MONGODB_PORT")
+    user = os.getenv("MONGODB_USER")
+    password = os.getenv("MONGODB_PASS")
     saga_db = os.getenv("DB_SAGA_NAME")
     saga_collection = os.getenv("DB_SAGA_COLLECTION_NAME")
 
     connection_url = f"mongodb://{user}:{password}@{host}:{port}"
     mongodb = MongoDB(
         connection_str=connection_url, db_name=saga_db, collection_name=saga_collection
     )
@@ -44,18 +44,18 @@
 
 
 def test_saga_update():
     """
     test updating a saga instance in db
     """
     load_dotenv()
-    host = os.getenv("DB_HOST")
-    port = os.getenv("DB_PORT")
-    user = os.getenv("DB_USER")
-    password = os.getenv("DB_PASSWORD")
+    host = os.getenv("MONGODB_HOST")
+    port = os.getenv("MONGODB_PORT")
+    user = os.getenv("MONGODB_USER")
+    password = os.getenv("MONGODB_PASS")
 
     connection_creds = {}
     connection_creds["connection_str"] = f"mongodb://{user}:{password}@{host}:{port}"
     connection_creds["db_name"] = os.getenv("DB_SAGA_NAME")
     connection_creds["collection_name"] = os.getenv("DB_SAGA_COLLECTION_NAME")
 
     choreography = IChoreography(
```

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_choreagraphy_base.py` & `tc_messagebroker-1.6.7/tests/unit/test_choreagraphy_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_event.py` & `tc_messagebroker-1.6.7/tests/unit/test_event.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_interaction_callback_data.py` & `tc_messagebroker-1.6.7/tests/unit/test_interaction_callback_data.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_interaction_response.py` & `tc_messagebroker-1.6.7/tests/unit/test_interaction_response.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_message_broker.py` & `tc_messagebroker-1.6.7/tests/unit/test_message_broker.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_payload.py` & `tc_messagebroker-1.6.7/tests/unit/test_payload.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_payload_discord_chat_input_interaction.py` & `tc_messagebroker-1.6.7/tests/unit/test_payload_discord_chat_input_interaction.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_payload_discord_followup_data.py` & `tc_messagebroker-1.6.7/tests/unit/test_payload_discord_followup_data.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_payload_discord_guild.py` & `tc_messagebroker-1.6.7/tests/unit/test_payload_discord_guild.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_payload_discord_member.py` & `tc_messagebroker-1.6.7/tests/unit/test_payload_discord_member.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_payload_discord_user.py` & `tc_messagebroker-1.6.7/tests/unit/test_payload_discord_user.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_predefined_transactions.py` & `tc_messagebroker-1.6.7/tests/unit/test_predefined_transactions.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_queue_declare_params.py` & `tc_messagebroker-1.6.7/tests/unit/test_queue_declare_params.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_saga_base.py` & `tc_messagebroker-1.6.7/tests/unit/test_saga_base.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_saga_base_utils.py` & `tc_messagebroker-1.6.7/tests/unit/test_saga_base_utils.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_saga_next.py` & `tc_messagebroker-1.6.7/tests/unit/test_saga_next.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_saga_start.py` & `tc_messagebroker-1.6.7/tests/unit/test_saga_start.py`

 * *Files identical despite different names*

### Comparing `tc-messageBroker-1.6.6/tests/unit/test_transactions.py` & `tc_messagebroker-1.6.7/tests/unit/test_transactions.py`

 * *Files identical despite different names*

