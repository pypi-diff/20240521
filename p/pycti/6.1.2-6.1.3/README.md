# Comparing `tmp/pycti-6.1.2.tar.gz` & `tmp/pycti-6.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-6.1.2.tar", last modified: Thu May 16 22:05:21 2024, max compression
+gzip compressed data, was "pycti-6.1.3.tar", last modified: Mon May 20 23:00:26 2024, max compression
```

## Comparing `pycti-6.1.2.tar` & `pycti-6.1.3.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.893986 pycti-6.1.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-16 22:05:07.000000 pycti-6.1.2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-16 22:05:21.893986 pycti-6.1.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-05-16 22:05:07.000000 pycti-6.1.2/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.881986 pycti-6.1.2/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5035 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.881986 pycti-6.1.2/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29575 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/api/opencti_api_playbook.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7615 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.881986 pycti-6.1.2/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    60606 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/connector/opencti_connector_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/connector/opencti_metric_handler.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.889986 pycti-6.1.2/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18553 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27581 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18957 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21480 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33580 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    49559 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42895 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106785 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    78504 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17696 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_threat_actor_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_threat_actor_individual.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.889986 pycti-6.1.2/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10601 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/opencti_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   115786 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4138 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.889986 pycti-6.1.2/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-16 22:05:21.000000 pycti-6.1.2/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-16 22:05:21.000000 pycti-6.1.2/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-16 22:05:21.000000 pycti-6.1.2/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-16 22:05:21.000000 pycti-6.1.2/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-16 22:05:21.000000 pycti-6.1.2/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-16 22:05:07.000000 pycti-6.1.2/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-05-16 22:05:21.893986 pycti-6.1.2/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.435885 pycti-6.1.3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-20 23:00:12.000000 pycti-6.1.3/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-20 23:00:26.435885 pycti-6.1.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-05-20 23:00:12.000000 pycti-6.1.3/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.423885 pycti-6.1.3/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5035 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.423885 pycti-6.1.3/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29575 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/api/opencti_api_playbook.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7615 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.427885 pycti-6.1.3/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    60311 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/connector/opencti_connector_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/connector/opencti_metric_handler.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.431885 pycti-6.1.3/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18553 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27581 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18957 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21480 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33580 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    49559 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42895 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106785 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    78504 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17696 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_threat_actor_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_threat_actor_individual.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.435885 pycti-6.1.3/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10601 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/opencti_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   112457 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4138 2024-05-20 23:00:12.000000 pycti-6.1.3/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-20 23:00:26.435885 pycti-6.1.3/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-20 23:00:26.000000 pycti-6.1.3/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-20 23:00:26.000000 pycti-6.1.3/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-20 23:00:26.000000 pycti-6.1.3/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-20 23:00:26.000000 pycti-6.1.3/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-20 23:00:26.000000 pycti-6.1.3/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-20 23:00:12.000000 pycti-6.1.3/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-05-20 23:00:26.435885 pycti-6.1.3/setup.cfg
```

### Comparing `pycti-6.1.2/LICENSE` & `pycti-6.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/PKG-INFO` & `pycti-6.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.1.2
+Version: 6.1.3
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycti-6.1.2/README.md` & `pycti-6.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/__init__.py` & `pycti-6.1.3/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "6.1.2"
+__version__ = "6.1.3"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-6.1.2/pycti/api/opencti_api_client.py` & `pycti-6.1.3/pycti/api/opencti_api_client.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/api/opencti_api_connector.py` & `pycti-6.1.3/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/api/opencti_api_playbook.py` & `pycti-6.1.3/pycti/api/opencti_api_playbook.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/api/opencti_api_work.py` & `pycti-6.1.3/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/connector/opencti_connector.py` & `pycti-6.1.3/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/connector/opencti_connector_helper.py` & `pycti-6.1.3/pycti/connector/opencti_connector_helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,25 +258,18 @@
             self.helper.enrichment_shared_organizations = None
             if self.helper.connect_type == "INTERNAL_ENRICHMENT":
                 # For enrichment connectors only, pre resolve the information
                 if entity_id is None:
                     raise ValueError(
                         "Internal enrichment must be based on a specific id"
                     )
