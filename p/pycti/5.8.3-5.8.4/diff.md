# Comparing `tmp/pycti-5.8.3.tar.gz` & `tmp/pycti-5.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycti-5.8.3.tar", last modified: Fri Jun 23 11:17:04 2023, max compression
+gzip compressed data, was "pycti-5.8.4.tar", last modified: Sun Jun 25 20:10:55 2023, max compression
```

## Comparing `pycti-5.8.3.tar` & `pycti-5.8.4.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.363731 pycti-5.8.3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-06-23 11:16:52.000000 pycti-5.8.3/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-06-23 11:17:04.363731 pycti-5.8.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-06-23 11:16:52.000000 pycti-5.8.3/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.355731 pycti-5.8.3/pycti/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3856 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.355731 pycti-5.8.3/pycti/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    28410 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/api/opencti_api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/api/opencti_api_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6825 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/api/opencti_api_work.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.355731 pycti-5.8.3/pycti/connector/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/connector/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/connector/opencti_connector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45735 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/connector/opencti_connector_helper.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.363731 pycti-5.8.3/pycti/entities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18880 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_attack_pattern.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13376 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_campaign.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25113 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_case_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24427 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_case_rfi.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24435 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_case_rft.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_channel.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14512 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_course_of_action.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14598 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_data_component.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14155 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_data_source.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_event.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10891 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_external_reference.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25480 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_feedback.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22913 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_grouping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17564 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_identity.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14024 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_incident.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23077 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_indicator.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15944 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_infrastructure.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14455 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_intrusion_set.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_kill_chain_phase.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_label.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_language.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_location.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16288 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_malware.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17551 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_malware_analysis.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_marking_definition.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_narrative.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22348 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_note.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22667 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_observed_data.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20971 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_opinion.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23782 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_report.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_core_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_core_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_cyber_observable.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_domain_object.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_nested_ref_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_object_or_stix_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_stix_sighting_relationship.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23493 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_task.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18371 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_threat_actor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14210 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_tool.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_vocabulary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17683 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/entities/opencti_vulnerability.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.363731 pycti-5.8.3/pycti/utils/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/utils/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3397 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/utils/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   103481 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/utils/opencti_stix2.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/utils/opencti_stix2_splitter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14520 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/utils/opencti_stix2_update.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-06-23 11:16:52.000000 pycti-5.8.3/pycti/utils/opencti_stix2_utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-23 11:17:04.355731 pycti-5.8.3/pycti.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-06-23 11:17:04.000000 pycti-5.8.3/pycti.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-06-23 11:17:04.000000 pycti-5.8.3/pycti.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-23 11:17:04.000000 pycti-5.8.3/pycti.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-06-23 11:17:04.000000 pycti-5.8.3/pycti.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-23 11:17:04.000000 pycti-5.8.3/pycti.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-06-23 11:16:52.000000 pycti-5.8.3/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-06-23 11:17:04.363731 pycti-5.8.3/setup.cfg
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 20:10:55.481634 pycti-5.8.4/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11357 2023-06-25 20:10:43.000000 pycti-5.8.4/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-06-25 20:10:55.481634 pycti-5.8.4/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3177 2023-06-25 20:10:43.000000 pycti-5.8.4/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 20:10:55.469634 pycti-5.8.4/pycti/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4262 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 20:10:55.469634 pycti-5.8.4/pycti/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    28410 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/api/opencti_api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3565 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/api/opencti_api_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6825 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/api/opencti_api_work.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 20:10:55.473634 pycti-5.8.4/pycti/connector/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/connector/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2294 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/connector/opencti_connector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45735 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/connector/opencti_connector_helper.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 20:10:55.481634 pycti-5.8.4/pycti/entities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       53 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18880 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_attack_pattern.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13376 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_campaign.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25217 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_case_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24565 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_case_rfi.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24546 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_case_rft.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13858 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_channel.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14512 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_course_of_action.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14598 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_data_component.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14155 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_data_source.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14003 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_event.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10891 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_external_reference.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25480 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_feedback.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22913 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_grouping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17564 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_identity.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14162 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_incident.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23077 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_indicator.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15944 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_infrastructure.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14455 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_intrusion_set.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7854 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_kill_chain_phase.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7350 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_label.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13006 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_language.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14554 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_location.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16288 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_malware.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17551 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_malware_analysis.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12156 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_marking_definition.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13948 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_narrative.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22348 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_note.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22667 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_observed_data.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20971 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_opinion.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23782 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_report.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2399 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_stix.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32440 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_stix_core_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    41865 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_stix_core_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    92142 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_stix_cyber_observable.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    64861 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_stix_domain_object.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12081 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_stix_nested_ref_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16091 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_stix_object_or_stix_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    27612 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_stix_sighting_relationship.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23507 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_task.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18371 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_threat_actor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14210 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_tool.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_vocabulary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17683 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/entities/opencti_vulnerability.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 20:10:55.481634 pycti-5.8.4/pycti/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6581 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/utils/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   104930 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/utils/opencti_stix2.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4496 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/utils/opencti_stix2_splitter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14515 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/utils/opencti_stix2_update.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3677 2023-06-25 20:10:43.000000 pycti-5.8.4/pycti/utils/opencti_stix2_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-06-25 20:10:55.469634 pycti-5.8.4/pycti.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4087 2023-06-25 20:10:55.000000 pycti-5.8.4/pycti.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-06-25 20:10:55.000000 pycti-5.8.4/pycti.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-06-25 20:10:55.000000 pycti-5.8.4/pycti.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      581 2023-06-25 20:10:55.000000 pycti-5.8.4/pycti.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        6 2023-06-25 20:10:55.000000 pycti-5.8.4/pycti.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2023-06-25 20:10:43.000000 pycti-5.8.4/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1596 2023-06-25 20:10:55.481634 pycti-5.8.4/setup.cfg
```

### Comparing `pycti-5.8.3/LICENSE` & `pycti-5.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/PKG-INFO` & `pycti-5.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.8.3
+Version: 5.8.4
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.8.3 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.8.4 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.8.3/README.md` & `pycti-5.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/api/opencti_api_client.py` & `pycti-5.8.4/pycti/api/opencti_api_client.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/api/opencti_api_connector.py` & `pycti-5.8.4/pycti/api/opencti_api_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/api/opencti_api_work.py` & `pycti-5.8.4/pycti/api/opencti_api_work.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/connector/opencti_connector.py` & `pycti-5.8.4/pycti/connector/opencti_connector.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/connector/opencti_connector_helper.py` & `pycti-5.8.4/pycti/connector/opencti_connector_helper.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_attack_pattern.py` & `pycti-5.8.4/pycti/entities/opencti_attack_pattern.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_campaign.py` & `pycti-5.8.4/pycti/entities/opencti_campaign.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_case_incident.py` & `pycti-5.8.4/pycti/entities/opencti_case_incident.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import json
 import uuid
 
 from dateutil.parser import parse
 from stix2.canonicalization.Canonicalize import canonicalize
 
 from pycti.entities import LOGGER
