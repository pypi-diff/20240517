# Comparing `tmp/pycti-6.1.1.tar.gz` & `tmp/pycti-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-6.1.1.tar", last modified: Wed May 15 09:35:07 2024, max compression
+gzip compressed data, was "pycti-6.1.2.tar", last modified: Thu May 16 22:05:21 2024, max compression
```

## Comparing `pycti-6.1.1.tar` & `pycti-6.1.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.657570 pycti-6.1.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-15 09:34:55.000000 pycti-6.1.1/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-15 09:35:07.657570 pycti-6.1.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-05-15 09:34:55.000000 pycti-6.1.1/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.645570 pycti-6.1.1/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5035 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.649570 pycti-6.1.1/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29575 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/api/opencti_api_playbook.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7615 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.649570 pycti-6.1.1/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    60606 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/connector/opencti_connector_helper.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/connector/opencti_metric_handler.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.657570 pycti-6.1.1/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18553 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27581 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18957 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21480 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33580 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    49559 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42895 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   106785 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    78504 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17696 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_threat_actor_group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_threat_actor_individual.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.657570 pycti-6.1.1/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10601 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/opencti_logger.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   115786 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4138 2024-05-15 09:34:55.000000 pycti-6.1.1/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-15 09:35:07.657570 pycti-6.1.1/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-15 09:35:07.000000 pycti-6.1.1/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-15 09:35:07.000000 pycti-6.1.1/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-15 09:35:07.000000 pycti-6.1.1/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-15 09:35:07.000000 pycti-6.1.1/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-15 09:35:07.000000 pycti-6.1.1/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-15 09:34:55.000000 pycti-6.1.1/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-05-15 09:35:07.661570 pycti-6.1.1/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.893986 pycti-6.1.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2024-05-16 22:05:07.000000 pycti-6.1.2/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-16 22:05:21.893986 pycti-6.1.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3156 2024-05-16 22:05:07.000000 pycti-6.1.2/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.881986 pycti-6.1.2/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5035 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.881986 pycti-6.1.2/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29575 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3549 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1470 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/api/opencti_api_playbook.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7615 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.881986 pycti-6.1.2/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2449 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    60606 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/connector/opencti_connector_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/connector/opencti_metric_handler.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.889986 pycti-6.1.2/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21471 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17107 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33699 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31876 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32760 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16608 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18001 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18582 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17470 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16706 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13216 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31738 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29320 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22879 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18553 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27581 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19353 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18957 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8062 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8800 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16176 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16970 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20411 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21480 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12862 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16468 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29938 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    30550 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21837 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    33580 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2275 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    49559 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42895 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   106785 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    78504 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12330 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17696 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27584 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24668 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9950 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18996 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_threat_actor_group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19238 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_threat_actor_individual.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14661 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20094 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.889986 pycti-6.1.2/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10601 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2199 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/opencti_logger.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   115786 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14658 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4138 2024-05-16 22:05:07.000000 pycti-6.1.2/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 22:05:21.889986 pycti-6.1.2/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5271 2024-05-16 22:05:21.000000 pycti-6.1.2/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2525 2024-05-16 22:05:21.000000 pycti-6.1.2/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-16 22:05:21.000000 pycti-6.1.2/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-05-16 22:05:21.000000 pycti-6.1.2/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2024-05-16 22:05:21.000000 pycti-6.1.2/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-05-16 22:05:07.000000 pycti-6.1.2/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1626 2024-05-16 22:05:21.893986 pycti-6.1.2/setup.cfg
```

### Comparing `pycti-6.1.1/LICENSE` & `pycti-6.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/PKG-INFO` & `pycti-6.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.1.1
+Version: 6.1.2
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycti-6.1.1/README.md` & `pycti-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/__init__.py` & `pycti-6.1.2/pycti/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-__version__ = "6.1.1"
+__version__ = "6.1.2"
 
 from .api.opencti_api_client import OpenCTIApiClient
 from .api.opencti_api_connector import OpenCTIApiConnector
 from .api.opencti_api_work import OpenCTIApiWork
 from .connector.opencti_connector import ConnectorType, OpenCTIConnector
 from .connector.opencti_connector_helper import (
     OpenCTIConnectorHelper,
```

### Comparing `pycti-6.1.1/pycti/api/opencti_api_client.py` & `pycti-6.1.2/pycti/api/opencti_api_client.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/api/opencti_api_connector.py` & `pycti-6.1.2/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/api/opencti_api_playbook.py` & `pycti-6.1.2/pycti/api/opencti_api_playbook.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/api/opencti_api_work.py` & `pycti-6.1.2/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/connector/opencti_connector.py` & `pycti-6.1.2/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/connector/opencti_connector_helper.py` & `pycti-6.1.2/pycti/connector/opencti_connector_helper.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/connector/opencti_metric_handler.py` & `pycti-6.1.2/pycti/connector/opencti_metric_handler.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_attack_pattern.py` & `pycti-6.1.2/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_campaign.py` & `pycti-6.1.2/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_case_incident.py` & `pycti-6.1.2/pycti/entities/opencti_case_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_case_rfi.py` & `pycti-6.1.2/pycti/entities/opencti_case_rfi.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_case_rft.py` & `pycti-6.1.2/pycti/entities/opencti_case_rft.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_channel.py` & `pycti-6.1.2/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_course_of_action.py` & `pycti-6.1.2/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_data_component.py` & `pycti-6.1.2/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_data_source.py` & `pycti-6.1.2/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_event.py` & `pycti-6.1.2/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_external_reference.py` & `pycti-6.1.2/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_feedback.py` & `pycti-6.1.2/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_grouping.py` & `pycti-6.1.2/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_identity.py` & `pycti-6.1.2/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_incident.py` & `pycti-6.1.2/pycti/entities/opencti_incident.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_indicator.py` & `pycti-6.1.2/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_infrastructure.py` & `pycti-6.1.2/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_intrusion_set.py` & `pycti-6.1.2/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_kill_chain_phase.py` & `pycti-6.1.2/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_label.py` & `pycti-6.1.2/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_language.py` & `pycti-6.1.2/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_location.py` & `pycti-6.1.2/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_malware.py` & `pycti-6.1.2/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_malware_analysis.py` & `pycti-6.1.2/pycti/entities/opencti_malware_analysis.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_marking_definition.py` & `pycti-6.1.2/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_narrative.py` & `pycti-6.1.2/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_note.py` & `pycti-6.1.2/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_observed_data.py` & `pycti-6.1.2/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_opinion.py` & `pycti-6.1.2/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_report.py` & `pycti-6.1.2/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_stix.py` & `pycti-6.1.2/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_stix_core_object.py` & `pycti-6.1.2/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_stix_core_relationship.py` & `pycti-6.1.2/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-6.1.2/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_stix_domain_object.py` & `pycti-6.1.2/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-6.1.2/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-6.1.2/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-6.1.2/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_task.py` & `pycti-6.1.2/pycti/entities/opencti_task.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_threat_actor.py` & `pycti-6.1.2/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_threat_actor_group.py` & `pycti-6.1.2/pycti/entities/opencti_threat_actor_group.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_threat_actor_individual.py` & `pycti-6.1.2/pycti/entities/opencti_threat_actor_individual.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_tool.py` & `pycti-6.1.2/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_vocabulary.py` & `pycti-6.1.2/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/entities/opencti_vulnerability.py` & `pycti-6.1.2/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/utils/constants.py` & `pycti-6.1.2/pycti/utils/constants.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/utils/opencti_logger.py` & `pycti-6.1.2/pycti/utils/opencti_logger.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/utils/opencti_stix2.py` & `pycti-6.1.2/pycti/utils/opencti_stix2.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/utils/opencti_stix2_splitter.py` & `pycti-6.1.2/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/utils/opencti_stix2_update.py` & `pycti-6.1.2/pycti/utils/opencti_stix2_update.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti/utils/opencti_stix2_utils.py` & `pycti-6.1.2/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti.egg-info/PKG-INFO` & `pycti-6.1.2/pycti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 6.1.1
+Version: 6.1.2
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pycti-6.1.1/pycti.egg-info/SOURCES.txt` & `pycti-6.1.2/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pycti.egg-info/requires.txt` & `pycti-6.1.2/pycti.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/pyproject.toml` & `pycti-6.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-6.1.1/setup.cfg` & `pycti-6.1.2/setup.cfg`

 * *Files identical despite different names*