-                default_reader_type = "Stix-Core-Object"
-                readers = self.helper.api.stix2.get_readers()
-                reader_type = (
-                    entity_type if entity_type is not None else default_reader_type
+                do_read = self.helper.api.stix2.get_reader(
+                    entity_type if entity_type is not None else "Stix-Core-Object"
                 )
-                selected_reader = (
-                    readers[reader_type]
-                    if reader_type in readers
-                    else readers[default_reader_type]
-                )
-                opencti_entity = selected_reader(id=entity_id, withFiles=True)
+                opencti_entity = do_read(id=entity_id, withFiles=True)
                 if opencti_entity is None:
                     raise ValueError(
                         "Unable to read/access to the entity, please check that the connector permission"
                     )
                 event_data["enrichment_entity"] = opencti_entity
                 # Handle action vs playbook behavior
                 is_playbook = "playbook" in json_data["internal"]
```

### Comparing `pycti-6.1.2/pycti/connector/opencti_metric_handler.py` & `pycti-6.1.3/pycti/connector/opencti_metric_handler.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_attack_pattern.py` & `pycti-6.1.3/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_campaign.py` & `pycti-6.1.3/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_case_incident.py` & `pycti-6.1.3/pycti/entities/opencti_case_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_case_rfi.py` & `pycti-6.1.3/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_case_rft.py` & `pycti-6.1.3/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_channel.py` & `pycti-6.1.3/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_course_of_action.py` & `pycti-6.1.3/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_data_component.py` & `pycti-6.1.3/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_data_source.py` & `pycti-6.1.3/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_event.py` & `pycti-6.1.3/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_external_reference.py` & `pycti-6.1.3/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_feedback.py` & `pycti-6.1.3/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_grouping.py` & `pycti-6.1.3/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_identity.py` & `pycti-6.1.3/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_incident.py` & `pycti-6.1.3/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_indicator.py` & `pycti-6.1.3/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_infrastructure.py` & `pycti-6.1.3/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_intrusion_set.py` & `pycti-6.1.3/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_kill_chain_phase.py` & `pycti-6.1.3/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_label.py` & `pycti-6.1.3/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_language.py` & `pycti-6.1.3/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_location.py` & `pycti-6.1.3/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_malware.py` & `pycti-6.1.3/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_malware_analysis.py` & `pycti-6.1.3/pycti/entities/opencti_malware_analysis.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_marking_definition.py` & `pycti-6.1.3/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_narrative.py` & `pycti-6.1.3/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_note.py` & `pycti-6.1.3/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_observed_data.py` & `pycti-6.1.3/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_opinion.py` & `pycti-6.1.3/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_report.py` & `pycti-6.1.3/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_stix.py` & `pycti-6.1.3/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_stix_core_object.py` & `pycti-6.1.3/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_stix_core_relationship.py` & `pycti-6.1.3/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-6.1.3/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_stix_domain_object.py` & `pycti-6.1.3/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-6.1.3/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-6.1.3/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-6.1.3/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_task.py` & `pycti-6.1.3/pycti/entities/opencti_task.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_threat_actor.py` & `pycti-6.1.3/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_threat_actor_group.py` & `pycti-6.1.3/pycti/entities/opencti_threat_actor_group.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_threat_actor_individual.py` & `pycti-6.1.3/pycti/entities/opencti_threat_actor_individual.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_tool.py` & `pycti-6.1.3/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_vocabulary.py` & `pycti-6.1.3/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/entities/opencti_vulnerability.py` & `pycti-6.1.3/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/utils/constants.py` & `pycti-6.1.3/pycti/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/utils/opencti_logger.py` & `pycti-6.1.3/pycti/utils/opencti_logger.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/utils/opencti_stix2.py` & `pycti-6.1.3/pycti/utils/opencti_stix2.py`

 * *Files 2% similar despite different names*

```diff
@@ -750,56 +750,15 @@
             "object_refs": object_refs_ids,
             "granted_refs": granted_refs_ids,
             "sample_refs": sample_refs_ids,
             "external_references": external_references_ids,
             "reports": reports,
         }
 