@@ -237,17 +238,19 @@
                         }
                     }
                 }
             }
         """
 
     @staticmethod
-    def generate_id(name):
+    def generate_id(name, created):
         name = name.lower().strip()
-        data = {"name": name}
+        if isinstance(created, datetime.datetime):
+            created = created.isoformat()
+        data = {"name": name, "created": created}
         data = canonicalize(data, utf8=False)
         id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
         return "case-incident--" + id
 
     """
         List Case Incident objects
         
@@ -267,18 +270,15 @@
         order_mode = kwargs.get("orderMode", None)
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
             first = 500
 
-        self.opencti.log(
-            "info",
-            "Listing Case Incidents with filters " + json.dumps(filters) + ".",
-        )
+        LOGGER.info("Listing Case Incidents with filters " + json.dumps(filters) + ".")
         query = (
             """
                 query CaseIncidents($filters: [CaseIncidentsFiltering!], $search: String, $first: Int, $after: ID, $orderBy: CaseIncidentsOrdering, $orderMode: OrderingMode) {
                     caseIncidents(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
                         edges {
                             node {
                                 """
@@ -561,15 +561,15 @@
         else:
             self.opencti.log(
                 "error",
                 "[opencti_caseIncident] Missing parameters: id and stixObjectOrStixRelationshipId",
             )
             return False
 
-        """
+    """
         Remove a Stix-Entity object to Case Incident object (object_refs)
 
         :param id: the id of the Case Incident
         :param stixObjectOrStixRelationshipId: the id of the Stix-Entity
         :return Boolean
     """
 
@@ -608,20 +608,20 @@
         else:
             self.opencti.log(
                 "error",
                 "[opencti_caseIncident] Missing parameters: id and stixObjectOrStixRelationshipId",
             )
             return False
 
-        """
+    """
         Import a Case Incident object from a STIX2 object
 
         :param stixObject: the Stix-Object Case Incident
         :return Case Incident object
-        """
+    """
 
     def import_from_stix2(self, **kwargs):
         stix_object = kwargs.get("stixObject", None)
         extras = kwargs.get("extras", {})
         update = kwargs.get("update", False)
         if stix_object is not None:
             # Search in extensions
@@ -679,19 +679,19 @@
             self.opencti.log(
                 "error", "[opencti_caseIncident] Missing parameters: stixObject"
             )
 
     def delete(self, **kwargs):
         id = kwargs.get("id", None)
         if id is not None:
-            LOGGER.info("Deleting Case Incident {%s}.", id)
+            self.opencti.log("info", "Deleting Case Incident {%s}.", id)
             query = """
                  mutation CaseIncidentDelete($id: ID!) {
                      stixDomainObjectEdit(id: $id) {
                          delete
                      }
                  }
              """
             self.opencti.query(query, {"id": id})
         else:
-            LOGGER.error("[opencti_case_incident] Missing parameters: id")
+            self.opencti.log("error", "[opencti_case_incident] Missing parameters: id")
             return None
```

### Comparing `pycti-5.8.3/pycti/entities/opencti_case_rfi.py` & `pycti-5.8.4/pycti/entities/opencti_case_rfi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import json
 import uuid
 
 from dateutil.parser import parse
 from stix2.canonicalization.Canonicalize import canonicalize
 
 from pycti.entities import LOGGER
@@ -234,17 +235,19 @@
                         }
                     }
                 }
             }
         """
 
     @staticmethod
-    def generate_id(name):
+    def generate_id(name, created):
         name = name.lower().strip()
-        data = {"name": name}
+        if isinstance(created, datetime.datetime):
+            created = created.isoformat()
+        data = {"name": name, "created": created}
         data = canonicalize(data, utf8=False)
         id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
         return "case-rfi--" + id
 
     """
         List Case Rfi objects
```

### Comparing `pycti-5.8.3/pycti/entities/opencti_case_rft.py` & `pycti-5.8.4/pycti/entities/opencti_case_rft.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import json
 import uuid
 
 from dateutil.parser import parse
 from stix2.canonicalization.Canonicalize import canonicalize
 
 from pycti.entities import LOGGER
@@ -234,17 +235,19 @@
                         }
                     }
                 }
             }
         """
 
     @staticmethod
-    def generate_id(name):
+    def generate_id(name, created):
         name = name.lower().strip()
-        data = {"name": name}
+        if isinstance(created, datetime.datetime):
+            created = created.isoformat()
+        data = {"name": name, "created": created}
         data = canonicalize(data, utf8=False)
         id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
         return "case-rft--" + id
 
     """
         List Case Rft objects
         
@@ -263,19 +266,15 @@
         order_by = kwargs.get("orderBy", None)
         order_mode = kwargs.get("orderMode", None)
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
             first = 500
-
-        self.opencti.log(
-            "info",
-            "Listing Case Rfts with filters " + json.dumps(filters) + ".",
-        )
+        LOGGER.info("Listing Case Rfts with filters " + json.dumps(filters) + ".")
         query = (
             """
                         query CaseRfts($filters: [CaseRftsFiltering!], $search: String, $first: Int, $after: ID, $orderBy: CaseRftsOrdering, $orderMode: OrderingMode) {
                             caseRfts(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
                                 edges {
                                     node {
                                         """
@@ -552,15 +551,15 @@
         else:
             self.opencti.log(
                 "error",
                 "[opencti_caseRft] Missing parameters: id and stixObjectOrStixRelationshipId",
             )
             return False
 
-        """
+    """
         Remove a Stix-Entity object to Case Rft object (object_refs)
 
         :param id: the id of the Case Rft
         :param stixObjectOrStixRelationshipId: the id of the Stix-Entity
         :return Boolean
     """
 
@@ -668,19 +667,19 @@
             self.opencti.log(
                 "error", "[opencti_caseRft] Missing parameters: stixObject"
             )
 
     def delete(self, **kwargs):
         id = kwargs.get("id", None)
         if id is not None:
-            LOGGER.info("Deleting Case RFT {%s}.", id)
+            self.opencti.log("info", "Deleting Case RFT {%s}.", id)
             query = """
                  mutation CaseRFTDelete($id: ID!) {
                      stixDomainObjectEdit(id: $id) {
                          delete
                      }
                  }
              """
             self.opencti.query(query, {"id": id})
         else:
-            LOGGER.error("[opencti_case_rft] Missing parameters: id")
+            self.opencti.log("error", "[opencti_case_rft] Missing parameters: id")
             return None
```

### Comparing `pycti-5.8.3/pycti/entities/opencti_channel.py` & `pycti-5.8.4/pycti/entities/opencti_channel.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_course_of_action.py` & `pycti-5.8.4/pycti/entities/opencti_course_of_action.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_data_component.py` & `pycti-5.8.4/pycti/entities/opencti_data_component.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_data_source.py` & `pycti-5.8.4/pycti/entities/opencti_data_source.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_event.py` & `pycti-5.8.4/pycti/entities/opencti_event.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_external_reference.py` & `pycti-5.8.4/pycti/entities/opencti_external_reference.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_feedback.py` & `pycti-5.8.4/pycti/entities/opencti_feedback.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_grouping.py` & `pycti-5.8.4/pycti/entities/opencti_grouping.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_identity.py` & `pycti-5.8.4/pycti/entities/opencti_identity.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_incident.py` & `pycti-5.8.4/pycti/entities/opencti_incident.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # coding: utf-8
 
+import datetime
 import json
 import uuid
 
 from stix2.canonicalization.Canonicalize import canonicalize
 
 from pycti.entities import LOGGER
 
@@ -131,17 +132,19 @@
                         }
                     }
                 }
             }
         """
 
     @staticmethod
-    def generate_id(name):
+    def generate_id(name, created):
         name = name.lower().strip()
-        data = {"name": name}
+        if isinstance(created, datetime.datetime):
+            created = created.isoformat()
+        data = {"name": name, "created": created}
         data = canonicalize(data, utf8=False)
         id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
         return "incident--" + id
 
     """
         List Incident objects
```

### Comparing `pycti-5.8.3/pycti/entities/opencti_indicator.py` & `pycti-5.8.4/pycti/entities/opencti_indicator.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_infrastructure.py` & `pycti-5.8.4/pycti/entities/opencti_infrastructure.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_intrusion_set.py` & `pycti-5.8.4/pycti/entities/opencti_intrusion_set.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_kill_chain_phase.py` & `pycti-5.8.4/pycti/entities/opencti_kill_chain_phase.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_label.py` & `pycti-5.8.4/pycti/entities/opencti_label.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_language.py` & `pycti-5.8.4/pycti/entities/opencti_language.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_location.py` & `pycti-5.8.4/pycti/entities/opencti_location.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_malware.py` & `pycti-5.8.4/pycti/entities/opencti_malware.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_malware_analysis.py` & `pycti-5.8.4/pycti/entities/opencti_malware_analysis.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_marking_definition.py` & `pycti-5.8.4/pycti/entities/opencti_marking_definition.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_narrative.py` & `pycti-5.8.4/pycti/entities/opencti_narrative.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_note.py` & `pycti-5.8.4/pycti/entities/opencti_note.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_observed_data.py` & `pycti-5.8.4/pycti/entities/opencti_observed_data.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_opinion.py` & `pycti-5.8.4/pycti/entities/opencti_opinion.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_report.py` & `pycti-5.8.4/pycti/entities/opencti_report.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_stix.py` & `pycti-5.8.4/pycti/entities/opencti_stix.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_stix_core_object.py` & `pycti-5.8.4/pycti/entities/opencti_stix_core_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_stix_core_relationship.py` & `pycti-5.8.4/pycti/entities/opencti_stix_core_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_stix_cyber_observable.py` & `pycti-5.8.4/pycti/entities/opencti_stix_cyber_observable.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_stix_domain_object.py` & `pycti-5.8.4/pycti/entities/opencti_stix_domain_object.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_stix_nested_ref_relationship.py` & `pycti-5.8.4/pycti/entities/opencti_stix_nested_ref_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_stix_object_or_stix_relationship.py` & `pycti-5.8.4/pycti/entities/opencti_stix_object_or_stix_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_stix_sighting_relationship.py` & `pycti-5.8.4/pycti/entities/opencti_stix_sighting_relationship.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_task.py` & `pycti-5.8.4/pycti/entities/opencti_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import datetime
 import json
 import uuid
 
 from dateutil.parser import parse
 from stix2.canonicalization.Canonicalize import canonicalize
 
 from pycti.entities import LOGGER
@@ -234,17 +235,19 @@
                         }
                     }
                 }
             }
         """
 
     @staticmethod
-    def generate_id(name):
+    def generate_id(name, created):
         name = name.lower().strip()
-        data = {"name": name}
+        if isinstance(created, datetime.datetime):
+            created = created.isoformat()
+        data = {"name": name, "created": created}
         data = canonicalize(data, utf8=False)
         id = str(uuid.uuid5(uuid.UUID("00abedb4-aa42-466c-9c01-fed23315a9b7"), data))
         return "task--" + id
 
     """
         List Task objects
         