-    def get_listers(self):
-        return {
-            "Stix-Core-Object": self.opencti.stix_core_object.list,
-            "Stix-Domain-Object": self.opencti.stix_domain_object.list,
-            "Administrative-Area": self.opencti.location.list,
-            "Attack-Pattern": self.opencti.attack_pattern.list,
-            "Campaign": self.opencti.campaign.list,
-            "Channel": self.opencti.channel.list,
-            "Event": self.opencti.event.list,
-            "Note": self.opencti.note.list,
-            "Observed-Data": self.opencti.observed_data.list,
-            "Opinion": self.opencti.opinion.list,
-            "Report": self.opencti.report.list,
-            "Grouping": self.opencti.grouping.list,
-            "Case-Incident": self.opencti.case_incident.list,
-            "Feedback": self.opencti.feedback.list,
-            "Case-Rfi": self.opencti.case_rfi.list,
-            "Case-Rft": self.opencti.case_rft.list,
-            "Task": self.opencti.task.list,
-            "Course-Of-Action": self.opencti.course_of_action.list,
-            "Data-Component": self.opencti.data_component.list,
-            "Data-Source": self.opencti.data_source.list,
-            "Identity": self.opencti.identity.list,
-            "Indicator": self.opencti.indicator.list,
-            "Infrastructure": self.opencti.infrastructure.list,
-            "Intrusion-Set": self.opencti.intrusion_set.list,
-            "Location": self.opencti.location.list,
-            "Language": self.opencti.language.list,
-            "Malware": self.opencti.malware.list,
-            "Malware-Analysis": self.opencti.malware_analysis.list,
-            "Threat-Actor": self.opencti.threat_actor_group.list,
-            "Threat-Actor-Group": self.opencti.threat_actor_group.list,
-            "Threat-Actor-Individual": self.opencti.threat_actor_individual.list,
-            "Tool": self.opencti.tool.list,
-            "Narrative": self.opencti.narrative.list,
-            "Vulnerability": self.opencti.vulnerability.list,
-            "Incident": self.opencti.incident.list,
-            "Stix-Cyber-Observable": self.opencti.stix_cyber_observable.list,
-            "stix-sighting-relationship": self.opencti.stix_sighting_relationship.list,
-            "stix-core-relationship": self.opencti.stix_core_relationship.list,
-        }
-
+    # Please use get_reader instead of this definition
     def get_readers(self):
         return {
             "Attack-Pattern": self.opencti.attack_pattern.read,
             "Campaign": self.opencti.campaign.read,
             "Case-Incident": self.opencti.case_incident.read,
             "Case-Rfi": self.opencti.case_rfi.read,
             "Case-Rft": self.opencti.case_rft.read,
@@ -847,16 +806,19 @@
         # Map types
         if entity_type == "StixFile":
             entity_type = "File"
         if IdentityTypes.has_value(entity_type):
             entity_type = "Identity"
         if LocationTypes.has_value(entity_type):
             entity_type = "Location"
+        if entity_type == "Container":
+            entity_type = "Stix-Domain-Object"
         if StixCyberObservableTypes.has_value(entity_type):
             entity_type = "Stix-Cyber-Observable"
+
         readers = self.get_readers()
         return readers.get(
             entity_type, lambda **kwargs: self.unknown_type({"type": entity_type})
         )
 
     # endregion
 
@@ -1868,29 +1830,29 @@
             relationships_from_filter = self.prepare_id_filters_export(
                 id=from_to_check, access_filter=access_filter
             )
             x = self.opencti.opencti_stix_object_or_stix_relationship.list(
                 filters=relationships_from_filter
             )
             if len(x) > 0:
-                entity["sighting_of_ref"] = entity["from"]["id"]
+                entity["sighting_of_ref"] = entity["from"]["standard_id"]
                 # handle from and to separately like Stix Core Relationship and call 2 requests
                 objects_to_get.append(
                     entity["from"]
                 )  # what happen with unauthorized objects ?
 
             to_to_check = [entity["to"]["id"]]
             relationships_to_filter = self.prepare_id_filters_export(
                 id=to_to_check, access_filter=access_filter
             )
             y = self.opencti.opencti_stix_object_or_stix_relationship.list(
                 filters=relationships_to_filter
             )
             if len(y) > 0:
-                entity["where_sighted_refs"] = [entity["to"]["id"]]
+                entity["where_sighted_refs"] = [entity["to"]["standard_id"]]
                 objects_to_get.append(entity["to"])
 
             del entity["from"]
             del entity["to"]
         # Stix Core Relationship
         if "from" in entity or "to" in entity:
             entity["type"] = "relationship"
@@ -1899,30 +1861,30 @@
             relationships_from_filter = self.prepare_id_filters_export(
                 id=from_to_check, access_filter=access_filter
             )
             x = self.opencti.opencti_stix_object_or_stix_relationship.list(
                 filters=relationships_from_filter
             )
             if len(x) > 0:
-                entity["source_ref"] = entity["from"]["id"]
+                entity["source_ref"] = entity["from"]["standard_id"]
                 # handle from and to separately like Stix Core Relationship and call 2 requests
                 objects_to_get.append(
                     entity["from"]
                 )  # what happen with unauthorized objects ?
             del entity["from"]
         if "to" in entity:
             to_to_check = [entity["to"]["id"]]
             relationships_to_filter = self.prepare_id_filters_export(
                 id=to_to_check, access_filter=access_filter
             )
             y = self.opencti.opencti_stix_object_or_stix_relationship.list(
                 filters=relationships_to_filter
             )
             if len(y) > 0:
-                entity["target_ref"] = entity["to"]["id"]
+                entity["target_ref"] = entity["to"]["standard_id"]
                 objects_to_get.append(entity["to"])
             del entity["to"]
         # Stix Domain Object
         if "attribute_abstract" in entity:
             entity["abstract"] = entity["attribute_abstract"]
             del entity["attribute_abstract"]
         # Stix Cyber Observable
@@ -2091,40 +2053,22 @@
                     uuids, relation_object_data
                 )
                 uuids = uuids + [x["id"] for x in relation_object_bundle]
                 result = result + relation_object_bundle
 
             if no_custom_attributes:
                 del entity["x_opencti_id"]
-            # Export
-            reader = self.get_readers()
             # Get extra objects
             for entity_object in objects_to_get:
-                # Map types
-                if entity_object["entity_type"] == "StixFile":
-                    entity_object["entity_type"] = "File"
-
-                if IdentityTypes.has_value(entity_object["entity_type"]):
-                    entity_object["entity_type"] = "Identity"
-                elif LocationTypes.has_value(entity_object["entity_type"]):
-                    entity_object["entity_type"] = "Location"
-                elif StixCyberObservableTypes.has_value(entity_object["entity_type"]):
-                    entity_object["entity_type"] = "Stix-Cyber-Observable"
-                elif "stix-core-relationship" in entity_object["parent_types"]:
-                    entity_object["entity_type"] = "stix-core-relationship"
-                elif "stix-ref-relationship" in entity_object["parent_types"]:
-                    entity_object["entity_type"] = "stix-ref-relationship"
-
-                do_read = reader.get(
-                    entity_object["entity_type"],
-                    lambda **kwargs: self.unknown_type(
-                        {"type": entity_object["entity_type"]}
-                    ),
-                )
-
+                resolve_type = entity_object["entity_type"]
+                if "stix-core-relationship" in entity_object["parent_types"]:
+                    resolve_type = "stix-core-relationship"
+                if "stix-ref-relationship" in entity_object["parent_types"]:
+                    resolve_type = "stix-ref-relationship"
+                do_read = self.get_reader(resolve_type)
                 query_filters = self.prepare_id_filters_export(
                     entity_object["id"], access_filter
                 )
                 entity_object_data = do_read(filters=query_filters)
                 if entity_object_data is not None:
                     stix_entity_object = self.prepare_export(
                         entity=self.generate_export(entity_object_data),
@@ -2221,28 +2165,15 @@
         only_entity: bool = False,
     ) -> Dict:
         bundle = {
             "type": "bundle",
             "id": "bundle--" + str(uuid.uuid4()),
             "objects": [],
         }
-
-        if entity_type == "StixFile":
-            entity_type = "File"
-
-        # Map types
-        if IdentityTypes.has_value(entity_type):
-            entity_type = "Identity"
-        if LocationTypes.has_value(entity_type):
-            entity_type = "Location"
-
-        readers = self.get_readers()
-        do_read = readers.get(
-            entity_type, lambda **kwargs: self.unknown_type({"type": entity_type})
-        )
+        do_read = self.get_reader(entity_type)
         entity = do_read(id=entity_id)
         if entity is None:
             self.opencti.app_logger.error(
                 "Cannot export entity (not found)", {"id": entity_id}
             )
             return bundle
         entity_standard_id = entity["standard_id"]
```

### Comparing `pycti-6.1.2/pycti/utils/opencti_stix2_splitter.py` & `pycti-6.1.3/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/utils/opencti_stix2_update.py` & `pycti-6.1.3/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti/utils/opencti_stix2_utils.py` & `pycti-6.1.3/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti.egg-info/PKG-INFO` & `pycti-6.1.3/pycti.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.1.2
+Version: 6.1.3
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycti-6.1.2/pycti.egg-info/SOURCES.txt` & `pycti-6.1.3/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pycti.egg-info/requires.txt` & `pycti-6.1.3/pycti.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/pyproject.toml` & `pycti-6.1.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-6.1.2/setup.cfg` & `pycti-6.1.3/setup.cfg`

 * *Files identical despite different names*