@@ -264,25 +267,22 @@
         order_mode = kwargs.get("orderMode", None)
         custom_attributes = kwargs.get("customAttributes", None)
         get_all = kwargs.get("getAll", False)
         with_pagination = kwargs.get("withPagination", False)
         if get_all:
             first = 500
 
-        self.opencti.log(
-            "info",
-            "Listing Tasks with filters " + json.dumps(filters) + ".",
-        )
+        LOGGER.info("Listing Tasks with filters " + json.dumps(filters) + ".")
         query = (
             """
-                                query tasks($filters: [TasksFiltering!], $search: String, $first: Int, $after: ID, $orderBy: TasksOrdering, $orderMode: OrderingMode) {
-                                    tasks(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
-                                        edges {
-                                            node {
-                                                """
+        query tasks($filters: [TasksFiltering!], $search: String, $first: Int, $after: ID, $orderBy: TasksOrdering, $orderMode: OrderingMode) {
+            tasks(filters: $filters, search: $search, first: $first, after: $after, orderBy: $orderBy, orderMode: $orderMode) {
+                edges {
+                    node {
+                            """
             + (custom_attributes if custom_attributes is not None else self.properties)
             + """
                         }
                     }
                     pageInfo {
                         startCursor
                         endCursor
@@ -490,15 +490,15 @@
         else:
             self.opencti.log(
                 "error",
                 "[opencti_task] Missing parameters: name",
             )
 
     def update_field(self, **kwargs):
-        LOGGER.info("Updating Task {%s}.", json.dumps(kwargs))
+        self.opencti.log("info", "Updating Task {%s}.", json.dumps(kwargs))
         id = kwargs.get("id", None)
         input = kwargs.get("input", None)
         if id is not None and input is not None:
             query = """
                         mutation TaskEdit($id: ID!, $input: [EditInput!]!) {
                            taskFieldPatch(id: $id, input: $input) {
                                 id
@@ -508,18 +508,20 @@
                         }
                     """
             result = self.opencti.query(query, {"id": id, "input": input})
             return self.opencti.process_multiple_fields(
                 result["data"]["taskFieldPatch"]
             )
         else:
-            LOGGER.error("[opencti_Task] Missing parameters: id and key and value")
+            self.opencti.log(
+                "error", "[opencti_Task] Missing parameters: id and key and value"
+            )
             return None
 
-        """
+    """
         Add a Stix-Entity object to Task object (object_refs)
 
         :param id: the id of the Task
         :param stixObjectOrStixRelationshipId: the id of the Stix-Entity
         :return Boolean
     """
 
@@ -558,15 +560,15 @@
         else:
             self.opencti.log(
                 "error",
                 "[opencti_task] Missing parameters: id and stixObjectOrStixRelationshipId",
             )
             return False
 
-        """
+    """
         Remove a Stix-Entity object to Task object (object_refs)
 
         :param id: the id of the Task
         :param stixObjectOrStixRelationshipId: the id of the Stix-Entity
         :return Boolean
     """
 
@@ -603,20 +605,20 @@
         else:
             self.opencti.log(
                 "error",
                 "[opencti_task] Missing parameters: id and stixObjectOrStixRelationshipId",
             )
             return False
 
-        """
+    """
         Import a Task object from a STIX2 object
 
         :param stixObject: the Stix-Object Task
         :return Task object
-        """
+    """
 
     def import_from_stix2(self, **kwargs):
         stix_object = kwargs.get("stixObject", None)
         extras = kwargs.get("extras", {})
         update = kwargs.get("update", False)
         if stix_object is not None:
             # Search in extensions
```

### Comparing `pycti-5.8.3/pycti/entities/opencti_threat_actor.py` & `pycti-5.8.4/pycti/entities/opencti_threat_actor.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_tool.py` & `pycti-5.8.4/pycti/entities/opencti_tool.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_vocabulary.py` & `pycti-5.8.4/pycti/entities/opencti_vocabulary.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/entities/opencti_vulnerability.py` & `pycti-5.8.4/pycti/entities/opencti_vulnerability.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/utils/opencti_stix2.py` & `pycti-5.8.4/pycti/utils/opencti_stix2.py`

 * *Files 1% similar despite different names*

```diff
@@ -775,18 +775,23 @@
             "event": self.opencti.event.import_from_stix2,
             "note": self.opencti.note.import_from_stix2,
             "observed-data": self.opencti.observed_data.import_from_stix2,
             "opinion": self.opencti.opinion.import_from_stix2,
             "report": self.opencti.report.import_from_stix2,
             "grouping": self.opencti.grouping.import_from_stix2,
             "case-rfi": self.opencti.case_rfi.import_from_stix2,
+            "x-opencti-case-rfi": self.opencti.case_rfi.import_from_stix2,
             "case-rft": self.opencti.case_rft.import_from_stix2,
+            "x-opencti-case-rft": self.opencti.case_rft.import_from_stix2,
             "task": self.opencti.task.import_from_stix2,
+            "x-opencti-task": self.opencti.task.import_from_stix2,
             "case-incident": self.opencti.case_incident.import_from_stix2,
+            "x-opencti-case-incident": self.opencti.case_incident.import_from_stix2,
             "feedback": self.opencti.feedback.import_from_stix2,
+            "x-opencti-feedback": self.opencti.feedback.import_from_stix2,
             "course-of-action": self.opencti.course_of_action.import_from_stix2,
             "data-component": self.opencti.data_component.import_from_stix2,
             "x-mitre-data-component": self.opencti.data_component.import_from_stix2,
             "data-source": self.opencti.data_source.import_from_stix2,
             "x-mitre-data-source": self.opencti.data_source.import_from_stix2,
             "identity": self.opencti.identity.import_from_stix2,
             "indicator": self.opencti.indicator.import_from_stix2,
@@ -1252,14 +1257,39 @@
             if "is_family" not in entity or not isinstance(entity["is_family"], bool):
                 entity["is_family"] = True
 
         # Files
         if entity["entity_type"] == "StixFile":
             entity["entity_type"] = "File"
 
+        # Case Incident
+        if entity["entity_type"] == "Case-Incident":
+            entity["standard_id"] = "x-opencti-" + entity["standard_id"]
+            entity["entity_type"] = "x-opencti-" + entity["entity_type"]
+
+        # Case RFI
+        if entity["entity_type"] == "Case-Rfi":
+            entity["standard_id"] = "x-opencti-" + entity["standard_id"]
+            entity["entity_type"] = "x-opencti-" + entity["entity_type"]
+
+        # Case RFT
+        if entity["entity_type"] == "Case-Rft":
+            entity["standard_id"] = "x-opencti-" + entity["standard_id"]
+            entity["entity_type"] = "x-opencti-" + entity["entity_type"]
+
+        # Feedback
+        if entity["entity_type"] == "Feedback":
+            entity["standard_id"] = "x-opencti-" + entity["standard_id"]
+            entity["entity_type"] = "x-opencti-" + entity["entity_type"]
+
+        # Task
+        if entity["entity_type"] == "Task":
+            entity["standard_id"] = "x-opencti-" + entity["standard_id"]
+            entity["entity_type"] = "x-opencti-" + entity["entity_type"]
+
         # Data component
         if entity["entity_type"] == "Data-Component":
             entity["standard_id"] = "x-mitre-" + entity["standard_id"]
             entity["entity_type"] = "x-mitre-" + entity["entity_type"]
 
         # Data source
         if entity["entity_type"] == "Data-Source":
```

### Comparing `pycti-5.8.3/pycti/utils/opencti_stix2_splitter.py` & `pycti-5.8.4/pycti/utils/opencti_stix2_splitter.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti/utils/opencti_stix2_update.py` & `pycti-5.8.4/pycti/utils/opencti_stix2_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # coding: utf-8
 
+import traceback
+
 from pycti.api import LOGGER as API_LOGGER
 from pycti.utils.constants import StixCyberObservableTypes
 
 
 class OpenCTIStix2Update:
     """Python API for Stix2 Update in OpenCTI
 
@@ -294,11 +296,10 @@
                                 if (
                                     type(current_val) is dict and "value" in current_val
                                 )
                                 else str(current_val)
                             )
                             inputs.append({"key": key, "value": values})
             self.update_attribute(data["type"], data["id"], inputs)
-        except Exception as e:
-            print(e)
-            print(data)
-            API_LOGGER.error("Cannot process this message")
+        except Exception:
+            error_msg = traceback.format_exc()
+            API_LOGGER.error(error_msg)
```

### Comparing `pycti-5.8.3/pycti/utils/opencti_stix2_utils.py` & `pycti-5.8.4/pycti/utils/opencti_stix2_utils.py`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti.egg-info/PKG-INFO` & `pycti-5.8.4/pycti.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycti
-Version: 5.8.3
+Version: 5.8.4
 Summary: Python API client for OpenCTI.
 Home-page: https://github.com/OpenCTI-Platform/client-python
 Author: Filigran
 Author-email: contact@filigran.io
 Maintainer: Filigran
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pycti Version: 5.8.3 Summary: Python API client for
+Metadata-Version: 2.1 Name: pycti Version: 5.8.4 Summary: Python API client for
 OpenCTI. Home-page: https://github.com/OpenCTI-Platform/client-python Author:
 Filigran Author-email: contact@filigran.io Maintainer: Filigran License: Apache
 Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: Apache Software License Classifier: Natural Language :: English
 Classifier: Natural Language :: French Classifier: Operating System :: OS
```

### Comparing `pycti-5.8.3/pycti.egg-info/SOURCES.txt` & `pycti-5.8.4/pycti.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/pycti.egg-info/requires.txt` & `pycti-5.8.4/pycti.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 build~=0.10.0
 isort~=5.12.0
 types-pytz~=2023.3.0.0
 pre-commit~=3.3.2
 pytest-cases~=3.6.13
 pytest-cov~=4.1.0
 pytest_randomly~=3.12.0
-pytest~=7.3.2
+pytest~=7.4.0
 types-python-dateutil~=2.8.19
 wheel~=0.40.0
 
 [doc]
 autoapi~=2.0.1
 sphinx-autodoc-typehints~=1.23.0
 sphinx-rtd-theme~=1.2.1
```

### Comparing `pycti-5.8.3/pyproject.toml` & `pycti-5.8.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pycti-5.8.3/setup.cfg` & `pycti-5.8.4/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 	build~=0.10.0
 	isort~=5.12.0
 	types-pytz~=2023.3.0.0
 	pre-commit~=3.3.2
 	pytest-cases~=3.6.13
 	pytest-cov~=4.1.0
 	pytest_randomly~=3.12.0
-	pytest~=7.3.2
+	pytest~=7.4.0
 	types-python-dateutil~=2.8.19
 	wheel~=0.40.0
 doc = 
 	autoapi~=2.0.1
 	sphinx-autodoc-typehints~=1.23.0
 	sphinx-rtd-theme~=1.2.1
```

